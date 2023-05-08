# Comparing `tmp/cdktf-cdktf-provider-tfe-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-tfe-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-tfe-6.0.1.tar", last modified: Fri Apr 21 13:56:14 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-tfe-6.0.2.tar", last modified: Mon May  8 10:59:39 2023, max compression
```

## Comparing `cdktf-cdktf-provider-tfe-6.0.1.tar` & `cdktf-cdktf-provider-tfe-6.0.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.145719 cdktf-cdktf-provider-tfe-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   261489 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/_jsii/provider-tfe@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/admin_organization_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/admin_organization_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/agent_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/agent_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/agent_token/
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/agent_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/
--rw-r--r--   0 runner    (1001) docker     (123)    26559 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization/
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_members/
--rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_membership/
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_run_task/
--rw-r--r--   0 runner    (1001) docker     (123)    30279 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_run_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_tags/
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organizations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_outputs/
--rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_policy_set/
--rw-r--r--   0 runner    (1001) docker     (123)    36408 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_policy_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_project/
--rw-r--r--   0 runner    (1001) docker     (123)    22555 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_slug/
--rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_slug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_ssh_key/
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_ssh_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team/
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team_access/
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team_project_access/
--rw-r--r--   0 runner    (1001) docker     (123)    20235 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team_project_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_variable_set/
--rw-r--r--   0 runner    (1001) docker     (123)    25728 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_variable_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_variables/
--rw-r--r--   0 runner    (1001) docker     (123)    49966 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace/
--rw-r--r--   0 runner    (1001) docker     (123)    37511 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_ids/
--rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_run_task/
--rw-r--r--   0 runner    (1001) docker     (123)    20637 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_run_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/no_code_module/
--rw-r--r--   0 runner    (1001) docker     (123)    44867 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/no_code_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/notification_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    37847 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/notification_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/oauth_client/
--rw-r--r--   0 runner    (1001) docker     (123)    38121 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/oauth_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization/
--rw-r--r--   0 runner    (1001) docker     (123)    45712 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_membership/
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_membership/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_module_sharing/
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_module_sharing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_run_task/
--rw-r--r--   0 runner    (1001) docker     (123)    32051 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_run_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_token/
--rw-r--r--   0 runner    (1001) docker     (123)    21534 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy/
--rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy_set/
--rw-r--r--   0 runner    (1001) docker     (123)    58173 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy_set_parameter/
--rw-r--r--   0 runner    (1001) docker     (123)    25034 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy_set_parameter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/project/
--rw-r--r--   0 runner    (1001) docker     (123)    19750 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/project_variable_set/
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/project_variable_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/registry_module/
--rw-r--r--   0 runner    (1001) docker     (123)    45817 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/registry_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/run_trigger/
--rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/run_trigger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/sentinel_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/sentinel_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/ssh_key/
--rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/ssh_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team/
--rw-r--r--   0 runner    (1001) docker     (123)    60476 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_access/
--rw-r--r--   0 runner    (1001) docker     (123)    47608 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.157719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_member/
--rw-r--r--   0 runner    (1001) docker     (123)    19564 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_members/
--rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_organization_member/
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_organization_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_organization_members/
--rw-r--r--   0 runner    (1001) docker     (123)    20837 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_organization_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_project_access/
--rw-r--r--   0 runner    (1001) docker     (123)    21876 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_project_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_token/
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/terraform_version/
--rw-r--r--   0 runner    (1001) docker     (123)    35550 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/terraform_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/variable/
--rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/variable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/variable_set/
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/variable_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)   104821 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_policy_set/
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_policy_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_run_task/
--rw-r--r--   0 runner    (1001) docker     (123)    25375 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_run_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.161718 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_variable_set/
--rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-04-21 13:56:01.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_variable_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:56:14.153719 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-21 13:56:14.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-21 13:56:14.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:56:14.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 13:56:14.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 13:56:14.000000 cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.151063 cdktf-cdktf-provider-tfe-6.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.155063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   261494 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/_jsii/provider-tfe@6.0.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/admin_organization_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/admin_organization_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/agent_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/agent_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/agent_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/agent_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    26559 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization/
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_run_task/
+-rw-r--r--   0 runner    (1001) docker     (123)    30279 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_run_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organizations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_policy_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    36408 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_policy_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_project/
+-rw-r--r--   0 runner    (1001) docker     (123)    22555 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_slug/
+-rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_slug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_ssh_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_ssh_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team/
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team_project_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    20235 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team_project_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_variable_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    25728 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_variable_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    49966 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)    37511 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_run_task/
+-rw-r--r--   0 runner    (1001) docker     (123)    20637 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_run_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/no_code_module/
+-rw-r--r--   0 runner    (1001) docker     (123)    44867 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/no_code_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/notification_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    37847 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/notification_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/oauth_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    38121 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/oauth_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)    45712 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_membership/
+-rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_membership/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_module_sharing/
+-rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_module_sharing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_run_task/
+-rw-r--r--   0 runner    (1001) docker     (123)    32051 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_run_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    21534 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    58173 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy_set_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)    25034 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy_set_parameter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    19750 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/project_variable_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/project_variable_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/registry_module/
+-rw-r--r--   0 runner    (1001) docker     (123)    45817 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/registry_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/run_trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/run_trigger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/sentinel_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/sentinel_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/ssh_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/ssh_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team/
+-rw-r--r--   0 runner    (1001) docker     (123)    60476 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    47608 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    19564 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.163063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_organization_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_organization_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_organization_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    20837 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_organization_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_project_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    21876 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_project_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/terraform_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    35550 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/terraform_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/variable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/variable_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/variable_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)   104821 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_policy_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_policy_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_run_task/
+-rw-r--r--   0 runner    (1001) docker     (123)    25375 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_run_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.167063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_variable_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-05-08 10:59:26.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_variable_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:59:39.159063 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-08 10:59:39.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-08 10:59:39.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:59:39.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 10:59:39.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 10:59:39.000000 cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/LICENSE` & `cdktf-cdktf-provider-tfe-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-tfe-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-tfe
-Version: 6.0.1
+Version: 6.0.2
 Summary: Prebuilt tfe Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-tfe.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-tfe.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/README.md` & `cdktf-cdktf-provider-tfe-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/setup.py` & `cdktf-cdktf-provider-tfe-6.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-tfe",
-    "version": "6.0.1",
+    "version": "6.0.2",
     "description": "Prebuilt tfe Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-tfe.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -81,15 +81,15 @@
         "cdktf_cdktf_provider_tfe.workspace",
         "cdktf_cdktf_provider_tfe.workspace_policy_set",
         "cdktf_cdktf_provider_tfe.workspace_run_task",
         "cdktf_cdktf_provider_tfe.workspace_variable_set"
     ],
     "package_data": {
         "cdktf_cdktf_provider_tfe._jsii": [
-            "provider-tfe@6.0.1.jsii.tgz"
+            "provider-tfe@6.0.2.jsii.tgz"
         ],
         "cdktf_cdktf_provider_tfe": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/admin_organization_settings/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/admin_organization_settings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_admin_organization_settings`
 
-Refer to the Terraform Registory for docs: [`tfe_admin_organization_settings`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings).
+Refer to the Terraform Registory for docs: [`tfe_admin_organization_settings`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AdminOrganizationSettings(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.adminOrganizationSettings.AdminOrganizationSettings",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings tfe_admin_organization_settings}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings tfe_admin_organization_settings}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         access_beta_tools: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings tfe_admin_organization_settings} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings tfe_admin_organization_settings} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param access_beta_tools: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#access_beta_tools AdminOrganizationSettings#access_beta_tools}.
-        :param global_module_sharing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#global_module_sharing AdminOrganizationSettings#global_module_sharing}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#id AdminOrganizationSettings#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param module_sharing_consumer_organizations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#module_sharing_consumer_organizations AdminOrganizationSettings#module_sharing_consumer_organizations}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#organization AdminOrganizationSettings#organization}.
-        :param workspace_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#workspace_limit AdminOrganizationSettings#workspace_limit}.
+        :param access_beta_tools: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#access_beta_tools AdminOrganizationSettings#access_beta_tools}.
+        :param global_module_sharing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#global_module_sharing AdminOrganizationSettings#global_module_sharing}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#id AdminOrganizationSettings#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param module_sharing_consumer_organizations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#module_sharing_consumer_organizations AdminOrganizationSettings#module_sharing_consumer_organizations}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#organization AdminOrganizationSettings#organization}.
+        :param workspace_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#workspace_limit AdminOrganizationSettings#workspace_limit}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -288,20 +288,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param access_beta_tools: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#access_beta_tools AdminOrganizationSettings#access_beta_tools}.
-        :param global_module_sharing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#global_module_sharing AdminOrganizationSettings#global_module_sharing}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#id AdminOrganizationSettings#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param module_sharing_consumer_organizations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#module_sharing_consumer_organizations AdminOrganizationSettings#module_sharing_consumer_organizations}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#organization AdminOrganizationSettings#organization}.
-        :param workspace_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#workspace_limit AdminOrganizationSettings#workspace_limit}.
+        :param access_beta_tools: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#access_beta_tools AdminOrganizationSettings#access_beta_tools}.
+        :param global_module_sharing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#global_module_sharing AdminOrganizationSettings#global_module_sharing}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#id AdminOrganizationSettings#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param module_sharing_consumer_organizations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#module_sharing_consumer_organizations AdminOrganizationSettings#module_sharing_consumer_organizations}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#organization AdminOrganizationSettings#organization}.
+        :param workspace_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#workspace_limit AdminOrganizationSettings#workspace_limit}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e4319388d3295be9001de409fd83ced0642929bca854f80b540aee9f9ea6786b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -408,53 +408,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def access_beta_tools(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#access_beta_tools AdminOrganizationSettings#access_beta_tools}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#access_beta_tools AdminOrganizationSettings#access_beta_tools}.'''
         result = self._values.get("access_beta_tools")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def global_module_sharing(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#global_module_sharing AdminOrganizationSettings#global_module_sharing}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#global_module_sharing AdminOrganizationSettings#global_module_sharing}.'''
         result = self._values.get("global_module_sharing")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#id AdminOrganizationSettings#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#id AdminOrganizationSettings#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def module_sharing_consumer_organizations(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#module_sharing_consumer_organizations AdminOrganizationSettings#module_sharing_consumer_organizations}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#module_sharing_consumer_organizations AdminOrganizationSettings#module_sharing_consumer_organizations}.'''
         result = self._values.get("module_sharing_consumer_organizations")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#organization AdminOrganizationSettings#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#organization AdminOrganizationSettings#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def workspace_limit(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/admin_organization_settings#workspace_limit AdminOrganizationSettings#workspace_limit}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/admin_organization_settings#workspace_limit AdminOrganizationSettings#workspace_limit}.'''
         result = self._values.get("workspace_limit")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/agent_pool/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/agent_pool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_agent_pool`
 
-Refer to the Terraform Registory for docs: [`tfe_agent_pool`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool).
+Refer to the Terraform Registory for docs: [`tfe_agent_pool`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AgentPool(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.agentPool.AgentPool",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool tfe_agent_pool}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool tfe_agent_pool}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool tfe_agent_pool} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool tfe_agent_pool} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#name AgentPool#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#id AgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#organization AgentPool#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#name AgentPool#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#id AgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#organization AgentPool#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -182,17 +182,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#name AgentPool#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#id AgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#organization AgentPool#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#name AgentPool#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#id AgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#organization AgentPool#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e1f7e0ef535716bfbe9009c5f7d1724d707a0a01e0a5941bd59778399bad156d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,32 +288,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#name AgentPool#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#name AgentPool#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#id AgentPool#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#id AgentPool#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_pool#organization AgentPool#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_pool#organization AgentPool#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/agent_token/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/agent_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_agent_token`
 
-Refer to the Terraform Registory for docs: [`tfe_agent_token`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token).
+Refer to the Terraform Registory for docs: [`tfe_agent_token`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AgentToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.agentToken.AgentToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token tfe_agent_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token tfe_agent_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         agent_pool_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token tfe_agent_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token tfe_agent_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#agent_pool_id AgentToken#agent_pool_id}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#description AgentToken#description}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#id AgentToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#agent_pool_id AgentToken#agent_pool_id}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#description AgentToken#description}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#id AgentToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -183,17 +183,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#agent_pool_id AgentToken#agent_pool_id}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#description AgentToken#description}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#id AgentToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#agent_pool_id AgentToken#agent_pool_id}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#description AgentToken#description}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#id AgentToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fb7ccffba1afe9eb6b958af7a8ce6a096692ccee45e3098215f4c4169e5ceb51)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,29 +288,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def agent_pool_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#agent_pool_id AgentToken#agent_pool_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#agent_pool_id AgentToken#agent_pool_id}.'''
         result = self._values.get("agent_pool_id")
         assert result is not None, "Required property 'agent_pool_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#description AgentToken#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#description AgentToken#description}.'''
         result = self._values.get("description")
         assert result is not None, "Required property 'description' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/agent_token#id AgentToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/agent_token#id AgentToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_agent_pool`
 
-Refer to the Terraform Registory for docs: [`data_tfe_agent_pool`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool).
+Refer to the Terraform Registory for docs: [`data_tfe_agent_pool`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeAgentPool(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeAgentPool.DataTfeAgentPool",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool tfe_agent_pool}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool tfe_agent_pool}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool tfe_agent_pool} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool tfe_agent_pool} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#name DataTfeAgentPool#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#id DataTfeAgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#organization DataTfeAgentPool#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#name DataTfeAgentPool#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#id DataTfeAgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#organization DataTfeAgentPool#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -182,17 +182,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#name DataTfeAgentPool#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#id DataTfeAgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#organization DataTfeAgentPool#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#name DataTfeAgentPool#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#id DataTfeAgentPool#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#organization DataTfeAgentPool#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__17c6ec001f081f472a07af5a0a08105c11c854ccf56ff1e2c0cb4d2fa2372987)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,32 +288,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#name DataTfeAgentPool#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#name DataTfeAgentPool#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#id DataTfeAgentPool#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#id DataTfeAgentPool#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/agent_pool#organization DataTfeAgentPool#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/agent_pool#organization DataTfeAgentPool#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_github_app_installation`
 
-Refer to the Terraform Registory for docs: [`data_tfe_github_app_installation`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation).
+Refer to the Terraform Registory for docs: [`data_tfe_github_app_installation`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeGithubAppInstallation(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeGithubAppInstallation.DataTfeGithubAppInstallation",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation tfe_github_app_installation}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation tfe_github_app_installation}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         installation_id: typing.Optional[jsii.Number] = None,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation tfe_github_app_installation} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation tfe_github_app_installation} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation#installation_id DataTfeGithubAppInstallation#installation_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation#name DataTfeGithubAppInstallation#name}.
+        :param installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation#installation_id DataTfeGithubAppInstallation#installation_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation#name DataTfeGithubAppInstallation#name}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -165,16 +165,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation#installation_id DataTfeGithubAppInstallation#installation_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation#name DataTfeGithubAppInstallation#name}.
+        :param installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation#installation_id DataTfeGithubAppInstallation#installation_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation#name DataTfeGithubAppInstallation#name}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d377c67899a34018642b068d1ffc007eadcabdba548a84dfee367114e136f3ae)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -267,21 +267,21 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def installation_id(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation#installation_id DataTfeGithubAppInstallation#installation_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation#installation_id DataTfeGithubAppInstallation#installation_id}.'''
         result = self._values.get("installation_id")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/github_app_installation#name DataTfeGithubAppInstallation#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/github_app_installation#name DataTfeGithubAppInstallation#name}.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_ip_ranges`
 
-Refer to the Terraform Registory for docs: [`data_tfe_ip_ranges`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ip_ranges).
+Refer to the Terraform Registory for docs: [`data_tfe_ip_ranges`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ip_ranges).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeIpRanges(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeIpRanges.DataTfeIpRanges",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ip_ranges tfe_ip_ranges}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ip_ranges tfe_ip_ranges}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -38,19 +38,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ip_ranges tfe_ip_ranges} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ip_ranges tfe_ip_ranges} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ip_ranges#id DataTfeIpRanges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ip_ranges#id DataTfeIpRanges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -154,15 +154,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ip_ranges#id DataTfeIpRanges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ip_ranges#id DataTfeIpRanges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__48fa5a316bda710fbe1b6d4a5a008d7dbe921c066f10c2f2186a344c6ef09f65)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -252,15 +252,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ip_ranges#id DataTfeIpRanges#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ip_ranges#id DataTfeIpRanges#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_oauth_client`
 
-Refer to the Terraform Registory for docs: [`data_tfe_oauth_client`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client).
+Refer to the Terraform Registory for docs: [`data_tfe_oauth_client`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOauthClient(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOauthClient.DataTfeOauthClient",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client tfe_oauth_client}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client tfe_oauth_client}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client tfe_oauth_client} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client tfe_oauth_client} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#id DataTfeOauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#name DataTfeOauthClient#name}.
-        :param oauth_client_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#oauth_client_id DataTfeOauthClient#oauth_client_id}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#organization DataTfeOauthClient#organization}.
-        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#service_provider DataTfeOauthClient#service_provider}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#id DataTfeOauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#name DataTfeOauthClient#name}.
+        :param oauth_client_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#oauth_client_id DataTfeOauthClient#oauth_client_id}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#organization DataTfeOauthClient#organization}.
+        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#service_provider DataTfeOauthClient#service_provider}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -268,19 +268,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#id DataTfeOauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#name DataTfeOauthClient#name}.
-        :param oauth_client_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#oauth_client_id DataTfeOauthClient#oauth_client_id}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#organization DataTfeOauthClient#organization}.
-        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#service_provider DataTfeOauthClient#service_provider}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#id DataTfeOauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#name DataTfeOauthClient#name}.
+        :param oauth_client_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#oauth_client_id DataTfeOauthClient#oauth_client_id}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#organization DataTfeOauthClient#organization}.
+        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#service_provider DataTfeOauthClient#service_provider}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f24d7975a037de689a5de9356ff44a8c12f24b7e4688d46254f6fffce3d543d9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -382,43 +382,43 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#id DataTfeOauthClient#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#id DataTfeOauthClient#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#name DataTfeOauthClient#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#name DataTfeOauthClient#name}.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def oauth_client_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#oauth_client_id DataTfeOauthClient#oauth_client_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#oauth_client_id DataTfeOauthClient#oauth_client_id}.'''
         result = self._values.get("oauth_client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#organization DataTfeOauthClient#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#organization DataTfeOauthClient#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def service_provider(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/oauth_client#service_provider DataTfeOauthClient#service_provider}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/oauth_client#service_provider DataTfeOauthClient#service_provider}.'''
         result = self._values.get("service_provider")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_organization`
 
-Refer to the Terraform Registory for docs: [`data_tfe_organization`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization).
+Refer to the Terraform Registory for docs: [`data_tfe_organization`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOrganization(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOrganization.DataTfeOrganization",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization tfe_organization}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization tfe_organization}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization tfe_organization} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization tfe_organization} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization#name DataTfeOrganization#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization#id DataTfeOrganization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization#name DataTfeOrganization#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization#id DataTfeOrganization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -203,16 +203,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization#name DataTfeOrganization#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization#id DataTfeOrganization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization#name DataTfeOrganization#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization#id DataTfeOrganization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1b686c4f10689b9be4172cf55b7fb762ca51f3750bbe8e749c14e1afd8ca28d9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -305,22 +305,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization#name DataTfeOrganization#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization#name DataTfeOrganization#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization#id DataTfeOrganization#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization#id DataTfeOrganization#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_members/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_members/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_organization_members`
 
-Refer to the Terraform Registory for docs: [`data_tfe_organization_members`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members).
+Refer to the Terraform Registory for docs: [`data_tfe_organization_members`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOrganizationMembers(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOrganizationMembers.DataTfeOrganizationMembers",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members tfe_organization_members}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members tfe_organization_members}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members tfe_organization_members} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members tfe_organization_members} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members#id DataTfeOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members#organization DataTfeOrganizationMembers#organization}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members#id DataTfeOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members#organization DataTfeOrganizationMembers#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -170,16 +170,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members#id DataTfeOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members#organization DataTfeOrganizationMembers#organization}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members#id DataTfeOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members#organization DataTfeOrganizationMembers#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ae48e98e72d31298f98fa740f15c9137982998b928eae8ffc8228e911d22e772)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -272,25 +272,25 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members#id DataTfeOrganizationMembers#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members#id DataTfeOrganizationMembers#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_members#organization DataTfeOrganizationMembers#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_members#organization DataTfeOrganizationMembers#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_membership/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_membership/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_organization_membership`
 
-Refer to the Terraform Registory for docs: [`data_tfe_organization_membership`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership).
+Refer to the Terraform Registory for docs: [`data_tfe_organization_membership`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOrganizationMembership(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOrganizationMembership.DataTfeOrganizationMembership",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership tfe_organization_membership}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership tfe_organization_membership}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: typing.Optional[builtins.str] = None,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership tfe_organization_membership} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership tfe_organization_membership} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#email DataTfeOrganizationMembership#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#id DataTfeOrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#organization DataTfeOrganizationMembership#organization}.
-        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#username DataTfeOrganizationMembership#username}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#email DataTfeOrganizationMembership#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#id DataTfeOrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#organization DataTfeOrganizationMembership#organization}.
+        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#username DataTfeOrganizationMembership#username}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -217,18 +217,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#email DataTfeOrganizationMembership#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#id DataTfeOrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#organization DataTfeOrganizationMembership#organization}.
-        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#username DataTfeOrganizationMembership#username}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#email DataTfeOrganizationMembership#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#id DataTfeOrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#organization DataTfeOrganizationMembership#organization}.
+        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#username DataTfeOrganizationMembership#username}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__31345a5d05c53bffb011099cfda2593540eba08b7acdc96f57ec6e0b24936bca)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -327,37 +327,37 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#email DataTfeOrganizationMembership#email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#email DataTfeOrganizationMembership#email}.'''
         result = self._values.get("email")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#id DataTfeOrganizationMembership#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#id DataTfeOrganizationMembership#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#organization DataTfeOrganizationMembership#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#organization DataTfeOrganizationMembership#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_membership#username DataTfeOrganizationMembership#username}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_membership#username DataTfeOrganizationMembership#username}.'''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_run_task/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_run_task/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_organization_run_task`
 
-Refer to the Terraform Registory for docs: [`data_tfe_organization_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task).
+Refer to the Terraform Registory for docs: [`data_tfe_organization_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOrganizationRunTask(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOrganizationRunTask.DataTfeOrganizationRunTask",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task tfe_organization_run_task}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task tfe_organization_run_task}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task tfe_organization_run_task} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task tfe_organization_run_task} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#name DataTfeOrganizationRunTask#name}.
-        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#category DataTfeOrganizationRunTask#category}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#description DataTfeOrganizationRunTask#description}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#enabled DataTfeOrganizationRunTask#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#id DataTfeOrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#organization DataTfeOrganizationRunTask#organization}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#url DataTfeOrganizationRunTask#url}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#name DataTfeOrganizationRunTask#name}.
+        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#category DataTfeOrganizationRunTask#category}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#description DataTfeOrganizationRunTask#description}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#enabled DataTfeOrganizationRunTask#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#id DataTfeOrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#organization DataTfeOrganizationRunTask#organization}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#url DataTfeOrganizationRunTask#url}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -291,21 +291,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#name DataTfeOrganizationRunTask#name}.
-        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#category DataTfeOrganizationRunTask#category}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#description DataTfeOrganizationRunTask#description}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#enabled DataTfeOrganizationRunTask#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#id DataTfeOrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#organization DataTfeOrganizationRunTask#organization}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#url DataTfeOrganizationRunTask#url}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#name DataTfeOrganizationRunTask#name}.
+        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#category DataTfeOrganizationRunTask#category}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#description DataTfeOrganizationRunTask#description}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#enabled DataTfeOrganizationRunTask#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#id DataTfeOrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#organization DataTfeOrganizationRunTask#organization}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#url DataTfeOrganizationRunTask#url}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__db30db2443f1b2b635bfeb52337df89f861374e84007493d826702723fd66b36)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -413,58 +413,58 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#name DataTfeOrganizationRunTask#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#name DataTfeOrganizationRunTask#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def category(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#category DataTfeOrganizationRunTask#category}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#category DataTfeOrganizationRunTask#category}.'''
         result = self._values.get("category")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#description DataTfeOrganizationRunTask#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#description DataTfeOrganizationRunTask#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#enabled DataTfeOrganizationRunTask#enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#enabled DataTfeOrganizationRunTask#enabled}.'''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#id DataTfeOrganizationRunTask#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#id DataTfeOrganizationRunTask#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#organization DataTfeOrganizationRunTask#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#organization DataTfeOrganizationRunTask#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_run_task#url DataTfeOrganizationRunTask#url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_run_task#url DataTfeOrganizationRunTask#url}.'''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organization_tags/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organization_tags/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_organization_tags`
 
-Refer to the Terraform Registory for docs: [`data_tfe_organization_tags`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags).
+Refer to the Terraform Registory for docs: [`data_tfe_organization_tags`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOrganizationTags(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOrganizationTags.DataTfeOrganizationTags",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags tfe_organization_tags}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags tfe_organization_tags}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags tfe_organization_tags} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags tfe_organization_tags} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags#id DataTfeOrganizationTags#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags#organization DataTfeOrganizationTags#organization}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags#id DataTfeOrganizationTags#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags#organization DataTfeOrganizationTags#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -165,16 +165,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags#id DataTfeOrganizationTags#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags#organization DataTfeOrganizationTags#organization}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags#id DataTfeOrganizationTags#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags#organization DataTfeOrganizationTags#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4775b5af19c2c1cc356201b8cacca008fd4f20cfdf5aa758f4b6a0c1780cf881)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -267,25 +267,25 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags#id DataTfeOrganizationTags#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags#id DataTfeOrganizationTags#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organization_tags#organization DataTfeOrganizationTags#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organization_tags#organization DataTfeOrganizationTags#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_organizations/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_organizations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_organizations`
 
-Refer to the Terraform Registory for docs: [`data_tfe_organizations`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations).
+Refer to the Terraform Registory for docs: [`data_tfe_organizations`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOrganizations(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOrganizations.DataTfeOrganizations",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations tfe_organizations}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations tfe_organizations}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         admin: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations tfe_organizations} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations tfe_organizations} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param admin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations#admin DataTfeOrganizations#admin}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations#id DataTfeOrganizations#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param admin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations#admin DataTfeOrganizations#admin}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations#id DataTfeOrganizations#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -175,16 +175,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param admin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations#admin DataTfeOrganizations#admin}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations#id DataTfeOrganizations#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param admin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations#admin DataTfeOrganizations#admin}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations#id DataTfeOrganizations#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__69047a531072607fd9db88f984c3184ace1afde21cd0678751a7664da3546921)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -279,21 +279,21 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def admin(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations#admin DataTfeOrganizations#admin}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations#admin DataTfeOrganizations#admin}.'''
         result = self._values.get("admin")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/organizations#id DataTfeOrganizations#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/organizations#id DataTfeOrganizations#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_outputs/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_outputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_outputs`
 
-Refer to the Terraform Registory for docs: [`data_tfe_outputs`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs).
+Refer to the Terraform Registory for docs: [`data_tfe_outputs`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeOutputs(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeOutputs.DataTfeOutputs",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs tfe_outputs}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs tfe_outputs}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         workspace: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs tfe_outputs} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs tfe_outputs} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param workspace: The workspace to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#workspace DataTfeOutputs#workspace}
-        :param organization: The organization to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#organization DataTfeOutputs#organization}
-        :param values: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#values DataTfeOutputs#values}.
+        :param workspace: The workspace to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#workspace DataTfeOutputs#workspace}
+        :param organization: The organization to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#organization DataTfeOutputs#organization}
+        :param values: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#values DataTfeOutputs#values}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -192,17 +192,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param workspace: The workspace to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#workspace DataTfeOutputs#workspace}
-        :param organization: The organization to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#organization DataTfeOutputs#organization}
-        :param values: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#values DataTfeOutputs#values}.
+        :param workspace: The workspace to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#workspace DataTfeOutputs#workspace}
+        :param organization: The organization to fetch the remote state from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#organization DataTfeOutputs#organization}
+        :param values: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#values DataTfeOutputs#values}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d32784b9b8fe1f5881f23a0cf8d372b5854b3ff74a91ce6b1b0afb35724454a9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -300,32 +300,32 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def workspace(self) -> builtins.str:
         '''The workspace to fetch the remote state from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#workspace DataTfeOutputs#workspace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#workspace DataTfeOutputs#workspace}
         '''
         result = self._values.get("workspace")
         assert result is not None, "Required property 'workspace' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
         '''The organization to fetch the remote state from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#organization DataTfeOutputs#organization}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#organization DataTfeOutputs#organization}
         '''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def values(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/outputs#values DataTfeOutputs#values}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/outputs#values DataTfeOutputs#values}.'''
         result = self._values.get("values")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_policy_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_policy_set/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_policy_set`
 
-Refer to the Terraform Registory for docs: [`data_tfe_policy_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set).
+Refer to the Terraform Registory for docs: [`data_tfe_policy_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfePolicySet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfePolicySet.DataTfePolicySet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set tfe_policy_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set tfe_policy_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set tfe_policy_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set tfe_policy_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#name DataTfePolicySet#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#id DataTfePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#kind DataTfePolicySet#kind}
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#organization DataTfePolicySet#organization}.
-        :param overridable: Whether users can override this policy when it fails during a run. Only valid for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#overridable DataTfePolicySet#overridable}
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#name DataTfePolicySet#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#id DataTfePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#kind DataTfePolicySet#kind}
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#organization DataTfePolicySet#organization}.
+        :param overridable: Whether users can override this policy when it fails during a run. Only valid for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#overridable DataTfePolicySet#overridable}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -269,19 +269,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#name DataTfePolicySet#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#id DataTfePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#kind DataTfePolicySet#kind}
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#organization DataTfePolicySet#organization}.
-        :param overridable: Whether users can override this policy when it fails during a run. Only valid for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#overridable DataTfePolicySet#overridable}
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#name DataTfePolicySet#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#id DataTfePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#kind DataTfePolicySet#kind}
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#organization DataTfePolicySet#organization}.
+        :param overridable: Whether users can override this policy when it fails during a run. Only valid for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#overridable DataTfePolicySet#overridable}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__de04a2374b67ea79390b7ea0eb18c1f7f51aeaf63d037c2d64a7ab6264d30606)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -383,51 +383,51 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#name DataTfePolicySet#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#name DataTfePolicySet#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#id DataTfePolicySet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#id DataTfePolicySet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def kind(self) -> typing.Optional[builtins.str]:
         '''The policy-as-code framework for the policy. Valid values are sentinel and opa.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#kind DataTfePolicySet#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#kind DataTfePolicySet#kind}
         '''
         result = self._values.get("kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#organization DataTfePolicySet#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#organization DataTfePolicySet#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def overridable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether users can override this policy when it fails during a run. Only valid for OPA policies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/policy_set#overridable DataTfePolicySet#overridable}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/policy_set#overridable DataTfePolicySet#overridable}
         '''
         result = self._values.get("overridable")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_project/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_project`
 
-Refer to the Terraform Registory for docs: [`data_tfe_project`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project).
+Refer to the Terraform Registory for docs: [`data_tfe_project`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeProject(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeProject.DataTfeProject",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project tfe_project}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project tfe_project}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project tfe_project} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project tfe_project} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#name DataTfeProject#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#id DataTfeProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#organization DataTfeProject#organization}.
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#workspace_ids DataTfeProject#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#name DataTfeProject#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#id DataTfeProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#organization DataTfeProject#organization}.
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#workspace_ids DataTfeProject#workspace_ids}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -208,18 +208,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#name DataTfeProject#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#id DataTfeProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#organization DataTfeProject#organization}.
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#workspace_ids DataTfeProject#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#name DataTfeProject#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#id DataTfeProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#organization DataTfeProject#organization}.
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#workspace_ids DataTfeProject#workspace_ids}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0379b1c44eb470f3476f7354d5340fbf682a36030739e1cc88ca7fba603ce4aa)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -318,38 +318,38 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#name DataTfeProject#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#name DataTfeProject#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#id DataTfeProject#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#id DataTfeProject#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#organization DataTfeProject#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#organization DataTfeProject#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def workspace_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/project#workspace_ids DataTfeProject#workspace_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/project#workspace_ids DataTfeProject#workspace_ids}.'''
         result = self._values.get("workspace_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_slug/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_slug/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_slug`
 
-Refer to the Terraform Registory for docs: [`data_tfe_slug`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug).
+Refer to the Terraform Registory for docs: [`data_tfe_slug`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeSlug(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeSlug.DataTfeSlug",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug tfe_slug}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug tfe_slug}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         source_path: builtins.str,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug tfe_slug} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug tfe_slug} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param source_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug#source_path DataTfeSlug#source_path}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug#id DataTfeSlug#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param source_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug#source_path DataTfeSlug#source_path}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug#id DataTfeSlug#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -156,16 +156,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param source_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug#source_path DataTfeSlug#source_path}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug#id DataTfeSlug#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param source_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug#source_path DataTfeSlug#source_path}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug#id DataTfeSlug#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cc5d5f7ff234f741948a741c769a4221809a3780f689d4f788279779bc4b448e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -258,22 +258,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def source_path(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug#source_path DataTfeSlug#source_path}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug#source_path DataTfeSlug#source_path}.'''
         result = self._values.get("source_path")
         assert result is not None, "Required property 'source_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/slug#id DataTfeSlug#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/slug#id DataTfeSlug#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_ssh_key/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_ssh_key/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_ssh_key`
 
-Refer to the Terraform Registory for docs: [`data_tfe_ssh_key`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key).
+Refer to the Terraform Registory for docs: [`data_tfe_ssh_key`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeSshKey(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeSshKey.DataTfeSshKey",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key tfe_ssh_key}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key tfe_ssh_key}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key tfe_ssh_key} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key tfe_ssh_key} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#name DataTfeSshKey#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#id DataTfeSshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#organization DataTfeSshKey#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#name DataTfeSshKey#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#id DataTfeSshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#organization DataTfeSshKey#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -182,17 +182,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#name DataTfeSshKey#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#id DataTfeSshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#organization DataTfeSshKey#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#name DataTfeSshKey#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#id DataTfeSshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#organization DataTfeSshKey#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b8693cb6aed64c80c545b2eb4fb7172957a82084023e10545785505ad4a1437f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,32 +288,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#name DataTfeSshKey#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#name DataTfeSshKey#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#id DataTfeSshKey#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#id DataTfeSshKey#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/ssh_key#organization DataTfeSshKey#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/ssh_key#organization DataTfeSshKey#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_team`
 
-Refer to the Terraform Registory for docs: [`data_tfe_team`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team).
+Refer to the Terraform Registory for docs: [`data_tfe_team`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeTeam(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeTeam.DataTfeTeam",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team tfe_team}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team tfe_team}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team tfe_team} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team tfe_team} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#name DataTfeTeam#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#id DataTfeTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#organization DataTfeTeam#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#name DataTfeTeam#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#id DataTfeTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#organization DataTfeTeam#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -187,17 +187,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#name DataTfeTeam#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#id DataTfeTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#organization DataTfeTeam#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#name DataTfeTeam#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#id DataTfeTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#organization DataTfeTeam#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8337553cc49ec80e3dfff0ba847bfe255a4644be58c96901fc77971d00a61544)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -293,32 +293,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#name DataTfeTeam#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#name DataTfeTeam#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#id DataTfeTeam#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#id DataTfeTeam#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team#organization DataTfeTeam#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team#organization DataTfeTeam#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team_access/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team_access/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_team_access`
 
-Refer to the Terraform Registory for docs: [`data_tfe_team_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access).
+Refer to the Terraform Registory for docs: [`data_tfe_team_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeTeamAccess(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeTeamAccess.DataTfeTeamAccess",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access tfe_team_access}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access tfe_team_access}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         team_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access tfe_team_access} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access tfe_team_access} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#team_id DataTfeTeamAccess#team_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#workspace_id DataTfeTeamAccess#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#id DataTfeTeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#team_id DataTfeTeamAccess#team_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#workspace_id DataTfeTeamAccess#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#id DataTfeTeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -188,17 +188,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#team_id DataTfeTeamAccess#team_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#workspace_id DataTfeTeamAccess#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#id DataTfeTeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#team_id DataTfeTeamAccess#team_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#workspace_id DataTfeTeamAccess#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#id DataTfeTeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8af74129dee144ab8c5345f4ee129cfeba6a30420bb71ca41db13dcddbc2292f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -293,29 +293,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#team_id DataTfeTeamAccess#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#team_id DataTfeTeamAccess#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#workspace_id DataTfeTeamAccess#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#workspace_id DataTfeTeamAccess#workspace_id}.'''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_access#id DataTfeTeamAccess#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_access#id DataTfeTeamAccess#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_team_project_access/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_team_project_access/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_team_project_access`
 
-Refer to the Terraform Registory for docs: [`data_tfe_team_project_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access).
+Refer to the Terraform Registory for docs: [`data_tfe_team_project_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeTeamProjectAccess(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeTeamProjectAccess.DataTfeTeamProjectAccess",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access tfe_team_project_access}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access tfe_team_project_access}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         project_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access tfe_team_project_access} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access tfe_team_project_access} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#project_id DataTfeTeamProjectAccess#project_id}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#team_id DataTfeTeamProjectAccess#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#id DataTfeTeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#project_id DataTfeTeamProjectAccess#project_id}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#team_id DataTfeTeamProjectAccess#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#id DataTfeTeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -183,17 +183,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#project_id DataTfeTeamProjectAccess#project_id}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#team_id DataTfeTeamProjectAccess#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#id DataTfeTeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#project_id DataTfeTeamProjectAccess#project_id}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#team_id DataTfeTeamProjectAccess#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#id DataTfeTeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8e8469301577c7c79674d6bea30ea6284ad7aad4efdd14a4838c216555cf05d0)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,29 +288,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def project_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#project_id DataTfeTeamProjectAccess#project_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#project_id DataTfeTeamProjectAccess#project_id}.'''
         result = self._values.get("project_id")
         assert result is not None, "Required property 'project_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#team_id DataTfeTeamProjectAccess#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#team_id DataTfeTeamProjectAccess#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/team_project_access#id DataTfeTeamProjectAccess#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/team_project_access#id DataTfeTeamProjectAccess#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_variable_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_variable_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_variable_set`
 
-Refer to the Terraform Registory for docs: [`data_tfe_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set).
+Refer to the Terraform Registory for docs: [`data_tfe_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeVariableSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeVariableSet.DataTfeVariableSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set tfe_variable_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set tfe_variable_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set tfe_variable_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set tfe_variable_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#name DataTfeVariableSet#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#id DataTfeVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#organization DataTfeVariableSet#organization}.
-        :param variable_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#variable_ids DataTfeVariableSet#variable_ids}.
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#workspace_ids DataTfeVariableSet#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#name DataTfeVariableSet#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#id DataTfeVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#organization DataTfeVariableSet#organization}.
+        :param variable_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#variable_ids DataTfeVariableSet#variable_ids}.
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#workspace_ids DataTfeVariableSet#workspace_ids}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -244,19 +244,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#name DataTfeVariableSet#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#id DataTfeVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#organization DataTfeVariableSet#organization}.
-        :param variable_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#variable_ids DataTfeVariableSet#variable_ids}.
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#workspace_ids DataTfeVariableSet#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#name DataTfeVariableSet#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#id DataTfeVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#organization DataTfeVariableSet#organization}.
+        :param variable_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#variable_ids DataTfeVariableSet#variable_ids}.
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#workspace_ids DataTfeVariableSet#workspace_ids}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e9df0f24d73a8965cadefcbd639a3705f00d00f33ddab99aa2dfedf4174f8c0f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -358,44 +358,44 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#name DataTfeVariableSet#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#name DataTfeVariableSet#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#id DataTfeVariableSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#id DataTfeVariableSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#organization DataTfeVariableSet#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#organization DataTfeVariableSet#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def variable_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#variable_ids DataTfeVariableSet#variable_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#variable_ids DataTfeVariableSet#variable_ids}.'''
         result = self._values.get("variable_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def workspace_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variable_set#workspace_ids DataTfeVariableSet#workspace_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variable_set#workspace_ids DataTfeVariableSet#workspace_ids}.'''
         result = self._values.get("workspace_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_variables/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_variables/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_variables`
 
-Refer to the Terraform Registory for docs: [`data_tfe_variables`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables).
+Refer to the Terraform Registory for docs: [`data_tfe_variables`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeVariables(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeVariables.DataTfeVariables",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables tfe_variables}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables tfe_variables}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables tfe_variables} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables tfe_variables} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#id DataTfeVariables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#variable_set_id DataTfeVariables#variable_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#workspace_id DataTfeVariables#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#id DataTfeVariables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#variable_set_id DataTfeVariables#variable_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#workspace_id DataTfeVariables#workspace_id}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -201,17 +201,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#id DataTfeVariables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#variable_set_id DataTfeVariables#variable_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#workspace_id DataTfeVariables#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#id DataTfeVariables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#variable_set_id DataTfeVariables#variable_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#workspace_id DataTfeVariables#workspace_id}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__42b34927b1443d696703a56b5ca5703cb3410cfcf58ca958597f8f724195fe78)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -307,31 +307,31 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#id DataTfeVariables#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#id DataTfeVariables#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def variable_set_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#variable_set_id DataTfeVariables#variable_set_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#variable_set_id DataTfeVariables#variable_set_id}.'''
         result = self._values.get("variable_set_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def workspace_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/variables#workspace_id DataTfeVariables#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/variables#workspace_id DataTfeVariables#workspace_id}.'''
         result = self._values.get("workspace_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_workspace`
 
-Refer to the Terraform Registory for docs: [`data_tfe_workspace`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace).
+Refer to the Terraform Registory for docs: [`data_tfe_workspace`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeWorkspace(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeWorkspace.DataTfeWorkspace",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace tfe_workspace}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace tfe_workspace}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace tfe_workspace} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace tfe_workspace} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#name DataTfeWorkspace#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#id DataTfeWorkspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#organization DataTfeWorkspace#organization}.
-        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#tag_names DataTfeWorkspace#tag_names}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#name DataTfeWorkspace#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#id DataTfeWorkspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#organization DataTfeWorkspace#organization}.
+        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#tag_names DataTfeWorkspace#tag_names}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -338,18 +338,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#name DataTfeWorkspace#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#id DataTfeWorkspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#organization DataTfeWorkspace#organization}.
-        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#tag_names DataTfeWorkspace#tag_names}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#name DataTfeWorkspace#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#id DataTfeWorkspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#organization DataTfeWorkspace#organization}.
+        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#tag_names DataTfeWorkspace#tag_names}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5b95abeab60c90a34d62075a37ab76da2c178e6d3f85a264e568ccd01265f0b1)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -448,38 +448,38 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#name DataTfeWorkspace#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#name DataTfeWorkspace#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#id DataTfeWorkspace#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#id DataTfeWorkspace#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#organization DataTfeWorkspace#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#organization DataTfeWorkspace#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tag_names(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace#tag_names DataTfeWorkspace#tag_names}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace#tag_names DataTfeWorkspace#tag_names}.'''
         result = self._values.get("tag_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_ids/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_ids/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_workspace_ids`
 
-Refer to the Terraform Registory for docs: [`data_tfe_workspace_ids`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids).
+Refer to the Terraform Registory for docs: [`data_tfe_workspace_ids`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeWorkspaceIds(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeWorkspaceIds.DataTfeWorkspaceIds",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids tfe_workspace_ids}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids tfe_workspace_ids}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         exclude_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids tfe_workspace_ids} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids tfe_workspace_ids} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param exclude_tags: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#exclude_tags DataTfeWorkspaceIds#exclude_tags}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#id DataTfeWorkspaceIds#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#names DataTfeWorkspaceIds#names}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#organization DataTfeWorkspaceIds#organization}.
-        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#tag_names DataTfeWorkspaceIds#tag_names}.
+        :param exclude_tags: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#exclude_tags DataTfeWorkspaceIds#exclude_tags}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#id DataTfeWorkspaceIds#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#names DataTfeWorkspaceIds#names}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#organization DataTfeWorkspaceIds#organization}.
+        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#tag_names DataTfeWorkspaceIds#tag_names}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -248,19 +248,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param exclude_tags: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#exclude_tags DataTfeWorkspaceIds#exclude_tags}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#id DataTfeWorkspaceIds#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#names DataTfeWorkspaceIds#names}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#organization DataTfeWorkspaceIds#organization}.
-        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#tag_names DataTfeWorkspaceIds#tag_names}.
+        :param exclude_tags: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#exclude_tags DataTfeWorkspaceIds#exclude_tags}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#id DataTfeWorkspaceIds#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#names DataTfeWorkspaceIds#names}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#organization DataTfeWorkspaceIds#organization}.
+        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#tag_names DataTfeWorkspaceIds#tag_names}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7df5a5704f85566d0392a0dcf84ea57c8db2a0aa26fd73f44b58c8c9a619450)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -362,43 +362,43 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def exclude_tags(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#exclude_tags DataTfeWorkspaceIds#exclude_tags}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#exclude_tags DataTfeWorkspaceIds#exclude_tags}.'''
         result = self._values.get("exclude_tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#id DataTfeWorkspaceIds#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#id DataTfeWorkspaceIds#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def names(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#names DataTfeWorkspaceIds#names}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#names DataTfeWorkspaceIds#names}.'''
         result = self._values.get("names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#organization DataTfeWorkspaceIds#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#organization DataTfeWorkspaceIds#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tag_names(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_ids#tag_names DataTfeWorkspaceIds#tag_names}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_ids#tag_names DataTfeWorkspaceIds#tag_names}.'''
         result = self._values.get("tag_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_run_task/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/data_tfe_workspace_run_task/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_tfe_workspace_run_task`
 
-Refer to the Terraform Registory for docs: [`data_tfe_workspace_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task).
+Refer to the Terraform Registory for docs: [`data_tfe_workspace_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataTfeWorkspaceRunTask(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.dataTfeWorkspaceRunTask.DataTfeWorkspaceRunTask",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task tfe_workspace_run_task}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task tfe_workspace_run_task}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         task_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task tfe_workspace_run_task} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task tfe_workspace_run_task} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param task_id: The id of the run task. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#task_id DataTfeWorkspaceRunTask#task_id}
-        :param workspace_id: The id of the workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#workspace_id DataTfeWorkspaceRunTask#workspace_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#id DataTfeWorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param task_id: The id of the run task. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#task_id DataTfeWorkspaceRunTask#task_id}
+        :param workspace_id: The id of the workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#workspace_id DataTfeWorkspaceRunTask#workspace_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#id DataTfeWorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -188,17 +188,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param task_id: The id of the run task. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#task_id DataTfeWorkspaceRunTask#task_id}
-        :param workspace_id: The id of the workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#workspace_id DataTfeWorkspaceRunTask#workspace_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#id DataTfeWorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param task_id: The id of the run task. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#task_id DataTfeWorkspaceRunTask#task_id}
+        :param workspace_id: The id of the workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#workspace_id DataTfeWorkspaceRunTask#workspace_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#id DataTfeWorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ac559d8c0b2d128e97b2765cb638447f05a3c909625d68dc621711774b27c324)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -295,33 +295,33 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def task_id(self) -> builtins.str:
         '''The id of the run task.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#task_id DataTfeWorkspaceRunTask#task_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#task_id DataTfeWorkspaceRunTask#task_id}
         '''
         result = self._values.get("task_id")
         assert result is not None, "Required property 'task_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
         '''The id of the workspace.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#workspace_id DataTfeWorkspaceRunTask#workspace_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#workspace_id DataTfeWorkspaceRunTask#workspace_id}
         '''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/data-sources/workspace_run_task#id DataTfeWorkspaceRunTask#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/data-sources/workspace_run_task#id DataTfeWorkspaceRunTask#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/no_code_module/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/no_code_module/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_no_code_module`
 
-Refer to the Terraform Registory for docs: [`tfe_no_code_module`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module).
+Refer to the Terraform Registory for docs: [`tfe_no_code_module`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class NoCodeModule(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.noCodeModule.NoCodeModule",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module tfe_no_code_module}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module tfe_no_code_module}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         registry_module: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module tfe_no_code_module} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module tfe_no_code_module} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param registry_module: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#registry_module NoCodeModule#registry_module}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#enabled NoCodeModule#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#id NoCodeModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#organization NoCodeModule#organization}.
-        :param variable_options: variable_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#variable_options NoCodeModule#variable_options}
-        :param version_pin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#version_pin NoCodeModule#version_pin}.
+        :param registry_module: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#registry_module NoCodeModule#registry_module}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#enabled NoCodeModule#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#id NoCodeModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#organization NoCodeModule#organization}.
+        :param variable_options: variable_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#variable_options NoCodeModule#variable_options}
+        :param version_pin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#version_pin NoCodeModule#version_pin}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -273,20 +273,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param registry_module: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#registry_module NoCodeModule#registry_module}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#enabled NoCodeModule#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#id NoCodeModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#organization NoCodeModule#organization}.
-        :param variable_options: variable_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#variable_options NoCodeModule#variable_options}
-        :param version_pin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#version_pin NoCodeModule#version_pin}.
+        :param registry_module: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#registry_module NoCodeModule#registry_module}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#enabled NoCodeModule#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#id NoCodeModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#organization NoCodeModule#organization}.
+        :param variable_options: variable_options block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#variable_options NoCodeModule#variable_options}
+        :param version_pin: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#version_pin NoCodeModule#version_pin}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__173525379707bfb387d5e41e76baddbd8bba09d6d3594b4865da84da022cb567)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -391,57 +391,57 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def registry_module(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#registry_module NoCodeModule#registry_module}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#registry_module NoCodeModule#registry_module}.'''
         result = self._values.get("registry_module")
         assert result is not None, "Required property 'registry_module' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#enabled NoCodeModule#enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#enabled NoCodeModule#enabled}.'''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#id NoCodeModule#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#id NoCodeModule#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#organization NoCodeModule#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#organization NoCodeModule#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def variable_options(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["NoCodeModuleVariableOptions"]]]:
         '''variable_options block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#variable_options NoCodeModule#variable_options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#variable_options NoCodeModule#variable_options}
         '''
         result = self._values.get("variable_options")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["NoCodeModuleVariableOptions"]]], result)
 
     @builtins.property
     def version_pin(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#version_pin NoCodeModule#version_pin}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#version_pin NoCodeModule#version_pin}.'''
         result = self._values.get("version_pin")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -463,46 +463,46 @@
         self,
         *,
         name: builtins.str,
         options: typing.Sequence[builtins.str],
         type: builtins.str,
     ) -> None:
         '''
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#name NoCodeModule#name}.
-        :param options: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#options NoCodeModule#options}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#type NoCodeModule#type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#name NoCodeModule#name}.
+        :param options: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#options NoCodeModule#options}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#type NoCodeModule#type}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1c5ed47881a2e7c72bece878eff42b97e9a4dbcf44def461cf4b73d103b2f6fd)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument options", value=options, expected_type=type_hints["options"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
             "options": options,
             "type": type,
         }
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#name NoCodeModule#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#name NoCodeModule#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def options(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#options NoCodeModule#options}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#options NoCodeModule#options}.'''
         result = self._values.get("options")
         assert result is not None, "Required property 'options' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/no_code_module#type NoCodeModule#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/no_code_module#type NoCodeModule#type}.'''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/notification_configuration/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/notification_configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_notification_configuration`
 
-Refer to the Terraform Registory for docs: [`tfe_notification_configuration`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration).
+Refer to the Terraform Registory for docs: [`tfe_notification_configuration`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class NotificationConfiguration(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.notificationConfiguration.NotificationConfiguration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration tfe_notification_configuration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration tfe_notification_configuration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         destination_type: builtins.str,
@@ -47,28 +47,28 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration tfe_notification_configuration} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration tfe_notification_configuration} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param destination_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#destination_type NotificationConfiguration#destination_type}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#name NotificationConfiguration#name}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#workspace_id NotificationConfiguration#workspace_id}.
-        :param email_addresses: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#email_addresses NotificationConfiguration#email_addresses}.
-        :param email_user_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#email_user_ids NotificationConfiguration#email_user_ids}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#enabled NotificationConfiguration#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#id NotificationConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#token NotificationConfiguration#token}.
-        :param triggers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#triggers NotificationConfiguration#triggers}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#url NotificationConfiguration#url}.
+        :param destination_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#destination_type NotificationConfiguration#destination_type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#name NotificationConfiguration#name}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#workspace_id NotificationConfiguration#workspace_id}.
+        :param email_addresses: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#email_addresses NotificationConfiguration#email_addresses}.
+        :param email_user_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#email_user_ids NotificationConfiguration#email_user_ids}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#enabled NotificationConfiguration#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#id NotificationConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#token NotificationConfiguration#token}.
+        :param triggers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#triggers NotificationConfiguration#triggers}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#url NotificationConfiguration#url}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -361,24 +361,24 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param destination_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#destination_type NotificationConfiguration#destination_type}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#name NotificationConfiguration#name}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#workspace_id NotificationConfiguration#workspace_id}.
-        :param email_addresses: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#email_addresses NotificationConfiguration#email_addresses}.
-        :param email_user_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#email_user_ids NotificationConfiguration#email_user_ids}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#enabled NotificationConfiguration#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#id NotificationConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#token NotificationConfiguration#token}.
-        :param triggers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#triggers NotificationConfiguration#triggers}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#url NotificationConfiguration#url}.
+        :param destination_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#destination_type NotificationConfiguration#destination_type}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#name NotificationConfiguration#name}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#workspace_id NotificationConfiguration#workspace_id}.
+        :param email_addresses: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#email_addresses NotificationConfiguration#email_addresses}.
+        :param email_user_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#email_user_ids NotificationConfiguration#email_user_ids}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#enabled NotificationConfiguration#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#id NotificationConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#token NotificationConfiguration#token}.
+        :param triggers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#triggers NotificationConfiguration#triggers}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#url NotificationConfiguration#url}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf60f4f2785c2ba3015ff934a101f122826a3e0bb648979f71afdde2cff691c4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -493,78 +493,78 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def destination_type(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#destination_type NotificationConfiguration#destination_type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#destination_type NotificationConfiguration#destination_type}.'''
         result = self._values.get("destination_type")
         assert result is not None, "Required property 'destination_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#name NotificationConfiguration#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#name NotificationConfiguration#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#workspace_id NotificationConfiguration#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#workspace_id NotificationConfiguration#workspace_id}.'''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def email_addresses(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#email_addresses NotificationConfiguration#email_addresses}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#email_addresses NotificationConfiguration#email_addresses}.'''
         result = self._values.get("email_addresses")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def email_user_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#email_user_ids NotificationConfiguration#email_user_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#email_user_ids NotificationConfiguration#email_user_ids}.'''
         result = self._values.get("email_user_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#enabled NotificationConfiguration#enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#enabled NotificationConfiguration#enabled}.'''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#id NotificationConfiguration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#id NotificationConfiguration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#token NotificationConfiguration#token}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#token NotificationConfiguration#token}.'''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def triggers(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#triggers NotificationConfiguration#triggers}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#triggers NotificationConfiguration#triggers}.'''
         result = self._values.get("triggers")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/notification_configuration#url NotificationConfiguration#url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/notification_configuration#url NotificationConfiguration#url}.'''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/oauth_client/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/oauth_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_oauth_client`
 
-Refer to the Terraform Registory for docs: [`tfe_oauth_client`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client).
+Refer to the Terraform Registory for docs: [`tfe_oauth_client`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class OauthClient(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.oauthClient.OauthClient",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client tfe_oauth_client}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client tfe_oauth_client}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         api_url: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client tfe_oauth_client} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client tfe_oauth_client} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param api_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#api_url OauthClient#api_url}.
-        :param http_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#http_url OauthClient#http_url}.
-        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#service_provider OauthClient#service_provider}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#id OauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#key OauthClient#key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#name OauthClient#name}.
-        :param oauth_token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#oauth_token OauthClient#oauth_token}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#organization OauthClient#organization}.
-        :param private_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#private_key OauthClient#private_key}.
-        :param rsa_public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#rsa_public_key OauthClient#rsa_public_key}.
-        :param secret: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#secret OauthClient#secret}.
+        :param api_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#api_url OauthClient#api_url}.
+        :param http_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#http_url OauthClient#http_url}.
+        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#service_provider OauthClient#service_provider}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#id OauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#key OauthClient#key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#name OauthClient#name}.
+        :param oauth_token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#oauth_token OauthClient#oauth_token}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#organization OauthClient#organization}.
+        :param private_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#private_key OauthClient#private_key}.
+        :param rsa_public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#rsa_public_key OauthClient#rsa_public_key}.
+        :param secret: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#secret OauthClient#secret}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -387,25 +387,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param api_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#api_url OauthClient#api_url}.
-        :param http_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#http_url OauthClient#http_url}.
-        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#service_provider OauthClient#service_provider}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#id OauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#key OauthClient#key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#name OauthClient#name}.
-        :param oauth_token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#oauth_token OauthClient#oauth_token}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#organization OauthClient#organization}.
-        :param private_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#private_key OauthClient#private_key}.
-        :param rsa_public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#rsa_public_key OauthClient#rsa_public_key}.
-        :param secret: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#secret OauthClient#secret}.
+        :param api_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#api_url OauthClient#api_url}.
+        :param http_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#http_url OauthClient#http_url}.
+        :param service_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#service_provider OauthClient#service_provider}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#id OauthClient#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#key OauthClient#key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#name OauthClient#name}.
+        :param oauth_token: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#oauth_token OauthClient#oauth_token}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#organization OauthClient#organization}.
+        :param private_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#private_key OauthClient#private_key}.
+        :param rsa_public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#rsa_public_key OauthClient#rsa_public_key}.
+        :param secret: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#secret OauthClient#secret}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5ddcac0b50ee416c007705fb8ea4aec4ecaa5ad576501b7c4833579a95a88e02)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -523,82 +523,82 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def api_url(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#api_url OauthClient#api_url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#api_url OauthClient#api_url}.'''
         result = self._values.get("api_url")
         assert result is not None, "Required property 'api_url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def http_url(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#http_url OauthClient#http_url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#http_url OauthClient#http_url}.'''
         result = self._values.get("http_url")
         assert result is not None, "Required property 'http_url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def service_provider(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#service_provider OauthClient#service_provider}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#service_provider OauthClient#service_provider}.'''
         result = self._values.get("service_provider")
         assert result is not None, "Required property 'service_provider' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#id OauthClient#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#id OauthClient#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def key(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#key OauthClient#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#key OauthClient#key}.'''
         result = self._values.get("key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#name OauthClient#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#name OauthClient#name}.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def oauth_token(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#oauth_token OauthClient#oauth_token}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#oauth_token OauthClient#oauth_token}.'''
         result = self._values.get("oauth_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#organization OauthClient#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#organization OauthClient#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def private_key(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#private_key OauthClient#private_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#private_key OauthClient#private_key}.'''
         result = self._values.get("private_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rsa_public_key(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#rsa_public_key OauthClient#rsa_public_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#rsa_public_key OauthClient#rsa_public_key}.'''
         result = self._values.get("rsa_public_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secret(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/oauth_client#secret OauthClient#secret}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/oauth_client#secret OauthClient#secret}.'''
         result = self._values.get("secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_organization`
 
-Refer to the Terraform Registory for docs: [`tfe_organization`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization).
+Refer to the Terraform Registory for docs: [`tfe_organization`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Organization(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.organization.Organization",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization tfe_organization}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization tfe_organization}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization tfe_organization} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization tfe_organization} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#email Organization#email}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#name Organization#name}.
-        :param allow_force_delete_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#allow_force_delete_workspaces Organization#allow_force_delete_workspaces}.
-        :param assessments_enforced: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#assessments_enforced Organization#assessments_enforced}.
-        :param collaborator_auth_policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#collaborator_auth_policy Organization#collaborator_auth_policy}.
-        :param cost_estimation_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#cost_estimation_enabled Organization#cost_estimation_enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#id Organization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param owners_team_saml_role_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#owners_team_saml_role_id Organization#owners_team_saml_role_id}.
-        :param send_passing_statuses_for_untriggered_speculative_plans: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#send_passing_statuses_for_untriggered_speculative_plans Organization#send_passing_statuses_for_untriggered_speculative_plans}.
-        :param session_remember_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#session_remember_minutes Organization#session_remember_minutes}.
-        :param session_timeout_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#session_timeout_minutes Organization#session_timeout_minutes}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#email Organization#email}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#name Organization#name}.
+        :param allow_force_delete_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#allow_force_delete_workspaces Organization#allow_force_delete_workspaces}.
+        :param assessments_enforced: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#assessments_enforced Organization#assessments_enforced}.
+        :param collaborator_auth_policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#collaborator_auth_policy Organization#collaborator_auth_policy}.
+        :param cost_estimation_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#cost_estimation_enabled Organization#cost_estimation_enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#id Organization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param owners_team_saml_role_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#owners_team_saml_role_id Organization#owners_team_saml_role_id}.
+        :param send_passing_statuses_for_untriggered_speculative_plans: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#send_passing_statuses_for_untriggered_speculative_plans Organization#send_passing_statuses_for_untriggered_speculative_plans}.
+        :param session_remember_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#session_remember_minutes Organization#session_remember_minutes}.
+        :param session_timeout_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#session_timeout_minutes Organization#session_timeout_minutes}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -419,25 +419,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#email Organization#email}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#name Organization#name}.
-        :param allow_force_delete_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#allow_force_delete_workspaces Organization#allow_force_delete_workspaces}.
-        :param assessments_enforced: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#assessments_enforced Organization#assessments_enforced}.
-        :param collaborator_auth_policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#collaborator_auth_policy Organization#collaborator_auth_policy}.
-        :param cost_estimation_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#cost_estimation_enabled Organization#cost_estimation_enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#id Organization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param owners_team_saml_role_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#owners_team_saml_role_id Organization#owners_team_saml_role_id}.
-        :param send_passing_statuses_for_untriggered_speculative_plans: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#send_passing_statuses_for_untriggered_speculative_plans Organization#send_passing_statuses_for_untriggered_speculative_plans}.
-        :param session_remember_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#session_remember_minutes Organization#session_remember_minutes}.
-        :param session_timeout_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#session_timeout_minutes Organization#session_timeout_minutes}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#email Organization#email}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#name Organization#name}.
+        :param allow_force_delete_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#allow_force_delete_workspaces Organization#allow_force_delete_workspaces}.
+        :param assessments_enforced: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#assessments_enforced Organization#assessments_enforced}.
+        :param collaborator_auth_policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#collaborator_auth_policy Organization#collaborator_auth_policy}.
+        :param cost_estimation_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#cost_estimation_enabled Organization#cost_estimation_enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#id Organization#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param owners_team_saml_role_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#owners_team_saml_role_id Organization#owners_team_saml_role_id}.
+        :param send_passing_statuses_for_untriggered_speculative_plans: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#send_passing_statuses_for_untriggered_speculative_plans Organization#send_passing_statuses_for_untriggered_speculative_plans}.
+        :param session_remember_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#session_remember_minutes Organization#session_remember_minutes}.
+        :param session_timeout_minutes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#session_timeout_minutes Organization#session_timeout_minutes}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f91fe2dabc5e7b94e8a3c960d4e164fa7bfc7284e306e9061f5b602bddd44d73)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -556,89 +556,89 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#email Organization#email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#email Organization#email}.'''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#name Organization#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#name Organization#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def allow_force_delete_workspaces(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#allow_force_delete_workspaces Organization#allow_force_delete_workspaces}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#allow_force_delete_workspaces Organization#allow_force_delete_workspaces}.'''
         result = self._values.get("allow_force_delete_workspaces")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def assessments_enforced(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#assessments_enforced Organization#assessments_enforced}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#assessments_enforced Organization#assessments_enforced}.'''
         result = self._values.get("assessments_enforced")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def collaborator_auth_policy(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#collaborator_auth_policy Organization#collaborator_auth_policy}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#collaborator_auth_policy Organization#collaborator_auth_policy}.'''
         result = self._values.get("collaborator_auth_policy")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cost_estimation_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#cost_estimation_enabled Organization#cost_estimation_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#cost_estimation_enabled Organization#cost_estimation_enabled}.'''
         result = self._values.get("cost_estimation_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#id Organization#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#id Organization#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def owners_team_saml_role_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#owners_team_saml_role_id Organization#owners_team_saml_role_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#owners_team_saml_role_id Organization#owners_team_saml_role_id}.'''
         result = self._values.get("owners_team_saml_role_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def send_passing_statuses_for_untriggered_speculative_plans(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#send_passing_statuses_for_untriggered_speculative_plans Organization#send_passing_statuses_for_untriggered_speculative_plans}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#send_passing_statuses_for_untriggered_speculative_plans Organization#send_passing_statuses_for_untriggered_speculative_plans}.'''
         result = self._values.get("send_passing_statuses_for_untriggered_speculative_plans")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def session_remember_minutes(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#session_remember_minutes Organization#session_remember_minutes}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#session_remember_minutes Organization#session_remember_minutes}.'''
         result = self._values.get("session_remember_minutes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def session_timeout_minutes(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization#session_timeout_minutes Organization#session_timeout_minutes}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization#session_timeout_minutes Organization#session_timeout_minutes}.'''
         result = self._values.get("session_timeout_minutes")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_membership/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_membership/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_organization_membership`
 
-Refer to the Terraform Registory for docs: [`tfe_organization_membership`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership).
+Refer to the Terraform Registory for docs: [`tfe_organization_membership`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class OrganizationMembership(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.organizationMembership.OrganizationMembership",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership tfe_organization_membership}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership tfe_organization_membership}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership tfe_organization_membership} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership tfe_organization_membership} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#email OrganizationMembership#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#id OrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#organization OrganizationMembership#organization}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#email OrganizationMembership#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#id OrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#organization OrganizationMembership#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -192,17 +192,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#email OrganizationMembership#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#id OrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#organization OrganizationMembership#organization}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#email OrganizationMembership#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#id OrganizationMembership#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#organization OrganizationMembership#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cd3191f34bf5dfc6aa8f1d7ce9efc4bef8e99b4f8d8ff9cde9dc8b908a74c8df)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -298,32 +298,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#email OrganizationMembership#email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#email OrganizationMembership#email}.'''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#id OrganizationMembership#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#id OrganizationMembership#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_membership#organization OrganizationMembership#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_membership#organization OrganizationMembership#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_module_sharing/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_module_sharing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_organization_module_sharing`
 
-Refer to the Terraform Registory for docs: [`tfe_organization_module_sharing`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing).
+Refer to the Terraform Registory for docs: [`tfe_organization_module_sharing`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class OrganizationModuleSharing(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.organizationModuleSharing.OrganizationModuleSharing",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing tfe_organization_module_sharing}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing tfe_organization_module_sharing}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         module_consumers: typing.Sequence[builtins.str],
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing tfe_organization_module_sharing} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing tfe_organization_module_sharing} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param module_consumers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#module_consumers OrganizationModuleSharing#module_consumers}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#id OrganizationModuleSharing#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#organization OrganizationModuleSharing#organization}.
+        :param module_consumers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#module_consumers OrganizationModuleSharing#module_consumers}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#id OrganizationModuleSharing#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#organization OrganizationModuleSharing#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -182,17 +182,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param module_consumers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#module_consumers OrganizationModuleSharing#module_consumers}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#id OrganizationModuleSharing#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#organization OrganizationModuleSharing#organization}.
+        :param module_consumers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#module_consumers OrganizationModuleSharing#module_consumers}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#id OrganizationModuleSharing#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#organization OrganizationModuleSharing#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__93fb459133af36d2fb87fd2876ace00b1c11bff4ed5874c602caf5da9e4716ef)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,32 +288,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def module_consumers(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#module_consumers OrganizationModuleSharing#module_consumers}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#module_consumers OrganizationModuleSharing#module_consumers}.'''
         result = self._values.get("module_consumers")
         assert result is not None, "Required property 'module_consumers' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#id OrganizationModuleSharing#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#id OrganizationModuleSharing#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_module_sharing#organization OrganizationModuleSharing#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_module_sharing#organization OrganizationModuleSharing#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_run_task/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_run_task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_organization_run_task`
 
-Refer to the Terraform Registory for docs: [`tfe_organization_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task).
+Refer to the Terraform Registory for docs: [`tfe_organization_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class OrganizationRunTask(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.organizationRunTask.OrganizationRunTask",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task tfe_organization_run_task}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task tfe_organization_run_task}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task tfe_organization_run_task} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task tfe_organization_run_task} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#name OrganizationRunTask#name}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#url OrganizationRunTask#url}.
-        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#category OrganizationRunTask#category}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#description OrganizationRunTask#description}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#enabled OrganizationRunTask#enabled}.
-        :param hmac_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#hmac_key OrganizationRunTask#hmac_key}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#id OrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#organization OrganizationRunTask#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#name OrganizationRunTask#name}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#url OrganizationRunTask#url}.
+        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#category OrganizationRunTask#category}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#description OrganizationRunTask#description}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#enabled OrganizationRunTask#enabled}.
+        :param hmac_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#hmac_key OrganizationRunTask#hmac_key}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#id OrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#organization OrganizationRunTask#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -313,22 +313,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#name OrganizationRunTask#name}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#url OrganizationRunTask#url}.
-        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#category OrganizationRunTask#category}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#description OrganizationRunTask#description}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#enabled OrganizationRunTask#enabled}.
-        :param hmac_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#hmac_key OrganizationRunTask#hmac_key}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#id OrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#organization OrganizationRunTask#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#name OrganizationRunTask#name}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#url OrganizationRunTask#url}.
+        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#category OrganizationRunTask#category}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#description OrganizationRunTask#description}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#enabled OrganizationRunTask#enabled}.
+        :param hmac_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#hmac_key OrganizationRunTask#hmac_key}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#id OrganizationRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#organization OrganizationRunTask#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8ed911870f063b52dd52c628c0bd9571851697fff7152f5af690ca6cd510bded)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -438,65 +438,65 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#name OrganizationRunTask#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#name OrganizationRunTask#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def url(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#url OrganizationRunTask#url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#url OrganizationRunTask#url}.'''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def category(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#category OrganizationRunTask#category}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#category OrganizationRunTask#category}.'''
         result = self._values.get("category")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#description OrganizationRunTask#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#description OrganizationRunTask#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#enabled OrganizationRunTask#enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#enabled OrganizationRunTask#enabled}.'''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def hmac_key(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#hmac_key OrganizationRunTask#hmac_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#hmac_key OrganizationRunTask#hmac_key}.'''
         result = self._values.get("hmac_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#id OrganizationRunTask#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#id OrganizationRunTask#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_run_task#organization OrganizationRunTask#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_run_task#organization OrganizationRunTask#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/organization_token/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/organization_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_organization_token`
 
-Refer to the Terraform Registory for docs: [`tfe_organization_token`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token).
+Refer to the Terraform Registory for docs: [`tfe_organization_token`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class OrganizationToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.organizationToken.OrganizationToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token tfe_organization_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token tfe_organization_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         force_regenerate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token tfe_organization_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token tfe_organization_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#force_regenerate OrganizationToken#force_regenerate}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#id OrganizationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#organization OrganizationToken#organization}.
+        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#force_regenerate OrganizationToken#force_regenerate}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#id OrganizationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#organization OrganizationToken#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -198,17 +198,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#force_regenerate OrganizationToken#force_regenerate}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#id OrganizationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#organization OrganizationToken#organization}.
+        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#force_regenerate OrganizationToken#force_regenerate}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#id OrganizationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#organization OrganizationToken#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2b9bb754d7b34de37ecf2f40a309fded3a26148291845726d246cbb7555425b6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -306,31 +306,31 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def force_regenerate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#force_regenerate OrganizationToken#force_regenerate}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#force_regenerate OrganizationToken#force_regenerate}.'''
         result = self._values.get("force_regenerate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#id OrganizationToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#id OrganizationToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/organization_token#organization OrganizationToken#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/organization_token#organization OrganizationToken#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_policy`
 
-Refer to the Terraform Registory for docs: [`tfe_policy`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy).
+Refer to the Terraform Registory for docs: [`tfe_policy`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Policy(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.policy.Policy",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy tfe_policy}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy tfe_policy}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy tfe_policy} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy tfe_policy} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#name Policy#name}
-        :param policy: Text of a valid Sentinel or OPA policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#policy Policy#policy}
-        :param description: Text describing the policy's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#description Policy#description}
-        :param enforce_mode: The enforcement configuration of the policy. For Sentinel, valid values are ``hard-mandatory``, ``soft-mandatory`` and ``advisory``. For OPA, Valid values are ``mandatory` and `advisory`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#enforce_mode Policy#enforce_mode}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#id Policy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#kind Policy#kind}
-        :param organization: Name of the organization that this policy belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#organization Policy#organization}
-        :param query: The OPA query to run. Required for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#query Policy#query}
+        :param name: The name of the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#name Policy#name}
+        :param policy: Text of a valid Sentinel or OPA policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#policy Policy#policy}
+        :param description: Text describing the policy's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#description Policy#description}
+        :param enforce_mode: The enforcement configuration of the policy. For Sentinel, valid values are ``hard-mandatory``, ``soft-mandatory`` and ``advisory``. For OPA, Valid values are ``mandatory` and `advisory`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#enforce_mode Policy#enforce_mode}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#id Policy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#kind Policy#kind}
+        :param organization: Name of the organization that this policy belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#organization Policy#organization}
+        :param query: The OPA query to run. Required for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#query Policy#query}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -308,22 +308,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#name Policy#name}
-        :param policy: Text of a valid Sentinel or OPA policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#policy Policy#policy}
-        :param description: Text describing the policy's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#description Policy#description}
-        :param enforce_mode: The enforcement configuration of the policy. For Sentinel, valid values are ``hard-mandatory``, ``soft-mandatory`` and ``advisory``. For OPA, Valid values are ``mandatory` and `advisory`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#enforce_mode Policy#enforce_mode}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#id Policy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#kind Policy#kind}
-        :param organization: Name of the organization that this policy belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#organization Policy#organization}
-        :param query: The OPA query to run. Required for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#query Policy#query}
+        :param name: The name of the policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#name Policy#name}
+        :param policy: Text of a valid Sentinel or OPA policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#policy Policy#policy}
+        :param description: Text describing the policy's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#description Policy#description}
+        :param enforce_mode: The enforcement configuration of the policy. For Sentinel, valid values are ``hard-mandatory``, ``soft-mandatory`` and ``advisory``. For OPA, Valid values are ``mandatory` and `advisory`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#enforce_mode Policy#enforce_mode}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#id Policy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kind: The policy-as-code framework for the policy. Valid values are sentinel and opa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#kind Policy#kind}
+        :param organization: Name of the organization that this policy belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#organization Policy#organization}
+        :param query: The OPA query to run. Required for OPA policies. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#query Policy#query}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e015e07ca315f3999c160f7214c3fe3a64c72965091b1e1e48001f32764d57e8)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -435,83 +435,83 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the policy.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#name Policy#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#name Policy#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(self) -> builtins.str:
         '''Text of a valid Sentinel or OPA policy.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#policy Policy#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#policy Policy#policy}
         '''
         result = self._values.get("policy")
         assert result is not None, "Required property 'policy' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Text describing the policy's purpose.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#description Policy#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#description Policy#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enforce_mode(self) -> typing.Optional[builtins.str]:
         '''The enforcement configuration of the policy.
 
         For Sentinel, valid values are ``hard-mandatory``, ``soft-mandatory`` and ``advisory``. For OPA, Valid values are ``mandatory`` and ``advisory``
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#enforce_mode Policy#enforce_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#enforce_mode Policy#enforce_mode}
         '''
         result = self._values.get("enforce_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#id Policy#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#id Policy#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def kind(self) -> typing.Optional[builtins.str]:
         '''The policy-as-code framework for the policy. Valid values are sentinel and opa.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#kind Policy#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#kind Policy#kind}
         '''
         result = self._values.get("kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
         '''Name of the organization that this policy belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#organization Policy#organization}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#organization Policy#organization}
         '''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def query(self) -> typing.Optional[builtins.str]:
         '''The OPA query to run. Required for OPA policies.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy#query Policy#query}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy#query Policy#query}
         '''
         result = self._values.get("query")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_policy_set`
 
-Refer to the Terraform Registory for docs: [`tfe_policy_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set).
+Refer to the Terraform Registory for docs: [`tfe_policy_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class PolicySet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.policySet.PolicySet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set tfe_policy_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set tfe_policy_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -49,30 +49,30 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set tfe_policy_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set tfe_policy_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#name PolicySet#name}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#description PolicySet#description}.
-        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#global PolicySet#global}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#id PolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kind: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#kind PolicySet#kind}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#organization PolicySet#organization}.
-        :param overridable: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#overridable PolicySet#overridable}.
-        :param policies_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#policies_path PolicySet#policies_path}.
-        :param policy_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#policy_ids PolicySet#policy_ids}.
-        :param slug: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#slug PolicySet#slug}.
-        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#vcs_repo PolicySet#vcs_repo}
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#workspace_ids PolicySet#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#name PolicySet#name}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#description PolicySet#description}.
+        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#global PolicySet#global}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#id PolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kind: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#kind PolicySet#kind}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#organization PolicySet#organization}.
+        :param overridable: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#overridable PolicySet#overridable}.
+        :param policies_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#policies_path PolicySet#policies_path}.
+        :param policy_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#policy_ids PolicySet#policy_ids}.
+        :param slug: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#slug PolicySet#slug}.
+        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#vcs_repo PolicySet#vcs_repo}
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#workspace_ids PolicySet#workspace_ids}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -112,19 +112,19 @@
         identifier: builtins.str,
         branch: typing.Optional[builtins.str] = None,
         github_app_installation_id: typing.Optional[builtins.str] = None,
         ingress_submodules: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         oauth_token_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#identifier PolicySet#identifier}.
-        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#branch PolicySet#branch}.
-        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#github_app_installation_id PolicySet#github_app_installation_id}.
-        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#ingress_submodules PolicySet#ingress_submodules}.
-        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#oauth_token_id PolicySet#oauth_token_id}.
+        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#identifier PolicySet#identifier}.
+        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#branch PolicySet#branch}.
+        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#github_app_installation_id PolicySet#github_app_installation_id}.
+        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#ingress_submodules PolicySet#ingress_submodules}.
+        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#oauth_token_id PolicySet#oauth_token_id}.
         '''
         value = PolicySetVcsRepo(
             identifier=identifier,
             branch=branch,
             github_app_installation_id=github_app_installation_id,
             ingress_submodules=ingress_submodules,
             oauth_token_id=oauth_token_id,
@@ -446,26 +446,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#name PolicySet#name}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#description PolicySet#description}.
-        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#global PolicySet#global}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#id PolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param kind: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#kind PolicySet#kind}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#organization PolicySet#organization}.
-        :param overridable: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#overridable PolicySet#overridable}.
-        :param policies_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#policies_path PolicySet#policies_path}.
-        :param policy_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#policy_ids PolicySet#policy_ids}.
-        :param slug: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#slug PolicySet#slug}.
-        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#vcs_repo PolicySet#vcs_repo}
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#workspace_ids PolicySet#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#name PolicySet#name}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#description PolicySet#description}.
+        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#global PolicySet#global}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#id PolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param kind: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#kind PolicySet#kind}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#organization PolicySet#organization}.
+        :param overridable: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#overridable PolicySet#overridable}.
+        :param policies_path: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#policies_path PolicySet#policies_path}.
+        :param policy_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#policy_ids PolicySet#policy_ids}.
+        :param slug: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#slug PolicySet#slug}.
+        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#vcs_repo PolicySet#vcs_repo}
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#workspace_ids PolicySet#workspace_ids}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(vcs_repo, dict):
             vcs_repo = PolicySetVcsRepo(**vcs_repo)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__34272394142fda496142ddd73d885bb2e530b79a46b0d1167588d25bbbef158a)
@@ -590,93 +590,93 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#name PolicySet#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#name PolicySet#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#description PolicySet#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#description PolicySet#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def global_(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#global PolicySet#global}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#global PolicySet#global}.'''
         result = self._values.get("global_")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#id PolicySet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#id PolicySet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def kind(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#kind PolicySet#kind}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#kind PolicySet#kind}.'''
         result = self._values.get("kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#organization PolicySet#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#organization PolicySet#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def overridable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#overridable PolicySet#overridable}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#overridable PolicySet#overridable}.'''
         result = self._values.get("overridable")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def policies_path(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#policies_path PolicySet#policies_path}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#policies_path PolicySet#policies_path}.'''
         result = self._values.get("policies_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policy_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#policy_ids PolicySet#policy_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#policy_ids PolicySet#policy_ids}.'''
         result = self._values.get("policy_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def slug(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#slug PolicySet#slug}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#slug PolicySet#slug}.'''
         result = self._values.get("slug")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def vcs_repo(self) -> typing.Optional["PolicySetVcsRepo"]:
         '''vcs_repo block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#vcs_repo PolicySet#vcs_repo}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#vcs_repo PolicySet#vcs_repo}
         '''
         result = self._values.get("vcs_repo")
         return typing.cast(typing.Optional["PolicySetVcsRepo"], result)
 
     @builtins.property
     def workspace_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#workspace_ids PolicySet#workspace_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#workspace_ids PolicySet#workspace_ids}.'''
         result = self._values.get("workspace_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -706,19 +706,19 @@
         identifier: builtins.str,
         branch: typing.Optional[builtins.str] = None,
         github_app_installation_id: typing.Optional[builtins.str] = None,
         ingress_submodules: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         oauth_token_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#identifier PolicySet#identifier}.
-        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#branch PolicySet#branch}.
-        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#github_app_installation_id PolicySet#github_app_installation_id}.
-        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#ingress_submodules PolicySet#ingress_submodules}.
-        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#oauth_token_id PolicySet#oauth_token_id}.
+        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#identifier PolicySet#identifier}.
+        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#branch PolicySet#branch}.
+        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#github_app_installation_id PolicySet#github_app_installation_id}.
+        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#ingress_submodules PolicySet#ingress_submodules}.
+        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#oauth_token_id PolicySet#oauth_token_id}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c142443d7f869111fd8d8055bce18abd2a6c6fd69d0edd53c6a917bf64236e3a)
             check_type(argname="argument identifier", value=identifier, expected_type=type_hints["identifier"])
             check_type(argname="argument branch", value=branch, expected_type=type_hints["branch"])
             check_type(argname="argument github_app_installation_id", value=github_app_installation_id, expected_type=type_hints["github_app_installation_id"])
             check_type(argname="argument ingress_submodules", value=ingress_submodules, expected_type=type_hints["ingress_submodules"])
@@ -733,42 +733,42 @@
         if ingress_submodules is not None:
             self._values["ingress_submodules"] = ingress_submodules
         if oauth_token_id is not None:
             self._values["oauth_token_id"] = oauth_token_id
 
     @builtins.property
     def identifier(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#identifier PolicySet#identifier}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#identifier PolicySet#identifier}.'''
         result = self._values.get("identifier")
         assert result is not None, "Required property 'identifier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def branch(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#branch PolicySet#branch}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#branch PolicySet#branch}.'''
         result = self._values.get("branch")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def github_app_installation_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#github_app_installation_id PolicySet#github_app_installation_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#github_app_installation_id PolicySet#github_app_installation_id}.'''
         result = self._values.get("github_app_installation_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ingress_submodules(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#ingress_submodules PolicySet#ingress_submodules}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#ingress_submodules PolicySet#ingress_submodules}.'''
         result = self._values.get("ingress_submodules")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def oauth_token_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set#oauth_token_id PolicySet#oauth_token_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set#oauth_token_id PolicySet#oauth_token_id}.'''
         result = self._values.get("oauth_token_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/policy_set_parameter/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/policy_set_parameter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_policy_set_parameter`
 
-Refer to the Terraform Registory for docs: [`tfe_policy_set_parameter`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter).
+Refer to the Terraform Registory for docs: [`tfe_policy_set_parameter`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class PolicySetParameter(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.policySetParameter.PolicySetParameter",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter tfe_policy_set_parameter}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter tfe_policy_set_parameter}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter tfe_policy_set_parameter} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter tfe_policy_set_parameter} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#key PolicySetParameter#key}.
-        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#policy_set_id PolicySetParameter#policy_set_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#id PolicySetParameter#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#sensitive PolicySetParameter#sensitive}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#value PolicySetParameter#value}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#key PolicySetParameter#key}.
+        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#policy_set_id PolicySetParameter#policy_set_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#id PolicySetParameter#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#sensitive PolicySetParameter#sensitive}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#value PolicySetParameter#value}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -235,19 +235,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#key PolicySetParameter#key}.
-        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#policy_set_id PolicySetParameter#policy_set_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#id PolicySetParameter#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#sensitive PolicySetParameter#sensitive}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#value PolicySetParameter#value}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#key PolicySetParameter#key}.
+        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#policy_set_id PolicySetParameter#policy_set_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#id PolicySetParameter#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#sensitive PolicySetParameter#sensitive}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#value PolicySetParameter#value}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cce93162e7670776e7f1ece03294940b044b90f96929cdf0542a703de4381eea)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,47 +348,47 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#key PolicySetParameter#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#key PolicySetParameter#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy_set_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#policy_set_id PolicySetParameter#policy_set_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#policy_set_id PolicySetParameter#policy_set_id}.'''
         result = self._values.get("policy_set_id")
         assert result is not None, "Required property 'policy_set_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#id PolicySetParameter#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#id PolicySetParameter#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sensitive(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#sensitive PolicySetParameter#sensitive}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#sensitive PolicySetParameter#sensitive}.'''
         result = self._values.get("sensitive")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/policy_set_parameter#value PolicySetParameter#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/policy_set_parameter#value PolicySetParameter#value}.'''
         result = self._values.get("value")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/project/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_project`
 
-Refer to the Terraform Registory for docs: [`tfe_project`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project).
+Refer to the Terraform Registory for docs: [`tfe_project`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Project(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.project.Project",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project tfe_project}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project tfe_project}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project tfe_project} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project tfe_project} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#name Project#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#organization Project#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#name Project#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#organization Project#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -182,17 +182,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#name Project#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#organization Project#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#name Project#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#organization Project#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__45aa95a81609c5d8572e8640242da14d87ad90af288213139bc7b2e37876495b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,32 +288,32 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#name Project#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#name Project#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#id Project#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#id Project#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project#organization Project#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project#organization Project#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/project_variable_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/project_variable_set/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_project_variable_set`
 
-Refer to the Terraform Registory for docs: [`tfe_project_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set).
+Refer to the Terraform Registory for docs: [`tfe_project_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ProjectVariableSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.projectVariableSet.ProjectVariableSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set tfe_project_variable_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set tfe_project_variable_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         project_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set tfe_project_variable_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set tfe_project_variable_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#project_id ProjectVariableSet#project_id}.
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#variable_set_id ProjectVariableSet#variable_set_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#id ProjectVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#project_id ProjectVariableSet#project_id}.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#variable_set_id ProjectVariableSet#variable_set_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#id ProjectVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#project_id ProjectVariableSet#project_id}.
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#variable_set_id ProjectVariableSet#variable_set_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#id ProjectVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#project_id ProjectVariableSet#project_id}.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#variable_set_id ProjectVariableSet#variable_set_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#id ProjectVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8e56af2075d1f7a803b523bf1e07da7e448c69b8821b97fd4ec44760c77da5ca)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def project_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#project_id ProjectVariableSet#project_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#project_id ProjectVariableSet#project_id}.'''
         result = self._values.get("project_id")
         assert result is not None, "Required property 'project_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variable_set_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#variable_set_id ProjectVariableSet#variable_set_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#variable_set_id ProjectVariableSet#variable_set_id}.'''
         result = self._values.get("variable_set_id")
         assert result is not None, "Required property 'variable_set_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/project_variable_set#id ProjectVariableSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/project_variable_set#id ProjectVariableSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/provider/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`tfe`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs).
+Refer to the Terraform Registory for docs: [`tfe`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,36 +22,36 @@
 
 
 class TfeProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.provider.TfeProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs tfe}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs tfe}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
         hostname: typing.Optional[builtins.str] = None,
         organization: typing.Optional[builtins.str] = None,
         ssl_skip_verify: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs tfe} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs tfe} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#alias TfeProvider#alias}
-        :param hostname: The Terraform Enterprise hostname to connect to. Defaults to app.terraform.io. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#hostname TfeProvider#hostname}
-        :param organization: The organization to apply to a resource if one is not defined on the resource itself. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#organization TfeProvider#organization}
-        :param ssl_skip_verify: Whether or not to skip certificate verifications. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#ssl_skip_verify TfeProvider#ssl_skip_verify}
-        :param token: The token used to authenticate with Terraform Enterprise. We recommend omitting the token which can be set as credentials in the CLI config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#token TfeProvider#token}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#alias TfeProvider#alias}
+        :param hostname: The Terraform Enterprise hostname to connect to. Defaults to app.terraform.io. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#hostname TfeProvider#hostname}
+        :param organization: The organization to apply to a resource if one is not defined on the resource itself. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#organization TfeProvider#organization}
+        :param ssl_skip_verify: Whether or not to skip certificate verifications. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#ssl_skip_verify TfeProvider#ssl_skip_verify}
+        :param token: The token used to authenticate with Terraform Enterprise. We recommend omitting the token which can be set as credentials in the CLI config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#token TfeProvider#token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__049200213ad1b10e27791506b4c753aea6f02c7d91bea2cbed4b36fd3ad22376)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = TfeProviderConfig(
             alias=alias,
@@ -203,19 +203,19 @@
         alias: typing.Optional[builtins.str] = None,
         hostname: typing.Optional[builtins.str] = None,
         organization: typing.Optional[builtins.str] = None,
         ssl_skip_verify: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#alias TfeProvider#alias}
-        :param hostname: The Terraform Enterprise hostname to connect to. Defaults to app.terraform.io. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#hostname TfeProvider#hostname}
-        :param organization: The organization to apply to a resource if one is not defined on the resource itself. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#organization TfeProvider#organization}
-        :param ssl_skip_verify: Whether or not to skip certificate verifications. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#ssl_skip_verify TfeProvider#ssl_skip_verify}
-        :param token: The token used to authenticate with Terraform Enterprise. We recommend omitting the token which can be set as credentials in the CLI config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#token TfeProvider#token}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#alias TfeProvider#alias}
+        :param hostname: The Terraform Enterprise hostname to connect to. Defaults to app.terraform.io. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#hostname TfeProvider#hostname}
+        :param organization: The organization to apply to a resource if one is not defined on the resource itself. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#organization TfeProvider#organization}
+        :param ssl_skip_verify: Whether or not to skip certificate verifications. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#ssl_skip_verify TfeProvider#ssl_skip_verify}
+        :param token: The token used to authenticate with Terraform Enterprise. We recommend omitting the token which can be set as credentials in the CLI config file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#token TfeProvider#token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dccebcf7b481da73a5f7e45a4a4c9de0069b5cc0efcbb5111b7823647cd51cbb)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument hostname", value=hostname, expected_type=type_hints["hostname"])
             check_type(argname="argument organization", value=organization, expected_type=type_hints["organization"])
             check_type(argname="argument ssl_skip_verify", value=ssl_skip_verify, expected_type=type_hints["ssl_skip_verify"])
@@ -232,56 +232,56 @@
         if token is not None:
             self._values["token"] = token
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#alias TfeProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#alias TfeProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def hostname(self) -> typing.Optional[builtins.str]:
         '''The Terraform Enterprise hostname to connect to. Defaults to app.terraform.io.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#hostname TfeProvider#hostname}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#hostname TfeProvider#hostname}
         '''
         result = self._values.get("hostname")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
         '''The organization to apply to a resource if one is not defined on the resource itself.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#organization TfeProvider#organization}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#organization TfeProvider#organization}
         '''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ssl_skip_verify(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to skip certificate verifications.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#ssl_skip_verify TfeProvider#ssl_skip_verify}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#ssl_skip_verify TfeProvider#ssl_skip_verify}
         '''
         result = self._values.get("ssl_skip_verify")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''The token used to authenticate with Terraform Enterprise.
 
         We recommend omitting
         the token which can be set as credentials in the CLI config file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs#token TfeProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs#token TfeProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/registry_module/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/registry_module/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_registry_module`
 
-Refer to the Terraform Registory for docs: [`tfe_registry_module`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module).
+Refer to the Terraform Registory for docs: [`tfe_registry_module`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class RegistryModule(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.registryModule.RegistryModule",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module tfe_registry_module}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module tfe_registry_module}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module tfe_registry_module} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module tfe_registry_module} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#id RegistryModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param module_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#module_provider RegistryModule#module_provider}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#name RegistryModule#name}.
-        :param namespace: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#namespace RegistryModule#namespace}.
-        :param no_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#no_code RegistryModule#no_code}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#organization RegistryModule#organization}.
-        :param registry_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#registry_name RegistryModule#registry_name}.
-        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#vcs_repo RegistryModule#vcs_repo}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#id RegistryModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param module_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#module_provider RegistryModule#module_provider}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#name RegistryModule#name}.
+        :param namespace: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#namespace RegistryModule#namespace}.
+        :param no_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#no_code RegistryModule#no_code}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#organization RegistryModule#organization}.
+        :param registry_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#registry_name RegistryModule#registry_name}.
+        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#vcs_repo RegistryModule#vcs_repo}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,18 +99,18 @@
         *,
         display_identifier: builtins.str,
         identifier: builtins.str,
         github_app_installation_id: typing.Optional[builtins.str] = None,
         oauth_token_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param display_identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#display_identifier RegistryModule#display_identifier}.
-        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#identifier RegistryModule#identifier}.
-        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#github_app_installation_id RegistryModule#github_app_installation_id}.
-        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#oauth_token_id RegistryModule#oauth_token_id}.
+        :param display_identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#display_identifier RegistryModule#display_identifier}.
+        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#identifier RegistryModule#identifier}.
+        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#github_app_installation_id RegistryModule#github_app_installation_id}.
+        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#oauth_token_id RegistryModule#oauth_token_id}.
         '''
         value = RegistryModuleVcsRepo(
             display_identifier=display_identifier,
             identifier=identifier,
             github_app_installation_id=github_app_installation_id,
             oauth_token_id=oauth_token_id,
         )
@@ -338,22 +338,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#id RegistryModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param module_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#module_provider RegistryModule#module_provider}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#name RegistryModule#name}.
-        :param namespace: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#namespace RegistryModule#namespace}.
-        :param no_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#no_code RegistryModule#no_code}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#organization RegistryModule#organization}.
-        :param registry_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#registry_name RegistryModule#registry_name}.
-        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#vcs_repo RegistryModule#vcs_repo}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#id RegistryModule#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param module_provider: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#module_provider RegistryModule#module_provider}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#name RegistryModule#name}.
+        :param namespace: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#namespace RegistryModule#namespace}.
+        :param no_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#no_code RegistryModule#no_code}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#organization RegistryModule#organization}.
+        :param registry_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#registry_name RegistryModule#registry_name}.
+        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#vcs_repo RegistryModule#vcs_repo}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(vcs_repo, dict):
             vcs_repo = RegistryModuleVcsRepo(**vcs_repo)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf2b8194db05af8ae1bfe2c05ed0797afcb760684cd15ffc160e6b00f2465144)
@@ -466,65 +466,65 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#id RegistryModule#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#id RegistryModule#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def module_provider(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#module_provider RegistryModule#module_provider}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#module_provider RegistryModule#module_provider}.'''
         result = self._values.get("module_provider")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#name RegistryModule#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#name RegistryModule#name}.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#namespace RegistryModule#namespace}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#namespace RegistryModule#namespace}.'''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def no_code(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#no_code RegistryModule#no_code}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#no_code RegistryModule#no_code}.'''
         result = self._values.get("no_code")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#organization RegistryModule#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#organization RegistryModule#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def registry_name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#registry_name RegistryModule#registry_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#registry_name RegistryModule#registry_name}.'''
         result = self._values.get("registry_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def vcs_repo(self) -> typing.Optional["RegistryModuleVcsRepo"]:
         '''vcs_repo block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#vcs_repo RegistryModule#vcs_repo}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#vcs_repo RegistryModule#vcs_repo}
         '''
         result = self._values.get("vcs_repo")
         return typing.cast(typing.Optional["RegistryModuleVcsRepo"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -553,18 +553,18 @@
         *,
         display_identifier: builtins.str,
         identifier: builtins.str,
         github_app_installation_id: typing.Optional[builtins.str] = None,
         oauth_token_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param display_identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#display_identifier RegistryModule#display_identifier}.
-        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#identifier RegistryModule#identifier}.
-        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#github_app_installation_id RegistryModule#github_app_installation_id}.
-        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#oauth_token_id RegistryModule#oauth_token_id}.
+        :param display_identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#display_identifier RegistryModule#display_identifier}.
+        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#identifier RegistryModule#identifier}.
+        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#github_app_installation_id RegistryModule#github_app_installation_id}.
+        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#oauth_token_id RegistryModule#oauth_token_id}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ff17e2a43a1fe6421059a5a0a63bfe3416046a7e27a15064abb7286f34ffc2c5)
             check_type(argname="argument display_identifier", value=display_identifier, expected_type=type_hints["display_identifier"])
             check_type(argname="argument identifier", value=identifier, expected_type=type_hints["identifier"])
             check_type(argname="argument github_app_installation_id", value=github_app_installation_id, expected_type=type_hints["github_app_installation_id"])
             check_type(argname="argument oauth_token_id", value=oauth_token_id, expected_type=type_hints["oauth_token_id"])
@@ -575,35 +575,35 @@
         if github_app_installation_id is not None:
             self._values["github_app_installation_id"] = github_app_installation_id
         if oauth_token_id is not None:
             self._values["oauth_token_id"] = oauth_token_id
 
     @builtins.property
     def display_identifier(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#display_identifier RegistryModule#display_identifier}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#display_identifier RegistryModule#display_identifier}.'''
         result = self._values.get("display_identifier")
         assert result is not None, "Required property 'display_identifier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def identifier(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#identifier RegistryModule#identifier}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#identifier RegistryModule#identifier}.'''
         result = self._values.get("identifier")
         assert result is not None, "Required property 'identifier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def github_app_installation_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#github_app_installation_id RegistryModule#github_app_installation_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#github_app_installation_id RegistryModule#github_app_installation_id}.'''
         result = self._values.get("github_app_installation_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def oauth_token_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/registry_module#oauth_token_id RegistryModule#oauth_token_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/registry_module#oauth_token_id RegistryModule#oauth_token_id}.'''
         result = self._values.get("oauth_token_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/run_trigger/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/run_trigger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_run_trigger`
 
-Refer to the Terraform Registory for docs: [`tfe_run_trigger`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger).
+Refer to the Terraform Registory for docs: [`tfe_run_trigger`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class RunTrigger(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.runTrigger.RunTrigger",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger tfe_run_trigger}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger tfe_run_trigger}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         sourceable_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger tfe_run_trigger} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger tfe_run_trigger} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param sourceable_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#sourceable_id RunTrigger#sourceable_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#workspace_id RunTrigger#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#id RunTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param sourceable_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#sourceable_id RunTrigger#sourceable_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#workspace_id RunTrigger#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#id RunTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param sourceable_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#sourceable_id RunTrigger#sourceable_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#workspace_id RunTrigger#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#id RunTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param sourceable_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#sourceable_id RunTrigger#sourceable_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#workspace_id RunTrigger#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#id RunTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__22dc6a9aff3bfb0120e45121aa3b2c63b98b4a4ce0c70508d83e96b31f735a72)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def sourceable_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#sourceable_id RunTrigger#sourceable_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#sourceable_id RunTrigger#sourceable_id}.'''
         result = self._values.get("sourceable_id")
         assert result is not None, "Required property 'sourceable_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#workspace_id RunTrigger#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#workspace_id RunTrigger#workspace_id}.'''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/run_trigger#id RunTrigger#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/run_trigger#id RunTrigger#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/sentinel_policy/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/sentinel_policy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_sentinel_policy`
 
-Refer to the Terraform Registory for docs: [`tfe_sentinel_policy`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy).
+Refer to the Terraform Registory for docs: [`tfe_sentinel_policy`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class SentinelPolicy(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.sentinelPolicy.SentinelPolicy",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy tfe_sentinel_policy}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy tfe_sentinel_policy}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy tfe_sentinel_policy} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy tfe_sentinel_policy} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#name SentinelPolicy#name}.
-        :param policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#policy SentinelPolicy#policy}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#description SentinelPolicy#description}.
-        :param enforce_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#enforce_mode SentinelPolicy#enforce_mode}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#organization SentinelPolicy#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#name SentinelPolicy#name}.
+        :param policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#policy SentinelPolicy#policy}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#description SentinelPolicy#description}.
+        :param enforce_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#enforce_mode SentinelPolicy#enforce_mode}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#organization SentinelPolicy#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -256,20 +256,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#name SentinelPolicy#name}.
-        :param policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#policy SentinelPolicy#policy}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#description SentinelPolicy#description}.
-        :param enforce_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#enforce_mode SentinelPolicy#enforce_mode}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#organization SentinelPolicy#organization}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#name SentinelPolicy#name}.
+        :param policy: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#policy SentinelPolicy#policy}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#description SentinelPolicy#description}.
+        :param enforce_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#enforce_mode SentinelPolicy#enforce_mode}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#id SentinelPolicy#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#organization SentinelPolicy#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c2e034284df9f702d6aeb5061009d06cb15c6e18bde632f21bfef044ac862e07)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -373,51 +373,51 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#name SentinelPolicy#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#name SentinelPolicy#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#policy SentinelPolicy#policy}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#policy SentinelPolicy#policy}.'''
         result = self._values.get("policy")
         assert result is not None, "Required property 'policy' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#description SentinelPolicy#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#description SentinelPolicy#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enforce_mode(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#enforce_mode SentinelPolicy#enforce_mode}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#enforce_mode SentinelPolicy#enforce_mode}.'''
         result = self._values.get("enforce_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#id SentinelPolicy#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#id SentinelPolicy#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/sentinel_policy#organization SentinelPolicy#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/sentinel_policy#organization SentinelPolicy#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/ssh_key/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/ssh_key/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_ssh_key`
 
-Refer to the Terraform Registory for docs: [`tfe_ssh_key`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key).
+Refer to the Terraform Registory for docs: [`tfe_ssh_key`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class SshKey(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.sshKey.SshKey",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key tfe_ssh_key}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key tfe_ssh_key}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key tfe_ssh_key} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key tfe_ssh_key} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#key SshKey#key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#name SshKey#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#id SshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#organization SshKey#organization}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#key SshKey#key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#name SshKey#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#id SshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#organization SshKey#organization}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -204,18 +204,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#key SshKey#key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#name SshKey#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#id SshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#organization SshKey#organization}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#key SshKey#key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#name SshKey#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#id SshKey#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#organization SshKey#organization}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fc67fada239f596588105ed467a4d5af4cdd2a1a8460af168e1fb13aa7f20e20)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -313,39 +313,39 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#key SshKey#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#key SshKey#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#name SshKey#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#name SshKey#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#id SshKey#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#id SshKey#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/ssh_key#organization SshKey#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/ssh_key#organization SshKey#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team`
 
-Refer to the Terraform Registory for docs: [`tfe_team`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team).
+Refer to the Terraform Registory for docs: [`tfe_team`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Team(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.team.Team",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team tfe_team}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team tfe_team}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team tfe_team} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team tfe_team} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#name Team#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#organization Team#organization}.
-        :param organization_access: organization_access block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#organization_access Team#organization_access}
-        :param sso_team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#sso_team_id Team#sso_team_id}.
-        :param visibility: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#visibility Team#visibility}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#name Team#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#organization Team#organization}.
+        :param organization_access: organization_access block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#organization_access Team#organization_access}
+        :param sso_team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#sso_team_id Team#sso_team_id}.
+        :param visibility: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#visibility Team#visibility}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,24 +99,24 @@
         manage_run_tasks: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         manage_vcs_settings: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         manage_workspaces: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         read_projects: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         read_workspaces: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param manage_modules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_modules Team#manage_modules}.
-        :param manage_policies: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_policies Team#manage_policies}.
-        :param manage_policy_overrides: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_policy_overrides Team#manage_policy_overrides}.
-        :param manage_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_projects Team#manage_projects}.
-        :param manage_providers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_providers Team#manage_providers}.
-        :param manage_run_tasks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_run_tasks Team#manage_run_tasks}.
-        :param manage_vcs_settings: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_vcs_settings Team#manage_vcs_settings}.
-        :param manage_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_workspaces Team#manage_workspaces}.
-        :param read_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#read_projects Team#read_projects}.
-        :param read_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#read_workspaces Team#read_workspaces}.
+        :param manage_modules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_modules Team#manage_modules}.
+        :param manage_policies: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_policies Team#manage_policies}.
+        :param manage_policy_overrides: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_policy_overrides Team#manage_policy_overrides}.
+        :param manage_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_projects Team#manage_projects}.
+        :param manage_providers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_providers Team#manage_providers}.
+        :param manage_run_tasks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_run_tasks Team#manage_run_tasks}.
+        :param manage_vcs_settings: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_vcs_settings Team#manage_vcs_settings}.
+        :param manage_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_workspaces Team#manage_workspaces}.
+        :param read_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#read_projects Team#read_projects}.
+        :param read_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#read_workspaces Team#read_workspaces}.
         '''
         value = TeamOrganizationAccess(
             manage_modules=manage_modules,
             manage_policies=manage_policies,
             manage_policy_overrides=manage_policy_overrides,
             manage_projects=manage_projects,
             manage_providers=manage_providers,
@@ -295,20 +295,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#name Team#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#organization Team#organization}.
-        :param organization_access: organization_access block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#organization_access Team#organization_access}
-        :param sso_team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#sso_team_id Team#sso_team_id}.
-        :param visibility: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#visibility Team#visibility}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#name Team#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#organization Team#organization}.
+        :param organization_access: organization_access block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#organization_access Team#organization_access}
+        :param sso_team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#sso_team_id Team#sso_team_id}.
+        :param visibility: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#visibility Team#visibility}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(organization_access, dict):
             organization_access = TeamOrganizationAccess(**organization_access)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bcade32830944edb54717c39f8a57168078022bfa52a7e471830c9c401c92c5f)
@@ -415,53 +415,53 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#name Team#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#name Team#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#id Team#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#id Team#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#organization Team#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#organization Team#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization_access(self) -> typing.Optional["TeamOrganizationAccess"]:
         '''organization_access block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#organization_access Team#organization_access}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#organization_access Team#organization_access}
         '''
         result = self._values.get("organization_access")
         return typing.cast(typing.Optional["TeamOrganizationAccess"], result)
 
     @builtins.property
     def sso_team_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#sso_team_id Team#sso_team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#sso_team_id Team#sso_team_id}.'''
         result = self._values.get("sso_team_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def visibility(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#visibility Team#visibility}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#visibility Team#visibility}.'''
         result = self._values.get("visibility")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -501,24 +501,24 @@
         manage_run_tasks: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         manage_vcs_settings: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         manage_workspaces: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         read_projects: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         read_workspaces: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param manage_modules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_modules Team#manage_modules}.
-        :param manage_policies: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_policies Team#manage_policies}.
-        :param manage_policy_overrides: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_policy_overrides Team#manage_policy_overrides}.
-        :param manage_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_projects Team#manage_projects}.
-        :param manage_providers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_providers Team#manage_providers}.
-        :param manage_run_tasks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_run_tasks Team#manage_run_tasks}.
-        :param manage_vcs_settings: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_vcs_settings Team#manage_vcs_settings}.
-        :param manage_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_workspaces Team#manage_workspaces}.
-        :param read_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#read_projects Team#read_projects}.
-        :param read_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#read_workspaces Team#read_workspaces}.
+        :param manage_modules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_modules Team#manage_modules}.
+        :param manage_policies: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_policies Team#manage_policies}.
+        :param manage_policy_overrides: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_policy_overrides Team#manage_policy_overrides}.
+        :param manage_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_projects Team#manage_projects}.
+        :param manage_providers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_providers Team#manage_providers}.
+        :param manage_run_tasks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_run_tasks Team#manage_run_tasks}.
+        :param manage_vcs_settings: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_vcs_settings Team#manage_vcs_settings}.
+        :param manage_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_workspaces Team#manage_workspaces}.
+        :param read_projects: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#read_projects Team#read_projects}.
+        :param read_workspaces: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#read_workspaces Team#read_workspaces}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__301acc631f035baf4345707f25c24f29742b4c5bd4f221141a0ccd949f90641f)
             check_type(argname="argument manage_modules", value=manage_modules, expected_type=type_hints["manage_modules"])
             check_type(argname="argument manage_policies", value=manage_policies, expected_type=type_hints["manage_policies"])
             check_type(argname="argument manage_policy_overrides", value=manage_policy_overrides, expected_type=type_hints["manage_policy_overrides"])
             check_type(argname="argument manage_projects", value=manage_projects, expected_type=type_hints["manage_projects"])
@@ -550,87 +550,87 @@
         if read_workspaces is not None:
             self._values["read_workspaces"] = read_workspaces
 
     @builtins.property
     def manage_modules(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_modules Team#manage_modules}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_modules Team#manage_modules}.'''
         result = self._values.get("manage_modules")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_policies(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_policies Team#manage_policies}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_policies Team#manage_policies}.'''
         result = self._values.get("manage_policies")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_policy_overrides(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_policy_overrides Team#manage_policy_overrides}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_policy_overrides Team#manage_policy_overrides}.'''
         result = self._values.get("manage_policy_overrides")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_projects(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_projects Team#manage_projects}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_projects Team#manage_projects}.'''
         result = self._values.get("manage_projects")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_providers(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_providers Team#manage_providers}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_providers Team#manage_providers}.'''
         result = self._values.get("manage_providers")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_run_tasks(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_run_tasks Team#manage_run_tasks}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_run_tasks Team#manage_run_tasks}.'''
         result = self._values.get("manage_run_tasks")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_vcs_settings(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_vcs_settings Team#manage_vcs_settings}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_vcs_settings Team#manage_vcs_settings}.'''
         result = self._values.get("manage_vcs_settings")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def manage_workspaces(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#manage_workspaces Team#manage_workspaces}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#manage_workspaces Team#manage_workspaces}.'''
         result = self._values.get("manage_workspaces")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def read_projects(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#read_projects Team#read_projects}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#read_projects Team#read_projects}.'''
         result = self._values.get("read_projects")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def read_workspaces(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team#read_workspaces Team#read_workspaces}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team#read_workspaces Team#read_workspaces}.'''
         result = self._values.get("read_workspaces")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_access/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_access/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_access`
 
-Refer to the Terraform Registory for docs: [`tfe_team_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access).
+Refer to the Terraform Registory for docs: [`tfe_team_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamAccess(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamAccess.TeamAccess",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access tfe_team_access}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access tfe_team_access}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         team_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access tfe_team_access} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access tfe_team_access} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#team_id TeamAccess#team_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#workspace_id TeamAccess#workspace_id}.
-        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#access TeamAccess#access}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#id TeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param permissions: permissions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#permissions TeamAccess#permissions}
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#team_id TeamAccess#team_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#workspace_id TeamAccess#workspace_id}.
+        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#access TeamAccess#access}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#id TeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param permissions: permissions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#permissions TeamAccess#permissions}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -238,19 +238,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#team_id TeamAccess#team_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#workspace_id TeamAccess#workspace_id}.
-        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#access TeamAccess#access}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#id TeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param permissions: permissions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#permissions TeamAccess#permissions}
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#team_id TeamAccess#team_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#workspace_id TeamAccess#workspace_id}.
+        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#access TeamAccess#access}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#id TeamAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param permissions: permissions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#permissions TeamAccess#permissions}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85a2c84b18a9b10da64f60649f48a5c0ebcba59f849a45718ddd5bd5c3d34a82)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -351,49 +351,49 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#team_id TeamAccess#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#team_id TeamAccess#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#workspace_id TeamAccess#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#workspace_id TeamAccess#workspace_id}.'''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def access(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#access TeamAccess#access}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#access TeamAccess#access}.'''
         result = self._values.get("access")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#id TeamAccess#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#id TeamAccess#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def permissions(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["TeamAccessPermissions"]]]:
         '''permissions block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#permissions TeamAccess#permissions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#permissions TeamAccess#permissions}
         '''
         result = self._values.get("permissions")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["TeamAccessPermissions"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -426,20 +426,20 @@
         run_tasks: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         sentinel_mocks: builtins.str,
         state_versions: builtins.str,
         variables: builtins.str,
         workspace_locking: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     ) -> None:
         '''
-        :param runs: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#runs TeamAccess#runs}.
-        :param run_tasks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#run_tasks TeamAccess#run_tasks}.
-        :param sentinel_mocks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#sentinel_mocks TeamAccess#sentinel_mocks}.
-        :param state_versions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#state_versions TeamAccess#state_versions}.
-        :param variables: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#variables TeamAccess#variables}.
-        :param workspace_locking: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#workspace_locking TeamAccess#workspace_locking}.
+        :param runs: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#runs TeamAccess#runs}.
+        :param run_tasks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#run_tasks TeamAccess#run_tasks}.
+        :param sentinel_mocks: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#sentinel_mocks TeamAccess#sentinel_mocks}.
+        :param state_versions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#state_versions TeamAccess#state_versions}.
+        :param variables: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#variables TeamAccess#variables}.
+        :param workspace_locking: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#workspace_locking TeamAccess#workspace_locking}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0eace29ae0eba15f82ad6328b3dfc04e7ad208eef0a0623b7877ccb0e3afe14a)
             check_type(argname="argument runs", value=runs, expected_type=type_hints["runs"])
             check_type(argname="argument run_tasks", value=run_tasks, expected_type=type_hints["run_tasks"])
             check_type(argname="argument sentinel_mocks", value=sentinel_mocks, expected_type=type_hints["sentinel_mocks"])
             check_type(argname="argument state_versions", value=state_versions, expected_type=type_hints["state_versions"])
@@ -452,52 +452,52 @@
             "state_versions": state_versions,
             "variables": variables,
             "workspace_locking": workspace_locking,
         }
 
     @builtins.property
     def runs(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#runs TeamAccess#runs}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#runs TeamAccess#runs}.'''
         result = self._values.get("runs")
         assert result is not None, "Required property 'runs' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def run_tasks(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#run_tasks TeamAccess#run_tasks}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#run_tasks TeamAccess#run_tasks}.'''
         result = self._values.get("run_tasks")
         assert result is not None, "Required property 'run_tasks' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def sentinel_mocks(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#sentinel_mocks TeamAccess#sentinel_mocks}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#sentinel_mocks TeamAccess#sentinel_mocks}.'''
         result = self._values.get("sentinel_mocks")
         assert result is not None, "Required property 'sentinel_mocks' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def state_versions(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#state_versions TeamAccess#state_versions}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#state_versions TeamAccess#state_versions}.'''
         result = self._values.get("state_versions")
         assert result is not None, "Required property 'state_versions' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variables(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#variables TeamAccess#variables}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#variables TeamAccess#variables}.'''
         result = self._values.get("variables")
         assert result is not None, "Required property 'variables' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_locking(
         self,
     ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_access#workspace_locking TeamAccess#workspace_locking}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_access#workspace_locking TeamAccess#workspace_locking}.'''
         result = self._values.get("workspace_locking")
         assert result is not None, "Required property 'workspace_locking' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_member/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_member/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_member`
 
-Refer to the Terraform Registory for docs: [`tfe_team_member`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member).
+Refer to the Terraform Registory for docs: [`tfe_team_member`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamMember(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamMember.TeamMember",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member tfe_team_member}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member tfe_team_member}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         team_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member tfe_team_member} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member tfe_team_member} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#team_id TeamMember#team_id}.
-        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#username TeamMember#username}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#team_id TeamMember#team_id}.
+        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#username TeamMember#username}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#team_id TeamMember#team_id}.
-        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#username TeamMember#username}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#team_id TeamMember#team_id}.
+        :param username: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#username TeamMember#username}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cba7eeca3a4a69c5d62babff409c5c46d5f4f0e1c97a5bcea14dd1d3c1e968d2)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#team_id TeamMember#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#team_id TeamMember#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#username TeamMember#username}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#username TeamMember#username}.'''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_member#id TeamMember#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_member#id TeamMember#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_members/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_members/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_members`
 
-Refer to the Terraform Registory for docs: [`tfe_team_members`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members).
+Refer to the Terraform Registory for docs: [`tfe_team_members`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamMembers(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamMembers.TeamMembers",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members tfe_team_members}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members tfe_team_members}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         team_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members tfe_team_members} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members tfe_team_members} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#team_id TeamMembers#team_id}.
-        :param usernames: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#usernames TeamMembers#usernames}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#id TeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#team_id TeamMembers#team_id}.
+        :param usernames: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#usernames TeamMembers#usernames}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#id TeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#team_id TeamMembers#team_id}.
-        :param usernames: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#usernames TeamMembers#usernames}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#id TeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#team_id TeamMembers#team_id}.
+        :param usernames: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#usernames TeamMembers#usernames}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#id TeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b98e7adf05f16dd97cab4e26f06159659bb7c435a409e596ed84dc74b7c91405)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#team_id TeamMembers#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#team_id TeamMembers#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def usernames(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#usernames TeamMembers#usernames}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#usernames TeamMembers#usernames}.'''
         result = self._values.get("usernames")
         assert result is not None, "Required property 'usernames' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_members#id TeamMembers#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_members#id TeamMembers#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_organization_member/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_organization_member/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_organization_member`
 
-Refer to the Terraform Registory for docs: [`tfe_team_organization_member`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member).
+Refer to the Terraform Registory for docs: [`tfe_team_organization_member`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamOrganizationMember(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamOrganizationMember.TeamOrganizationMember",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member tfe_team_organization_member}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member tfe_team_organization_member}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         organization_membership_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member tfe_team_organization_member} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member tfe_team_organization_member} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param organization_membership_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#organization_membership_id TeamOrganizationMember#organization_membership_id}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#team_id TeamOrganizationMember#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#id TeamOrganizationMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization_membership_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#organization_membership_id TeamOrganizationMember#organization_membership_id}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#team_id TeamOrganizationMember#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#id TeamOrganizationMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param organization_membership_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#organization_membership_id TeamOrganizationMember#organization_membership_id}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#team_id TeamOrganizationMember#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#id TeamOrganizationMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization_membership_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#organization_membership_id TeamOrganizationMember#organization_membership_id}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#team_id TeamOrganizationMember#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#id TeamOrganizationMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2c63e119e45e7fe81d51e24d02218421b58bac97bf1659324dd7366435e44de4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def organization_membership_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#organization_membership_id TeamOrganizationMember#organization_membership_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#organization_membership_id TeamOrganizationMember#organization_membership_id}.'''
         result = self._values.get("organization_membership_id")
         assert result is not None, "Required property 'organization_membership_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#team_id TeamOrganizationMember#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#team_id TeamOrganizationMember#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_member#id TeamOrganizationMember#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_member#id TeamOrganizationMember#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_organization_members/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_organization_members/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_organization_members`
 
-Refer to the Terraform Registory for docs: [`tfe_team_organization_members`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members).
+Refer to the Terraform Registory for docs: [`tfe_team_organization_members`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamOrganizationMembers(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamOrganizationMembers.TeamOrganizationMembers",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members tfe_team_organization_members}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members tfe_team_organization_members}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         organization_membership_ids: typing.Sequence[builtins.str],
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members tfe_team_organization_members} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members tfe_team_organization_members} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param organization_membership_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#organization_membership_ids TeamOrganizationMembers#organization_membership_ids}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#team_id TeamOrganizationMembers#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#id TeamOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization_membership_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#organization_membership_ids TeamOrganizationMembers#organization_membership_ids}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#team_id TeamOrganizationMembers#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#id TeamOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -180,17 +180,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param organization_membership_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#organization_membership_ids TeamOrganizationMembers#organization_membership_ids}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#team_id TeamOrganizationMembers#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#id TeamOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization_membership_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#organization_membership_ids TeamOrganizationMembers#organization_membership_ids}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#team_id TeamOrganizationMembers#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#id TeamOrganizationMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__264066d3cb77a35e06a6d200c0833c1e3e1ce5c03da589b0de6abf5c619f37a7)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -285,29 +285,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def organization_membership_ids(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#organization_membership_ids TeamOrganizationMembers#organization_membership_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#organization_membership_ids TeamOrganizationMembers#organization_membership_ids}.'''
         result = self._values.get("organization_membership_ids")
         assert result is not None, "Required property 'organization_membership_ids' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#team_id TeamOrganizationMembers#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#team_id TeamOrganizationMembers#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_organization_members#id TeamOrganizationMembers#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_organization_members#id TeamOrganizationMembers#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_project_access/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_project_access/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_project_access`
 
-Refer to the Terraform Registory for docs: [`tfe_team_project_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access).
+Refer to the Terraform Registory for docs: [`tfe_team_project_access`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamProjectAccess(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamProjectAccess.TeamProjectAccess",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access tfe_team_project_access}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access tfe_team_project_access}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         access: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access tfe_team_project_access} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access tfe_team_project_access} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#access TeamProjectAccess#access}.
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#project_id TeamProjectAccess#project_id}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#team_id TeamProjectAccess#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#id TeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#access TeamProjectAccess#access}.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#project_id TeamProjectAccess#project_id}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#team_id TeamProjectAccess#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#id TeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -200,18 +200,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#access TeamProjectAccess#access}.
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#project_id TeamProjectAccess#project_id}.
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#team_id TeamProjectAccess#team_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#id TeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param access: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#access TeamProjectAccess#access}.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#project_id TeamProjectAccess#project_id}.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#team_id TeamProjectAccess#team_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#id TeamProjectAccess#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce3d8759bee7cd90cf749afa56695b37f438665971270ad84407f12b10ef7c86)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -308,36 +308,36 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def access(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#access TeamProjectAccess#access}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#access TeamProjectAccess#access}.'''
         result = self._values.get("access")
         assert result is not None, "Required property 'access' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#project_id TeamProjectAccess#project_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#project_id TeamProjectAccess#project_id}.'''
         result = self._values.get("project_id")
         assert result is not None, "Required property 'project_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#team_id TeamProjectAccess#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#team_id TeamProjectAccess#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_project_access#id TeamProjectAccess#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_project_access#id TeamProjectAccess#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/team_token/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/team_token/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_team_token`
 
-Refer to the Terraform Registory for docs: [`tfe_team_token`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token).
+Refer to the Terraform Registory for docs: [`tfe_team_token`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.teamToken.TeamToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token tfe_team_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token tfe_team_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         team_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token tfe_team_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token tfe_team_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#team_id TeamToken#team_id}.
-        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#force_regenerate TeamToken#force_regenerate}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#id TeamToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#team_id TeamToken#team_id}.
+        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#force_regenerate TeamToken#force_regenerate}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#id TeamToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -194,17 +194,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#team_id TeamToken#team_id}.
-        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#force_regenerate TeamToken#force_regenerate}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#id TeamToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param team_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#team_id TeamToken#team_id}.
+        :param force_regenerate: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#force_regenerate TeamToken#force_regenerate}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#id TeamToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5819d6b01e765a40e2d126f5334f47277b339f12680c9bc4af58330100e3db92)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -300,30 +300,30 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def team_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#team_id TeamToken#team_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#team_id TeamToken#team_id}.'''
         result = self._values.get("team_id")
         assert result is not None, "Required property 'team_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def force_regenerate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#force_regenerate TeamToken#force_regenerate}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#force_regenerate TeamToken#force_regenerate}.'''
         result = self._values.get("force_regenerate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/team_token#id TeamToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/team_token#id TeamToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/terraform_version/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/terraform_version/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_terraform_version`
 
-Refer to the Terraform Registory for docs: [`tfe_terraform_version`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version).
+Refer to the Terraform Registory for docs: [`tfe_terraform_version`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TerraformVersion(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.terraformVersion.TerraformVersion",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version tfe_terraform_version}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version tfe_terraform_version}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         sha: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version tfe_terraform_version} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version tfe_terraform_version} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param sha: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#sha TerraformVersion#sha}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#url TerraformVersion#url}.
-        :param version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#version TerraformVersion#version}.
-        :param beta: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#beta TerraformVersion#beta}.
-        :param deprecated: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#deprecated TerraformVersion#deprecated}.
-        :param deprecated_reason: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#deprecated_reason TerraformVersion#deprecated_reason}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#enabled TerraformVersion#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#id TerraformVersion#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param official: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#official TerraformVersion#official}.
+        :param sha: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#sha TerraformVersion#sha}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#url TerraformVersion#url}.
+        :param version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#version TerraformVersion#version}.
+        :param beta: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#beta TerraformVersion#beta}.
+        :param deprecated: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#deprecated TerraformVersion#deprecated}.
+        :param deprecated_reason: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#deprecated_reason TerraformVersion#deprecated_reason}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#enabled TerraformVersion#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#id TerraformVersion#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param official: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#official TerraformVersion#official}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -350,23 +350,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param sha: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#sha TerraformVersion#sha}.
-        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#url TerraformVersion#url}.
-        :param version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#version TerraformVersion#version}.
-        :param beta: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#beta TerraformVersion#beta}.
-        :param deprecated: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#deprecated TerraformVersion#deprecated}.
-        :param deprecated_reason: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#deprecated_reason TerraformVersion#deprecated_reason}.
-        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#enabled TerraformVersion#enabled}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#id TerraformVersion#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param official: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#official TerraformVersion#official}.
+        :param sha: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#sha TerraformVersion#sha}.
+        :param url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#url TerraformVersion#url}.
+        :param version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#version TerraformVersion#version}.
+        :param beta: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#beta TerraformVersion#beta}.
+        :param deprecated: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#deprecated TerraformVersion#deprecated}.
+        :param deprecated_reason: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#deprecated_reason TerraformVersion#deprecated_reason}.
+        :param enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#enabled TerraformVersion#enabled}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#id TerraformVersion#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param official: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#official TerraformVersion#official}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__047888c5e2b85c5714a6d2723042b12e7d0321a9b50ef8c79413fdb06fac6ef6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -478,78 +478,78 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def sha(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#sha TerraformVersion#sha}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#sha TerraformVersion#sha}.'''
         result = self._values.get("sha")
         assert result is not None, "Required property 'sha' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def url(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#url TerraformVersion#url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#url TerraformVersion#url}.'''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def version(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#version TerraformVersion#version}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#version TerraformVersion#version}.'''
         result = self._values.get("version")
         assert result is not None, "Required property 'version' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def beta(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#beta TerraformVersion#beta}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#beta TerraformVersion#beta}.'''
         result = self._values.get("beta")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def deprecated(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#deprecated TerraformVersion#deprecated}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#deprecated TerraformVersion#deprecated}.'''
         result = self._values.get("deprecated")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def deprecated_reason(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#deprecated_reason TerraformVersion#deprecated_reason}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#deprecated_reason TerraformVersion#deprecated_reason}.'''
         result = self._values.get("deprecated_reason")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#enabled TerraformVersion#enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#enabled TerraformVersion#enabled}.'''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#id TerraformVersion#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#id TerraformVersion#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def official(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/terraform_version#official TerraformVersion#official}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/terraform_version#official TerraformVersion#official}.'''
         result = self._values.get("official")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/variable/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/variable/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_variable`
 
-Refer to the Terraform Registory for docs: [`tfe_variable`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable).
+Refer to the Terraform Registory for docs: [`tfe_variable`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Variable(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.variable.Variable",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable tfe_variable}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable tfe_variable}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         category: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable tfe_variable} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable tfe_variable} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#category Variable#category}.
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#key Variable#key}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#description Variable#description}.
-        :param hcl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#hcl Variable#hcl}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#id Variable#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#sensitive Variable#sensitive}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#value Variable#value}.
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#variable_set_id Variable#variable_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#workspace_id Variable#workspace_id}.
+        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#category Variable#category}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#key Variable#key}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#description Variable#description}.
+        :param hcl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#hcl Variable#hcl}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#id Variable#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#sensitive Variable#sensitive}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#value Variable#value}.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#variable_set_id Variable#variable_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#workspace_id Variable#workspace_id}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -344,23 +344,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#category Variable#category}.
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#key Variable#key}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#description Variable#description}.
-        :param hcl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#hcl Variable#hcl}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#id Variable#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#sensitive Variable#sensitive}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#value Variable#value}.
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#variable_set_id Variable#variable_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#workspace_id Variable#workspace_id}.
+        :param category: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#category Variable#category}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#key Variable#key}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#description Variable#description}.
+        :param hcl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#hcl Variable#hcl}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#id Variable#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param sensitive: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#sensitive Variable#sensitive}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#value Variable#value}.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#variable_set_id Variable#variable_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#workspace_id Variable#workspace_id}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__06b5c44a14f75926cd79c37de830c49e128a218a9f6d2eaa2aeb137bc2ac423e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -473,73 +473,73 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def category(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#category Variable#category}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#category Variable#category}.'''
         result = self._values.get("category")
         assert result is not None, "Required property 'category' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#key Variable#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#key Variable#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#description Variable#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#description Variable#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def hcl(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#hcl Variable#hcl}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#hcl Variable#hcl}.'''
         result = self._values.get("hcl")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#id Variable#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#id Variable#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sensitive(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#sensitive Variable#sensitive}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#sensitive Variable#sensitive}.'''
         result = self._values.get("sensitive")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#value Variable#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#value Variable#value}.'''
         result = self._values.get("value")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def variable_set_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#variable_set_id Variable#variable_set_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#variable_set_id Variable#variable_set_id}.'''
         result = self._values.get("variable_set_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def workspace_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable#workspace_id Variable#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable#workspace_id Variable#workspace_id}.'''
         result = self._values.get("workspace_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/variable_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/variable_set/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_variable_set`
 
-Refer to the Terraform Registory for docs: [`tfe_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set).
+Refer to the Terraform Registory for docs: [`tfe_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class VariableSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.variableSet.VariableSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set tfe_variable_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set tfe_variable_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set tfe_variable_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set tfe_variable_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#name VariableSet#name}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#description VariableSet#description}.
-        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#global VariableSet#global}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#id VariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#organization VariableSet#organization}.
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#workspace_ids VariableSet#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#name VariableSet#name}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#description VariableSet#description}.
+        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#global VariableSet#global}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#id VariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#organization VariableSet#organization}.
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#workspace_ids VariableSet#workspace_ids}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -265,20 +265,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#name VariableSet#name}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#description VariableSet#description}.
-        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#global VariableSet#global}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#id VariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#organization VariableSet#organization}.
-        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#workspace_ids VariableSet#workspace_ids}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#name VariableSet#name}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#description VariableSet#description}.
+        :param global_: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#global VariableSet#global}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#id VariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#organization VariableSet#organization}.
+        :param workspace_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#workspace_ids VariableSet#workspace_ids}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d1eb0519dd029b82d5cac753c82486f9c25ed5aa17d82709f3afea7078ca129b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -383,52 +383,52 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#name VariableSet#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#name VariableSet#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#description VariableSet#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#description VariableSet#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def global_(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#global VariableSet#global}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#global VariableSet#global}.'''
         result = self._values.get("global_")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#id VariableSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#id VariableSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#organization VariableSet#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#organization VariableSet#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def workspace_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/variable_set#workspace_ids VariableSet#workspace_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/variable_set#workspace_ids VariableSet#workspace_ids}.'''
         result = self._values.get("workspace_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_workspace`
 
-Refer to the Terraform Registory for docs: [`tfe_workspace`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace).
+Refer to the Terraform Registory for docs: [`tfe_workspace`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Workspace(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.workspace.Workspace",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace tfe_workspace}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace tfe_workspace}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -64,45 +64,45 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace tfe_workspace} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace tfe_workspace} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#name Workspace#name}.
-        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#agent_pool_id Workspace#agent_pool_id}.
-        :param allow_destroy_plan: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#allow_destroy_plan Workspace#allow_destroy_plan}.
-        :param assessments_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#assessments_enabled Workspace#assessments_enabled}.
-        :param auto_apply: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#auto_apply Workspace#auto_apply}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#description Workspace#description}.
-        :param execution_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#execution_mode Workspace#execution_mode}.
-        :param file_triggers_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#file_triggers_enabled Workspace#file_triggers_enabled}.
-        :param force_delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#force_delete Workspace#force_delete}.
-        :param global_remote_state: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#global_remote_state Workspace#global_remote_state}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#id Workspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param operations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#operations Workspace#operations}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#organization Workspace#organization}.
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#project_id Workspace#project_id}.
-        :param queue_all_runs: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#queue_all_runs Workspace#queue_all_runs}.
-        :param remote_state_consumer_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#remote_state_consumer_ids Workspace#remote_state_consumer_ids}.
-        :param source_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#source_name Workspace#source_name}.
-        :param source_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#source_url Workspace#source_url}.
-        :param speculative_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#speculative_enabled Workspace#speculative_enabled}.
-        :param ssh_key_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#ssh_key_id Workspace#ssh_key_id}.
-        :param structured_run_output_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#structured_run_output_enabled Workspace#structured_run_output_enabled}.
-        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#tag_names Workspace#tag_names}.
-        :param terraform_version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#terraform_version Workspace#terraform_version}.
-        :param trigger_patterns: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#trigger_patterns Workspace#trigger_patterns}.
-        :param trigger_prefixes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#trigger_prefixes Workspace#trigger_prefixes}.
-        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#vcs_repo Workspace#vcs_repo}
-        :param working_directory: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#working_directory Workspace#working_directory}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#name Workspace#name}.
+        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#agent_pool_id Workspace#agent_pool_id}.
+        :param allow_destroy_plan: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#allow_destroy_plan Workspace#allow_destroy_plan}.
+        :param assessments_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#assessments_enabled Workspace#assessments_enabled}.
+        :param auto_apply: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#auto_apply Workspace#auto_apply}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#description Workspace#description}.
+        :param execution_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#execution_mode Workspace#execution_mode}.
+        :param file_triggers_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#file_triggers_enabled Workspace#file_triggers_enabled}.
+        :param force_delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#force_delete Workspace#force_delete}.
+        :param global_remote_state: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#global_remote_state Workspace#global_remote_state}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#id Workspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param operations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#operations Workspace#operations}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#organization Workspace#organization}.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#project_id Workspace#project_id}.
+        :param queue_all_runs: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#queue_all_runs Workspace#queue_all_runs}.
+        :param remote_state_consumer_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#remote_state_consumer_ids Workspace#remote_state_consumer_ids}.
+        :param source_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#source_name Workspace#source_name}.
+        :param source_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#source_url Workspace#source_url}.
+        :param speculative_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#speculative_enabled Workspace#speculative_enabled}.
+        :param ssh_key_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#ssh_key_id Workspace#ssh_key_id}.
+        :param structured_run_output_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#structured_run_output_enabled Workspace#structured_run_output_enabled}.
+        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#tag_names Workspace#tag_names}.
+        :param terraform_version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#terraform_version Workspace#terraform_version}.
+        :param trigger_patterns: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#trigger_patterns Workspace#trigger_patterns}.
+        :param trigger_prefixes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#trigger_prefixes Workspace#trigger_prefixes}.
+        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#vcs_repo Workspace#vcs_repo}
+        :param working_directory: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#working_directory Workspace#working_directory}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -158,20 +158,20 @@
         branch: typing.Optional[builtins.str] = None,
         github_app_installation_id: typing.Optional[builtins.str] = None,
         ingress_submodules: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         oauth_token_id: typing.Optional[builtins.str] = None,
         tags_regex: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#identifier Workspace#identifier}.
-        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#branch Workspace#branch}.
-        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#github_app_installation_id Workspace#github_app_installation_id}.
-        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#ingress_submodules Workspace#ingress_submodules}.
-        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#oauth_token_id Workspace#oauth_token_id}.
-        :param tags_regex: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#tags_regex Workspace#tags_regex}.
+        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#identifier Workspace#identifier}.
+        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#branch Workspace#branch}.
+        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#github_app_installation_id Workspace#github_app_installation_id}.
+        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#ingress_submodules Workspace#ingress_submodules}.
+        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#oauth_token_id Workspace#oauth_token_id}.
+        :param tags_regex: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#tags_regex Workspace#tags_regex}.
         '''
         value = WorkspaceVcsRepo(
             identifier=identifier,
             branch=branch,
             github_app_installation_id=github_app_installation_id,
             ingress_submodules=ingress_submodules,
             oauth_token_id=oauth_token_id,
@@ -905,41 +905,41 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#name Workspace#name}.
-        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#agent_pool_id Workspace#agent_pool_id}.
-        :param allow_destroy_plan: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#allow_destroy_plan Workspace#allow_destroy_plan}.
-        :param assessments_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#assessments_enabled Workspace#assessments_enabled}.
-        :param auto_apply: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#auto_apply Workspace#auto_apply}.
-        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#description Workspace#description}.
-        :param execution_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#execution_mode Workspace#execution_mode}.
-        :param file_triggers_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#file_triggers_enabled Workspace#file_triggers_enabled}.
-        :param force_delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#force_delete Workspace#force_delete}.
-        :param global_remote_state: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#global_remote_state Workspace#global_remote_state}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#id Workspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param operations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#operations Workspace#operations}.
-        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#organization Workspace#organization}.
-        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#project_id Workspace#project_id}.
-        :param queue_all_runs: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#queue_all_runs Workspace#queue_all_runs}.
-        :param remote_state_consumer_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#remote_state_consumer_ids Workspace#remote_state_consumer_ids}.
-        :param source_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#source_name Workspace#source_name}.
-        :param source_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#source_url Workspace#source_url}.
-        :param speculative_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#speculative_enabled Workspace#speculative_enabled}.
-        :param ssh_key_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#ssh_key_id Workspace#ssh_key_id}.
-        :param structured_run_output_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#structured_run_output_enabled Workspace#structured_run_output_enabled}.
-        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#tag_names Workspace#tag_names}.
-        :param terraform_version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#terraform_version Workspace#terraform_version}.
-        :param trigger_patterns: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#trigger_patterns Workspace#trigger_patterns}.
-        :param trigger_prefixes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#trigger_prefixes Workspace#trigger_prefixes}.
-        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#vcs_repo Workspace#vcs_repo}
-        :param working_directory: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#working_directory Workspace#working_directory}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#name Workspace#name}.
+        :param agent_pool_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#agent_pool_id Workspace#agent_pool_id}.
+        :param allow_destroy_plan: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#allow_destroy_plan Workspace#allow_destroy_plan}.
+        :param assessments_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#assessments_enabled Workspace#assessments_enabled}.
+        :param auto_apply: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#auto_apply Workspace#auto_apply}.
+        :param description: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#description Workspace#description}.
+        :param execution_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#execution_mode Workspace#execution_mode}.
+        :param file_triggers_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#file_triggers_enabled Workspace#file_triggers_enabled}.
+        :param force_delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#force_delete Workspace#force_delete}.
+        :param global_remote_state: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#global_remote_state Workspace#global_remote_state}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#id Workspace#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param operations: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#operations Workspace#operations}.
+        :param organization: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#organization Workspace#organization}.
+        :param project_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#project_id Workspace#project_id}.
+        :param queue_all_runs: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#queue_all_runs Workspace#queue_all_runs}.
+        :param remote_state_consumer_ids: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#remote_state_consumer_ids Workspace#remote_state_consumer_ids}.
+        :param source_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#source_name Workspace#source_name}.
+        :param source_url: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#source_url Workspace#source_url}.
+        :param speculative_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#speculative_enabled Workspace#speculative_enabled}.
+        :param ssh_key_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#ssh_key_id Workspace#ssh_key_id}.
+        :param structured_run_output_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#structured_run_output_enabled Workspace#structured_run_output_enabled}.
+        :param tag_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#tag_names Workspace#tag_names}.
+        :param terraform_version: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#terraform_version Workspace#terraform_version}.
+        :param trigger_patterns: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#trigger_patterns Workspace#trigger_patterns}.
+        :param trigger_prefixes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#trigger_prefixes Workspace#trigger_prefixes}.
+        :param vcs_repo: vcs_repo block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#vcs_repo Workspace#vcs_repo}
+        :param working_directory: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#working_directory Workspace#working_directory}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(vcs_repo, dict):
             vcs_repo = WorkspaceVcsRepo(**vcs_repo)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__935ff8f3ff09b89bd591d0174fd65e196b049b8e278a96819817bc647017fe85)
@@ -1109,199 +1109,199 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#name Workspace#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#name Workspace#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def agent_pool_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#agent_pool_id Workspace#agent_pool_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#agent_pool_id Workspace#agent_pool_id}.'''
         result = self._values.get("agent_pool_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def allow_destroy_plan(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#allow_destroy_plan Workspace#allow_destroy_plan}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#allow_destroy_plan Workspace#allow_destroy_plan}.'''
         result = self._values.get("allow_destroy_plan")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def assessments_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#assessments_enabled Workspace#assessments_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#assessments_enabled Workspace#assessments_enabled}.'''
         result = self._values.get("assessments_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def auto_apply(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#auto_apply Workspace#auto_apply}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#auto_apply Workspace#auto_apply}.'''
         result = self._values.get("auto_apply")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#description Workspace#description}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#description Workspace#description}.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def execution_mode(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#execution_mode Workspace#execution_mode}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#execution_mode Workspace#execution_mode}.'''
         result = self._values.get("execution_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def file_triggers_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#file_triggers_enabled Workspace#file_triggers_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#file_triggers_enabled Workspace#file_triggers_enabled}.'''
         result = self._values.get("file_triggers_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def force_delete(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#force_delete Workspace#force_delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#force_delete Workspace#force_delete}.'''
         result = self._values.get("force_delete")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def global_remote_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#global_remote_state Workspace#global_remote_state}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#global_remote_state Workspace#global_remote_state}.'''
         result = self._values.get("global_remote_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#id Workspace#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#id Workspace#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def operations(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#operations Workspace#operations}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#operations Workspace#operations}.'''
         result = self._values.get("operations")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def organization(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#organization Workspace#organization}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#organization Workspace#organization}.'''
         result = self._values.get("organization")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#project_id Workspace#project_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#project_id Workspace#project_id}.'''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def queue_all_runs(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#queue_all_runs Workspace#queue_all_runs}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#queue_all_runs Workspace#queue_all_runs}.'''
         result = self._values.get("queue_all_runs")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def remote_state_consumer_ids(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#remote_state_consumer_ids Workspace#remote_state_consumer_ids}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#remote_state_consumer_ids Workspace#remote_state_consumer_ids}.'''
         result = self._values.get("remote_state_consumer_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def source_name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#source_name Workspace#source_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#source_name Workspace#source_name}.'''
         result = self._values.get("source_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_url(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#source_url Workspace#source_url}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#source_url Workspace#source_url}.'''
         result = self._values.get("source_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def speculative_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#speculative_enabled Workspace#speculative_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#speculative_enabled Workspace#speculative_enabled}.'''
         result = self._values.get("speculative_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def ssh_key_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#ssh_key_id Workspace#ssh_key_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#ssh_key_id Workspace#ssh_key_id}.'''
         result = self._values.get("ssh_key_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def structured_run_output_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#structured_run_output_enabled Workspace#structured_run_output_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#structured_run_output_enabled Workspace#structured_run_output_enabled}.'''
         result = self._values.get("structured_run_output_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tag_names(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#tag_names Workspace#tag_names}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#tag_names Workspace#tag_names}.'''
         result = self._values.get("tag_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def terraform_version(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#terraform_version Workspace#terraform_version}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#terraform_version Workspace#terraform_version}.'''
         result = self._values.get("terraform_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def trigger_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#trigger_patterns Workspace#trigger_patterns}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#trigger_patterns Workspace#trigger_patterns}.'''
         result = self._values.get("trigger_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def trigger_prefixes(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#trigger_prefixes Workspace#trigger_prefixes}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#trigger_prefixes Workspace#trigger_prefixes}.'''
         result = self._values.get("trigger_prefixes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def vcs_repo(self) -> typing.Optional["WorkspaceVcsRepo"]:
         '''vcs_repo block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#vcs_repo Workspace#vcs_repo}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#vcs_repo Workspace#vcs_repo}
         '''
         result = self._values.get("vcs_repo")
         return typing.cast(typing.Optional["WorkspaceVcsRepo"], result)
 
     @builtins.property
     def working_directory(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#working_directory Workspace#working_directory}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#working_directory Workspace#working_directory}.'''
         result = self._values.get("working_directory")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1333,20 +1333,20 @@
         branch: typing.Optional[builtins.str] = None,
         github_app_installation_id: typing.Optional[builtins.str] = None,
         ingress_submodules: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         oauth_token_id: typing.Optional[builtins.str] = None,
         tags_regex: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#identifier Workspace#identifier}.
-        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#branch Workspace#branch}.
-        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#github_app_installation_id Workspace#github_app_installation_id}.
-        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#ingress_submodules Workspace#ingress_submodules}.
-        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#oauth_token_id Workspace#oauth_token_id}.
-        :param tags_regex: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#tags_regex Workspace#tags_regex}.
+        :param identifier: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#identifier Workspace#identifier}.
+        :param branch: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#branch Workspace#branch}.
+        :param github_app_installation_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#github_app_installation_id Workspace#github_app_installation_id}.
+        :param ingress_submodules: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#ingress_submodules Workspace#ingress_submodules}.
+        :param oauth_token_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#oauth_token_id Workspace#oauth_token_id}.
+        :param tags_regex: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#tags_regex Workspace#tags_regex}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__aff975a6bd7030cca9ebdacd6fe620a9c9aa60a26f549dfd175758974455ba8f)
             check_type(argname="argument identifier", value=identifier, expected_type=type_hints["identifier"])
             check_type(argname="argument branch", value=branch, expected_type=type_hints["branch"])
             check_type(argname="argument github_app_installation_id", value=github_app_installation_id, expected_type=type_hints["github_app_installation_id"])
             check_type(argname="argument ingress_submodules", value=ingress_submodules, expected_type=type_hints["ingress_submodules"])
@@ -1364,48 +1364,48 @@
         if oauth_token_id is not None:
             self._values["oauth_token_id"] = oauth_token_id
         if tags_regex is not None:
             self._values["tags_regex"] = tags_regex
 
     @builtins.property
     def identifier(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#identifier Workspace#identifier}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#identifier Workspace#identifier}.'''
         result = self._values.get("identifier")
         assert result is not None, "Required property 'identifier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def branch(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#branch Workspace#branch}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#branch Workspace#branch}.'''
         result = self._values.get("branch")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def github_app_installation_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#github_app_installation_id Workspace#github_app_installation_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#github_app_installation_id Workspace#github_app_installation_id}.'''
         result = self._values.get("github_app_installation_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ingress_submodules(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#ingress_submodules Workspace#ingress_submodules}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#ingress_submodules Workspace#ingress_submodules}.'''
         result = self._values.get("ingress_submodules")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def oauth_token_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#oauth_token_id Workspace#oauth_token_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#oauth_token_id Workspace#oauth_token_id}.'''
         result = self._values.get("oauth_token_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags_regex(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace#tags_regex Workspace#tags_regex}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace#tags_regex Workspace#tags_regex}.'''
         result = self._values.get("tags_regex")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_policy_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_policy_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_workspace_policy_set`
 
-Refer to the Terraform Registory for docs: [`tfe_workspace_policy_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set).
+Refer to the Terraform Registory for docs: [`tfe_workspace_policy_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class WorkspacePolicySet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.workspacePolicySet.WorkspacePolicySet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set tfe_workspace_policy_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set tfe_workspace_policy_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         policy_set_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set tfe_workspace_policy_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set tfe_workspace_policy_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#policy_set_id WorkspacePolicySet#policy_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#workspace_id WorkspacePolicySet#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#id WorkspacePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#policy_set_id WorkspacePolicySet#policy_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#workspace_id WorkspacePolicySet#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#id WorkspacePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#policy_set_id WorkspacePolicySet#policy_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#workspace_id WorkspacePolicySet#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#id WorkspacePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#policy_set_id WorkspacePolicySet#policy_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#workspace_id WorkspacePolicySet#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#id WorkspacePolicySet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__22dbc36aed15ca4506faefb35870c4a8ecf46149ce00a0602e5fd0e64e67a5ac)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def policy_set_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#policy_set_id WorkspacePolicySet#policy_set_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#policy_set_id WorkspacePolicySet#policy_set_id}.'''
         result = self._values.get("policy_set_id")
         assert result is not None, "Required property 'policy_set_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#workspace_id WorkspacePolicySet#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#workspace_id WorkspacePolicySet#workspace_id}.'''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_policy_set#id WorkspacePolicySet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_policy_set#id WorkspacePolicySet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_run_task/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_run_task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_workspace_run_task`
 
-Refer to the Terraform Registory for docs: [`tfe_workspace_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task).
+Refer to the Terraform Registory for docs: [`tfe_workspace_run_task`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class WorkspaceRunTask(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.workspaceRunTask.WorkspaceRunTask",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task tfe_workspace_run_task}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task tfe_workspace_run_task}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         enforcement_level: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task tfe_workspace_run_task} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task tfe_workspace_run_task} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param enforcement_level: The enforcement level of the task. Valid values are ``advisory`` and ``mandatory``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#enforcement_level WorkspaceRunTask#enforcement_level}
-        :param task_id: The id of the Run task to associate to the Workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#task_id WorkspaceRunTask#task_id}
-        :param workspace_id: The id of the workspace to associate the Run task to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#workspace_id WorkspaceRunTask#workspace_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#id WorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param stage: The stage to run the task in. Valid values are ``pre_plan``, ``post_plan`` and ``pre_apply``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#stage WorkspaceRunTask#stage}
+        :param enforcement_level: The enforcement level of the task. Valid values are ``advisory`` and ``mandatory``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#enforcement_level WorkspaceRunTask#enforcement_level}
+        :param task_id: The id of the Run task to associate to the Workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#task_id WorkspaceRunTask#task_id}
+        :param workspace_id: The id of the workspace to associate the Run task to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#workspace_id WorkspaceRunTask#workspace_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#id WorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param stage: The stage to run the task in. Valid values are ``pre_plan``, ``post_plan`` and ``pre_apply``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#stage WorkspaceRunTask#stage}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -226,19 +226,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param enforcement_level: The enforcement level of the task. Valid values are ``advisory`` and ``mandatory``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#enforcement_level WorkspaceRunTask#enforcement_level}
-        :param task_id: The id of the Run task to associate to the Workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#task_id WorkspaceRunTask#task_id}
-        :param workspace_id: The id of the workspace to associate the Run task to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#workspace_id WorkspaceRunTask#workspace_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#id WorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param stage: The stage to run the task in. Valid values are ``pre_plan``, ``post_plan`` and ``pre_apply``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#stage WorkspaceRunTask#stage}
+        :param enforcement_level: The enforcement level of the task. Valid values are ``advisory`` and ``mandatory``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#enforcement_level WorkspaceRunTask#enforcement_level}
+        :param task_id: The id of the Run task to associate to the Workspace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#task_id WorkspaceRunTask#task_id}
+        :param workspace_id: The id of the workspace to associate the Run task to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#workspace_id WorkspaceRunTask#workspace_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#id WorkspaceRunTask#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param stage: The stage to run the task in. Valid values are ``pre_plan``, ``post_plan`` and ``pre_apply``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#stage WorkspaceRunTask#stage}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__95584cd5d66d82b2337061a0b6cdb361fa60914e2f40651470c5f212aedf55f9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -340,55 +340,55 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def enforcement_level(self) -> builtins.str:
         '''The enforcement level of the task. Valid values are ``advisory`` and ``mandatory``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#enforcement_level WorkspaceRunTask#enforcement_level}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#enforcement_level WorkspaceRunTask#enforcement_level}
         '''
         result = self._values.get("enforcement_level")
         assert result is not None, "Required property 'enforcement_level' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def task_id(self) -> builtins.str:
         '''The id of the Run task to associate to the Workspace.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#task_id WorkspaceRunTask#task_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#task_id WorkspaceRunTask#task_id}
         '''
         result = self._values.get("task_id")
         assert result is not None, "Required property 'task_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
         '''The id of the workspace to associate the Run task to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#workspace_id WorkspaceRunTask#workspace_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#workspace_id WorkspaceRunTask#workspace_id}
         '''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#id WorkspaceRunTask#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#id WorkspaceRunTask#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def stage(self) -> typing.Optional[builtins.str]:
         '''The stage to run the task in. Valid values are ``pre_plan``, ``post_plan`` and ``pre_apply``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_run_task#stage WorkspaceRunTask#stage}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_run_task#stage WorkspaceRunTask#stage}
         '''
         result = self._values.get("stage")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe/workspace_variable_set/__init__.py` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe/workspace_variable_set/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `tfe_workspace_variable_set`
 
-Refer to the Terraform Registory for docs: [`tfe_workspace_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set).
+Refer to the Terraform Registory for docs: [`tfe_workspace_variable_set`](https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class WorkspaceVariableSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-tfe.workspaceVariableSet.WorkspaceVariableSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set tfe_workspace_variable_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set tfe_workspace_variable_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         variable_set_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set tfe_workspace_variable_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set tfe_workspace_variable_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#variable_set_id WorkspaceVariableSet#variable_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#workspace_id WorkspaceVariableSet#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#id WorkspaceVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#variable_set_id WorkspaceVariableSet#variable_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#workspace_id WorkspaceVariableSet#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#id WorkspaceVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -178,17 +178,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#variable_set_id WorkspaceVariableSet#variable_set_id}.
-        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#workspace_id WorkspaceVariableSet#workspace_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#id WorkspaceVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param variable_set_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#variable_set_id WorkspaceVariableSet#variable_set_id}.
+        :param workspace_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#workspace_id WorkspaceVariableSet#workspace_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#id WorkspaceVariableSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a3bace0b587f68fe045ca68ec23ae33610f027fa6d2b272c5887a7862fe67e41)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -283,29 +283,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def variable_set_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#variable_set_id WorkspaceVariableSet#variable_set_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#variable_set_id WorkspaceVariableSet#variable_set_id}.'''
         result = self._values.get("variable_set_id")
         assert result is not None, "Required property 'variable_set_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#workspace_id WorkspaceVariableSet#workspace_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#workspace_id WorkspaceVariableSet#workspace_id}.'''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.0/docs/resources/workspace_variable_set#id WorkspaceVariableSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/tfe/0.44.1/docs/resources/workspace_variable_set#id WorkspaceVariableSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/PKG-INFO` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-tfe
-Version: 6.0.1
+Version: 6.0.2
 Summary: Prebuilt tfe Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-tfe.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-tfe.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-tfe-6.0.1/src/cdktf_cdktf_provider_tfe.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-tfe-6.0.2/src/cdktf_cdktf_provider_tfe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_tfe/py.typed
 src/cdktf_cdktf_provider_tfe.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_tfe.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_tfe.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_tfe.egg-info/requires.txt
 src/cdktf_cdktf_provider_tfe.egg-info/top_level.txt
 src/cdktf_cdktf_provider_tfe/_jsii/__init__.py
-src/cdktf_cdktf_provider_tfe/_jsii/provider-tfe@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_tfe/_jsii/provider-tfe@6.0.2.jsii.tgz
 src/cdktf_cdktf_provider_tfe/admin_organization_settings/__init__.py
 src/cdktf_cdktf_provider_tfe/agent_pool/__init__.py
 src/cdktf_cdktf_provider_tfe/agent_token/__init__.py
 src/cdktf_cdktf_provider_tfe/data_tfe_agent_pool/__init__.py
 src/cdktf_cdktf_provider_tfe/data_tfe_github_app_installation/__init__.py
 src/cdktf_cdktf_provider_tfe/data_tfe_ip_ranges/__init__.py
 src/cdktf_cdktf_provider_tfe/data_tfe_oauth_client/__init__.py
```


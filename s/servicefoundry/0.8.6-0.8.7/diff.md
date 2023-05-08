# Comparing `tmp/servicefoundry-0.8.6.tar.gz` & `tmp/servicefoundry-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.8.6.tar", max compression
+gzip compressed data, was "servicefoundry-0.8.7.tar", max compression
```

## Comparing `servicefoundry-0.8.6.tar` & `servicefoundry-0.8.7.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      672 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/README.md
--rw-r--r--   0        0        0     2116 2023-04-28 08:43:45.366068 servicefoundry-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     1269 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/__init__.py
--rw-r--r--   0        0        0    36574 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4159 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      531 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1357 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6479 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6458 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2795 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3875 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3863 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      228 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     3032 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-04-28 08:43:32.982165 servicefoundry-0.8.6/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23939 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5624 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1028 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9608 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5196 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-04-28 08:43:32.986165 servicefoundry-0.8.6/servicefoundry/version.py
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/README.md
+-rw-r--r--   0        0        0     2116 2023-05-08 06:54:49.631181 servicefoundry-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     1269 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    36574 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4159 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1357 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6479 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6458 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     2795 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     3587 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     3863 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2492 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    23939 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     5624 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0     9147 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0     9914 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5196 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.8.7/PKG-INFO
```

### Comparing `servicefoundry-0.8.6/README.md` & `servicefoundry-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/pyproject.toml` & `servicefoundry-0.8.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.8.6"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.7"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.8.6/servicefoundry/__init__.py` & `servicefoundry-0.8.7/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/auto_gen/models.py` & `servicefoundry-0.8.7/servicefoundry/auto_gen/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/builder/__init__.py` & `servicefoundry-0.8.7/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.8.7/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.8.7/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/builder/docker_service.py` & `servicefoundry-0.8.7/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/cli_main.py` & `servicefoundry-0.8.7/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/list_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,57 +47,62 @@
     )
     if not workspaces:
         output_hook = RichOutputCallBack()
         output_hook.print_line(PROMPT_NO_WORKSPACES)
     else:
         workspaces.sort(key=lambda s: s.createdAt, reverse=True)
 
-    if CliConfig.get("json"):
-        print_json(data=workspaces)
-    else:
-        print_entity_list(
-            "Workspaces",
-            workspaces,
-        )
+    print_entity_list(
+        "Workspaces",
+        workspaces,
+    )
 
 
 @click.command(name="applications", cls=COMMAND_CLS, help="List Applications")
 @click.option(
     "-w",
     "--workspace-fqn",
     "--workspace_fqn",
     type=click.STRING,
     default=None,
     help="FQN of the Workspace",
 )
 @click.option(
     "--application-type",
     "--application_type",
-    type=click.Choice(["service", "job", "model-deployment", "all"]),
+    type=click.Choice(
+        [
+            "service",
+            "job",
+            "model-deployment",
+            "volume",
+            "notebook",
+            "intercept",
+            "helm",
+            "all",
+        ]
+    ),
     default="all",
     help="Application Type",
 )
 @handle_exception_wrapper
 def list_applications(workspace_fqn, application_type):
     applications = application_lib.list_applications(
         workspace_fqn=workspace_fqn, application_type=application_type
     )
     if not applications:
         output_hook = RichOutputCallBack()
         output_hook.print_line(PROMPT_NO_APPLICATIONS)
     else:
         applications.sort(key=lambda s: s.createdAt, reverse=True)
-    if CliConfig.get("json"):
-        print_json(data=applications)
-    else:
-        # TODO (chiragjn): Display columns here need to show workspace and cluster name!
-        print_entity_list(
-            "Applications",
-            applications,
-        )
+
+    print_entity_list(
+        "Applications",
+        applications,
+    )
 
 
 @click.command(
     name="application-versions", cls=COMMAND_CLS, help="List Application Versions"
 )
 @click.option(
     "--application-fqn",
@@ -113,22 +118,19 @@
         application_fqn=application_fqn,
     )
     if not versions:
         output_hook = RichOutputCallBack()
         output_hook.print_line(PROMPT_NO_VERSIONS)
     else:
         versions.sort(key=lambda s: s.createdAt, reverse=True)
-    if CliConfig.get("json"):
-        print_json(data=versions)
-    else:
-        # TODO (chiragjn): Display columns here need to show workspace and cluster name!
-        print_entity_list(
-            "Application Versions",
-            versions,
-        )
+
+    print_entity_list(
+        "Application Versions",
+        versions,
+    )
 
 
 def get_list_command():
     list_command.add_command(list_workspaces)
     list_command.add_command(list_applications)
     list_command.add_command(list_versions)
```

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.8.7/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/display_util.py` & `servicefoundry-0.8.7/servicefoundry/cli/display_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,69 +10,49 @@
 from servicefoundry.cli.const import DISPLAY_DATETIME_FORMAT
 from servicefoundry.json_util import json_default_encoder
 
 print_json = functools.partial(
     _rich_print_json, highlight=False, default=json_default_encoder
 )
 
+NO_WRAP_COLUMNS = {"fqn"}
+
 
 def get_table(title):
     return Table(title=title, show_lines=False, safe_box=True, box=box.MINIMAL)
 
 
 def stringify(x):
     if isinstance(x, datetime.datetime):
         return x.astimezone().strftime(DISPLAY_DATETIME_FORMAT)
     elif isinstance(x, str):
         return x
     else:
         return str(x)
 
 
-def print_list(title, items, columns=None):
-    if CliConfig.get("json"):
-        print_json(data=items)
-        return
-
-    table = get_table(title)
-
-    if items:
-        if not columns:
-            columns = items[0].keys()
-        for column in columns:
-            no_wrap = column in ["id", "fqn"]
-            table.add_column(column, justify="left", overflow="fold", no_wrap=no_wrap)
-
-    for item in items:
-        row = []
-        for c in columns:
-            row.append(stringify(item[c]))
-        table.add_row(*row)
-    console.print(table)
-
-
 def print_entity_list(title, items):
+    items = [item.list_row_data() for item in items]
     if CliConfig.get("json"):
         print_json(data=items)
         return
 
     table = get_table(title)
 
     columns = []
     if items:
-        columns = items[0].list_row_data().keys()
+        columns = items[0].keys()
         for column in columns:
-            no_wrap = "FQN" in column or "Name" in column
+            no_wrap = column in NO_WRAP_COLUMNS
             table.add_column(column, justify="left", overflow="fold", no_wrap=no_wrap)
 
     for item in items:
-        entity = item.list_row_data()
         row = []
         for c in columns:
-            row.append(stringify(entity[c]))
+            row.append(stringify(item[c]))
         table.add_row(*row)
     console.print(table)
 
 
 def print_obj(title, item, columns=None):
     if CliConfig.get("json"):
         print_json(data=item)
@@ -83,15 +63,15 @@
     if not columns:
         columns = item.keys()
 
     # transpose
     keys, columns = columns, ["key", "value"]
 
     for column in columns:
-        no_wrap = column in ["id", "fqn"]
+        no_wrap = column in NO_WRAP_COLUMNS
         table.add_column(column, justify="left", overflow="fold", no_wrap=no_wrap)
     for key in keys:
         table.add_row(f"[bold]{stringify(key)}[/]", stringify(item[key]))
     console.print(table)
 
 
 def print_entity_obj(title, entity):
```

### Comparing `servicefoundry-0.8.6/servicefoundry/cli/util.py` & `servicefoundry-0.8.7/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/__main__.py` & `servicefoundry-0.8.7/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/app.py` & `servicefoundry-0.8.7/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/build.py` & `servicefoundry-0.8.7/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.8.7/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.8.7/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/route.py` & `servicefoundry-0.8.7/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/service.py` & `servicefoundry-0.8.7/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/function_service/utils.py` & `servicefoundry-0.8.7/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/internal/experimental.py` & `servicefoundry-0.8.7/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/io/output_callback.py` & `servicefoundry-0.8.7/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.8.7/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.8.7/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.8.7/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.8.7/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.8.7/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.8.7/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.8.7/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.8.7/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.8.7/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.8.7/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.8.7/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.8.7/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.8.7/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.8.7/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.8.7/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/const.py` & `servicefoundry-0.8.7/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/dao/application.py` & `servicefoundry-0.8.7/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/dao/version.py` & `servicefoundry-0.8.7/servicefoundry/lib/dao/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from typing import Optional
+from typing import List, Optional
 
 from servicefoundry.lib.clients.service_foundry_client import (
     ServiceFoundryServiceClient,
 )
+from servicefoundry.lib.model.entity import Deployment
 
 
 def list_versions(
     application_fqn: str,
     client: Optional[ServiceFoundryServiceClient] = None,
-):
+) -> List[Deployment]:
     client = client or ServiceFoundryServiceClient()
     application = client.get_id_from_fqn(fqn=application_fqn, fqn_type="app")
     versions = client.list_versions(application_id=application["applicationId"])
     return versions
 
 
 def get_version(
     application_fqn: str,
     version: int,
     client: Optional[ServiceFoundryServiceClient] = None,
-):
+) -> Deployment:
     client = client or ServiceFoundryServiceClient()
     application = client.get_id_from_fqn(fqn=application_fqn, fqn_type="app")
     versions = client.list_versions(
         application_id=application["applicationId"], deployment_version=version
     )
     if len(versions) == 0:
         raise ValueError(
```

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.8.7/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/exceptions.py` & `servicefoundry-0.8.7/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.8.7/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.8.7/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.8.7/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.8.7/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.8.7/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.8.7/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/messages.py` & `servicefoundry-0.8.7/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/model/entity.py` & `servicefoundry-0.8.7/servicefoundry/lib/model/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import time
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 import jwt
 from pydantic import BaseModel, Extra, Field, constr, validator
 
+from servicefoundry.lib.util import get_application_fqn_from_deployment_fqn
+
 # TODO: switch to Enums for str literals
 # TODO: Need a better approach to keep fields in sync with server
 #       most fields should have a default in case server adds/removes a field
 # TODO: Implement NotImplementedError sections
 UNDEFINED_STRING = "<Undefined>"
 
 
@@ -32,71 +34,38 @@
 
 class Entity(Base):
     createdAt: datetime.datetime = Field(repr=False)
     updatedAt: datetime.datetime = Field(repr=False)
     createdBy: str = Field(repr=False)
 
 
-class Cluster(Entity):
-    id: str = Field(repr=False)
-    name: str
-    fqn: str
-    region: str = Field(repr=False)
-    isTenantDefault: bool = False
-    isAvailable: bool = False
-
-    def list_row_data(self) -> Dict[str, Any]:
-        return {
-            "ClusterName": self.name,
-            "Region": self.region,
-            "CreatedAt": self.createdAt,
-        }
-
-    def get_data(self) -> Dict[str, Any]:
-        return {
-            "ClusterName": self.name,
-            "Region": self.region,
-            "CreatedAt": self.createdAt,
-            "UpdatedAt": self.updatedAt,
-            "CreatedBy": self.createdBy,
-        }
-
-    @property
-    def workspaces(self) -> List["Workspace"]:
-        raise NotImplementedError
-
-
 class Workspace(Entity):
     id: str = Field(repr=False)
     name: str
     fqn: str
     clusterId: str = Field(repr=False)
 
     def list_row_data(self) -> Dict[str, Any]:
         return {
-            "WorkspaceName": self.name,
-            "WorkspaceFQN": self.fqn,
-            "ClusterName": self.clusterId,
-            "CreatedAt": self.createdAt,
+            "name": self.name,
+            "fqn": self.fqn,
+            "cluster_fqn": self.clusterId,
+            "created_at": self.createdAt,
         }
 
     def get_data(self) -> Dict[str, Any]:
         return {
-            "WorkspaceName": self.name,
-            "WorkspaceFQN": self.fqn,
-            "ClusterName": self.clusterId,
-            "CreatedAt": self.createdAt,
-            "UpdatedAt": self.updatedAt,
-            "CreatedBy": self.createdBy,
+            "name": self.name,
+            "fqn": self.fqn,
+            "cluster_fqn": self.clusterId,
+            "created_at": self.createdAt,
+            "updated_at": self.updatedAt,
+            "created_by": self.createdBy,
         }
 
-    @property
-    def cluster(self) -> Cluster:
-        raise NotImplementedError
-
 
 class WorkspaceResources(BaseModel):
     cpu_limit: Optional[float]
     memory_limit: Optional[int]
     ephemeral_storage_limit: Optional[int]
 
 
@@ -144,45 +113,54 @@
     fqn: str
     version: int
     currentStatusId: str = Field(repr=False)
     applicationId: str = Field(repr=False)
     manifest: DeploymentManifest = Field(repr=False)
     failureReason: Optional[str]
     deploymentStatuses: Optional[List[DeploymentStatus]]
-    # TODO: Dict -> pydantic model if required
-    # application: Dict[str, Any]
-    # TODO: Dict -> pydantic model if required
-    # workspace: Dict[str, Any]
-    # baseDomainURL: str
-    # builds: List[BuildResponse]
     metadata: Optional[
         Union[Dict[str, Any], List[Dict[str, Any]]]
     ]  # TODO (chiragjn): revisit the type of this field
     currentStatus: Optional[DeploymentStatus]  # Server was not returning CurrentStatus
+    application_fqn: str
+
+    def __init__(self, **kwargs) -> None:
+        deployment_fqn = kwargs.get("fqn")
+        if not deployment_fqn:
+            raise ValueError("'fqn' field is required")
+        application_fqn = ":".join(deployment_fqn.split(":")[:3])
+        kwargs["application_fqn"] = application_fqn
+        return super().__init__(**kwargs)
+
+    @property
+    def application_fqn(self) -> str:
+        return get_application_fqn_from_deployment_fqn(self.fqn)
 
     def list_row_data(self) -> Dict[str, Any]:
         return {
-            "DeploymentFQN": self.fqn,
-            "ApplicationName": self.manifest.name,
-            "ApplicationType": self.manifest.type,
-            "Version": self.version,
-            "CreatedAt": self.createdAt,
+            "fqn": self.fqn,
+            "application_name": self.manifest.name,
+            "version": self.version,
+            "created_at": self.createdAt,
         }
 
     def get_data(self) -> Dict[str, Any]:
-        return {
-            "DeploymentFQN": self.fqn,
-            "ApplicationName": self.manifest.name,
-            "ApplicationType": self.manifest.type,
-            "Version": self.version,
-            "WorkspaceName": self.fqn.split(":")[1],  # TODO: change hardcoding
-            "ClusterName": self.fqn.split(":")[0],  # TODO: change hardcoding
-            "CreatedAt": self.createdAt,
-            "UpdatedAt": self.updatedAt,
-            "CreatedBy": self.createdBy,
+        # TODO: Remove this splitting logic
+        cluster_fqn, workspace_name, *_ = self.fqn.split(":")
+        workspace_fqn = ":".join([cluster_fqn, workspace_name])
+        return {
+            "fqn": self.fqn,
+            "application_name": self.manifest.name,
+            "application_type": self.manifest.type,
+            "version": self.version,
+            "workspace_fqn": workspace_fqn,
+            "cluster_fqn": cluster_fqn,
+            "created_at": self.createdAt,
+            "updated_at": self.updatedAt,
+            "created_by": self.createdBy,
         }
 
     class Config:
         extra = Extra.allow
 
 
 class ApplicationWorkspace(Base):
@@ -202,33 +180,34 @@
     workspace: ApplicationWorkspace
     deployment: Deployment
     activeDeploymentId: Optional[str] = Field(repr=False)
     lastDeploymentId: str = Field(repr=False)
 
     def list_row_data(self) -> Dict[str, Any]:
         return {
-            "ApplicationName": self.name,
-            "ApplicationFQN": self.fqn,
-            "ActiveVersion": self.activeVersion,
-            "LastVersion": self.lastVersion,
-            "WorkspaceName": self.workspace.name,
-            "CreatedAt": self.createdAt,
+            "name": self.name,
+            "type": self.deployment.manifest.type,
+            "fqn": self.fqn,
+            "active_version": self.activeVersion,
+            "workspace_name": self.workspace.name,
+            "created_at": self.createdAt,
         }
 
     def get_data(self) -> Dict[str, Any]:
         return {
-            "ApplicationName": self.name,
-            "ApplicationFQN": self.fqn,
-            "ActiveVersion": self.activeVersion,
-            "LastVersion": self.lastVersion,
-            "WorkspaceFQN": self.workspace.fqn,
-            "ClusterFQN": self.workspace.clusterId,
-            "CreatedAt": self.createdAt,
-            "UpdatedAt": self.updatedAt,
-            "CreatedBy": self.createdBy,
+            "name": self.name,
+            "type": self.deployment.manifest.type,
+            "fqn": self.fqn,
+            "active_version": self.activeVersion,
+            "last_version": self.lastVersion,
+            "workspace_fqn": self.workspace.fqn,
+            "cluster_fqn": self.workspace.clusterId,
+            "created_at": self.createdAt,
+            "updated_at": self.updatedAt,
+            "created_by": self.createdBy,
         }
 
 
 class UserType(Enum):
     user = "user"
     serviceaccount = "serviceaccount"
```

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/session.py` & `servicefoundry-0.8.7/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/util.py` & `servicefoundry-0.8.7/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/lib/win32.py` & `servicefoundry-0.8.7/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/logger.py` & `servicefoundry-0.8.7/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.8.7/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.8.7/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/lib/models.py` & `servicefoundry-0.8.7/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.8.7/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/servicefoundry/v2/lib/source.py` & `servicefoundry-0.8.7/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.6/PKG-INFO` & `servicefoundry-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.8.6
+Version: 0.8.7
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```


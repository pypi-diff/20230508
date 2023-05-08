# Comparing `tmp/flytekit-1.6.0b2.tar.gz` & `tmp/flytekit-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.0b2.tar", last modified: Fri May  5 17:49:35 2023, max compression
+gzip compressed data, was "flytekit-1.6.0b3.tar", last modified: Mon May  8 20:18:31 2023, max compression
```

## Comparing `flytekit-1.6.0b2.tar` & `flytekit-1.6.0b3.tar`

### file list

```diff
@@ -1,244 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-05 17:49:34.000000 flytekit-1.6.0b2/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    29387 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.181979 flytekit-1.6.0b2/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36193 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    75520 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.185979 flytekit-1.6.0b2/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/interfaces/stats/taggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.189979 flytekit-1.6.0b2/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.193980 flytekit-1.6.0b2/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.177979 flytekit-1.6.0b2/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 17:49:35.000000 flytekit-1.6.0b2/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-05 17:49:25.000000 flytekit-1.6.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 17:49:35.197980 flytekit-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-05 17:49:34.000000 flytekit-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-08 20:18:29.000000 flytekit-1.6.0b3/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50556 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.220901 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.220901 flytekit-1.6.0b3/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    35947 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76873 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extend/backend/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extend/backend/external_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.224901 flytekit-1.6.0b3/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.228901 flytekit-1.6.0b3/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.228901 flytekit-1.6.0b3/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.228901 flytekit-1.6.0b3/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.228901 flytekit-1.6.0b3/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83386 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.228901 flytekit-1.6.0b3/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.228901 flytekit-1.6.0b3/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.216901 flytekit-1.6.0b3/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-08 20:18:31.000000 flytekit-1.6.0b3/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-08 20:18:31.000000 flytekit-1.6.0b3/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:31.000000 flytekit-1.6.0b3/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 20:18:31.000000 flytekit-1.6.0b3/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-08 20:18:31.000000 flytekit-1.6.0b3/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 20:18:31.000000 flytekit-1.6.0b3/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 20:18:20.000000 flytekit-1.6.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-08 20:18:31.232901 flytekit-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-08 20:18:29.000000 flytekit-1.6.0b3/setup.py
```

### Comparing `flytekit-1.6.0b2/LICENSE` & `flytekit-1.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/MANIFEST.in` & `flytekit-1.6.0b3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/PKG-INFO` & `flytekit-1.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b2 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b3 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b2/README.md` & `flytekit-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/__init__.py` & `flytekit-1.6.0b3/flytekit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,16 @@
 
 """
 import sys
 from typing import Generator
 
 from rich import traceback
 
+from flytekit.lazy_import.lazy_module import lazy_module
+
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
 from flytekit.core.base_sql_task import SQLTask
 from flytekit.core.base_task import SecurityContext, TaskMetadata, kwtypes
@@ -220,32 +222,31 @@
 from flytekit.core.reference_entity import LaunchPlanReference, TaskReference, WorkflowReference
 from flytekit.core.resources import Resources
 from flytekit.core.schedule import CronSchedule, FixedRate
 from flytekit.core.task import Secret, reference_task, task
 from flytekit.core.workflow import ImperativeWorkflow as Workflow
 from flytekit.core.workflow import WorkflowFailurePolicy, reference_workflow, workflow
 from flytekit.deck import Deck
-from flytekit.extras import pytorch, sklearn, tensorflow
 from flytekit.image_spec import ImageSpec
 from flytekit.loggers import logger
 from flytekit.models.common import Annotations, AuthRole, Labels
 from flytekit.models.core.execution import WorkflowExecutionPhase
 from flytekit.models.core.types import BlobType
 from flytekit.models.documentation import Description, Documentation, SourceCode
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
-from flytekit.types import directory, file, numpy, schema
+from flytekit.types import directory, file
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.0b2/flytekit/bin/entrypoint.py` & `flytekit-1.6.0b3/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.0b3/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.0b3/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/auth/keyring.py` & `flytekit-1.6.0b3/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/auth/token_client.py` & `flytekit-1.6.0b3/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/auth_helper.py` & `flytekit-1.6.0b3/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/friendly.py` & `flytekit-1.6.0b3/flytekit/clients/friendly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
                 filename=filename,
                 expires_in=expires_in_pb,
             )
         )
 
     def get_download_signed_url(
         self, native_url: str, expires_in: datetime.timedelta = None
-    ) -> _data_proxy_pb2.CreateUploadLocationResponse:
+    ) -> _data_proxy_pb2.CreateDownloadLocationRequest:
         expires_in_pb = None
         if expires_in:
             expires_in_pb = Duration()
             expires_in_pb.FromTimedelta(expires_in)
         return super(SynchronousFlyteClient, self).create_download_location(
             _data_proxy_pb2.CreateDownloadLocationRequest(
                 native_url=native_url,
```

### Comparing `flytekit-1.6.0b2/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.0b3/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.0b3/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/helpers.py` & `flytekit-1.6.0b3/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clients/raw.py` & `flytekit-1.6.0b3/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.0b3/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/helpers.py` & `flytekit-1.6.0b3/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 CTX_TEST = "test"
 CTX_PACKAGES = "pkgs"
 CTX_NOTIFICATIONS = "notifications"
 CTX_CONFIG_FILE = "config_file"
 CTX_PROJECT_ROOT = "project_root"
 CTX_MODULE = "module"
 CTX_VERBOSE = "verbose"
+CTX_COPY_ALL = "copy_all"
 
 
 project_option = _click.option(
     "-p",
     "--project",
     required=True,
     type=str,
```

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from flytekit.clis.sdk_in_container.init import init
 from flytekit.clis.sdk_in_container.launchplan import launchplan
 from flytekit.clis.sdk_in_container.local_cache import local_cache
 from flytekit.clis.sdk_in_container.package import package
 from flytekit.clis.sdk_in_container.register import register
 from flytekit.clis.sdk_in_container.run import run
 from flytekit.clis.sdk_in_container.serialize import serialize
+from flytekit.clis.sdk_in_container.serve import serve
 from flytekit.configuration.internal import LocalSDK
 from flytekit.exceptions.base import FlyteException
 from flytekit.exceptions.user import FlyteInvalidInputException
 from flytekit.loggers import cli_logger
 
 
 def validate_package(ctx, param, values):
@@ -34,35 +35,34 @@
             pkgs.append(val)
     cli_logger.debug(f"Using packages: {pkgs}")
     return pkgs
 
 
 def pretty_print_grpc_error(e: grpc.RpcError):
     if isinstance(e, grpc._channel._InactiveRpcError):  # noqa
-        click.secho(f"RPC Failed, with Status: {e.code()}", fg="red")
-        click.secho(f"\tdetails: {e.details()}", fg="magenta")
+        click.secho(f"RPC Failed, with Status: {e.code()}", fg="red", bold=True)
+        click.secho(f"\tdetails: {e.details()}", fg="magenta", bold=True)
         click.secho(f"\tDebug string {e.debug_error_string()}", dim=True)
     return
 
 
 def pretty_print_exception(e: Exception):
     if isinstance(e, click.exceptions.Exit):
         raise e
 
     if isinstance(e, click.ClickException):
         click.secho(e.message, fg="red")
         raise e
 
     if isinstance(e, FlyteException):
+        click.secho(f"Failed with Exception Code: {e._ERROR_CODE}", fg="red")  # noqa
         if isinstance(e, FlyteInvalidInputException):
             click.secho("Request rejected by the API, due to Invalid input.", fg="red")
-            click.secho(f"\tReason: {str(e)}", dim=True)
             click.secho(f"\tInput Request: {MessageToJson(e.request)}", dim=True)
-            return
-        click.secho(f"Failed with Exception: Reason: {e._ERROR_CODE}", fg="red")  # noqa
+
         cause = e.__cause__
         if cause:
             if isinstance(cause, grpc.RpcError):
                 pretty_print_grpc_error(cause)
             else:
                 click.secho(f"Underlying Exception: {cause}")
         return
@@ -130,13 +130,14 @@
 main.add_command(serialize)
 main.add_command(package)
 main.add_command(local_cache)
 main.add_command(init)
 main.add_command(run)
 main.add_command(register)
 main.add_command(backfill)
+main.add_command(serve)
 main.add_command(build)
 main.add_command(launchplan)
 main.epilog
 
 if __name__ == "__main__":
     main()
```

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dataclasses_json import DataClassJsonMixin
 from pytimeparse import parse
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
 from flytekit.clis.sdk_in_container.constants import (
     CTX_CONFIG_FILE,
+    CTX_COPY_ALL,
     CTX_DOMAIN,
     CTX_MODULE,
     CTX_PROJECT,
     CTX_PROJECT_ROOT,
 )
 from flytekit.clis.sdk_in_container.helpers import (
     FLYTE_REMOTE_INSTANCE_KEY,
@@ -509,14 +510,21 @@
             param_decls=["--destination-dir", "destination_dir"],
             required=False,
             type=str,
             default="/root",
             help="Directory inside the image where the tar file containing the code will be copied to",
         ),
         click.Option(
+            param_decls=["--copy-all", "copy_all"],
+            required=False,
+            is_flag=True,
+            default=False,
+            help="Copy all files in the source root directory to the destination directory",
+        ),
+        click.Option(
             param_decls=["-i", "--image", "image_config"],
             required=False,
             multiple=True,
             type=click.UNPROCESSED,
             callback=ImageConfig.validate_image,
             default=[DefaultImages.default_image()],
             help="Image used to register and run.",
@@ -639,14 +647,15 @@
             entity,
             project=project,
             domain=domain,
             image_config=image_config,
             destination_dir=run_level_params.get("destination_dir"),
             source_path=ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_PROJECT_ROOT),
             module_name=ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_MODULE),
+            copy_all=ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_COPY_ALL),
         )
 
         options = None
         service_account = run_level_params.get("service_account")
         if service_account:
             # options are only passed for the execution. This is to prevent errors when registering a duplicate workflow
             # It is assumed that the users expectations is to override the service account only for the execution
```

### Comparing `flytekit-1.6.0b2/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.0b3/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/configuration/__init__.py` & `flytekit-1.6.0b3/flytekit/configuration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 import typing
 from dataclasses import dataclass, field
 from io import BytesIO
 from typing import Dict, List, Optional
 
 import yaml
 from dataclasses_json import dataclass_json
-from docker_image import reference
 
 from flytekit.configuration import internal as _internal
 from flytekit.configuration.default_images import DefaultImages
 from flytekit.configuration.file import ConfigEntry, ConfigFile, get_config_file, read_file_if_exists, set_if_exists
 from flytekit.image_spec import ImageSpec
 from flytekit.image_spec.image_spec import ImageBuildEngine
 from flytekit.loggers import logger
@@ -204,14 +203,16 @@
         like the sha of the latest commit.
 
         :param optional_tag:
         :param name:
         :param Text tag: e.g. somedocker.com/myimage:someversion123
         :rtype: Text
         """
+        from docker_image import reference
+
         if pathlib.Path(tag).is_file():
             with open(tag, "r") as f:
                 image_spec_dict = yaml.safe_load(f)
                 image_spec = ImageSpec(**image_spec_dict)
                 ImageBuildEngine.build(image_spec)
                 tag = image_spec.image_name()
```

### Comparing `flytekit-1.6.0b2/flytekit/configuration/default_images.py` & `flytekit-1.6.0b3/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/configuration/feature_flags.py` & `flytekit-1.6.0b3/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/configuration/file.py` & `flytekit-1.6.0b3/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/configuration/internal.py` & `flytekit-1.6.0b3/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/annotation.py` & `flytekit-1.6.0b3/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/base_sql_task.py` & `flytekit-1.6.0b3/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/base_task.py` & `flytekit-1.6.0b3/flytekit/core/base_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.tracker import TrackedInstance
 from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError
 from flytekit.core.utils import timeit
-from flytekit.deck.deck import Deck
 from flytekit.loggers import logger
 from flytekit.models import dynamic_job as _dynamic_job
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
 from flytekit.models import task as _task_model
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.documentation import Description, Documentation
@@ -586,14 +585,16 @@
                         # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
                         key = k if k != f"o{i}" else i
                         msg = f"Failed to convert outputs of task '{self.name}' at position {key}:\n  {e}"
                         logger.error(msg)
                         raise TypeError(msg) from e
 
             if self._disable_deck is False:
+                from flytekit.deck.deck import Deck
+
                 INPUT = "input"
                 OUTPUT = "output"
 
                 input_deck = Deck(INPUT)
                 for k, v in native_inputs.items():
                     input_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_input_var(k, v)))
```

### Comparing `flytekit-1.6.0b2/flytekit/core/checkpointer.py` & `flytekit-1.6.0b3/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/class_based_resolver.py` & `flytekit-1.6.0b3/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/condition.py` & `flytekit-1.6.0b3/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/constants.py` & `flytekit-1.6.0b3/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/container_task.py` & `flytekit-1.6.0b3/flytekit/core/container_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         requests: Optional[Resources] = None,
         limits: Optional[Resources] = None,
         input_data_dir: Optional[str] = None,
         output_data_dir: Optional[str] = None,
         metadata_format: MetadataFormat = MetadataFormat.JSON,
         io_strategy: Optional[IOStrategy] = None,
         secret_requests: Optional[List[Secret]] = None,
-        pod_template: Optional[PodTemplate] = None,
+        pod_template: Optional["PodTemplate"] = None,
         pod_template_name: Optional[str] = None,
         **kwargs,
     ):
         sec_ctx = None
         if secret_requests:
             for s in secret_requests:
                 if not isinstance(s, Secret):
```

### Comparing `flytekit-1.6.0b2/flytekit/core/context_manager.py` & `flytekit-1.6.0b3/flytekit/core/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 from contextlib import contextmanager
 from contextvars import ContextVar
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from typing import Generator, List, Optional, Union
 
-from flytekit.clients import friendly as friendly_client  # noqa
 from flytekit.configuration import Config, SecretsConfig, SerializationSettings
 from flytekit.core import mock_stats, utils
 from flytekit.core.checkpointer import Checkpoint, SyncCheckpoint
 from flytekit.core.data_persistence import FileAccessProvider, default_local_file_access_provider
 from flytekit.core.node import Node
 from flytekit.interfaces.cli_identifiers import WorkflowExecutionIdentifier
 from flytekit.interfaces.stats import taggable
 from flytekit.loggers import logger, user_space_logger
 from flytekit.models.core import identifier as _identifier
 
 if typing.TYPE_CHECKING:
-    from flytekit.deck.deck import Deck
+    from flytekit import Deck
+    from flytekit.clients import friendly as friendly_client  # noqa
 
 # TODO: resolve circular import from flytekit.core.python_auto_container import TaskResolverMixin
 
 # Enables static type checking https://docs.python.org/3/library/typing.html#typing.TYPE_CHECKING
 
 flyte_context_Var: ContextVar[typing.List[FlyteContext]] = ContextVar("", default=[])
 
@@ -258,15 +258,15 @@
         """
         A list of decks of the tasks, and it will be rendered to a html at the end of the task execution.
         """
         return self._decks
 
     @property
     def default_deck(self) -> Deck:
-        from flytekit.deck.deck import Deck
+        from flytekit import Deck
 
         return Deck("default")
 
     @property
     def timeline_deck(self) -> "TimeLineDeck":  # type: ignore
         from flytekit.deck.deck import TimeLineDeck
 
@@ -547,15 +547,15 @@
     :py:class:`flytekit.FlyteContextManager` object instead.
 
     Please do not confuse this object with the :py:class:`flytekit.ExecutionParameters` object.
     """
 
     file_access: FileAccessProvider
     level: int = 0
-    flyte_client: Optional[friendly_client.SynchronousFlyteClient] = None
+    flyte_client: Optional["friendly_client.SynchronousFlyteClient"] = None
     compilation_state: Optional[CompilationState] = None
     execution_state: Optional[ExecutionState] = None
     serialization_settings: Optional[SerializationSettings] = None
     in_a_condition: bool = False
     origin_stackframe: Optional[traceback.FrameSummary] = None
 
     @property
@@ -656,15 +656,15 @@
 
     @dataclass
     class Builder(object):
         file_access: FileAccessProvider
         level: int = 0
         compilation_state: Optional[CompilationState] = None
         execution_state: Optional[ExecutionState] = None
-        flyte_client: Optional[friendly_client.SynchronousFlyteClient] = None
+        flyte_client: Optional["friendly_client.SynchronousFlyteClient"] = None
         serialization_settings: Optional[SerializationSettings] = None
         in_a_condition: bool = False
 
         def build(self) -> FlyteContext:
             return FlyteContext(
                 level=self.level + 1,
                 file_access=self.file_access,
```

### Comparing `flytekit-1.6.0b2/flytekit/core/data_persistence.py` & `flytekit-1.6.0b3/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/docstring.py` & `flytekit-1.6.0b3/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.0b3/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/gate.py` & `flytekit-1.6.0b3/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/interface.py` & `flytekit-1.6.0b3/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/launch_plan.py` & `flytekit-1.6.0b3/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/local_cache.py` & `flytekit-1.6.0b3/flytekit/core/local_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Optional
 
-import joblib
 from diskcache import Cache
 
+from flytekit import lazy_module
 from flytekit.models.literals import Literal, LiteralCollection, LiteralMap
 
+joblib = lazy_module("joblib")
+
 # Location on the filesystem where serialized objects will be stored
 # TODO: read from config
 CACHE_LOCATION = "~/.flyte/local-cache"
 
 
 def _recursive_hash_placement(literal: Literal) -> Literal:
     if literal.collection is not None:
```

### Comparing `flytekit-1.6.0b2/flytekit/core/map_task.py` & `flytekit-1.6.0b3/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/mock_stats.py` & `flytekit-1.6.0b3/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/node.py` & `flytekit-1.6.0b3/flytekit/core/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,17 @@
 
     @property
     def metadata(self) -> _workflow_model.NodeMetadata:
         return self._metadata
 
     def with_overrides(self, *args, **kwargs):
         if "node_name" in kwargs:
-            self._id = kwargs["node_name"]
+            # Convert the node name into a DNS-compliant.
+            # https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-subdomain-names
+            self._id = _dnsify(kwargs["node_name"])
         if "aliases" in kwargs:
             alias_dict = kwargs["aliases"]
             if not isinstance(alias_dict, dict):
                 raise AssertionError("Aliases should be specified as dict[str, str]")
             self._aliases = []
             for k, v in alias_dict.items():
                 self._aliases.append(_workflow_model.Alias(var=k, alias=v))
```

### Comparing `flytekit-1.6.0b2/flytekit/core/node_creation.py` & `flytekit-1.6.0b3/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/notification.py` & `flytekit-1.6.0b3/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/promise.py` & `flytekit-1.6.0b3/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/python_auto_container.py` & `flytekit-1.6.0b3/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.0b3/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/python_function_task.py` & `flytekit-1.6.0b3/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/reference.py` & `flytekit-1.6.0b3/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/reference_entity.py` & `flytekit-1.6.0b3/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/resources.py` & `flytekit-1.6.0b3/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/schedule.py` & `flytekit-1.6.0b3/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/shim_task.py` & `flytekit-1.6.0b3/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/task.py` & `flytekit-1.6.0b3/flytekit/core/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     requests: Optional[Resources] = None,
     limits: Optional[Resources] = None,
     secret_requests: Optional[List[Secret]] = None,
     execution_mode: PythonFunctionTask.ExecutionBehavior = PythonFunctionTask.ExecutionBehavior.DEFAULT,
     task_resolver: Optional[TaskResolverMixin] = None,
     docs: Optional[Documentation] = None,
     disable_deck: bool = True,
-    pod_template: Optional[PodTemplate] = None,
+    pod_template: Optional["PodTemplate"] = None,
     pod_template_name: Optional[str] = None,
 ) -> Union[Callable, PythonFunctionTask]:
     """
     This is the core decorator to use for any task type in flytekit.
 
     Tasks are the building blocks of Flyte. They represent users code. Tasks have the following properties
```

### Comparing `flytekit-1.6.0b2/flytekit/core/testing.py` & `flytekit-1.6.0b3/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/tracker.py` & `flytekit-1.6.0b3/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/type_engine.py` & `flytekit-1.6.0b3/flytekit/core/type_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 from google.protobuf import json_format as _json_format
 from google.protobuf import struct_pb2 as _struct
 from google.protobuf.json_format import MessageToDict as _MessageToDict
 from google.protobuf.json_format import ParseDict as _ParseDict
 from google.protobuf.message import Message
 from google.protobuf.struct_pb2 import Struct
 from marshmallow_enum import EnumField, LoadDumpOptions
-from marshmallow_jsonschema import JSONSchema
 from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit.core.annotation import FlyteAnnotation
 from flytekit.core.context_manager import FlyteContext
 from flytekit.core.hash import HashMethod
 from flytekit.core.type_helpers import load_type_from_tag
 from flytekit.core.utils import timeit
 from flytekit.exceptions import user as user_exceptions
+from flytekit.lazy_import.lazy_module import is_imported
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import types as _type_models
 from flytekit.models.annotation import TypeAnnotation as TypeAnnotationModel
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import (
     Blob,
@@ -325,14 +325,16 @@
         try:
             s = cast(DataClassJsonMixin, self._get_origin_type_in_annotation(t)).schema()
             for _, v in s.fields.items():
                 # marshmallow-jsonschema only supports enums loaded by name.
                 # https://github.com/fuhrysteve/marshmallow-jsonschema/blob/81eada1a0c42ff67de216923968af0a6b54e5dcb/marshmallow_jsonschema/base.py#L228
                 if isinstance(v, EnumField):
                     v.load_by = LoadDumpOptions.name
+            from marshmallow_jsonschema import JSONSchema
+
             schema = JSONSchema().dump(s)
         except Exception as e:
             # https://github.com/lovasoa/marshmallow_dataclass/issues/13
             logger.warning(
                 f"Failed to extract schema for object {t}, (will run schemaless) error: {e}"
                 f"If you have postponed annotations turned on (PEP 563) turn it off please. Postponed"
                 f"evaluation doesn't work with json dataclasses"
@@ -372,15 +374,15 @@
             for field in dataclasses.fields(copy.deepcopy(python_type)):
                 field.type = self._get_origin_type_in_annotation(field.type)
         return python_type
 
     def _fix_structured_dataset_type(self, python_type: Type[T], python_val: typing.Any) -> T:
         # In python 3.7, 3.8, DataclassJson will deserialize Annotated[StructuredDataset, kwtypes(..)] to a dict,
         # so here we convert it back to the Structured Dataset.
-        from flytekit import StructuredDataset
+        from flytekit.types.structured import StructuredDataset
 
         if python_type == StructuredDataset and type(python_val) == dict:
             return StructuredDataset(**python_val)
         elif get_origin(python_type) is list:
             return [self._fix_structured_dataset_type(get_args(python_type)[0], v) for v in python_val]  # type: ignore
         elif get_origin(python_type) is dict:
             return {  # type: ignore
@@ -668,14 +670,15 @@
     Users can implement their own TypeTransformers and register them with the TypeEngine. This will allow special handling
     of user objects
     """
 
     _REGISTRY: typing.Dict[type, TypeTransformer[T]] = {}
     _RESTRICTED_TYPES: typing.List[type] = []
     _DATACLASS_TRANSFORMER: TypeTransformer = DataclassTransformer()  # type: ignore
+    has_lazy_import = False
 
     @classmethod
     def register(
         cls,
         transformer: TypeTransformer,
         additional_types: Optional[typing.List[Type]] = None,
     ):
@@ -725,15 +728,15 @@
             This is potentially non-deterministic - will depend on the registration pattern.
 
             TODO lets make this deterministic by using an ordered dict
 
         Step 4:
             if v is of type data class, use the dataclass transformer
         """
-
+        cls.lazy_import_transformers()
         # Step 1
         if get_origin(python_type) is Annotated:
             python_type = get_args(python_type)[0]
 
         if python_type in cls._REGISTRY:
             return cls._REGISTRY[python_type]
 
@@ -768,14 +771,47 @@
         # Step 4
         if dataclasses.is_dataclass(python_type):
             return cls._DATACLASS_TRANSFORMER
 
         raise ValueError(f"Type {python_type} not supported currently in Flytekit. Please register a new transformer")
 
     @classmethod
+    def lazy_import_transformers(cls):
+        """
+        Only load the transformers if needed.
+        """
+        if cls.has_lazy_import:
+            return
+        cls.has_lazy_import = True
+        from flytekit.types.structured import (
+            register_arrow_handlers,
+            register_bigquery_handlers,
+            register_pandas_handlers,
+        )
+
+        if is_imported("tensorflow"):
+            from flytekit.extras import tensorflow  # noqa: F401
+        if is_imported("torch"):
+            from flytekit.extras import pytorch  # noqa: F401
+        if is_imported("sklearn"):
+            from flytekit.extras import sklearn  # noqa: F401
+        if is_imported("pandas"):
+            try:
+                from flytekit.types import schema  # noqa: F401
+            except ValueError:
+                logger.debug("Transformer for pandas is already registered.")
+            register_pandas_handlers()
+        if is_imported("pyarrow"):
+            register_arrow_handlers()
+        if is_imported("google.cloud.bigquery"):
+            register_bigquery_handlers()
+        if is_imported("numpy"):
+            from flytekit.types import numpy  # noqa: F401
+
+    @classmethod
     def to_literal_type(cls, python_type: Type) -> LiteralType:
         """
         Converts a python type into a flyte specific ``LiteralType``
         """
         transformer = cls.get_transformer(python_type)
         res = transformer.get_literal_type(python_type)
         data = None
```

### Comparing `flytekit-1.6.0b2/flytekit/core/type_helpers.py` & `flytekit-1.6.0b3/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/core/utils.py` & `flytekit-1.6.0b3/flytekit/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 import os as _os
 import shutil as _shutil
 import tempfile as _tempfile
 import time as _time
 from functools import wraps
 from hashlib import sha224 as _sha224
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, cast
 
 from flyteidl.core import tasks_pb2 as _core_task
-from kubernetes.client import ApiClient
-from kubernetes.client.models import V1Container, V1EnvVar, V1ResourceRequirements
 
 from flytekit.core.pod_template import PodTemplate
 from flytekit.loggers import logger
-from flytekit.models import task as _task_model
-from flytekit.models import task as task_models
+
+if TYPE_CHECKING:
+    from flytekit.models import task as task_models
 
 
 def _dnsify(value: str) -> str:
     """
     Converts value into a DNS-compliant (RFC1035/RFC1123 DNS_LABEL). The resulting string must only consist of
     alphanumeric (lower-case a-z, and 0-9) and not exceed 63 characters. It's permitted to have '-' character as long
     as it's not in the first or last positions.
@@ -56,38 +55,40 @@
     return res
 
 
 def _get_container_definition(
     image: str,
     command: List[str],
     args: Optional[List[str]] = None,
-    data_loading_config: Optional[task_models.DataLoadingConfig] = None,
+    data_loading_config: Optional["task_models.DataLoadingConfig"] = None,
     storage_request: Optional[str] = None,
     ephemeral_storage_request: Optional[str] = None,
     cpu_request: Optional[str] = None,
     gpu_request: Optional[str] = None,
     memory_request: Optional[str] = None,
     storage_limit: Optional[str] = None,
     ephemeral_storage_limit: Optional[str] = None,
     cpu_limit: Optional[str] = None,
     gpu_limit: Optional[str] = None,
     memory_limit: Optional[str] = None,
     environment: Optional[Dict[str, str]] = None,
-) -> task_models.Container:
+) -> "task_models.Container":
     storage_limit = storage_limit
     storage_request = storage_request
     ephemeral_storage_limit = ephemeral_storage_limit
     ephemeral_storage_request = ephemeral_storage_request
     cpu_limit = cpu_limit
     cpu_request = cpu_request
     gpu_limit = gpu_limit
     gpu_request = gpu_request
     memory_limit = memory_limit
     memory_request = memory_request
 
+    from flytekit.models import task as task_models
+
     # TODO: Use convert_resources_to_resource_model instead of manually fixing the resources.
     requests = []
     if storage_request:
         requests.append(
             task_models.Resources.ResourceEntry(task_models.Resources.ResourceName.STORAGE, storage_request)
         )
     if ephemeral_storage_request:
@@ -129,20 +130,25 @@
         resources=task_models.Resources(limits=limits, requests=requests),
         env=environment,
         config={},
         data_loading_config=data_loading_config,
     )
 
 
-def _sanitize_resource_name(resource: _task_model.Resources.ResourceEntry) -> str:
+def _sanitize_resource_name(resource: "task_models.Resources.ResourceEntry") -> str:
     return _core_task.Resources.ResourceName.Name(resource.name).lower().replace("_", "-")
 
 
-def _serialize_pod_spec(pod_template: PodTemplate, primary_container: _task_model.Container) -> Dict[str, Any]:
-    containers = cast(PodTemplate, pod_template).pod_spec.containers
+def _serialize_pod_spec(pod_template: "PodTemplate", primary_container: "task_models.Container") -> Dict[str, Any]:
+    from kubernetes.client import ApiClient, V1PodSpec
+    from kubernetes.client.models import V1Container, V1EnvVar, V1ResourceRequirements
+
+    if pod_template.pod_spec is None:
+        return {}
+    containers = cast(V1PodSpec, pod_template.pod_spec).containers
     primary_exists = False
 
     for container in containers:
         if container.name == cast(PodTemplate, pod_template).primary_container_name:
             primary_exists = True
             break
 
@@ -169,15 +175,15 @@
                 # Important! Only copy over resource requirements if they are non-empty.
                 container.resources = resource_requirements
             if primary_container.env is not None:
                 container.env = [V1EnvVar(name=key, value=val) for key, val in primary_container.env.items()] + (
                     container.env or []
                 )
         final_containers.append(container)
-    cast(PodTemplate, pod_template).pod_spec.containers = final_containers
+    cast(V1PodSpec, pod_template.pod_spec).containers = final_containers
 
     return ApiClient().sanitize_for_serialization(cast(PodTemplate, pod_template).pod_spec)
 
 
 def load_proto_from_file(pb2_type, path):
     with open(path, "rb") as reader:
         out = pb2_type()
```

### Comparing `flytekit-1.6.0b2/flytekit/core/workflow.py` & `flytekit-1.6.0b3/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/deck/deck.py` & `flytekit-1.6.0b3/flytekit/deck/deck.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 import os
 import typing
 from typing import Optional
 
-from jinja2 import Environment, FileSystemLoader, select_autoescape
-
 from flytekit.core.context_manager import ExecutionParameters, ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.loggers import logger
 
 OUTPUT_DIR_JUPYTER_PREFIX = "jupyter"
 DECK_FILE_NAME = "deck.html"
 
 
-try:
-    from IPython.core.display import HTML
-except ImportError:
-    ...
-
-
 class Deck:
     """
     Deck enable users to get customizable and default visibility into their tasks.
 
     Deck contains a list of renderers (FrameRenderer, MarkdownRenderer) that can
     generate a html file. For example, FrameRenderer can render a DataFrame as an HTML table,
     MarkdownRenderer can convert Markdown string to HTML
@@ -152,16 +144,20 @@
     new_user_params: ExecutionParameters, ignore_jupyter: bool = False
 ) -> typing.Union[str, "IPython.core.display.HTML"]:  # type:ignore
     """
     Get flyte deck html string
     If ignore_jupyter is set to True, then it will return a str even in a jupyter environment.
     """
     deck_map = {deck.name: deck.html for deck in new_user_params.decks}
-    raw_html = template.render(metadata=deck_map)
+    raw_html = get_deck_template().render(metadata=deck_map)
     if not ignore_jupyter and _ipython_check():
+        try:
+            from IPython.core.display import HTML
+        except ImportError:
+            ...
         return HTML(raw_html)
     return raw_html
 
 
 def _output_deck(task_name: str, new_user_params: ExecutionParameters):
     ctx = FlyteContext.current_context()
     if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
@@ -170,19 +166,22 @@
         output_dir = ctx.file_access.get_random_local_directory()
     deck_path = os.path.join(output_dir, DECK_FILE_NAME)
     with open(deck_path, "w") as f:
         f.write(_get_deck(new_user_params, ignore_jupyter=True))
     logger.info(f"{task_name} task creates flyte deck html to file://{deck_path}")
 
 
-root = os.path.dirname(os.path.abspath(__file__))
-templates_dir = os.path.join(root, "html")
-env = Environment(
-    loader=FileSystemLoader(templates_dir),
-    # 🔥 include autoescaping for security purposes
-    # sources:
-    # - https://jinja.palletsprojects.com/en/3.0.x/api/#autoescaping
-    # - https://stackoverflow.com/a/38642558/8474894 (see in comments)
-    # - https://stackoverflow.com/a/68826578/8474894
-    autoescape=select_autoescape(enabled_extensions=("html",)),
-)
-template = env.get_template("template.html")
+def get_deck_template() -> "Template":
+    from jinja2 import Environment, FileSystemLoader, select_autoescape
+
+    root = os.path.dirname(os.path.abspath(__file__))
+    templates_dir = os.path.join(root, "html")
+    env = Environment(
+        loader=FileSystemLoader(templates_dir),
+        # 🔥 include autoescaping for security purposes
+        # sources:
+        # - https://jinja.palletsprojects.com/en/3.0.x/api/#autoescaping
+        # - https://stackoverflow.com/a/38642558/8474894 (see in comments)
+        # - https://stackoverflow.com/a/68826578/8474894
+        autoescape=select_autoescape(enabled_extensions=("html",)),
+    )
+    return env.get_template("template.html")
```

### Comparing `flytekit-1.6.0b2/flytekit/deck/html/template.html` & `flytekit-1.6.0b3/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/deck/renderer.py` & `flytekit-1.6.0b3/flytekit/deck/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-import pandas
-import pyarrow
 from typing_extensions import Protocol, runtime_checkable
 
+from flytekit import lazy_module
+
+if TYPE_CHECKING:
+    # Always import these modules in type-checking mode or when running pytest
+    import pandas
+    import pyarrow
+else:
+    pandas = lazy_module("pandas")
+    pyarrow = lazy_module("pyarrow")
+
 
 @runtime_checkable
 class Renderable(Protocol):
     def to_html(self, python_value: Any) -> str:
-        """Convert a object(markdown, pandas.dataframe) to HTML and return HTML as a unicode string.
+        """Convert an object(markdown, pandas.dataframe) to HTML and return HTML as a unicode string.
         Returns: An HTML document as a string.
         """
         raise NotImplementedError
 
 
 DEFAULT_MAX_ROWS = 10
 DEFAULT_MAX_COLS = 100
@@ -23,20 +31,20 @@
     Render a DataFrame as an HTML table.
     """
 
     def __init__(self, max_rows: int = DEFAULT_MAX_ROWS, max_cols: int = DEFAULT_MAX_COLS):
         self._max_rows = max_rows
         self._max_cols = max_cols
 
-    def to_html(self, df: pandas.DataFrame) -> str:
+    def to_html(self, df: "pandas.DataFrame") -> str:
         assert isinstance(df, pandas.DataFrame)
         return df.to_html(max_rows=self._max_rows, max_cols=self._max_cols)
 
 
 class ArrowRenderer:
     """
-    Render a Arrow dataframe as an HTML table.
+    Render an Arrow dataframe as an HTML table.
     """
 
-    def to_html(self, df: pyarrow.Table) -> str:
+    def to_html(self, df: "pyarrow.Table") -> str:
         assert isinstance(df, pyarrow.Table)
         return df.to_string()
```

### Comparing `flytekit-1.6.0b2/flytekit/exceptions/scopes.py` & `flytekit-1.6.0b3/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/exceptions/system.py` & `flytekit-1.6.0b3/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/exceptions/user.py` & `flytekit-1.6.0b3/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extend/__init__.py` & `flytekit-1.6.0b3/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.0b3/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.0b3/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.0b3/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/pytorch/native.py` & `flytekit-1.6.0b3/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.0b3/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/sklearn/native.py` & `flytekit-1.6.0b3/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.0b3/flytekit/extras/sqlite3/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from flytekit import FlyteContext, kwtypes
 from flytekit.configuration import DefaultImages, SerializationSettings
 from flytekit.core.base_sql_task import SQLTask
 from flytekit.core.python_customized_container_task import PythonCustomizedContainerTask
 from flytekit.core.shim_task import ShimTaskExecutor
 from flytekit.models import task as task_models
-from flytekit.types.schema import FlyteSchema
 
 
 def unarchive_file(local_path: str, to_dir: str):
     """
     Unarchive given archive and returns the unarchived file name. It is expected that only one file is unarchived.
     More than one file or 0 files will result in a ``RuntimeError``
     """
@@ -74,20 +73,22 @@
 
     def __init__(
         self,
         name: str,
         query_template: str,
         inputs: typing.Optional[typing.Dict[str, typing.Type]] = None,
         task_config: typing.Optional[SQLite3Config] = None,
-        output_schema_type: typing.Optional[typing.Type[FlyteSchema]] = None,
+        output_schema_type: typing.Optional[typing.Type["FlyteSchema"]] = None,  # type: ignore
         container_image: typing.Optional[str] = None,
         **kwargs,
     ):
         if task_config is None or task_config.uri is None:
             raise ValueError("SQLite DB uri is required.")
+        from flytekit.types.schema import FlyteSchema
+
         outputs = kwtypes(results=output_schema_type if output_schema_type else FlyteSchema)
         super().__init__(
             name=name,
             task_config=task_config,
             # if you use your own image, keep in mind to specify the container image here
             container_image=container_image or DefaultImages.default_image(),
             executor_type=SQLite3TaskExecutor,
```

### Comparing `flytekit-1.6.0b2/flytekit/extras/tasks/shell.py` & `flytekit-1.6.0b3/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.0b3/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.0b3/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.0b3/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/image_spec/image_spec.py` & `flytekit-1.6.0b3/flytekit/image_spec/image_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from abc import abstractmethod
 from copy import copy
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import List, Optional
 
 import click
-import docker
 import requests
 from dataclasses_json import dataclass_json
-from docker.errors import APIError, ImageNotFound
 
 DOCKER_HUB = "docker.io"
 _F_IMG_ID = "_F_IMG_ID"
 
 
 @dataclass_json
 @dataclass
@@ -65,14 +63,17 @@
         return True
 
     @lru_cache
     def exist(self) -> bool:
         """
         Check if the image exists in the registry.
         """
+        import docker
+        from docker.errors import APIError, ImageNotFound
+
         try:
             client = docker.from_env()
             if self.registry:
                 client.images.get_registry_data(self.image_name())
             else:
                 client.images.get(self.image_name())
             return True
```

### Comparing `flytekit-1.6.0b2/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.0b3/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.0b3/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/interfaces/random.py` & `flytekit-1.6.0b3/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/interfaces/stats/client.py` & `flytekit-1.6.0b3/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.0b3/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/loggers.py` & `flytekit-1.6.0b3/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/admin/common.py` & `flytekit-1.6.0b3/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/admin/task_execution.py` & `flytekit-1.6.0b3/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/admin/workflow.py` & `flytekit-1.6.0b3/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/annotation.py` & `flytekit-1.6.0b3/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/array_job.py` & `flytekit-1.6.0b3/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/common.py` & `flytekit-1.6.0b3/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/catalog.py` & `flytekit-1.6.0b3/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/compiler.py` & `flytekit-1.6.0b3/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/condition.py` & `flytekit-1.6.0b3/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/errors.py` & `flytekit-1.6.0b3/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/execution.py` & `flytekit-1.6.0b3/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/identifier.py` & `flytekit-1.6.0b3/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/types.py` & `flytekit-1.6.0b3/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/core/workflow.py` & `flytekit-1.6.0b3/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/documentation.py` & `flytekit-1.6.0b3/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/dynamic_job.py` & `flytekit-1.6.0b3/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/execution.py` & `flytekit-1.6.0b3/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/filters.py` & `flytekit-1.6.0b3/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/interface.py` & `flytekit-1.6.0b3/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/launch_plan.py` & `flytekit-1.6.0b3/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/literals.py` & `flytekit-1.6.0b3/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/matchable_resource.py` & `flytekit-1.6.0b3/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/named_entity.py` & `flytekit-1.6.0b3/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/node_execution.py` & `flytekit-1.6.0b3/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/presto.py` & `flytekit-1.6.0b3/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/project.py` & `flytekit-1.6.0b3/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/qubole.py` & `flytekit-1.6.0b3/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/schedule.py` & `flytekit-1.6.0b3/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/security.py` & `flytekit-1.6.0b3/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/task.py` & `flytekit-1.6.0b3/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/types.py` & `flytekit-1.6.0b3/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/models/workflow_closure.py` & `flytekit-1.6.0b3/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/remote/__init__.py` & `flytekit-1.6.0b3/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/remote/backfill.py` & `flytekit-1.6.0b3/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/remote/entities.py` & `flytekit-1.6.0b3/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/remote/executions.py` & `flytekit-1.6.0b3/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/remote/lazy_entity.py` & `flytekit-1.6.0b3/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/remote/remote.py` & `flytekit-1.6.0b3/flytekit/remote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -795,42 +795,47 @@
         self,
         entity: typing.Union[WorkflowBase, PythonTask],
         image_config: typing.Optional[ImageConfig] = None,
         version: typing.Optional[str] = None,
         project: typing.Optional[str] = None,
         domain: typing.Optional[str] = None,
         destination_dir: str = ".",
-        default_launch_plan: typing.Optional[bool] = True,
+        copy_all: bool = False,
+        default_launch_plan: bool = True,
         options: typing.Optional[Options] = None,
         source_path: typing.Optional[str] = None,
         module_name: typing.Optional[str] = None,
     ) -> typing.Union[FlyteWorkflow, FlyteTask]:
         """
         Use this method to register a workflow via script mode.
-        :param destination_dir:
-        :param domain:
-        :param project:
-        :param image_config:
+        :param destination_dir: The destination directory where the workflow will be copied to.
+        :param copy_all: If true, the entire source directory will be copied over to the destination directory.
+        :param domain: The domain to register the workflow in.
+        :param project: The project to register the workflow in.
+        :param image_config: The image config to use for the workflow.
         :param version: version for the entity to be registered as
         :param entity: The workflow to be registered or the task to be registered
         :param default_launch_plan: This should be true if a default launch plan should be created for the workflow
         :param options: Additional execution options that can be configured for the default launchplan
         :param source_path: The root of the project path
         :param module_name: the name of the module
         :return:
         """
         if image_config is None:
             image_config = ImageConfig.auto_default_image()
 
         with tempfile.TemporaryDirectory() as tmp_dir:
-            archive_fname = pathlib.Path(os.path.join(tmp_dir, "script_mode.tar.gz"))
-            compress_scripts(source_path, str(archive_fname), module_name)
-            md5_bytes, upload_native_url = self.upload_file(
-                archive_fname, project or self.default_project, domain or self.default_domain
-            )
+            if copy_all:
+                md5_bytes, upload_native_url = self.fast_package(pathlib.Path(source_path), False, tmp_dir)
+            else:
+                archive_fname = pathlib.Path(os.path.join(tmp_dir, "script_mode.tar.gz"))
+                compress_scripts(source_path, str(archive_fname), module_name)
+                md5_bytes, upload_native_url = self.upload_file(
+                    archive_fname, project or self.default_project, domain or self.default_domain
+                )
 
         serialization_settings = SerializationSettings(
             project=project,
             domain=domain,
             image_config=image_config,
             git_repo=_get_git_repo_url(source_path),
             fast_serialization_settings=FastSerializationSettings(
```

### Comparing `flytekit-1.6.0b2/flytekit/remote/remote_callable.py` & `flytekit-1.6.0b3/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/testing/__init__.py` & `flytekit-1.6.0b3/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/fast_registration.py` & `flytekit-1.6.0b3/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/ignore.py` & `flytekit-1.6.0b3/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/module_loader.py` & `flytekit-1.6.0b3/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/repo.py` & `flytekit-1.6.0b3/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/script_mode.py` & `flytekit-1.6.0b3/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.0b3/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/subprocess.py` & `flytekit-1.6.0b3/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/tools/translator.py` & `flytekit-1.6.0b3/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/directory/__init__.py` & `flytekit-1.6.0b3/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/directory/types.py` & `flytekit-1.6.0b3/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/file/__init__.py` & `flytekit-1.6.0b3/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/file/file.py` & `flytekit-1.6.0b3/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.0b3/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/pickle/pickle.py` & `flytekit-1.6.0b3/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/schema/types.py` & `flytekit-1.6.0b3/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.0b3/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.0b3/flytekit/types/structured/basic_dfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,22 @@
 from botocore.exceptions import NoCredentialsError
 from fsspec.core import split_protocol, strip_protocol
 from fsspec.utils import get_protocol
 
 from flytekit import FlyteContext, logger
 from flytekit.configuration import DataConfig
 from flytekit.core.data_persistence import s3_setup_args
-from flytekit.deck import TopFrameRenderer
-from flytekit.deck.renderer import ArrowRenderer
 from flytekit.models import literals
 from flytekit.models.literals import StructuredDatasetMetadata
 from flytekit.models.types import StructuredDatasetType
 from flytekit.types.structured.structured_dataset import (
     PARQUET,
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
-    StructuredDatasetTransformerEngine,
 )
 
 T = TypeVar("T")
 
 
 def get_storage_options(cfg: DataConfig, uri: str, anon: bool = False) -> typing.Optional[typing.Dict]:
     protocol = get_protocol(uri)
@@ -128,16 +125,7 @@
             return pq.read_table(path, filesystem=fs, columns=columns)
         except NoCredentialsError as e:
             logger.debug("S3 source detected, attempting anonymous S3 access")
             fs = ctx.file_access.get_filesystem_for_path(uri, anonymous=True)
             if fs is not None:
                 return pq.read_table(path, filesystem=fs, columns=columns)
             raise e
-
-
-StructuredDatasetTransformerEngine.register(PandasToParquetEncodingHandler(), default_format_for_type=True)
-StructuredDatasetTransformerEngine.register(ParquetToPandasDecodingHandler(), default_format_for_type=True)
-StructuredDatasetTransformerEngine.register(ArrowToParquetEncodingHandler(), default_format_for_type=True)
-StructuredDatasetTransformerEngine.register(ParquetToArrowDecodingHandler(), default_format_for_type=True)
-
-StructuredDatasetTransformerEngine.register_renderer(pd.DataFrame, TopFrameRenderer())
-StructuredDatasetTransformerEngine.register_renderer(pa.Table, ArrowRenderer())
```

### Comparing `flytekit-1.6.0b2/flytekit/types/structured/bigquery.py` & `flytekit-1.6.0b3/flytekit/types/structured/bigquery.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from flytekit.models import literals
 from flytekit.models.types import StructuredDatasetType
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
     StructuredDatasetMetadata,
-    StructuredDatasetTransformerEngine,
 )
 
 BIGQUERY = "bq"
 
 
 def _write_to_bq(structured_dataset: StructuredDataset):
     table_id = typing.cast(str, structured_dataset.uri).split("://", 1)[1].replace(":", ".")
@@ -106,13 +105,7 @@
     def decode(
         self,
         ctx: FlyteContext,
         flyte_value: literals.StructuredDataset,
         current_task_metadata: StructuredDatasetMetadata,
     ) -> pa.Table:
         return pa.Table.from_pandas(_read_from_bq(flyte_value, current_task_metadata))
-
-
-StructuredDatasetTransformerEngine.register(PandasToBQEncodingHandlers())
-StructuredDatasetTransformerEngine.register(BQToPandasDecodingHandler())
-StructuredDatasetTransformerEngine.register(ArrowToBQEncodingHandlers())
-StructuredDatasetTransformerEngine.register(BQToArrowDecodingHandler())
```

### Comparing `flytekit-1.6.0b2/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.0b3/flytekit/types/structured/structured_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,36 @@
 import types
 import typing
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Dict, Generator, Optional, Type, Union
 
 import _datetime
-import numpy as _np
-import pandas as pd
-import pyarrow as pa
 from dataclasses_json import config, dataclass_json
 from fsspec.utils import get_protocol
 from marshmallow import fields
 from typing_extensions import Annotated, TypeAlias, get_args, get_origin
 
+from flytekit import lazy_module
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
 from flytekit.core.type_engine import TypeEngine, TypeTransformer
 from flytekit.deck.renderer import Renderable
 from flytekit.loggers import logger
 from flytekit.models import literals
 from flytekit.models import types as type_models
 from flytekit.models.literals import Literal, Scalar, StructuredDatasetMetadata
 from flytekit.models.types import LiteralType, SchemaType, StructuredDatasetType
 
+if typing.TYPE_CHECKING:
+    import pandas as pd
+    import pyarrow as pa
+else:
+    pd = lazy_module("pandas")
+    pa = lazy_module("pyarrow")
+
 T = typing.TypeVar("T")  # StructuredDataset type or a dataframe type
 DF = typing.TypeVar("DF")  # Dataframe type
 
 # For specifying the storage formats of StructuredDatasets. It's just a string, nothing fancy.
 StructuredDatasetFormat: TypeAlias = str
 
 # Storage formats
@@ -106,15 +111,15 @@
         return flyte_dataset_transformer.iter_as(
             ctx, self.literal, self._dataframe_type, updated_metadata=self.metadata
         )
 
 
 def extract_cols_and_format(
     t: typing.Any,
-) -> typing.Tuple[Type[T], Optional[typing.OrderedDict[str, Type]], Optional[str], Optional[pa.lib.Schema]]:
+) -> typing.Tuple[Type[T], Optional[typing.OrderedDict[str, Type]], Optional[str], Optional["pa.lib.Schema"]]:
     """
     Helper function, just used to iterate through Annotations and extract out the following information:
       - base type, if not Annotated, it will just be the type that was passed in.
       - column information, as a collections.OrderedDict,
       - the storage format, as a ``StructuredDatasetFormat`` (str),
       - pa.lib.Schema
 
@@ -140,15 +145,15 @@
                 if fmt != "":
                     raise ValueError(f"A format was already specified {fmt}, cannot use {aa}")
                 fmt = aa
             elif isinstance(aa, collections.OrderedDict):
                 if ordered_dict_cols is not None:
                     raise ValueError(f"Column information was already found {ordered_dict_cols}, cannot use {aa}")
                 ordered_dict_cols = aa
-            elif isinstance(aa, pa.Schema):
+            elif isinstance(aa, pa.lib.Schema):
                 if pa_schema is not None:
                     raise ValueError(f"Arrow schema was already found {pa_schema}, cannot use {aa}")
                 pa_schema = aa
         return base_type, ordered_dict_cols, fmt, pa_schema
 
     # We return None as the format instead of parquet or something because the transformer engine may find
     # a better default for the given dataframe type.
@@ -287,24 +292,16 @@
         return type_models.SimpleType.DURATION
     if column_type == SchemaType.SchemaColumn.SchemaColumnType.BOOLEAN:
         return type_models.SimpleType.BOOLEAN
     else:
         raise AssertionError(f"Unrecognized SchemaColumnType: {column_type}")
 
 
-class DuplicateHandlerError(ValueError):
-    ...
-
-
-class StructuredDatasetTransformerEngine(TypeTransformer[StructuredDataset]):
-    """
-    Think of this transformer as a higher-level meta transformer that is used for all the dataframe types.
-    If you are bringing a custom data frame type, or any data frame type, to flytekit, instead of
-    registering with the main type engine, you should register with this transformer instead.
-    """
+def get_supported_types():
+    import numpy as _np
 
     _SUPPORTED_TYPES: typing.Dict[Type, LiteralType] = {
         _np.int32: type_models.LiteralType(simple=type_models.SimpleType.INTEGER),
         _np.int64: type_models.LiteralType(simple=type_models.SimpleType.INTEGER),
         _np.uint32: type_models.LiteralType(simple=type_models.SimpleType.INTEGER),
         _np.uint64: type_models.LiteralType(simple=type_models.SimpleType.INTEGER),
         int: type_models.LiteralType(simple=type_models.SimpleType.INTEGER),
@@ -318,14 +315,27 @@
         _np.timedelta64: type_models.LiteralType(simple=type_models.SimpleType.DURATION),
         _datetime.timedelta: type_models.LiteralType(simple=type_models.SimpleType.DURATION),
         _np.string_: type_models.LiteralType(simple=type_models.SimpleType.STRING),
         _np.str_: type_models.LiteralType(simple=type_models.SimpleType.STRING),
         _np.object_: type_models.LiteralType(simple=type_models.SimpleType.STRING),
         str: type_models.LiteralType(simple=type_models.SimpleType.STRING),
     }
+    return _SUPPORTED_TYPES
+
+
+class DuplicateHandlerError(ValueError):
+    ...
+
+
+class StructuredDatasetTransformerEngine(TypeTransformer[StructuredDataset]):
+    """
+    Think of this transformer as a higher-level meta transformer that is used for all the dataframe types.
+    If you are bringing a custom data frame type, or any data frame type, to flytekit, instead of
+    registering with the main type engine, you should register with this transformer instead.
+    """
 
     ENCODERS: Dict[Type, Dict[str, Dict[str, StructuredDatasetEncoder]]] = {}
     DECODERS: Dict[Type, Dict[str, Dict[str, StructuredDatasetDecoder]]] = {}
     DEFAULT_PROTOCOLS: Dict[Type, str] = {}
     DEFAULT_FORMATS: Dict[Type, str] = {}
 
     Handlers = Union[StructuredDatasetEncoder, StructuredDatasetDecoder]
@@ -548,15 +558,15 @@
                     return Literal(scalar=Scalar(structured_dataset=python_val._literal_sd))
                 if python_val.dataframe is not None:
                     raise ValueError(
                         f"Shouldn't have specified both literal {python_val._literal_sd} and dataframe {python_val.dataframe}"
                     )
                 return Literal(scalar=Scalar(structured_dataset=python_val._literal_sd))
 
-            # 2. A task returns a python StructuredDataset with a uri.
+            # 2. A task returns a python StructuredDataset with an uri.
             # Note: this case is also what happens we start a local execution of a task with a python StructuredDataset.
             #  It gets converted into a literal first, then back into a python StructuredDataset.
             #
             # Ex.
             #   def t2(uri: str) -> Annotated[StructuredDataset, my_cols]
             #       return StructuredDataset(uri=uri)
             if python_val.dataframe is None:
@@ -794,16 +804,16 @@
         decoder = self.DECODERS[df_type][protocol][sd.metadata.structured_dataset_type.format]
         result: Union[DF, typing.Iterator[DF]] = decoder.decode(ctx, sd, updated_metadata)
         if not isinstance(result, types.GeneratorType):
             raise ValueError(f"Decoder {decoder} didn't return iterator {result} but should have from {sd}")
         return result
 
     def _get_dataset_column_literal_type(self, t: Type) -> type_models.LiteralType:
-        if t in self._SUPPORTED_TYPES:
-            return self._SUPPORTED_TYPES[t]
+        if t in get_supported_types():
+            return get_supported_types()[t]
         if hasattr(t, "__origin__") and t.__origin__ == list:
             return type_models.LiteralType(collection_type=self._get_dataset_column_literal_type(t.__args__[0]))
         if hasattr(t, "__origin__") and t.__origin__ == dict:
             return type_models.LiteralType(map_value_type=self._get_dataset_column_literal_type(t.__args__[1]))
         raise AssertionError(f"type {t} is currently not supported by StructuredDataset")
 
     def _convert_ordered_dict_of_columns_to_list(
```

### Comparing `flytekit-1.6.0b2/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.0b3/flytekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b2 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b3 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b2/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.0b3/flytekit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 flytekit/clis/sdk_in_container/launchplan.py
 flytekit/clis/sdk_in_container/local_cache.py
 flytekit/clis/sdk_in_container/package.py
 flytekit/clis/sdk_in_container/pyflyte.py
 flytekit/clis/sdk_in_container/register.py
 flytekit/clis/sdk_in_container/run.py
 flytekit/clis/sdk_in_container/serialize.py
+flytekit/clis/sdk_in_container/serve.py
 flytekit/clis/sdk_in_container/utils.py
 flytekit/configuration/__init__.py
 flytekit/configuration/default_images.py
 flytekit/configuration/feature_flags.py
 flytekit/configuration/file.py
 flytekit/configuration/internal.py
 flytekit/core/__init__.py
@@ -101,14 +102,17 @@
 flytekit/deck/html/template.html
 flytekit/exceptions/__init__.py
 flytekit/exceptions/base.py
 flytekit/exceptions/scopes.py
 flytekit/exceptions/system.py
 flytekit/exceptions/user.py
 flytekit/extend/__init__.py
+flytekit/extend/backend/__init__.py
+flytekit/extend/backend/base_plugin.py
+flytekit/extend/backend/external_plugin_service.py
 flytekit/extras/__init__.py
 flytekit/extras/cloud_pickle_resolver.py
 flytekit/extras/pytorch/__init__.py
 flytekit/extras/pytorch/checkpoint.py
 flytekit/extras/pytorch/native.py
 flytekit/extras/sklearn/__init__.py
 flytekit/extras/sklearn/native.py
@@ -125,14 +129,16 @@
 flytekit/interaction/parse_stdin.py
 flytekit/interfaces/__init__.py
 flytekit/interfaces/cli_identifiers.py
 flytekit/interfaces/random.py
 flytekit/interfaces/stats/__init__.py
 flytekit/interfaces/stats/client.py
 flytekit/interfaces/stats/taggable.py
+flytekit/lazy_import/__init__.py
+flytekit/lazy_import/lazy_module.py
 flytekit/models/__init__.py
 flytekit/models/annotation.py
 flytekit/models/array_job.py
 flytekit/models/common.py
 flytekit/models/documentation.py
 flytekit/models/dynamic_job.py
 flytekit/models/execution.py
```

### Comparing `flytekit-1.6.0b2/flytekit.egg-info/requires.txt` & `flytekit-1.6.0b3/flytekit.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 googleapis-common-protos>=1.57
-flyteidl<1.4.0,>=1.3.12
+flyteidl<1.4.0,>=1.3.16
 wheel<1.0.0,>=0.30.0
 pandas<2.0.0,>=1.0.0
 pyarrow<11.0.0,>=4.0.0
 click<9.0,>=6.6
 croniter<4.0.0,>=0.3.20
 deprecated<2.0,>=1.0
 docker<7.0.0,>=4.0.0
```

### Comparing `flytekit-1.6.0b2/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.0b3/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b2/setup.py` & `flytekit-1.6.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -25,15 +25,15 @@
             "pyflyte-map-execute=flytekit.bin.entrypoint:map_execute_task_cmd",
             "pyflyte=flytekit.clis.sdk_in_container.pyflyte:main",
             "flyte-cli=flytekit.clis.flyte_cli.main:_flyte_cli",
         ]
     },
     install_requires=[
         "googleapis-common-protos>=1.57",
-        "flyteidl>=1.3.12,<1.4.0",
+        "flyteidl>=1.3.16,<1.4.0",
         "wheel>=0.30.0,<1.0.0",
         "pandas>=1.0.0,<2.0.0",
         "pyarrow>=4.0.0,<11.0.0",
         "click>=6.6,<9.0",
         "croniter>=0.3.20,<4.0.0",
         "deprecated>=1.0,<2.0",
         "docker>=4.0.0,<7.0.0",
```


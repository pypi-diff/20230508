# Comparing `tmp/tecton-0.7.0b8.tar.gz` & `tmp/tecton-0.7.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.7.0b8.tar", last modified: Tue Mar 28 20:28:16 2023, max compression
+gzip compressed data, was "tecton-0.7.0b9.tar", last modified: Thu Mar 30 19:24:57 2023, max compression
```

## Comparing `tecton-0.7.0b8.tar` & `tecton-0.7.0b9.tar`

### file list

```diff
@@ -1,522 +1,522 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.675367 tecton-0.7.0b8/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-03-28 20:28:13.000000 tecton-0.7.0b8/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3827 2023-03-28 20:28:16.675367 tecton-0.7.0b8/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-03-28 20:28:13.000000 tecton-0.7.0b8/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.623363 tecton-0.7.0b8/protoc_gen_swagger/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/protoc_gen_swagger/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.623363 tecton-0.7.0b8/protoc_gen_swagger/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/protoc_gen_swagger/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-03-28 20:28:13.000000 tecton-0.7.0b8/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-03-28 20:28:13.000000 tecton-0.7.0b8/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-03-28 20:28:16.675367 tecton-0.7.0b8/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     1992 2023-03-28 20:28:13.000000 tecton-0.7.0b8/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.623363 tecton-0.7.0b8/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3055 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.627363 tecton-0.7.0b8/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11203 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2190 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1197 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6128 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7859 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25363 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      536 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/fco.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      845 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12977 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      694 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.627363 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3170 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3122 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2511 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      197 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13751 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/query_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.627363 tecton-0.7.0b8/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11216 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10766 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15738 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8634 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8711 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    24254 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2842 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5971 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2008 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15447 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6177 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_internals/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      276 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      790 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.631363 tecton-0.7.0b8/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8927 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4055 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29966 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5957 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16440 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25059 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7948 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1663 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5814 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6468 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.631363 tecton-0.7.0b8/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6580 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    83902 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17157 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31192 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10624 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7570 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33317 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157104 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22597 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1821 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20947 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.631363 tecton-0.7.0b8/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1493 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3938 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10448 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1658 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3036 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2772 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2543 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.631363 tecton-0.7.0b8/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.631363 tecton-0.7.0b8/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.635364 tecton-0.7.0b8/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.635364 tecton-0.7.0b8/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.635364 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.639364 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.639364 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.643364 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.643364 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.643364 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.647365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.647365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.647365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.647365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.647365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.647365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.651365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.651365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.651365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.651365 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.627363 tecton-0.7.0b8/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3827 2023-03-28 20:28:15.000000 tecton-0.7.0b8/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17884 2023-03-28 20:28:15.000000 tecton-0.7.0b8/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-03-28 20:28:15.000000 tecton-0.7.0b8/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-03-28 20:28:15.000000 tecton-0.7.0b8/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      740 2023-03-28 20:28:15.000000 tecton-0.7.0b8/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-03-28 20:28:15.000000 tecton-0.7.0b8/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.651365 tecton-0.7.0b8/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14614 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8209 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5682 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/odfv_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16733 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21428 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.655365 tecton-0.7.0b8/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.655365 tecton-0.7.0b8/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10493 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18433 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6080 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4647 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4778 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15218 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8508 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2820 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1304 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/logger.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7353 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/materialization_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6633 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5905 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/pipeline_common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4367 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/pipeline_sql_builder.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.655365 tecton-0.7.0b8/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5273 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    24787 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8386 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    65452 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      496 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9100 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4764 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      765 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5523 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/schema_derivation_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      675 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34455 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1418 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5529 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29070 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3779 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2571 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6453 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37459 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38057 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8623 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17024 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2596 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6198 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4030 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30162 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5930 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4097 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6767 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.659366 tecton-0.7.0b8/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15940 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1814 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2917 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.663366 tecton-0.7.0b8/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.663366 tecton-0.7.0b8/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2661 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2204 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1626 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1196 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/common/spark_schema_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.663366 tecton-0.7.0b8/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2807 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6005 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4220 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14378 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5367 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11550 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3365 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1933 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9096 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1527 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7893 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2409 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5452 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4048 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12602 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6373 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2655 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9600 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   107701 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3450 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.667366 tecton-0.7.0b8/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7176 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.671367 tecton-0.7.0b8/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6508 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.671367 tecton-0.7.0b8/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.671367 tecton-0.7.0b8/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29291 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4384 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1993 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29771 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.671367 tecton-0.7.0b8/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      909 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      383 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      350 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7311 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1549 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2241 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6740 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.675367 tecton-0.7.0b8/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      454 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14566 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1704 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34514 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      403 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/feature_view_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2926 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/ingest_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.675367 tecton-0.7.0b8/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1567067 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4180 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22007 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10610 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29804 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:16.675367 tecton-0.7.0b8/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3395 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8467 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18311 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3603 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5862 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5066 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1052 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11008 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4852 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2150 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4850 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      414 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3243 2023-03-28 20:28:13.000000 tecton-0.7.0b8/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.562433 tecton-0.7.0b9/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-03-30 19:24:54.000000 tecton-0.7.0b9/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3827 2023-03-30 19:24:57.562433 tecton-0.7.0b9/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-03-30 19:24:54.000000 tecton-0.7.0b9/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.514429 tecton-0.7.0b9/protoc_gen_swagger/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/protoc_gen_swagger/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.514429 tecton-0.7.0b9/protoc_gen_swagger/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/protoc_gen_swagger/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-03-30 19:24:54.000000 tecton-0.7.0b9/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-03-30 19:24:54.000000 tecton-0.7.0b9/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-03-30 19:24:57.562433 tecton-0.7.0b9/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     1997 2023-03-30 19:24:54.000000 tecton-0.7.0b9/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.514429 tecton-0.7.0b9/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3055 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.518430 tecton-0.7.0b9/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11203 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2190 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1197 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6128 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7859 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25363 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      536 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/fco.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      845 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12977 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      694 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.518430 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3170 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3122 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2511 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      197 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13751 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/query_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.518430 tecton-0.7.0b9/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11216 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10766 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15738 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8634 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8711 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    24254 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2842 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5971 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2008 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15447 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6197 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_internals/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      276 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      790 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.518430 tecton-0.7.0b9/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8927 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4055 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29966 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5957 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16440 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25059 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7948 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1663 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5814 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6468 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.522430 tecton-0.7.0b9/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6580 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    83902 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17157 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31192 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10624 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7570 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33317 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157104 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22597 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1821 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20947 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.522430 tecton-0.7.0b9/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1493 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3938 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10448 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1658 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3036 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2772 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2543 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.522430 tecton-0.7.0b9/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.522430 tecton-0.7.0b9/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.522430 tecton-0.7.0b9/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.522430 tecton-0.7.0b9/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.526430 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.526430 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.526430 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.530431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.530431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.530431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.530431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.530431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.534431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.534431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.534431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.534431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.534431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.534431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.538431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.538431 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.514429 tecton-0.7.0b9/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3827 2023-03-30 19:24:56.000000 tecton-0.7.0b9/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17884 2023-03-30 19:24:56.000000 tecton-0.7.0b9/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-03-30 19:24:56.000000 tecton-0.7.0b9/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-03-30 19:24:56.000000 tecton-0.7.0b9/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      745 2023-03-30 19:24:56.000000 tecton-0.7.0b9/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-03-30 19:24:56.000000 tecton-0.7.0b9/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.538431 tecton-0.7.0b9/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14614 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8209 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5682 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/odfv_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16733 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21428 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.538431 tecton-0.7.0b9/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10493 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18433 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6080 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4647 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4778 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15218 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8508 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2820 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1304 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/logger.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7353 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/materialization_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6633 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5905 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/pipeline_common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4367 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/pipeline_sql_builder.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5273 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    24787 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8386 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    65452 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      496 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9100 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4764 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      765 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5523 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/schema_derivation_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      675 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34465 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1418 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5529 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29070 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3779 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2581 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6453 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37459 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.542431 tecton-0.7.0b9/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    38057 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8623 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.546432 tecton-0.7.0b9/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17024 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2596 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6198 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4030 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30162 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5930 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4097 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6767 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.546432 tecton-0.7.0b9/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15940 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1814 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2917 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.546432 tecton-0.7.0b9/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.546432 tecton-0.7.0b9/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2661 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2204 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1626 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1196 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/common/spark_schema_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.546432 tecton-0.7.0b9/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2807 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.550432 tecton-0.7.0b9/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6005 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4220 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14378 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5367 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11550 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3365 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1933 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9336 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1527 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.550432 tecton-0.7.0b9/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7943 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.550432 tecton-0.7.0b9/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2409 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5532 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4048 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.550432 tecton-0.7.0b9/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.550432 tecton-0.7.0b9/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12602 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.550432 tecton-0.7.0b9/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6373 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2655 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9600 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109537 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3450 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7176 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29291 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6514 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1993 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29771 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.554432 tecton-0.7.0b9/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      909 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      383 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      350 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7311 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1549 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2241 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6740 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.558433 tecton-0.7.0b9/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      454 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14566 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1704 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34514 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      403 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/feature_view_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2926 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/ingest_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.558433 tecton-0.7.0b9/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1567067 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4180 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22007 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10610 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29804 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:57.562433 tecton-0.7.0b9/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3395 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8467 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18311 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3603 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5862 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5066 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1052 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11008 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4852 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2150 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4850 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      414 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3243 2023-03-30 19:24:54.000000 tecton-0.7.0b9/tecton_spark/udfs.py
```

### Comparing `tecton-0.7.0b8/PKG-INFO` & `tecton-0.7.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.7.0b8
+Version: 0.7.0b9
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.7.0b8/README.md` & `tecton-0.7.0b9/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/protoc_gen_swagger/options/annotations_pb2.py` & `tecton-0.7.0b9/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/protoc_gen_swagger/options/openapiv2_pb2.py` & `tecton-0.7.0b9/protoc_gen_swagger/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/setup.py` & `tecton-0.7.0b9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.7.0b8',
+    version='0.7.0b9',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0.3', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf~=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas~=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard', 'sqlparse', 'semantic_version'],
+    install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0.3', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf~=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas~=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version'],
     extras_require={'databricks-connect': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'pyspark': ['pyspark[sql]~=3.1.2'], 'pyspark3': ['pyspark[sql]~=3.1.2'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'snowflake': ['snowflake-connector-python[pandas]~=2.8'], 'snowpark': ['snowflake-snowpark-python[pandas]~=1.0.0'], 'athena': ['awswrangler~=2.15']},
     packages=packages,
 )
```

### Comparing `tecton-0.7.0b8/tecton/__init__.py` & `tecton-0.7.0b9/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/analytics.py` & `tecton-0.7.0b9/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/athena_api.py` & `tecton-0.7.0b9/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/data_frame_helper.py` & `tecton-0.7.0b9/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/delete_keys_api.py` & `tecton-0.7.0b9/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/display.py` & `tecton-0.7.0b9/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/env_utils.py` & `tecton-0.7.0b9/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/errors.py` & `tecton-0.7.0b9/tecton/_internals/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/fco.py` & `tecton-0.7.0b9/tecton/_internals/fco.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/find_spark.py` & `tecton-0.7.0b9/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/materialization_api.py` & `tecton-0.7.0b9/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/metadata_service.py` & `tecton-0.7.0b9/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/metadata_service_impl/error_lib.py` & `tecton-0.7.0b9/tecton/_internals/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/metadata_service_impl/http_client.py` & `tecton-0.7.0b9/tecton/_internals/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.7.0b9/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/metadata_service_impl/response.py` & `tecton-0.7.0b9/tecton/_internals/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/metadata_service_impl/service_calls.py` & `tecton-0.7.0b9/tecton/_internals/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/query_helper.py` & `tecton-0.7.0b9/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/repo/function_serialization.py` & `tecton-0.7.0b9/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/rewrite.py` & `tecton-0.7.0b9/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/run_api.py` & `tecton-0.7.0b9/tecton/_internals/run_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/sdk_decorators.py` & `tecton-0.7.0b9/tecton/_internals/sdk_decorators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/snowflake_api.py` & `tecton-0.7.0b9/tecton/_internals/snowflake_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/spark_api.py` & `tecton-0.7.0b9/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/spark_utils.py` & `tecton-0.7.0b9/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/time_utils.py` & `tecton-0.7.0b9/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/type_utils.py` & `tecton-0.7.0b9/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/utils.py` & `tecton-0.7.0b9/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/_internals/validations_api.py` & `tecton-0.7.0b9/tecton/_internals/validations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,16 @@
     validation_request: validator_pb2.ValidationRequest,
     indentation_level: int,
 ) -> None:
     """Run validation against the Tecton backend.
 
     Raises an exception if validation fails. Prints message if successful.
     """
-    validation_request = metadata_service_pb2.ValidateLocalFcoRequest(
+    validation_local_fco_request = metadata_service_pb2.ValidateLocalFcoRequest(
         sdk_version=tecton_version.get_semantic_version() or "",
         validation_request=validation_request,
     )
-    response = metadata_service.instance().ValidateLocalFco(validation_request).response_proto
+    response = metadata_service.instance().ValidateLocalFco(validation_local_fco_request).response_proto
     if response.success:
         print_validation_success(tecton_object, indentation_level)
     else:
         raise errors.TectonValidationError(format_server_errors(tecton_object, response))
```

### Comparing `tecton-0.7.0b8/tecton/aggregation_functions.py` & `tecton-0.7.0b9/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/access_control.py` & `tecton-0.7.0b9/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/api_key.py` & `tecton-0.7.0b9/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/cli.py` & `tecton-0.7.0b9/tecton/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/cli_utils.py` & `tecton-0.7.0b9/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/command.py` & `tecton-0.7.0b9/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/common.py` & `tecton-0.7.0b9/tecton/cli/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/engine.py` & `tecton-0.7.0b9/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/engine_renderer.py` & `tecton-0.7.0b9/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/error_utils.py` & `tecton-0.7.0b9/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/printer.py` & `tecton-0.7.0b9/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/service_account.py` & `tecton-0.7.0b9/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/cli/workspace.py` & `tecton-0.7.0b9/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/fco_listers.py` & `tecton-0.7.0b9/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/base_tecton_object.py` & `tecton-0.7.0b9/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/compute_mode.py` & `tecton-0.7.0b9/tecton/framework/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/configs.py` & `tecton-0.7.0b9/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/data_frame.py` & `tecton-0.7.0b9/tecton/framework/data_frame.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/data_source.py` & `tecton-0.7.0b9/tecton/framework/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/dataset.py` & `tecton-0.7.0b9/tecton/framework/dataset.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/entity.py` & `tecton-0.7.0b9/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/feature_service.py` & `tecton-0.7.0b9/tecton/framework/feature_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/feature_view.py` & `tecton-0.7.0b9/tecton/framework/feature_view.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/filtered_source.py` & `tecton-0.7.0b9/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/transformation.py` & `tecton-0.7.0b9/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/utils.py` & `tecton-0.7.0b9/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/validation_mode.py` & `tecton-0.7.0b9/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/framework/workspace.py` & `tecton-0.7.0b9/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/identities/api_keys.py` & `tecton-0.7.0b9/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/identities/credentials.py` & `tecton-0.7.0b9/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/identities/okta.py` & `tecton-0.7.0b9/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/pytest_tecton.py` & `tecton-0.7.0b9/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/snowflake_context.py` & `tecton-0.7.0b9/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/tecton_context.py` & `tecton-0.7.0b9/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/types.py` & `tecton-0.7.0b9/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/__diff.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/__init__.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/_dill.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/_objects.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/detect.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/info.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/pointers.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/settings.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/source.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/dill/dill/temp.py` & `tecton-0.7.0b9/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.7.0b9/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/vendor_dill.py` & `tecton-0.7.0b9/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/vendor/vendor_pyspark.py` & `tecton-0.7.0b9/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton/version.py` & `tecton-0.7.0b9/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton.egg-info/PKG-INFO` & `tecton-0.7.0b9/tecton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.7.0b8
+Version: 0.7.0b9
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.7.0b8/tecton.egg-info/SOURCES.txt` & `tecton-0.7.0b9/tecton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton.egg-info/requires.txt` & `tecton-0.7.0b9/tecton.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 colorama~=0.4
 tqdm~=4.41
 yaspin<3,>=0.16
 typing-extensions~=4.1
 pygments>=2.7.4
 pytest
 click~=8.0
-typeguard
+typeguard~=2.0
 sqlparse
 semantic_version
 
 [athena]
 awswrangler~=2.15
 
 [databricks-connect]
```

### Comparing `tecton-0.7.0b8/tecton_athena/athena_session.py` & `tecton-0.7.0b9/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/data_catalog_helper.py` & `tecton-0.7.0b9/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/odfv_helper.py` & `tecton-0.7.0b9/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/pipeline_helper.py` & `tecton-0.7.0b9/tecton_athena/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/sql_helper.py` & `tecton-0.7.0b9/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/templates/create_table.sql` & `tecton-0.7.0b9/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/templates/historical_features.sql` & `tecton-0.7.0b9/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/templates/materialization_tile.sql` & `tecton-0.7.0b9/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.7.0b9/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/templates/time_limit.sql` & `tecton-0.7.0b9/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_athena/templates_utils.py` & `tecton-0.7.0b9/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/aggregation_utils.py` & `tecton-0.7.0b9/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/conf.py` & `tecton-0.7.0b9/tecton_core/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/data_types.py` & `tecton-0.7.0b9/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/errors.py` & `tecton-0.7.0b9/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/fco_container.py` & `tecton-0.7.0b9/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/feature_definition_wrapper.py` & `tecton-0.7.0b9/tecton_core/feature_definition_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/feature_set_config.py` & `tecton-0.7.0b9/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/feature_view_utils.py` & `tecton-0.7.0b9/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/function_deserialization.py` & `tecton-0.7.0b9/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/id_helper.py` & `tecton-0.7.0b9/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/logger.py` & `tecton-0.7.0b9/tecton_core/logger.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/materialization_context.py` & `tecton-0.7.0b9/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/offline_store.py` & `tecton-0.7.0b9/tecton_core/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/online_serving_index.py` & `tecton-0.7.0b9/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/pipeline_common.py` & `tecton-0.7.0b9/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/pipeline_sql_builder.py` & `tecton-0.7.0b9/tecton_core/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/query/aggregation_plans.py` & `tecton-0.7.0b9/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/query/builder.py` & `tecton-0.7.0b9/tecton_core/query/builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/query/node_interface.py` & `tecton-0.7.0b9/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/query/nodes.py` & `tecton-0.7.0b9/tecton_core/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/query/sql_compat.py` & `tecton-0.7.0b9/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/repo_file_handler.py` & `tecton-0.7.0b9/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/schema.py` & `tecton-0.7.0b9/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/schema_derivation_utils.py` & `tecton-0.7.0b9/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/specs/__init__.py` & `tecton-0.7.0b9/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/specs/data_source_spec.py` & `tecton-0.7.0b9/tecton_core/specs/data_source_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
 
 @utils.frozen_strict
 class StreamSourceSpec:
     """Base class for stream source specs, e.g. a KinesisSourceSpec or KafkaSourceSpec."""
 
     deduplication_column_names: Tuple[str, ...]
     options: Tuple[StreamOptionSpec, ...]
-    watermark_delay_threshold: pendulum.duration
+    watermark_delay_threshold: pendulum.Duration
     spark_schema: spark_schema_pb2.SparkSchema
 
 
 @typechecked
 def create_stream_source_from_data_proto(
     proto: stream_data_source__data_pb2.StreamDataSource, deserialize_funcs_to_main: bool = False
 ) -> Optional[Union["KinesisSourceSpec", "KafkaSourceSpec", "SparkStreamSourceSpec"]]:
@@ -564,15 +564,15 @@
 
 
 @utils.frozen_strict
 class KinesisSourceSpec(StreamSourceSpec):
     post_processor: Callable = attrs.field(metadata={utils.LOCAL_REMOTE_DIVERGENCE_ALLOWED: True})
     stream_name: str
     region: str
-    initial_stream_position: data_source_config_pb2.InitialStreamPosition
+    initial_stream_position: data_source_config_pb2.InitialStreamPosition.ValueType
 
     @classmethod
     @typechecked
     def from_data_proto(
         cls, proto: stream_data_source__data_pb2.StreamDataSource, deserialize_funcs_to_main: bool = False
     ) -> "KinesisSourceSpec":
         post_processor = None
```

### Comparing `tecton-0.7.0b8/tecton_core/specs/entity_spec.py` & `tecton-0.7.0b9/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/specs/feature_service_spec.py` & `tecton-0.7.0b9/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/specs/feature_view_spec.py` & `tecton-0.7.0b9/tecton_core/specs/feature_view_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/specs/tecton_object_spec.py` & `tecton-0.7.0b9/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/specs/transformation_spec.py` & `tecton-0.7.0b9/tecton_core/specs/transformation_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from tecton_proto.data import transformation_pb2 as transformation__data_pb2
 
 __all__ = ["TransformationSpec"]
 
 
 @utils.frozen_strict
 class TransformationSpec(tecton_object_spec.TectonObjectSpec):
-    transformation_mode: transformation__args_pb2.TransformationMode
+    transformation_mode: transformation__args_pb2.TransformationMode.ValueType
     user_function: Callable = attrs.field(metadata={utils.LOCAL_REMOTE_DIVERGENCE_ALLOWED: True})
 
     # Temporarily expose the underlying data proto during migration.
     # TODO(TEC-12443): Remove this attribute.
     data_proto: Optional[transformation__data_pb2.Transformation] = attrs.field(
         metadata={utils.LOCAL_REMOTE_DIVERGENCE_ALLOWED: True}
     )
```

### Comparing `tecton-0.7.0b8/tecton_core/specs/utils.py` & `tecton-0.7.0b9/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/time_utils.py` & `tecton-0.7.0b9/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/treelib/__init__.py` & `tecton-0.7.0b9/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.7.0b9/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/treelib/misc.py` & `tecton-0.7.0b9/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/treelib/node.py` & `tecton-0.7.0b9/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/treelib/plugins.py` & `tecton-0.7.0b9/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/treelib/tree.py` & `tecton-0.7.0b9/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_core/vendor/vendor_treelib.py` & `tecton-0.7.0b9/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.7.0b9/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.7.0b9/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.7.0b9/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.7.0b9/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/basic_info_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/data_source_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/diff_options_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/diff_test_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/entity_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/fco_args_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/feature_service_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/feature_view_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/pipeline_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/transformation_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.7.0b9/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/auth/acl_pb2.py` & `tecton-0.7.0b9/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.7.0b9/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/auth/principal_pb2.py` & `tecton-0.7.0b9/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/auth/resource_pb2.py` & `tecton-0.7.0b9/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/auth/service_pb2.py` & `tecton-0.7.0b9/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.7.0b9/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/column_type_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/data_type_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/framework_version_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/id_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/pair_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/schema_container_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/schema_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/secret_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.7.0b9/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.7.0b9/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/entity_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/fco_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/feature_service_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/feature_store_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/feature_view_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/onboarding_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/serving_status_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/state_update_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/summary_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/transformation_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from tecton_proto.common import secret_pb2 as tecton__proto_dot_common_dot_secret__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0tecton_proto/data/user_deployment_settings.proto\x12\x11tecton_proto.data\x1a tecton_proto/common/secret.proto\"\xfa\x02\n\x16UserDeploymentSettings\x12G\n user_deployment_settings_version\x18\x01 \x01(\x05R\x1duserDeploymentSettingsVersion\x12R\n\x11\x64\x61tabricks_config\x18\x02 \x01(\x0b\x32#.tecton_proto.data.DatabricksConfigH\x00R\x10\x64\x61tabricksConfig\x12T\n\x13user_spark_settings\x18\x03 \x01(\x0b\x32$.tecton_proto.data.UserSparkSettingsR\x11userSparkSettings\x12O\n\x0ftenant_settings\x18\x05 \x01(\x0b\x32&.tecton_proto.data.TenantSettingsProtoR\x0etenantSettingsB\x16\n\x14\x64\x61ta_platform_configJ\x04\x08\x04\x10\x05\"\xdf\x01\n\x10\x44\x61tabricksConfig\x12#\n\rworkspace_url\x18\x01 \x01(\tR\x0cworkspaceUrl\x12\x38\n\tapi_token\x18\x02 \x01(\x0b\x32\x1b.tecton_proto.common.SecretR\x08\x61piToken\x12\x1b\n\tuser_name\x18\x03 \x01(\tR\x08userName\x12*\n\x11user_display_name\x18\x04 \x01(\tR\x0fuserDisplayName\x12#\n\rspark_version\x18\x05 \x01(\tR\x0csparkVersion\"\xd7\x01\n\x11UserSparkSettings\x12\x30\n\x14instance_profile_arn\x18\x01 \x01(\tR\x12instanceProfileArn\x12R\n\nspark_conf\x18\x02 \x03(\x0b\x32\x33.tecton_proto.data.UserSparkSettings.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x94\x06\n\x13TenantSettingsProto\x12M\n\x14\x63hronosphere_api_key\x18\x01 \x01(\x0b\x32\x1b.tecton_proto.common.SecretR\x12\x63hronosphereApiKey\x12I\n!chronosphere_restrict_label_value\x18\x04 \x01(\tR\x1e\x63hronosphereRestrictLabelValue\x12M\n pseudonymize_amplitude_user_name\x18\x02 \x01(\x08:\x04trueR\x1dpseudonymizeAmplitudeUserName\x12T\n\'enable_user_editing_deployment_settings\x18\x03 \x01(\x08R#enableUserEditingDeploymentSettings\x12-\n\x13okta_admin_group_id\x18\x05 \x01(\tR\x10oktaAdminGroupId\x12+\n\x12okta_user_group_id\x18\x06 \x01(\tR\x0foktaUserGroupId\x12\x39\n\x19\x62\x61se_metadata_service_url\x18\x07 \x01(\tR\x16\x62\x61seMetadataServiceUrl\x12\x37\n\x18\x62\x61se_feature_service_url\x18\x08 \x01(\tR\x15\x62\x61seFeatureServiceUrl\x12:\n\x19spicedb_organization_name\x18\t \x01(\tR\x17spicedbOrganizationName\x12=\n\x1b\x63ustomer_facing_tenant_name\x18\n \x01(\tR\x18\x63ustomerFacingTenantName\x12\x41\n\x0c\x61ws_settings\x18\x0b \x01(\x0b\x32\x1e.tecton_proto.data.AwsSettingsR\x0b\x61wsSettings\x12\x30\n\x14internal_tenant_name\x18\x0c \x01(\tR\x12internalTenantName\"\xa8\x05\n\x0b\x41wsSettings\x12>\n\x0b\x64ynamo_role\x18\x06 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\ndynamoRole\x12_\n\x11\x64ynamo_extra_tags\x18\x08 \x03(\x0b\x32\x33.tecton_proto.data.AwsSettings.DynamoExtraTagsEntryR\x0f\x64ynamoExtraTags\x12\x62\n\x12\x63ompute_extra_tags\x18\t \x03(\x0b\x32\x34.tecton_proto.data.AwsSettings.ComputeExtraTagsEntryR\x10\x63omputeExtraTags\x12\x41\n\x0c\x65mr_settings\x18\x0c \x01(\x0b\x32\x1e.tecton_proto.data.EmrSettingsR\x0b\x65mrSettings\x12Q\n\x12\x64ynamo_table_names\x18\r \x01(\x0b\x32#.tecton_proto.data.DynamoTableNamesR\x10\x64ynamoTableNames\x12]\n\x16object_store_locations\x18\x0e \x01(\x0b\x32\'.tecton_proto.data.ObjectStoreLocationsR\x14objectStoreLocations\x1a\x42\n\x14\x44ynamoExtraTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a\x43\n\x15\x43omputeExtraTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01J\x04\x08\x01\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\x94\x01\n\nAwsIamRole\x12\x19\n\x08role_arn\x18\x01 \x01(\tR\x07roleArn\x12J\n\x11intermediate_role\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\x10intermediateRole\x12\x1f\n\x0b\x65xternal_id\x18\x03 \x01(\tR\nexternalId\"S\n\nS3Location\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x31\n\x04role\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\x04role\"\"\n\x0c\x44\x42\x46SLocation\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"\xad\x01\n\x13ObjectStoreLocation\x12@\n\x0bs3_location\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.S3LocationH\x00R\ns3Location\x12\x46\n\rdbfs_location\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.DBFSLocationH\x00R\x0c\x64\x62\x66sLocationB\x0c\n\nstore_type\"V\n\x0b\x45mrSettings\x12G\n\x10\x65mr_control_role\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\x0e\x65mrControlRole\"\xa8\x03\n\x10\x44ynamoTableNames\x12*\n\x11\x64\x61ta_table_prefix\x18\x01 \x01(\tR\x0f\x64\x61taTablePrefix\x12*\n\x11status_table_name\x18\x02 \x01(\tR\x0fstatusTableName\x12\x42\n\x1ejob_idempotence_key_table_name\x18\x03 \x01(\tR\x1ajobIdempotenceKeyTableName\x12*\n\x11\x63\x61nary_table_name\x18\x04 \x01(\tR\x0f\x63\x61naryTableName\x12/\n\x14\x64\x65lta_log_table_name\x18\x05 \x01(\tR\x11\x64\x65ltaLogTableName\x12.\n\x13metric_table_prefix\x18\x06 \x01(\tR\x11metricTablePrefix\x12\x34\n\x17\x64\x65lta_log_table_name_v2\x18\x07 \x01(\tR\x13\x64\x65ltaLogTableNameV2\x12\x35\n\x17job_metadata_table_name\x18\x08 \x01(\tR\x14jobMetadataTableName\"\xe0\x07\n\x14ObjectStoreLocations\x12P\n\x0fmaterialization\x18\x01 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x0fmaterialization\x12Y\n\x14streaming_checkpoint\x18\x02 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x13streamingCheckpoint\x12h\n\x1c\x66\x65\x61ture_server_configuration\x18\x03 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x1a\x66\x65\x61tureServerConfiguration\x12I\n\x0c\x66\x65\x61ture_repo\x18\x04 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x0b\x66\x65\x61tureRepo\x12G\n\x0b\x65mr_scripts\x18\x05 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\nemrScripts\x12]\n\x16materialization_params\x18\x06 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x15materializationParams\x12S\n\x11intermediate_data\x18\x07 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x10intermediateData\x12\\\n\x16\x66\x65\x61ture_server_logging\x18\x08 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x14\x66\x65\x61tureServerLogging\x12\\\n\x16kafka_credentials_base\x18\t \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x14kafkaCredentialsBase\x12\\\n\x16push_api_configuration\x18\n \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x14pushApiConfiguration\x12O\n\x0f\x64\x61ta_validation\x18\x0b \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x0e\x64\x61taValidationB\x13\n\x0f\x63om.tecton.dataP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0tecton_proto/data/user_deployment_settings.proto\x12\x11tecton_proto.data\x1a tecton_proto/common/secret.proto\"\xfa\x02\n\x16UserDeploymentSettings\x12G\n user_deployment_settings_version\x18\x01 \x01(\x05R\x1duserDeploymentSettingsVersion\x12R\n\x11\x64\x61tabricks_config\x18\x02 \x01(\x0b\x32#.tecton_proto.data.DatabricksConfigH\x00R\x10\x64\x61tabricksConfig\x12T\n\x13user_spark_settings\x18\x03 \x01(\x0b\x32$.tecton_proto.data.UserSparkSettingsR\x11userSparkSettings\x12O\n\x0ftenant_settings\x18\x05 \x01(\x0b\x32&.tecton_proto.data.TenantSettingsProtoR\x0etenantSettingsB\x16\n\x14\x64\x61ta_platform_configJ\x04\x08\x04\x10\x05\"\xdf\x01\n\x10\x44\x61tabricksConfig\x12#\n\rworkspace_url\x18\x01 \x01(\tR\x0cworkspaceUrl\x12\x38\n\tapi_token\x18\x02 \x01(\x0b\x32\x1b.tecton_proto.common.SecretR\x08\x61piToken\x12\x1b\n\tuser_name\x18\x03 \x01(\tR\x08userName\x12*\n\x11user_display_name\x18\x04 \x01(\tR\x0fuserDisplayName\x12#\n\rspark_version\x18\x05 \x01(\tR\x0csparkVersion\"\xd7\x01\n\x11UserSparkSettings\x12\x30\n\x14instance_profile_arn\x18\x01 \x01(\tR\x12instanceProfileArn\x12R\n\nspark_conf\x18\x02 \x03(\x0b\x32\x33.tecton_proto.data.UserSparkSettings.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x94\x06\n\x13TenantSettingsProto\x12M\n\x14\x63hronosphere_api_key\x18\x01 \x01(\x0b\x32\x1b.tecton_proto.common.SecretR\x12\x63hronosphereApiKey\x12I\n!chronosphere_restrict_label_value\x18\x04 \x01(\tR\x1e\x63hronosphereRestrictLabelValue\x12M\n pseudonymize_amplitude_user_name\x18\x02 \x01(\x08:\x04trueR\x1dpseudonymizeAmplitudeUserName\x12T\n\'enable_user_editing_deployment_settings\x18\x03 \x01(\x08R#enableUserEditingDeploymentSettings\x12-\n\x13okta_admin_group_id\x18\x05 \x01(\tR\x10oktaAdminGroupId\x12+\n\x12okta_user_group_id\x18\x06 \x01(\tR\x0foktaUserGroupId\x12\x39\n\x19\x62\x61se_metadata_service_url\x18\x07 \x01(\tR\x16\x62\x61seMetadataServiceUrl\x12\x37\n\x18\x62\x61se_feature_service_url\x18\x08 \x01(\tR\x15\x62\x61seFeatureServiceUrl\x12:\n\x19spicedb_organization_name\x18\t \x01(\tR\x17spicedbOrganizationName\x12=\n\x1b\x63ustomer_facing_tenant_name\x18\n \x01(\tR\x18\x63ustomerFacingTenantName\x12\x41\n\x0c\x61ws_settings\x18\x0b \x01(\x0b\x32\x1e.tecton_proto.data.AwsSettingsR\x0b\x61wsSettings\x12\x30\n\x14internal_tenant_name\x18\x0c \x01(\tR\x12internalTenantName\"\xa8\x05\n\x0b\x41wsSettings\x12>\n\x0b\x64ynamo_role\x18\x06 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\ndynamoRole\x12_\n\x11\x64ynamo_extra_tags\x18\x08 \x03(\x0b\x32\x33.tecton_proto.data.AwsSettings.DynamoExtraTagsEntryR\x0f\x64ynamoExtraTags\x12\x62\n\x12\x63ompute_extra_tags\x18\t \x03(\x0b\x32\x34.tecton_proto.data.AwsSettings.ComputeExtraTagsEntryR\x10\x63omputeExtraTags\x12\x41\n\x0c\x65mr_settings\x18\x0c \x01(\x0b\x32\x1e.tecton_proto.data.EmrSettingsR\x0b\x65mrSettings\x12Q\n\x12\x64ynamo_table_names\x18\r \x01(\x0b\x32#.tecton_proto.data.DynamoTableNamesR\x10\x64ynamoTableNames\x12]\n\x16object_store_locations\x18\x0e \x01(\x0b\x32\'.tecton_proto.data.ObjectStoreLocationsR\x14objectStoreLocations\x1a\x42\n\x14\x44ynamoExtraTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a\x43\n\x15\x43omputeExtraTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01J\x04\x08\x01\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\x94\x01\n\nAwsIamRole\x12\x19\n\x08role_arn\x18\x01 \x01(\tR\x07roleArn\x12J\n\x11intermediate_role\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\x10intermediateRole\x12\x1f\n\x0b\x65xternal_id\x18\x03 \x01(\tR\nexternalId\"S\n\nS3Location\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x31\n\x04role\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\x04role\"\"\n\x0c\x44\x42\x46SLocation\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"!\n\x0bGCSLocation\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"\xf2\x01\n\x13ObjectStoreLocation\x12@\n\x0bs3_location\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.S3LocationH\x00R\ns3Location\x12\x46\n\rdbfs_location\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.DBFSLocationH\x00R\x0c\x64\x62\x66sLocation\x12\x43\n\x0cgcs_location\x18\x03 \x01(\x0b\x32\x1e.tecton_proto.data.GCSLocationH\x00R\x0bgcsLocationB\x0c\n\nstore_type\"V\n\x0b\x45mrSettings\x12G\n\x10\x65mr_control_role\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.AwsIamRoleR\x0e\x65mrControlRole\"\xa8\x03\n\x10\x44ynamoTableNames\x12*\n\x11\x64\x61ta_table_prefix\x18\x01 \x01(\tR\x0f\x64\x61taTablePrefix\x12*\n\x11status_table_name\x18\x02 \x01(\tR\x0fstatusTableName\x12\x42\n\x1ejob_idempotence_key_table_name\x18\x03 \x01(\tR\x1ajobIdempotenceKeyTableName\x12*\n\x11\x63\x61nary_table_name\x18\x04 \x01(\tR\x0f\x63\x61naryTableName\x12/\n\x14\x64\x65lta_log_table_name\x18\x05 \x01(\tR\x11\x64\x65ltaLogTableName\x12.\n\x13metric_table_prefix\x18\x06 \x01(\tR\x11metricTablePrefix\x12\x34\n\x17\x64\x65lta_log_table_name_v2\x18\x07 \x01(\tR\x13\x64\x65ltaLogTableNameV2\x12\x35\n\x17job_metadata_table_name\x18\x08 \x01(\tR\x14jobMetadataTableName\"\xe0\x07\n\x14ObjectStoreLocations\x12P\n\x0fmaterialization\x18\x01 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x0fmaterialization\x12Y\n\x14streaming_checkpoint\x18\x02 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x13streamingCheckpoint\x12h\n\x1c\x66\x65\x61ture_server_configuration\x18\x03 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x1a\x66\x65\x61tureServerConfiguration\x12I\n\x0c\x66\x65\x61ture_repo\x18\x04 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x0b\x66\x65\x61tureRepo\x12G\n\x0b\x65mr_scripts\x18\x05 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\nemrScripts\x12]\n\x16materialization_params\x18\x06 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x15materializationParams\x12S\n\x11intermediate_data\x18\x07 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x10intermediateData\x12\\\n\x16\x66\x65\x61ture_server_logging\x18\x08 \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x14\x66\x65\x61tureServerLogging\x12\\\n\x16kafka_credentials_base\x18\t \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x14kafkaCredentialsBase\x12\\\n\x16push_api_configuration\x18\n \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x14pushApiConfiguration\x12O\n\x0f\x64\x61ta_validation\x18\x0b \x01(\x0b\x32&.tecton_proto.data.ObjectStoreLocationR\x0e\x64\x61taValidationB\x13\n\x0f\x63om.tecton.dataP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.data.user_deployment_settings_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.dataP\001'
@@ -46,16 +46,18 @@
   _AWSSETTINGS_COMPUTEEXTRATAGSENTRY._serialized_end=2378
   _AWSIAMROLE._serialized_start=2405
   _AWSIAMROLE._serialized_end=2553
   _S3LOCATION._serialized_start=2555
   _S3LOCATION._serialized_end=2638
   _DBFSLOCATION._serialized_start=2640
   _DBFSLOCATION._serialized_end=2674
-  _OBJECTSTORELOCATION._serialized_start=2677
-  _OBJECTSTORELOCATION._serialized_end=2850
-  _EMRSETTINGS._serialized_start=2852
-  _EMRSETTINGS._serialized_end=2938
-  _DYNAMOTABLENAMES._serialized_start=2941
-  _DYNAMOTABLENAMES._serialized_end=3365
-  _OBJECTSTORELOCATIONS._serialized_start=3368
-  _OBJECTSTORELOCATIONS._serialized_end=4360
+  _GCSLOCATION._serialized_start=2676
+  _GCSLOCATION._serialized_end=2709
+  _OBJECTSTORELOCATION._serialized_start=2712
+  _OBJECTSTORELOCATION._serialized_end=2954
+  _EMRSETTINGS._serialized_start=2956
+  _EMRSETTINGS._serialized_end=3042
+  _DYNAMOTABLENAMES._serialized_start=3045
+  _DYNAMOTABLENAMES._serialized_end=3469
+  _OBJECTSTORELOCATIONS._serialized_start=3472
+  _OBJECTSTORELOCATIONS._serialized_end=4464
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.7.0b8/tecton_proto/data/user_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/data/workspace_pb2.py` & `tecton-0.7.0b9/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from tecton_proto.spark_common import clusters_pb2 as tecton__proto_dot_spark__common_dot_clusters__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*tecton_proto/databricks_api/clusters.proto\x12\x1btecton_proto.databricks_api\x1a(tecton_proto/spark_common/clusters.proto\"3\n\x12\x43lustersGetRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xc2\x08\n\x14\x43lusterCreateRequest\x12_\n\nspark_conf\x18\x01 \x03(\x0b\x32@.tecton_proto.databricks_api.ClusterCreateRequest.SparkConfEntryR\tsparkConf\x12-\n\x13\x64river_node_type_id\x18\x02 \x01(\tR\x10\x64riverNodeTypeId\x12 \n\x0cnode_type_id\x18\x03 \x01(\tR\nnodeTypeId\x12\x1f\n\x0bnum_workers\x18\x04 \x01(\x05R\nnumWorkers\x12!\n\x0c\x63luster_name\x18\x05 \x01(\tR\x0b\x63lusterName\x12#\n\rspark_version\x18\x06 \x01(\tR\x0csparkVersion\x12O\n\x0e\x61ws_attributes\x18\x07 \x01(\x0b\x32(.tecton_proto.spark_common.AwsAttributesR\rawsAttributes\x12+\n\x11idempotency_token\x18\x08 \x01(\tR\x10idempotencyToken\x12i\n\x0espark_env_vars\x18\t \x03(\x0b\x32\x43.tecton_proto.databricks_api.ClusterCreateRequest.SparkEnvVarsEntryR\x0csparkEnvVars\x12\x62\n\x0b\x63ustom_tags\x18\n \x03(\x0b\x32\x41.tecton_proto.databricks_api.ClusterCreateRequest.CustomTagsEntryR\ncustomTags\x12\x37\n\x17\x61utotermination_minutes\x18\x0b \x01(\x05R\x16\x61utoterminationMinutes\x12.\n\x13\x65nable_elastic_disk\x18\x0c \x01(\x08R\x11\x65nableElasticDisk\x12K\n\tautoscale\x18\r \x01(\x0b\x32-.tecton_proto.databricks_api.ClusterAutoScaleR\tautoscale\x12N\n\x0cinit_scripts\x18\x0e \x03(\x0b\x32+.tecton_proto.spark_common.ResourceLocationR\x0binitScripts\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a?\n\x11SparkEnvVarsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a=\n\x0f\x43ustomTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"T\n\x10\x43lusterAutoScale\x12\x1f\n\x0bmin_workers\x18\x01 \x01(\x05R\nminWorkers\x12\x1f\n\x0bmax_workers\x18\x02 \x01(\x05R\nmaxWorkers\"6\n\x15\x43lusterCreateResponse\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"8\n\x17\x43lusterTerminateRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xf9\x01\n\x13\x43lustersGetResponse\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12#\n\rstate_message\x18\x02 \x01(\tR\x0cstateMessage\x12]\n\x12termination_reason\x18\x03 \x01(\x0b\x32..tecton_proto.databricks_api.TerminationReasonR\x11terminationReason\x12?\n\x05state\x18\x04 \x01(\x0e\x32).tecton_proto.databricks_api.ClusterStateR\x05state\"\x97\x01\n\x11TerminationReason\x12@\n\x04\x63ode\x18\x01 \x01(\x0e\x32,.tecton_proto.databricks_api.TerminationCodeR\x04\x63ode\x12@\n\x04type\x18\x02 \x01(\x0e\x32,.tecton_proto.databricks_api.TerminationTypeR\x04type\"W\n\x13\x43lusterListResponse\x12@\n\x08\x63lusters\x18\x01 \x03(\x0b\x32$.tecton_proto.databricks_api.ClusterR\x08\x63lusters\"\xc7\x02\n\x07\x43luster\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12!\n\x0c\x63luster_name\x18\x02 \x01(\tR\x0b\x63lusterName\x12#\n\rspark_version\x18\x03 \x01(\tR\x0csparkVersion\x12?\n\x05state\x18\x04 \x01(\x0e\x32).tecton_proto.databricks_api.ClusterStateR\x05state\x12U\n\x0b\x63ustom_tags\x18\x05 \x03(\x0b\x32\x34.tecton_proto.databricks_api.Cluster.CustomTagsEntryR\ncustomTags\x1a=\n\x0f\x43ustomTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01*\x7f\n\x0c\x43lusterState\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x0e\n\nRESTARTING\x10\x02\x12\x0c\n\x08RESIZING\x10\x03\x12\x0f\n\x0bTERMINATING\x10\x04\x12\x0e\n\nTERMINATED\x10\x05\x12\t\n\x05\x45RROR\x10\x06\x12\x0b\n\x07UNKNOWN\x10\x07*\xf0\x04\n\x0fTerminationCode\x12\x1d\n\x19UNKNOWN_TERMINATION_STATE\x10\x00\x12\x10\n\x0cUSER_REQUEST\x10\x01\x12\x10\n\x0cJOB_FINISHED\x10\x02\x12\x0e\n\nINACTIVITY\x10\x03\x12\x1b\n\x17\x43LOUD_PROVIDER_SHUTDOWN\x10\x04\x12\x16\n\x12\x43OMMUNICATION_LOST\x10\x05\x12!\n\x1d\x43LOUD_PROVIDER_LAUNCH_FAILURE\x10\x06\x12\x19\n\x15SPARK_STARTUP_FAILURE\x10\x07\x12\x14\n\x10INVALID_ARGUMENT\x10\x08\x12\x1d\n\x19UNEXPECTED_LAUNCH_FAILURE\x10\t\x12\x12\n\x0eINTERNAL_ERROR\x10\n\x12\x0f\n\x0bSPARK_ERROR\x10\x0b\x12!\n\x1dMETASTORE_COMPONENT_UNHEALTHY\x10\x0c\x12\x1c\n\x18\x44\x42\x46S_COMPONENT_UNHEALTHY\x10\r\x12\x16\n\x12\x44RIVER_UNREACHABLE\x10\x0e\x12\x17\n\x13\x44RIVER_UNRESPONSIVE\x10\x0f\x12\x18\n\x14INSTANCE_UNREACHABLE\x10\x10\x12\x1c\n\x18\x43ONTAINER_LAUNCH_FAILURE\x10\x11\x12!\n\x1dINSTANCE_POOL_CLUSTER_FAILURE\x10\x12\x12\x14\n\x10REQUEST_REJECTED\x10\x13\x12\x17\n\x13INIT_SCRIPT_FAILURE\x10\x14\x12\x11\n\rTRIAL_EXPIRED\x10\x15\x12.\n*AWS_INSUFFICIENT_INSTANCE_CAPACITY_FAILURE\x10\x16*t\n\x0fTerminationType\x12\x1c\n\x18UNKNOWN_TERMINATION_TYPE\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x10\n\x0c\x43LIENT_ERROR\x10\x02\x12\x11\n\rSERVICE_FAULT\x10\x03\x12\x11\n\rCLOUD_FAILURE\x10\x04\x42\x1d\n\x19\x63om.tecton.databricks_apiP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*tecton_proto/databricks_api/clusters.proto\x12\x1btecton_proto.databricks_api\x1a(tecton_proto/spark_common/clusters.proto\"3\n\x12\x43lustersGetRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xdf\x08\n\x14\x43lusterCreateRequest\x12_\n\nspark_conf\x18\x01 \x03(\x0b\x32@.tecton_proto.databricks_api.ClusterCreateRequest.SparkConfEntryR\tsparkConf\x12-\n\x13\x64river_node_type_id\x18\x02 \x01(\tR\x10\x64riverNodeTypeId\x12 \n\x0cnode_type_id\x18\x03 \x01(\tR\nnodeTypeId\x12\x1f\n\x0bnum_workers\x18\x04 \x01(\x05R\nnumWorkers\x12!\n\x0c\x63luster_name\x18\x05 \x01(\tR\x0b\x63lusterName\x12#\n\rspark_version\x18\x06 \x01(\tR\x0csparkVersion\x12O\n\x0e\x61ws_attributes\x18\x07 \x01(\x0b\x32(.tecton_proto.spark_common.AwsAttributesR\rawsAttributes\x12+\n\x11idempotency_token\x18\x08 \x01(\tR\x10idempotencyToken\x12i\n\x0espark_env_vars\x18\t \x03(\x0b\x32\x43.tecton_proto.databricks_api.ClusterCreateRequest.SparkEnvVarsEntryR\x0csparkEnvVars\x12\x62\n\x0b\x63ustom_tags\x18\n \x03(\x0b\x32\x41.tecton_proto.databricks_api.ClusterCreateRequest.CustomTagsEntryR\ncustomTags\x12\x37\n\x17\x61utotermination_minutes\x18\x0b \x01(\x05R\x16\x61utoterminationMinutes\x12.\n\x13\x65nable_elastic_disk\x18\x0c \x01(\x08R\x11\x65nableElasticDisk\x12K\n\tautoscale\x18\r \x01(\x0b\x32-.tecton_proto.databricks_api.ClusterAutoScaleR\tautoscale\x12N\n\x0cinit_scripts\x18\x0e \x03(\x0b\x32+.tecton_proto.spark_common.ResourceLocationR\x0binitScripts\x12\x1b\n\tpolicy_id\x18\x0f \x01(\tR\x08policyId\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a?\n\x11SparkEnvVarsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a=\n\x0f\x43ustomTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"T\n\x10\x43lusterAutoScale\x12\x1f\n\x0bmin_workers\x18\x01 \x01(\x05R\nminWorkers\x12\x1f\n\x0bmax_workers\x18\x02 \x01(\x05R\nmaxWorkers\"6\n\x15\x43lusterCreateResponse\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"8\n\x17\x43lusterTerminateRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xf9\x01\n\x13\x43lustersGetResponse\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12#\n\rstate_message\x18\x02 \x01(\tR\x0cstateMessage\x12]\n\x12termination_reason\x18\x03 \x01(\x0b\x32..tecton_proto.databricks_api.TerminationReasonR\x11terminationReason\x12?\n\x05state\x18\x04 \x01(\x0e\x32).tecton_proto.databricks_api.ClusterStateR\x05state\"\x97\x01\n\x11TerminationReason\x12@\n\x04\x63ode\x18\x01 \x01(\x0e\x32,.tecton_proto.databricks_api.TerminationCodeR\x04\x63ode\x12@\n\x04type\x18\x02 \x01(\x0e\x32,.tecton_proto.databricks_api.TerminationTypeR\x04type\"W\n\x13\x43lusterListResponse\x12@\n\x08\x63lusters\x18\x01 \x03(\x0b\x32$.tecton_proto.databricks_api.ClusterR\x08\x63lusters\"\xc7\x02\n\x07\x43luster\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12!\n\x0c\x63luster_name\x18\x02 \x01(\tR\x0b\x63lusterName\x12#\n\rspark_version\x18\x03 \x01(\tR\x0csparkVersion\x12?\n\x05state\x18\x04 \x01(\x0e\x32).tecton_proto.databricks_api.ClusterStateR\x05state\x12U\n\x0b\x63ustom_tags\x18\x05 \x03(\x0b\x32\x34.tecton_proto.databricks_api.Cluster.CustomTagsEntryR\ncustomTags\x1a=\n\x0f\x43ustomTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01*\x7f\n\x0c\x43lusterState\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x0e\n\nRESTARTING\x10\x02\x12\x0c\n\x08RESIZING\x10\x03\x12\x0f\n\x0bTERMINATING\x10\x04\x12\x0e\n\nTERMINATED\x10\x05\x12\t\n\x05\x45RROR\x10\x06\x12\x0b\n\x07UNKNOWN\x10\x07*\xf0\x04\n\x0fTerminationCode\x12\x1d\n\x19UNKNOWN_TERMINATION_STATE\x10\x00\x12\x10\n\x0cUSER_REQUEST\x10\x01\x12\x10\n\x0cJOB_FINISHED\x10\x02\x12\x0e\n\nINACTIVITY\x10\x03\x12\x1b\n\x17\x43LOUD_PROVIDER_SHUTDOWN\x10\x04\x12\x16\n\x12\x43OMMUNICATION_LOST\x10\x05\x12!\n\x1d\x43LOUD_PROVIDER_LAUNCH_FAILURE\x10\x06\x12\x19\n\x15SPARK_STARTUP_FAILURE\x10\x07\x12\x14\n\x10INVALID_ARGUMENT\x10\x08\x12\x1d\n\x19UNEXPECTED_LAUNCH_FAILURE\x10\t\x12\x12\n\x0eINTERNAL_ERROR\x10\n\x12\x0f\n\x0bSPARK_ERROR\x10\x0b\x12!\n\x1dMETASTORE_COMPONENT_UNHEALTHY\x10\x0c\x12\x1c\n\x18\x44\x42\x46S_COMPONENT_UNHEALTHY\x10\r\x12\x16\n\x12\x44RIVER_UNREACHABLE\x10\x0e\x12\x17\n\x13\x44RIVER_UNRESPONSIVE\x10\x0f\x12\x18\n\x14INSTANCE_UNREACHABLE\x10\x10\x12\x1c\n\x18\x43ONTAINER_LAUNCH_FAILURE\x10\x11\x12!\n\x1dINSTANCE_POOL_CLUSTER_FAILURE\x10\x12\x12\x14\n\x10REQUEST_REJECTED\x10\x13\x12\x17\n\x13INIT_SCRIPT_FAILURE\x10\x14\x12\x11\n\rTRIAL_EXPIRED\x10\x15\x12.\n*AWS_INSUFFICIENT_INSTANCE_CAPACITY_FAILURE\x10\x16*t\n\x0fTerminationType\x12\x1c\n\x18UNKNOWN_TERMINATION_TYPE\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x10\n\x0c\x43LIENT_ERROR\x10\x02\x12\x11\n\rSERVICE_FAULT\x10\x03\x12\x11\n\rCLOUD_FAILURE\x10\x04\x42\x1d\n\x19\x63om.tecton.databricks_apiP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.databricks_api.clusters_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\031com.tecton.databricks_apiP\001'
@@ -26,40 +26,40 @@
   _CLUSTERCREATEREQUEST_SPARKCONFENTRY._serialized_options = b'8\001'
   _CLUSTERCREATEREQUEST_SPARKENVVARSENTRY._options = None
   _CLUSTERCREATEREQUEST_SPARKENVVARSENTRY._serialized_options = b'8\001'
   _CLUSTERCREATEREQUEST_CUSTOMTAGSENTRY._options = None
   _CLUSTERCREATEREQUEST_CUSTOMTAGSENTRY._serialized_options = b'8\001'
   _CLUSTER_CUSTOMTAGSENTRY._options = None
   _CLUSTER_CUSTOMTAGSENTRY._serialized_options = b'8\001'
-  _CLUSTERSTATE._serialized_start=2288
-  _CLUSTERSTATE._serialized_end=2415
-  _TERMINATIONCODE._serialized_start=2418
-  _TERMINATIONCODE._serialized_end=3042
-  _TERMINATIONTYPE._serialized_start=3044
-  _TERMINATIONTYPE._serialized_end=3160
+  _CLUSTERSTATE._serialized_start=2317
+  _CLUSTERSTATE._serialized_end=2444
+  _TERMINATIONCODE._serialized_start=2447
+  _TERMINATIONCODE._serialized_end=3071
+  _TERMINATIONTYPE._serialized_start=3073
+  _TERMINATIONTYPE._serialized_end=3189
   _CLUSTERSGETREQUEST._serialized_start=117
   _CLUSTERSGETREQUEST._serialized_end=168
   _CLUSTERCREATEREQUEST._serialized_start=171
-  _CLUSTERCREATEREQUEST._serialized_end=1261
-  _CLUSTERCREATEREQUEST_SPARKCONFENTRY._serialized_start=1073
-  _CLUSTERCREATEREQUEST_SPARKCONFENTRY._serialized_end=1133
-  _CLUSTERCREATEREQUEST_SPARKENVVARSENTRY._serialized_start=1135
-  _CLUSTERCREATEREQUEST_SPARKENVVARSENTRY._serialized_end=1198
-  _CLUSTERCREATEREQUEST_CUSTOMTAGSENTRY._serialized_start=1200
-  _CLUSTERCREATEREQUEST_CUSTOMTAGSENTRY._serialized_end=1261
-  _CLUSTERAUTOSCALE._serialized_start=1263
-  _CLUSTERAUTOSCALE._serialized_end=1347
-  _CLUSTERCREATERESPONSE._serialized_start=1349
-  _CLUSTERCREATERESPONSE._serialized_end=1403
-  _CLUSTERTERMINATEREQUEST._serialized_start=1405
-  _CLUSTERTERMINATEREQUEST._serialized_end=1461
-  _CLUSTERSGETRESPONSE._serialized_start=1464
-  _CLUSTERSGETRESPONSE._serialized_end=1713
-  _TERMINATIONREASON._serialized_start=1716
-  _TERMINATIONREASON._serialized_end=1867
-  _CLUSTERLISTRESPONSE._serialized_start=1869
-  _CLUSTERLISTRESPONSE._serialized_end=1956
-  _CLUSTER._serialized_start=1959
-  _CLUSTER._serialized_end=2286
-  _CLUSTER_CUSTOMTAGSENTRY._serialized_start=1200
-  _CLUSTER_CUSTOMTAGSENTRY._serialized_end=1261
+  _CLUSTERCREATEREQUEST._serialized_end=1290
+  _CLUSTERCREATEREQUEST_SPARKCONFENTRY._serialized_start=1102
+  _CLUSTERCREATEREQUEST_SPARKCONFENTRY._serialized_end=1162
+  _CLUSTERCREATEREQUEST_SPARKENVVARSENTRY._serialized_start=1164
+  _CLUSTERCREATEREQUEST_SPARKENVVARSENTRY._serialized_end=1227
+  _CLUSTERCREATEREQUEST_CUSTOMTAGSENTRY._serialized_start=1229
+  _CLUSTERCREATEREQUEST_CUSTOMTAGSENTRY._serialized_end=1290
+  _CLUSTERAUTOSCALE._serialized_start=1292
+  _CLUSTERAUTOSCALE._serialized_end=1376
+  _CLUSTERCREATERESPONSE._serialized_start=1378
+  _CLUSTERCREATERESPONSE._serialized_end=1432
+  _CLUSTERTERMINATEREQUEST._serialized_start=1434
+  _CLUSTERTERMINATEREQUEST._serialized_end=1490
+  _CLUSTERSGETRESPONSE._serialized_start=1493
+  _CLUSTERSGETRESPONSE._serialized_end=1742
+  _TERMINATIONREASON._serialized_start=1745
+  _TERMINATIONREASON._serialized_end=1896
+  _CLUSTERLISTRESPONSE._serialized_start=1898
+  _CLUSTERLISTRESPONSE._serialized_end=1985
+  _CLUSTER._serialized_start=1988
+  _CLUSTER._serialized_end=2315
+  _CLUSTER_CUSTOMTAGSENTRY._serialized_start=1229
+  _CLUSTER_CUSTOMTAGSENTRY._serialized_end=1290
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.7.0b9/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/dataobs/config_pb2.py` & `tecton-0.7.0b9/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.7.0b9/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.7.0b9/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.7.0b9/tecton_proto/dataobs/validation_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,34 +12,34 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from tecton_proto.common import id_pb2 as tecton__proto_dot_common_dot_id__pb2
 from tecton_proto.dataobs import expectation_pb2 as tecton__proto_dot_dataobs_dot_expectation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%tecton_proto/dataobs/validation.proto\x12\x14tecton_proto.dataobs\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1ctecton_proto/common/id.proto\x1a&tecton_proto/dataobs/expectation.proto\"\x97\x05\n\x11\x45xpectationResult\x12\x43\n\x11validation_job_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x0fvalidationJobId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12\x43\n\x0fvalidation_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0evalidationTime\x12Y\n\x1b\x66\x65\x61ture_interval_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x18\x66\x65\x61tureIntervalStartTime\x12t\n\x1c\x66\x65\x61ture_expectation_metadata\x18\x06 \x01(\x0b\x32\x30.tecton_proto.dataobs.FeatureExpectationMetadataH\x00R\x1a\x66\x65\x61tureExpectationMetadata\x12q\n\x1bmetric_expectation_metadata\x18\x07 \x01(\x0b\x32/.tecton_proto.dataobs.MetricExpectationMetadataH\x00R\x19metricExpectationMetadata\x12\x43\n\x06result\x18\x08 \x01(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x06resultB\n\n\x08metadata\"\xeb\x01\n\x1a\x46\x65\x61tureExpectationMetadata\x12J\n\x0b\x65xpectation\x18\x01 \x01(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x0b\x65xpectation\x12\x1b\n\talert_msg\x18\x03 \x01(\tR\x08\x61lertMsg\x12-\n\x12\x66\x61ilure_percentage\x18\x04 \x01(\x01R\x11\x66\x61ilurePercentage\x12\x35\n\x17\x66\x61iled_join_key_samples\x18\x05 \x03(\tR\x14\x66\x61iledJoinKeySamples\"\x81\x03\n\x19MetricExpectationMetadata\x12I\n\x0b\x65xpectation\x18\x01 \x01(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x0b\x65xpectation\x12\x1b\n\talert_msg\x18\x03 \x01(\tR\x08\x61lertMsg\x12]\n\x0cparam_values\x18\x04 \x03(\x0b\x32:.tecton_proto.dataobs.MetricExpectationMetadata.ParamValueR\x0bparamValues\x1a\x9c\x01\n\nParamValue\x12\x1f\n\x0bmetric_name\x18\x01 \x01(\tR\nmetricName\x12!\n\x0c\x61\x63tual_value\x18\x02 \x01(\tR\x0b\x61\x63tualValue\x12J\n\x13interval_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11intervalStartTime\"o\n\rResultSummary\x12\x16\n\x06passed\x18\x01 \x01(\x05R\x06passed\x12\x16\n\x06\x66\x61iled\x18\x02 \x01(\x05R\x06\x66\x61iled\x12\x14\n\x05\x65rror\x18\x03 \x01(\x05R\x05\x65rror\x12\x18\n\x07unknown\x18\x04 \x01(\x05R\x07unknown\"\xd7\x01\n\x16WorkspaceResultSummary\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12=\n\x07summary\x18\x02 \x01(\x0b\x32#.tecton_proto.dataobs.ResultSummaryR\x07summary\x12`\n\x14\x66\x65\x61ture_view_summary\x18\x03 \x03(\x0b\x32..tecton_proto.dataobs.FeatureViewResultSummaryR\x12\x66\x65\x61tureViewSummary\"\xe6\x01\n\x18\x46\x65\x61tureViewResultSummary\x12*\n\x11\x66\x65\x61ture_view_name\x18\x01 \x01(\tR\x0f\x66\x65\x61tureViewName\x12=\n\x07summary\x18\x02 \x01(\x0b\x32#.tecton_proto.dataobs.ResultSummaryR\x07summary\x12_\n\x13\x65xpectation_summary\x18\x03 \x03(\x0b\x32..tecton_proto.dataobs.ExpectationResultSummaryR\x12\x65xpectationSummary\"\x84\x01\n\x18\x45xpectationResultSummary\x12)\n\x10\x65xpectation_name\x18\x01 \x01(\tR\x0f\x65xpectationName\x12=\n\x07summary\x18\x02 \x01(\x0b\x32#.tecton_proto.dataobs.ResultSummaryR\x07summary*c\n\x15\x45xpectationResultEnum\x12\x12\n\x0eRESULT_UNKNOWN\x10\x00\x12\x11\n\rRESULT_PASSED\x10\x01\x12\x11\n\rRESULT_FAILED\x10\x02\x12\x10\n\x0cRESULT_ERROR\x10\x03\x42\x16\n\x12\x63om.tecton.dataobsP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%tecton_proto/dataobs/validation.proto\x12\x14tecton_proto.dataobs\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1ctecton_proto/common/id.proto\x1a&tecton_proto/dataobs/expectation.proto\"\xc3\x05\n\x11\x45xpectationResult\x12\x43\n\x11validation_job_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x0fvalidationJobId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\t \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12\x43\n\x0fvalidation_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0evalidationTime\x12Y\n\x1b\x66\x65\x61ture_interval_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x18\x66\x65\x61tureIntervalStartTime\x12t\n\x1c\x66\x65\x61ture_expectation_metadata\x18\x06 \x01(\x0b\x32\x30.tecton_proto.dataobs.FeatureExpectationMetadataH\x00R\x1a\x66\x65\x61tureExpectationMetadata\x12q\n\x1bmetric_expectation_metadata\x18\x07 \x01(\x0b\x32/.tecton_proto.dataobs.MetricExpectationMetadataH\x00R\x19metricExpectationMetadata\x12\x43\n\x06result\x18\x08 \x01(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x06resultB\n\n\x08metadata\"\xeb\x01\n\x1a\x46\x65\x61tureExpectationMetadata\x12J\n\x0b\x65xpectation\x18\x01 \x01(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x0b\x65xpectation\x12\x1b\n\talert_msg\x18\x03 \x01(\tR\x08\x61lertMsg\x12-\n\x12\x66\x61ilure_percentage\x18\x04 \x01(\x01R\x11\x66\x61ilurePercentage\x12\x35\n\x17\x66\x61iled_join_key_samples\x18\x05 \x03(\tR\x14\x66\x61iledJoinKeySamples\"\x81\x03\n\x19MetricExpectationMetadata\x12I\n\x0b\x65xpectation\x18\x01 \x01(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x0b\x65xpectation\x12\x1b\n\talert_msg\x18\x03 \x01(\tR\x08\x61lertMsg\x12]\n\x0cparam_values\x18\x04 \x03(\x0b\x32:.tecton_proto.dataobs.MetricExpectationMetadata.ParamValueR\x0bparamValues\x1a\x9c\x01\n\nParamValue\x12\x1f\n\x0bmetric_name\x18\x01 \x01(\tR\nmetricName\x12!\n\x0c\x61\x63tual_value\x18\x02 \x01(\tR\x0b\x61\x63tualValue\x12J\n\x13interval_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11intervalStartTime\"o\n\rResultSummary\x12\x16\n\x06passed\x18\x01 \x01(\x05R\x06passed\x12\x16\n\x06\x66\x61iled\x18\x02 \x01(\x05R\x06\x66\x61iled\x12\x14\n\x05\x65rror\x18\x03 \x01(\x05R\x05\x65rror\x12\x18\n\x07unknown\x18\x04 \x01(\x05R\x07unknown\"\xd7\x01\n\x16WorkspaceResultSummary\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12=\n\x07summary\x18\x02 \x01(\x0b\x32#.tecton_proto.dataobs.ResultSummaryR\x07summary\x12`\n\x14\x66\x65\x61ture_view_summary\x18\x03 \x03(\x0b\x32..tecton_proto.dataobs.FeatureViewResultSummaryR\x12\x66\x65\x61tureViewSummary\"\xe6\x01\n\x18\x46\x65\x61tureViewResultSummary\x12*\n\x11\x66\x65\x61ture_view_name\x18\x01 \x01(\tR\x0f\x66\x65\x61tureViewName\x12=\n\x07summary\x18\x02 \x01(\x0b\x32#.tecton_proto.dataobs.ResultSummaryR\x07summary\x12_\n\x13\x65xpectation_summary\x18\x03 \x03(\x0b\x32..tecton_proto.dataobs.ExpectationResultSummaryR\x12\x65xpectationSummary\"\x84\x01\n\x18\x45xpectationResultSummary\x12)\n\x10\x65xpectation_name\x18\x01 \x01(\tR\x0f\x65xpectationName\x12=\n\x07summary\x18\x02 \x01(\x0b\x32#.tecton_proto.dataobs.ResultSummaryR\x07summary*c\n\x15\x45xpectationResultEnum\x12\x12\n\x0eRESULT_UNKNOWN\x10\x00\x12\x11\n\rRESULT_PASSED\x10\x01\x12\x11\n\rRESULT_FAILED\x10\x02\x12\x10\n\x0cRESULT_ERROR\x10\x03\x42\x16\n\x12\x63om.tecton.dataobsP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.dataobs.validation_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\022com.tecton.dataobsP\001'
-  _EXPECTATIONRESULTENUM._serialized_start=2157
-  _EXPECTATIONRESULTENUM._serialized_end=2256
+  _EXPECTATIONRESULTENUM._serialized_start=2201
+  _EXPECTATIONRESULTENUM._serialized_end=2300
   _EXPECTATIONRESULT._serialized_start=167
-  _EXPECTATIONRESULT._serialized_end=830
-  _FEATUREEXPECTATIONMETADATA._serialized_start=833
-  _FEATUREEXPECTATIONMETADATA._serialized_end=1068
-  _METRICEXPECTATIONMETADATA._serialized_start=1071
-  _METRICEXPECTATIONMETADATA._serialized_end=1456
-  _METRICEXPECTATIONMETADATA_PARAMVALUE._serialized_start=1300
-  _METRICEXPECTATIONMETADATA_PARAMVALUE._serialized_end=1456
-  _RESULTSUMMARY._serialized_start=1458
-  _RESULTSUMMARY._serialized_end=1569
-  _WORKSPACERESULTSUMMARY._serialized_start=1572
-  _WORKSPACERESULTSUMMARY._serialized_end=1787
-  _FEATUREVIEWRESULTSUMMARY._serialized_start=1790
-  _FEATUREVIEWRESULTSUMMARY._serialized_end=2020
-  _EXPECTATIONRESULTSUMMARY._serialized_start=2023
-  _EXPECTATIONRESULTSUMMARY._serialized_end=2155
+  _EXPECTATIONRESULT._serialized_end=874
+  _FEATUREEXPECTATIONMETADATA._serialized_start=877
+  _FEATUREEXPECTATIONMETADATA._serialized_end=1112
+  _METRICEXPECTATIONMETADATA._serialized_start=1115
+  _METRICEXPECTATIONMETADATA._serialized_end=1500
+  _METRICEXPECTATIONMETADATA_PARAMVALUE._serialized_start=1344
+  _METRICEXPECTATIONMETADATA_PARAMVALUE._serialized_end=1500
+  _RESULTSUMMARY._serialized_start=1502
+  _RESULTSUMMARY._serialized_end=1613
+  _WORKSPACERESULTSUMMARY._serialized_start=1616
+  _WORKSPACERESULTSUMMARY._serialized_end=1831
+  _FEATUREVIEWRESULTSUMMARY._serialized_start=1834
+  _FEATUREVIEWRESULTSUMMARY._serialized_end=2064
+  _EXPECTATIONRESULTSUMMARY._serialized_start=2067
+  _EXPECTATIONRESULTSUMMARY._serialized_end=2199
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.7.0b8/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.7.0b9/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.7.0b9/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.7.0b9/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.7.0b9/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.7.0b9/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.7.0b9/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.7.0b9/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.7.0b9/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.7.0b9/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from tecton_proto.amplitude import client_logging_pb2 as tecton__proto_dot_amplitude_dot_client__logging__pb2
 from tecton_proto.amplitude import amplitude_pb2 as tecton__proto_dot_amplitude_dot_amplitude__pb2
 from tecton_proto.validation import validator_pb2 as tecton__proto_dot_validation_dot_validator__pb2
 from tecton_proto.materialization import materialization_states_pb2 as tecton__proto_dot_materialization_dot_materialization__states__pb2
 from tecton_proto.materialization import spark_cluster_pb2 as tecton__proto_dot_materialization_dot_spark__cluster__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3tecton_proto/metadataservice/metadata_service.proto\x12\x1ctecton_proto.metadataservice\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a google/protobuf/field_mask.proto\x1a!tecton_proto/auth/principal.proto\x1a\x1etecton_proto/data/entity.proto\x1a tecton_proto/args/fco_args.proto\x1a\x1ftecton_proto/auth/service.proto\x1a\x1btecton_proto/data/fco.proto\x1a$tecton_proto/data/feature_view.proto\x1a\'tecton_proto/data/feature_service.proto\x1a&tecton_proto/data/hive_metastore.proto\x1a$tecton_proto/data/state_update.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a\x30tecton_proto/data/user_deployment_settings.proto\x1a\x1ctecton_proto/data/user.proto\x1a(tecton_proto/spark_common/clusters.proto\x1a&tecton_proto/dataobs/expectation.proto\x1a*tecton_proto/consumption/consumption.proto\x1a!tecton_proto/dataobs/metric.proto\x1a%tecton_proto/dataobs/validation.proto\x1a\x1ctecton_proto/common/id.proto\x1a%tecton_proto/common/fco_locator.proto\x1a&tecton_proto/common/spark_schema.proto\x1a.tecton_proto/data/materialization_status.proto\x1a(tecton_proto/data/freshness_status.proto\x1a&tecton_proto/data/serving_status.proto\x1a\x35tecton_proto/data/internal_spark_cluster_status.proto\x1a\x1ftecton_proto/data/summary.proto\x1a\x30tecton_proto/data/saved_feature_data_frame.proto\x1a\"tecton_proto/data/onboarding.proto\x1a&tecton_proto/data/transformation.proto\x1a+tecton_proto/data/virtual_data_source.proto\x1a!tecton_proto/data/workspace.proto\x1a+tecton_proto/amplitude/client_logging.proto\x1a&tecton_proto/amplitude/amplitude.proto\x1a\'tecton_proto/validation/validator.proto\x1a\x39tecton_proto/materialization/materialization_states.proto\x1a\x30tecton_proto/materialization/spark_cluster.proto\"p\n\nJobsKeySet\x12\x39\n\nupdated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"\xd0\x01\n\x11PaginationRequest\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x19\n\x08sort_key\x18\x03 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x04 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\x12\x1d\n\npage_token\x18\x05 \x01(\tR\tpageToken\"\xf0\x01\n\x12PaginationResponse\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x14\n\x05total\x18\x03 \x01(\rR\x05total\x12&\n\x0fnext_page_token\x18\x04 \x01(\tR\rnextPageToken\x12\x19\n\x08sort_key\x18\x05 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x06 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\"\x9a\x01\n\x18GetFeatureServiceRequest\x12+\n\x11service_reference\x18\x02 \x01(\tR\x10serviceReference\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02idJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"a\n\x19GetFeatureServiceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"<\n\x1cGetAllFeatureServicesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"m\n\x1dGetAllFeatureServicesResponse\x12L\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32!.tecton_proto.data.FeatureServiceR\x0f\x66\x65\x61tureServices\"\xc7\x01\n\x1fGetFeatureServiceSummaryRequest\x12G\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x32\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tH\x00R\x12\x66\x65\x61tureServiceName\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\t\n\x07locator\"\x8c\x01\n GetFeatureServiceSummaryResponse\x12\x43\n\rgeneral_items\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.SummaryItemR\x0cgeneralItems\x12#\n\rvariant_names\x18\x03 \x03(\tR\x0cvariantNames\"f\n\"GetVirtualDataSourceSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"e\n#GetVirtualDataSourceSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"c\n\x1fGetTransformationSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"b\n GetTransformationSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"[\n\x17GetEntitySummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"Z\n\x18GetEntitySummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"\xd9\x01\n\x17GetServingStatusRequest\x12G\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0e\n\x0crequest_type\"\xd6\x01\n\x1eGetFVServingStatusForFSRequest\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x02 \x02(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12O\n\npagination\x18\x04 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xe7\x01\n\x1fGetFVServingStatusForFSResponse\x12r\n\x1b\x66ull_serving_status_summary\x18\x01 \x01(\x0b\x32\x33.tecton_proto.data.FullFeatureServiceServingSummaryR\x18\x66ullServingStatusSummary\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"y\n\x18GetServingStatusResponse\x12]\n\x16serving_status_summary\x18\x05 \x01(\x0b\x32\'.tecton_proto.data.ServingStatusSummaryR\x14servingStatusSummary\"=\n\x1dGetAllFeatureFreshnessRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"s\n\x1eGetAllFeatureFreshnessResponse\x12Q\n\x12\x66reshness_statuses\x18\x01 \x03(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x11\x66reshnessStatuses\"^\n\x1aGetFeatureFreshnessRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"l\n\x1bGetFeatureFreshnessResponse\x12M\n\x10\x66reshness_status\x18\x01 \x01(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x0f\x66reshnessStatus\"`\n\x1cGetFeatureConsumptionRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"u\n\x1dGetFeatureConsumptionResponse\x12T\n\x10\x63onsumption_info\x18\x01 \x03(\x0b\x32).tecton_proto.consumption.ConsumptionInfoR\x0f\x63onsumptionInfo\"h\n\x1fGetMaterializationStatusRequest\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\"\x83\x01\n GetMaterializationStatusResponse\x12_\n\x16materialization_status\x18\x01 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"V\n2GetAllMaterializationStatusInLiveWorkspacesRequest\x12 \n\x0c\x63ut_off_days\x18\x01 \x01(\x05R\ncutOffDays\"4\n\nCountRange\x12\x14\n\x05start\x18\x01 \x01(\rR\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\rR\x03\x65nd\"m\n\rDurationRange\x12/\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05start\x12+\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03\x65nd\"o\n\rDateTimeRange\x12\x30\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05start\x12,\n\x03\x65nd\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03\x65nd\"\x82\x06\n\x0eGetJobsRequest\x12\x1e\n\nworkspaces\x18\x01 \x03(\tR\nworkspaces\x12#\n\rfeature_views\x18\x02 \x03(\tR\x0c\x66\x65\x61tureViews\x12R\n\x08statuses\x18\x03 \x03(\x0e\x32\x36.tecton_proto.materialization.MaterializationTaskStateR\x08statuses\x12J\n\ncreated_at\x18\x06 \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\tcreatedAt\x12\x43\n\ttask_type\x18\x04 \x03(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12K\n\x0cnum_attempts\x18\x05 \x01(\x0b\x32(.tecton_proto.metadataservice.CountRangeR\x0bnumAttempts\x12-\n\x12manually_triggered\x18\x07 \x01(\x08R\x11manuallyTriggered\x12G\n\x08\x64uration\x18\x08 \x01(\x0b\x32+.tecton_proto.metadataservice.DurationRangeR\x08\x64uration\x12Y\n\x12\x66\x65\x61ture_start_time\x18\n \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x10\x66\x65\x61tureStartTime\x12U\n\x10\x66\x65\x61ture_end_time\x18\x0b \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x0e\x66\x65\x61tureEndTime\x12O\n\npagination\x18\t \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xc5\x01\n FeatureViewMaterializationStatus\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"\xbe\x04\n\x10TaskWithAttempts\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12T\n\ttaskState\x18\x02 \x01(\x0e\x32\x36.tecton_proto.materialization.MaterializationTaskStateR\ttaskState\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\x12\x30\n\x07task_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x08 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12*\n\x11\x66\x65\x61ture_view_name\x18\x05 \x01(\tR\x0f\x66\x65\x61tureViewName\x12H\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\"\xc5\x01\n3GetAllMaterializationStatusInLiveWorkspacesResponse\x12\x8d\x01\n#feature_view_materialization_status\x18\x01 \x03(\x0b\x32>.tecton_proto.metadataservice.FeatureViewMaterializationStatusR featureViewMaterializationStatus\"\xc1\x01\n\x0fGetJobsResponse\x12\\\n\x11tasksWithAttempts\x18\x01 \x03(\x0b\x32..tecton_proto.metadataservice.TaskWithAttemptsR\x11tasksWithAttempts\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xa0\x01\n$ForceRetryMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\x12\'\n\x0f\x61llow_overwrite\x18\x02 \x01(\x08R\x0e\x61llowOverwrite\"L\n%ForceRetryMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\".\n\x0eGetFcosRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"W\n\x0fGetFcosResponse\x12\x44\n\rfco_container\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"a\n\x15GetSparkConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xb0\x01\n\x16GetSparkConfigResponse\x12I\n\x0c\x62\x61tch_config\x18\x01 \x01(\x0b\x32&.tecton_proto.spark_common.ClusterInfoR\x0b\x62\x61tchConfig\x12K\n\rstream_config\x18\x02 \x01(\x0b\x32&.tecton_proto.spark_common.ClusterInfoR\x0cstreamConfig\"t\n(GetMetricAndExpectationDefinitionRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xe4\x02\n)GetMetricAndExpectationDefinitionResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x36\n\x07metrics\x18\x03 \x03(\x0b\x32\x1c.tecton_proto.dataobs.MetricR\x07metrics\x12[\n\x14\x66\x65\x61ture_expectations\x18\x04 \x03(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x13\x66\x65\x61tureExpectations\x12X\n\x13metric_expectations\x18\x05 \x03(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x12metricExpectations\"\x91\x01\n\x15GetFeatureViewRequest\x12+\n\x11version_specifier\x18\x01 \x01(\tR\x10versionSpecifier\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02idJ\x04\x08\x05\x10\x06\"^\n\x16GetFeatureViewResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"`\n\x1cGetFeatureViewSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"_\n\x1dGetFeatureViewSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"R\n\x18QueryFeatureViewsRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceJ\x04\x08\x05\x10\x06\"a\n\x19QueryFeatureViewsResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"{\n4GetMaterializingFeatureViewsInLiveWorkspacesResponse\x12\x43\n\rfeature_views\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.FeatureViewR\x0c\x66\x65\x61tureViews\"\xba\x01\n\x1bGetVirtualDataSourceRequest\x12N\n\x16virtual_data_source_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x13virtualDataSourceId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"d\n\x1cGetVirtualDataSourceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"?\n\x1fGetAllVirtualDataSourcesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n GetAllVirtualDataSourcesResponse\x12V\n\x14virtual_data_sources\x18\x01 \x03(\x0b\x32$.tecton_proto.data.VirtualDataSourceR\x12virtualDataSources\"\x97\x01\n\x10GetEntityRequest\x12\x36\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x08\x65ntityId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"Y\n\x11GetEntityResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"5\n\x15GetAllEntitiesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"O\n\x16GetAllEntitiesResponse\x12\x35\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.tecton_proto.data.EntityR\x08\x65ntities\"\xaf\x01\n\x18GetTransformationRequest\x12\x46\n\x11transformation_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10transformationId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x04 \x01(\tR\tworkspaceB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"g\n\x19GetTransformationResponse\x12\x44\n\rfco_container\x18\x03 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainerJ\x04\x08\x01\x10\x02\"<\n\x1cGetAllTransformationsRequest\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"r\n\x1dGetAllTransformationsResponse\x12K\n\x0ftransformations\x18\x02 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformationsJ\x04\x08\x01\x10\x02\"B\n\x17\x46indFcoWorkspaceRequest\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"8\n\x18\x46indFcoWorkspaceResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n\x17IngestClientLogsRequest\x12_\n\x15sdk_method_invocation\x18\x01 \x01(\x0b\x32+.tecton_proto.amplitude.SDKMethodInvocationR\x13sdkMethodInvocation\"v\n\x16IngestAnalyticsRequest\x12>\n\x06\x65vents\x18\x01 \x03(\x0b\x32&.tecton_proto.amplitude.AmplitudeEventR\x06\x65vents\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xbf\x01\n\x15NewStateUpdateRequest\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\"\xfd\x01\n\x17NewStateUpdateRequestV2\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\x12\x19\n\x08no_color\x18\x04 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x05 \x01(\x08R\njsonOutput\"\xe7\x01\n\x16NewStateUpdateResponse\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12]\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x36.tecton_proto.metadataservice.QueryStateUpdateResponseR\reagerResponse\"\xeb\x01\n\x18NewStateUpdateResponseV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12_\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2R\reagerResponse\"k\n\x17QueryStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xa9\x01\n\x19QueryStateUpdateRequestV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x19\n\x08no_color\x18\x03 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x04 \x01(\x08R\njsonOutput\"\xd4\x02\n\x18QueryStateUpdateResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x31\n\x14recreates_suppressed\x18\x07 \x01(\x08R\x13recreatesSuppressed\x12P\n\x11validation_result\x18\x04 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x39\n\ndiff_items\x18\x05 \x03(\x0b\x32\x1a.tecton_proto.data.FcoDiffR\tdiffItems\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\"\xe9\x02\n\x1aQueryStateUpdateResponseV2\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\x12R\n\x11validation_errors\x18\x08 \x01(\x0b\x32#.tecton_proto.data.ValidationResultH\x00R\x10validationErrors\x12_\n\x16successful_plan_output\x18\t \x01(\x0b\x32\'.tecton_proto.data.SuccessfulPlanOutputH\x00R\x14successfulPlanOutputB\n\n\x08responseJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"T\n GetStateUpdatePlanSummaryRequest\x12\x30\n\x07plan_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06planId\"b\n!GetStateUpdatePlanSummaryResponse\x12=\n\x04plan\x18\x01 \x01(\x0b\x32).tecton_proto.data.StateUpdatePlanSummaryR\x04plan\"p\n\x17\x41pplyStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12!\n\napplied_by\x18\x02 \x01(\tB\x02\x18\x01R\tappliedBy\"\x1a\n\x18\x41pplyStateUpdateResponse\"\xb2\x01\n\x12GetConfigsResponse\x12^\n\nkey_values\x18\x01 \x03(\x0b\x32?.tecton_proto.metadataservice.GetConfigsResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc2\x01\n\x1aGetGlobalsForWebUIResponse\x12\x66\n\nkey_values\x18\x01 \x03(\x0b\x32G.tecton_proto.metadataservice.GetGlobalsForWebUIResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"N\n\x18GetStateUpdateLogRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"Z\n\x19GetStateUpdateLogResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32#.tecton_proto.data.StateUpdateEntryR\x07\x65ntries\"R\n\x15GetRestoreInfoRequest\x12\x1b\n\tcommit_id\x18\x01 \x01(\tR\x08\x63ommitId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\x96\x01\n\x16GetRestoreInfoResponse\x12>\n\x1csigned_url_for_repo_download\x18\x01 \x01(\tR\x18signedUrlForRepoDownload\x12\x1b\n\tcommit_id\x18\x02 \x01(\tR\x08\x63ommitId\x12\x1f\n\x0bsdk_version\x18\x03 \x01(\tR\nsdkVersion\"\x93\x01\n\x16\x43reateWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x02 \x01(\tR\rworkspaceName\x12L\n\x0c\x63\x61pabilities\x18\x03 \x01(\x0b\x32(.tecton_proto.data.WorkspaceCapabilitiesR\x0c\x63\x61pabilitiesJ\x04\x08\x01\x10\x02\"6\n\x16\x44\x65leteWorkspaceRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"2\n\x17IntrospectApiKeyRequest\x12\x17\n\x07\x61pi_key\x18\x01 \x01(\tR\x06\x61piKey\"\xcb\x01\n\x18IntrospectApiKeyResponse\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x03 \x01(\tR\tcreatedBy\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\"R\n\x13\x43reateApiKeyRequest\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x19\n\x08is_admin\x18\x02 \x01(\x08R\x07isAdmin\"Q\n\x14\x43reateApiKeyResponse\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\">\n\x13\x44\x65leteApiKeyRequest\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"?\n\x12ListApiKeysRequest\x12)\n\x10include_archived\x18\x01 \x01(\x08R\x0fincludeArchived\"Q\n\x13ListApiKeysResponse\x12:\n\x08\x61pi_keys\x18\x01 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x07\x61piKeys\"\xe4\x01\n\x0eServiceAccount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12\x36\n\x07\x63reator\x18\x05 \x01(\x0b\x32\x1c.tecton_proto.auth.PrincipalR\x07\x63reator\x12\x37\n\x05owner\x18\x06 \x01(\x0b\x32!.tecton_proto.auth.PrincipalBasicR\x05owner\"S\n\x1b\x43reateServiceAccountRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"\x9a\x01\n\x1c\x43reateServiceAccountResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12\x17\n\x07\x61pi_key\x18\x05 \x01(\tR\x06\x61piKey\"E\n\x19GetServiceAccountsRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\"u\n\x1aGetServiceAccountsResponse\x12W\n\x10service_accounts\x18\x01 \x03(\x0b\x32,.tecton_proto.metadataservice.ServiceAccountR\x0fserviceAccounts\"\x80\x01\n\x1bUpdateServiceAccountRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\"\x81\x01\n\x1cUpdateServiceAccountResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\"-\n\x1b\x44\x65leteServiceAccountRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x1e\n\x1c\x44\x65leteServiceAccountResponse\"\x17\n\x15ListWorkspacesRequest\"V\n\x16ListWorkspacesResponse\x12<\n\nworkspaces\x18\x01 \x03(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\nworkspaces\"<\n\x13GetWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\"R\n\x14GetWorkspaceResponse\x12:\n\tworkspace\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\tworkspace\"\x93\x03\n\"CreateSavedFeatureDataFrameRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x07 \x01(\tR\tworkspace\x12G\n\x12\x66\x65\x61ture_package_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x31\n\x15join_key_column_names\x18\x04 \x03(\tR\x12joinKeyColumnNames\x12\x32\n\x15timestamp_column_name\x18\x05 \x01(\tR\x13timestampColumnName\x12\x38\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x06schemaB\x08\n\x06source\"\x87\x01\n#CreateSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"{\n#ArchiveSavedFeatureDataFrameRequest\x12T\n\x1asaved_feature_dataframe_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x17savedFeatureDataframeId\"&\n$ArchiveSavedFeatureDataFrameResponse\"\xe7\x01\n\x1fGetSavedFeatureDataFrameRequest\x12\x41\n\x1csaved_feature_dataframe_name\x18\x01 \x01(\tH\x00R\x19savedFeatureDataframeName\x12V\n\x1asaved_feature_dataframe_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x17savedFeatureDataframeId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0b\n\treference\"\xa5\x01\n\x1bGetClusterAdminInfoResponse\x12&\n\x0f\x63\x61ller_is_admin\x18\x01 \x01(\x08R\rcallerIsAdmin\x12-\n\x05users\x18\x02 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x05users\x12/\n\x06\x61\x64mins\x18\x03 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x06\x61\x64mins\";\n\x18\x43reateClusterUserRequest\x12\x1f\n\x0blogin_email\x18\x01 \x01(\tR\nloginEmail\"@\n\x19\x43reateClusterUserResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"3\n\x18\x44\x65leteClusterUserRequest\x12\x17\n\x07okta_id\x18\x01 \x01(\tR\x06oktaId\"@\n\x19\x44\x65leteClusterUserResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"\xe2\x01\n\x18\x43lusterUserActionRequest\x12\x17\n\x07okta_id\x18\x01 \x01(\tR\x06oktaId\x12\x38\n\x17resend_activation_email\x18\x02 \x01(\x08H\x00R\x15resendActivationEmail\x12!\n\x0bunlock_user\x18\x03 \x01(\x08H\x00R\nunlockUser\x12!\n\x0bgrant_admin\x18\x04 \x01(\x08H\x00R\ngrantAdmin\x12#\n\x0crevoke_admin\x18\x05 \x01(\x08H\x00R\x0brevokeAdminB\x08\n\x06\x61\x63tion\"@\n\x19\x43lusterUserActionResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"\x84\x01\n GetSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"C\n#GetAllSavedFeatureDataFramesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x8a\x01\n$GetAllSavedFeatureDataFramesResponse\x12\x62\n\x18saved_feature_dataframes\x18\x01 \x03(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x16savedFeatureDataframes\"\x9c\x01\n\x16IngestDataframeRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\x12\x17\n\x07\x64\x66_path\x18\x02 \x01(\tR\x06\x64\x66Path\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\"\x19\n\x17IngestDataframeResponse\"o\n GetNewIngestDataframeInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"t\n!GetNewIngestDataframeInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x36\n\x18signed_url_for_df_upload\x18\x02 \x01(\tR\x14signedUrlForDfUpload\"\x88\x01\n!GetUserDeploymentSettingsResponse\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\"\xc5\x01\n#UpdateUserDeploymentSettingsRequest\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\x12\x39\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\tfieldMask\"e\n$UpdateUserDeploymentSettingsResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\"n\n%GetInternalSparkClusterStatusResponse\x12\x45\n\x06status\x18\x01 \x01(\x0b\x32-.tecton_proto.data.InternalSparkClusterStatusR\x06status\"k\n\x1cGetDeleteEntitiesInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"\xca\x01\n\x1dGetDeleteEntitiesInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x43\n\x1fsigned_url_for_df_upload_online\x18\x03 \x01(\tR\x1asignedUrlForDfUploadOnline\x12\x45\n signed_url_for_df_upload_offline\x18\x04 \x01(\tR\x1bsignedUrlForDfUploadOfflineJ\x04\x08\x02\x10\x03\"\xf3\x01\n\x15\x44\x65leteEntitiesRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12\x31\n\x15online_join_keys_path\x18\x02 \x01(\tR\x12onlineJoinKeysPath\x12\x33\n\x16offline_join_keys_path\x18\x03 \x01(\tR\x13offlineJoinKeysPath\x12\x16\n\x06online\x18\x04 \x01(\x08R\x06online\x12\x18\n\x07offline\x18\x05 \x01(\x08R\x07offline\"\x18\n\x16\x44\x65leteEntitiesResponse\"\xf9\x01\n\x16GetHiveMetadataRequest\x12S\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32;.tecton_proto.metadataservice.GetHiveMetadataRequest.ActionR\x06\x61\x63tion\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x14\n\x05table\x18\x03 \x01(\tR\x05table\"X\n\x06\x41\x63tion\x12\x19\n\x15\x41\x43TION_LIST_DATABASES\x10\x00\x12\x16\n\x12\x41\x43TION_LIST_TABLES\x10\x01\x12\x1b\n\x17\x41\x43TION_GET_TABLE_SCHEMA\x10\x02\"\xd1\x02\n\x17GetHiveMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12\x41\n\tdatabases\x18\x03 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\tdatabases\x12;\n\x06tables\x18\x04 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\x06tables\x12=\n\x07\x63olumns\x18\x05 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\x07\x63olumns\x12.\n\x13\x64\x65\x62ug_error_message\x18\x06 \x01(\tR\x11\x64\x65\x62ugErrorMessageB\x08\n\x06result\"K\n\x16GetFileMetadataRequest\x12\x10\n\x03uri\x18\x01 \x01(\tR\x03uri\x12\x1f\n\x0b\x66ile_format\x18\x02 \x01(\tR\nfileFormat\"\xab\x01\n\x17GetFileMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12!\n\x0c\x63olumn_names\x18\x03 \x03(\tR\x0b\x63olumnNames\x12.\n\x13\x64\x65\x62ug_error_message\x18\x04 \x01(\tR\x11\x64\x65\x62ugErrorMessage\"R\n\x13ValidateFcosRequest\x12\x35\n\x08\x66\x63o_args\x18\x02 \x03(\x0b\x32\x1a.tecton_proto.args.FcoArgsR\x07\x66\x63oArgsJ\x04\x08\x01\x10\x02\"\xe6\x01\n\x14ValidateFcosResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x32\n\x15\x64isplay_error_message\x18\x04 \x01(\tR\x13\x64isplayErrorMessage\x12.\n\x13\x64\x65\x62ug_error_message\x18\x03 \x01(\tR\x11\x64\x65\x62ugErrorMessage\"\x95\x01\n\x17ValidateLocalFcoRequest\x12Y\n\x12validation_request\x18\x01 \x01(\x0b\x32*.tecton_proto.validation.ValidationRequestR\x11validationRequest\x12\x1f\n\x0bsdk_version\x18\x02 \x01(\tR\nsdkVersion\"\x9c\x01\n\x18ValidateLocalFcoResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\":\n\x1aGetOnboardingStatusRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x9c\x02\n\x1bGetOnboardingStatusResponse\x12N\n\x0esetup_platform\x18\x03 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\rsetupPlatform\x12W\n\x13\x63reate_feature_view\x18\x01 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x11\x63reateFeatureView\x12T\n\x11\x66inish_onboarding\x18\x02 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x10\x66inishOnboarding\"]\n\x1aSetOnboardingStatusRequest\x12?\n\x06status\x18\x01 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x06status\"\x92\x01\n\"GetDataPlatformSetupStatusResponse\x12&\n\x0esetupCompleted\x18\x01 \x01(\x08R\x0esetupCompleted\x12\x44\n\x05tasks\x18\x02 \x03(\x0b\x32..tecton_proto.data.DataPlatformSetupTaskStatusR\x05tasks\"7\n#GetRetrieveFeaturesNotebookResponse\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\"i\n\x1dGetObservabilityConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xa5\x01\n\x1eGetObservabilityConfigResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x39\n\x19is_dataobs_metric_enabled\x18\x03 \x01(\x08R\x16isDataobsMetricEnabled\"\x93\x02\n\x12QueryMetricRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12\x39\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x35\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndTime\"\xf5\x03\n\x13QueryMetricResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12V\n\x1ametric_data_point_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17metricDataPointInterval\x12H\n\x12\x61ligned_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x61lignedStartTime\x12\x44\n\x10\x61ligned_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x61lignedEndTime\x12\x46\n\x0bmetric_data\x18\x04 \x03(\x0b\x32%.tecton_proto.dataobs.MetricDataPointR\nmetricData\x12!\n\x0c\x63olumn_names\x18\x06 \x03(\tR\x0b\x63olumnNames\"\x89\x01\n\"GetFeatureValidationHistoryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x19\n\x05limit\x18\x03 \x01(\x05:\x03\x31\x30\x30R\x05limit\"\xb2\x01\n#GetFeatureValidationHistoryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x07results\x18\x03 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\"\xde\x01\n\"GetFeatureValidationSummaryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\"\xba\x02\n#GetFeatureValidationSummaryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12Y\n\x11workspace_summary\x18\x04 \x01(\x0b\x32,.tecton_proto.dataobs.WorkspaceResultSummaryR\x10workspaceSummary\"6\n\x0eGetUserRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\"C\n\x0fGetUserResponse\x12\x30\n\x04user\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.auth.UserBasicR\x04user\"\x1f\n\x1dGetFeatureServerConfigRequest\"\x90\x01\n\x1eGetFeatureServerConfigResponse\x12\"\n\x0c\x63urrentCount\x18\x01 \x01(\rR\x0c\x63urrentCount\x12&\n\x0e\x61vailableCount\x18\x02 \x01(\rR\x0e\x61vailableCount\x12\"\n\x0c\x64\x65siredCount\x18\x03 \x01(\rR\x0c\x64\x65siredCount\"5\n\x1dSetFeatureServerConfigRequest\x12\x14\n\x05\x63ount\x18\x01 \x01(\rR\x05\x63ount*>\n\rSortDirection\x12\x10\n\x0cSORT_UNKNOWN\x10\x00\x12\x0c\n\x08SORT_ASC\x10\x01\x12\r\n\tSORT_DESC\x10\x02\x32\x98\x95\x01\n\x0fMetadataService\x12\xec\x01\n\x11GetFeatureService\x12\x36.tecton_proto.metadataservice.GetFeatureServiceRequest\x1a\x37.tecton_proto.metadataservice.GetFeatureServiceResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-feature-service:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfd\x01\n\x15GetAllFeatureServices\x12:.tecton_proto.metadataservice.GetAllFeatureServicesRequest\x1a;.tecton_proto.metadataservice.GetAllFeatureServicesResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-all-feature-services:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x98\x02\n\x18GetFeatureServiceSummary\x12=.tecton_proto.metadataservice.GetFeatureServiceSummaryRequest\x1a>.tecton_proto.metadataservice.GetFeatureServiceSummaryResponse\"}\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/get-feature-service-summary:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\xf7\x01\n\x10GetServingStatus\x12\x35.tecton_proto.metadataservice.GetServingStatusRequest\x1a\x36.tecton_proto.metadataservice.GetServingStatusResponse\"t\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-serving-status:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x96\x02\n\x17GetFVServingStatusForFS\x12<.tecton_proto.metadataservice.GetFVServingStatusForFSRequest\x1a=.tecton_proto.metadataservice.GetFVServingStatusForFSResponse\"~\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-fv-serving-status-for-fs:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x16GetAllFeatureFreshness\x12;.tecton_proto.metadataservice.GetAllFeatureFreshnessRequest\x1a<.tecton_proto.metadataservice.GetAllFeatureFreshnessResponse\"{\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-all-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x13GetFeatureFreshness\x12\x38.tecton_proto.metadataservice.GetFeatureFreshnessRequest\x1a\x39.tecton_proto.metadataservice.GetFeatureFreshnessResponse\"\x83\x01\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xdd\x01\n\x18GetMaterializationStatus\x12=.tecton_proto.metadataservice.GetMaterializationStatusRequest\x1a>.tecton_proto.metadataservice.GetMaterializationStatusResponse\"B\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-service/get-materialization-status:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xac\x02\n+GetAllMaterializationStatusInLiveWorkspaces\x12P.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesRequest\x1aQ.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesResponse\"X\x82\xd3\xe4\x93\x02J\"E/v1/metadata-service/get-all-materialization-status-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x94\x01\n\x07GetJobs\x12,.tecton_proto.metadataservice.GetJobsRequest\x1a-.tecton_proto.metadataservice.GetJobsResponse\",\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/metadata-service/jobs:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xf2\x01\n\x1d\x46orceRetryMaterializationTask\x12\x42.tecton_proto.metadataservice.ForceRetryMaterializationTaskRequest\x1a\x43.tecton_proto.metadataservice.ForceRetryMaterializationTaskResponse\"H\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/force-retry-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe0\x01\n\x0eGetSparkConfig\x12\x33.tecton_proto.metadataservice.GetSparkConfigRequest\x1a\x34.tecton_proto.metadataservice.GetSparkConfigResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-spark-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xae\x02\n!GetMetricAndExpectationDefinition\x12\x46.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionRequest\x1aG.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionResponse\"x\x82\xd3\xe4\x93\x02?\":/v1/metadata-service/get-metric-and-expectation-definition:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetFeatureView\x12\x33.tecton_proto.metadataservice.GetFeatureViewRequest\x1a\x34.tecton_proto.metadataservice.GetFeatureViewResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-feature-view:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf0\x01\n,GetMaterializingFeatureViewsInLiveWorkspaces\x12\x16.google.protobuf.Empty\x1aR.tecton_proto.metadataservice.GetMaterializingFeatureViewsInLiveWorkspacesResponse\"T\x82\xd3\xe4\x93\x02\x46\"A/v1/metadata-service/get-materializing-features-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xec\x01\n\x11QueryFeatureViews\x12\x36.tecton_proto.metadataservice.QueryFeatureViewsRequest\x1a\x37.tecton_proto.metadataservice.QueryFeatureViewsResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/query-feature-views:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x99\x02\n\x15GetFeatureViewSummary\x12:.tecton_proto.metadataservice.GetFeatureViewSummaryRequest\x1a;.tecton_proto.metadataservice.GetFeatureViewSummaryResponse\"\x86\x01\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-package/get-feature-view-summary:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\x8d\x02\n\x15GetFeatureConsumption\x12:.tecton_proto.metadataservice.GetFeatureConsumptionRequest\x1a;.tecton_proto.metadataservice.GetFeatureConsumptionResponse\"{\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-feature-view-consumption:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xf9\x01\n\x14GetVirtualDataSource\x12\x39.tecton_proto.metadataservice.GetVirtualDataSourceRequest\x1a:.tecton_proto.metadataservice.GetVirtualDataSourceResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-virtual-data-source:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8a\x02\n\x18GetAllVirtualDataSources\x12=.tecton_proto.metadataservice.GetAllVirtualDataSourcesRequest\x1a>.tecton_proto.metadataservice.GetAllVirtualDataSourcesResponse\"o\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-all-virtual-data-sources:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x90\x01\n\x10IngestClientLogs\x12\x35.tecton_proto.metadataservice.IngestClientLogsRequest\x1a\x16.google.protobuf.Empty\"-\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xbe\x01\n\x0fIngestAnalytics\x12\x34.tecton_proto.metadataservice.IngestAnalyticsRequest\x1a\x16.google.protobuf.Empty\"]\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/ingest-analytics:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa2\x02\n\x1bGetVirtualDataSourceSummary\x12@.tecton_proto.metadataservice.GetVirtualDataSourceSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetVirtualDataSourceSummaryResponse\"~\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/get-virtual-data-source-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xc3\x01\n\x07GetFcos\x12,.tecton_proto.metadataservice.GetFcosRequest\x1a-.tecton_proto.metadataservice.GetFcosResponse\"[\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-fcos:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xa1\x01\n\tGetEntity\x12..tecton_proto.metadataservice.GetEntityRequest\x1a/.tecton_proto.metadataservice.GetEntityResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetAllEntities\x12\x33.tecton_proto.metadataservice.GetAllEntitiesRequest\x1a\x34.tecton_proto.metadataservice.GetAllEntitiesResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-all-entities:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf4\x01\n\x10GetEntitySummary\x12\x35.tecton_proto.metadataservice.GetEntitySummaryRequest\x1a\x36.tecton_proto.metadataservice.GetEntitySummaryResponse\"q\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-package/get-entity-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xeb\x01\n\x11GetTransformation\x12\x36.tecton_proto.metadataservice.GetTransformationRequest\x1a\x37.tecton_proto.metadataservice.GetTransformationResponse\"e\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-transformation:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfc\x01\n\x15GetAllTransformations\x12:.tecton_proto.metadataservice.GetAllTransformationsRequest\x1a;.tecton_proto.metadataservice.GetAllTransformationsResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-all-transformations:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x94\x02\n\x18GetTransformationSummary\x12=.tecton_proto.metadataservice.GetTransformationSummaryRequest\x1a>.tecton_proto.metadataservice.GetTransformationSummaryResponse\"y\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-package/get-transformation-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xbd\x01\n\x10\x46indFcoWorkspace\x12\x35.tecton_proto.metadataservice.FindFcoWorkspaceRequest\x1a\x36.tecton_proto.metadataservice.FindFcoWorkspaceResponse\":\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/find-fco-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb8\x01\n\x0eNewStateUpdate\x12\x33.tecton_proto.metadataservice.NewStateUpdateRequest\x1a\x34.tecton_proto.metadataservice.NewStateUpdateResponse\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#read_config\x12\xbe\x01\n\x10NewStateUpdateV2\x12\x35.tecton_proto.metadataservice.NewStateUpdateRequestV2\x1a\x36.tecton_proto.metadataservice.NewStateUpdateResponseV2\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#read_config\x12\xb8\x01\n\x10ValidateLocalFco\x12\x35.tecton_proto.metadataservice.ValidateLocalFcoRequest\x1a\x36.tecton_proto.metadataservice.ValidateLocalFcoResponse\"5\xa2\xbc\xe6\xc0\x05/*-tecton/organization#validate_notebook_objects\x12\xb6\x01\n\x10QueryStateUpdate\x12\x35.tecton_proto.metadataservice.QueryStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.QueryStateUpdateResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xbc\x01\n\x12QueryStateUpdateV2\x12\x37.tecton_proto.metadataservice.QueryStateUpdateRequestV2\x1a\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8b\x01\n\x10\x41pplyStateUpdate\x12\x35.tecton_proto.metadataservice.ApplyStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.ApplyStateUpdateResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb0\x01\n\nGetConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/get-configs:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xcb\x01\n\x12GetGlobalsForWebUI\x12\x16.google.protobuf.Empty\x1a\x38.tecton_proto.metadataservice.GetGlobalsForWebUIResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-globals-for-web-ui:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x98\x01\n\x0fGetLoginConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\";\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-login-configs:\x01*\xa2\xbc\xe6\xc0\x05\x04\x08\x01\x10\x01\x12?\n\x03Nop\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x08\xa2\xbc\xe6\xc0\x05\x02\x10\x01\x12\xe3\x01\n\x19GetStateUpdatePlanSummary\x12>.tecton_proto.metadataservice.GetStateUpdatePlanSummaryRequest\x1a?.tecton_proto.metadataservice.GetStateUpdatePlanSummaryResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-state-update-plan-summary:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xed\x01\n\x11GetStateUpdateLog\x12\x36.tecton_proto.metadataservice.GetStateUpdateLogRequest\x1a\x37.tecton_proto.metadataservice.GetStateUpdateLogResponse\"g\x82\xd3\xe4\x93\x02.\")/v1/metadata-service/get-state-update-log:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x01\n\x0eGetRestoreInfo\x12\x33.tecton_proto.metadataservice.GetRestoreInfoRequest\x1a\x34.tecton_proto.metadataservice.GetRestoreInfoResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8e\x02\n\x0f\x43reateWorkspace\x12\x34.tecton_proto.metadataservice.CreateWorkspaceRequest\x1a\x16.google.protobuf.Empty\"\xac\x01\xa2\xbc\xe6\xc0\x05v*$tecton/organization#create_workspace2N\n\x1b\x63\x61pabilities.materializable\x12\x04true\x1a)tecton/organization#create_workspace_live\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/create-workspace:\x01*\x12\x99\x01\n\x0f\x44\x65leteWorkspace\x12\x34.tecton_proto.metadataservice.DeleteWorkspaceRequest\x1a\x16.google.protobuf.Empty\"8\xa2\xbc\xe6\xc0\x05\x32\x1a\r\x08\x01\x12\tworkspace*!tecton/workspace#delete_workspace\x12\xb4\x01\n\x0eListWorkspaces\x12\x33.tecton_proto.metadataservice.ListWorkspacesRequest\x1a\x34.tecton_proto.metadataservice.ListWorkspacesResponse\"7\x82\xd3\xe4\x93\x02)\"$/v1/metadata-service/list-workspaces:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xdf\x01\n\x0cGetWorkspace\x12\x31.tecton_proto.metadataservice.GetWorkspaceRequest\x1a\x32.tecton_proto.metadataservice.GetWorkspaceResponse\"h\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/get-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x35\x1a\x12\x08\x01\x12\x0eworkspace_name*\x1ftecton/workspace#read_workspace\x12\xe5\x01\n\x10IntrospectApiKey\x12\x35.tecton_proto.metadataservice.IntrospectApiKeyRequest\x1a\x36.tecton_proto.metadataservice.IntrospectApiKeyResponse\"b\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/introspect-api-key:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xf7\x01\n\x14\x43reateServiceAccount\x12\x39.tecton_proto.metadataservice.CreateServiceAccountRequest\x1a:.tecton_proto.metadataservice.CreateServiceAccountResponse\"h\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/create-service-account:\x01*\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\x12\xec\x01\n\x12GetServiceAccounts\x12\x37.tecton_proto.metadataservice.GetServiceAccountsRequest\x1a\x38.tecton_proto.metadataservice.GetServiceAccountsResponse\"c\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-service-account:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\x82\x02\n\x14UpdateServiceAccount\x12\x39.tecton_proto.metadataservice.UpdateServiceAccountRequest\x1a:.tecton_proto.metadataservice.UpdateServiceAccountResponse\"s\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/update-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\x12\x82\x02\n\x14\x44\x65leteServiceAccount\x12\x39.tecton_proto.metadataservice.DeleteServiceAccountRequest\x1a:.tecton_proto.metadataservice.DeleteServiceAccountResponse\"s\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/delete-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\x12\xef\x01\n\x0c\x43reateApiKey\x12\x31.tecton_proto.metadataservice.CreateApiKeyRequest\x1a\x32.tecton_proto.metadataservice.CreateApiKeyResponse\"x\xa2\xbc\xe6\xc0\x05r**tecton/organization#create_service_account2B\n\x08is_admin\x12\x04true\x1a\x30tecton/organization#create_service_account_admin8\x01\x12\x9a\x01\n\x0c\x44\x65leteApiKey\x12\x31.tecton_proto.metadataservice.DeleteApiKeyRequest\x1a\x16.google.protobuf.Empty\"?\xa2\xbc\xe6\xc0\x05\x39\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account8\x01\x12\xa4\x01\n\x0bListApiKeys\x12\x30.tecton_proto.metadataservice.ListApiKeysRequest\x1a\x31.tecton_proto.metadataservice.ListApiKeysResponse\"0\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xda\x01\n\x1b\x43reateSavedFeatureDataFrame\x12@.tecton_proto.metadataservice.CreateSavedFeatureDataFrameRequest\x1a\x41.tecton_proto.metadataservice.CreateSavedFeatureDataFrameResponse\"6\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#update_dataset\x12\xaf\x01\n\x1c\x41rchiveSavedFeatureDataFrame\x12\x41.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameRequest\x1a\x42.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xcf\x01\n\x18GetSavedFeatureDataFrame\x12=.tecton_proto.metadataservice.GetSavedFeatureDataFrameRequest\x1a>.tecton_proto.metadataservice.GetSavedFeatureDataFrameResponse\"4\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\x9b\x02\n\x1cGetAllSavedFeatureDataFrames\x12\x41.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesRequest\x1a\x42.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesResponse\"t\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/get-all-saved-feature-dataframes:\x01*\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\xa6\x01\n\x19GetNewIngestDataframeInfo\x12>.tecton_proto.metadataservice.GetNewIngestDataframeInfoRequest\x1a?.tecton_proto.metadataservice.GetNewIngestDataframeInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb7\x01\n\x0fIngestDataframe\x12\x34.tecton_proto.metadataservice.IngestDataframeRequest\x1a\x35.tecton_proto.metadataservice.IngestDataframeResponse\"7\xa2\xbc\xe6\xc0\x05\x31\x1a\r\x08\x01\x12\tworkspace* tecton/workspace#ingest_features\x12\xcd\x01\n\x13GetClusterAdminInfo\x12\x16.google.protobuf.Empty\x1a\x39.tecton_proto.metadataservice.GetClusterAdminInfoResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-cluster-admin-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xe0\x01\n\x11\x43reateClusterUser\x12\x36.tecton_proto.metadataservice.CreateClusterUserRequest\x1a\x37.tecton_proto.metadataservice.CreateClusterUserResponse\"Z\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/create-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#create_user\x12\xe0\x01\n\x11\x44\x65leteClusterUser\x12\x36.tecton_proto.metadataservice.DeleteClusterUserRequest\x1a\x37.tecton_proto.metadataservice.DeleteClusterUserResponse\"Z\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/delete-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\x12\xe0\x01\n\x11\x43lusterUserAction\x12\x36.tecton_proto.metadataservice.ClusterUserActionRequest\x1a\x37.tecton_proto.metadataservice.ClusterUserActionResponse\"Z\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/cluster-user-action:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\x12\xdf\x01\n\x19GetUserDeploymentSettings\x12\x16.google.protobuf.Empty\x1a?.tecton_proto.metadataservice.GetUserDeploymentSettingsResponse\"i\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9c\x02\n\x1cUpdateUserDeploymentSettings\x12\x41.tecton_proto.metadataservice.UpdateUserDeploymentSettingsRequest\x1a\x42.tecton_proto.metadataservice.UpdateUserDeploymentSettingsResponse\"u\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/update-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xec\x01\n\x1dGetInternalSparkClusterStatus\x12\x16.google.protobuf.Empty\x1a\x43.tecton_proto.metadataservice.GetInternalSparkClusterStatusResponse\"n\x82\xd3\xe4\x93\x02;\"6/v1/metadata-service/get-internal-spark-cluster-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9a\x01\n\x15GetDeleteEntitiesInfo\x12:.tecton_proto.metadataservice.GetDeleteEntitiesInfoRequest\x1a;.tecton_proto.metadataservice.GetDeleteEntitiesInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc0\x01\n\x0e\x44\x65leteEntities\x12\x33.tecton_proto.metadataservice.DeleteEntitiesRequest\x1a\x34.tecton_proto.metadataservice.DeleteEntitiesResponse\"C\xa2\xbc\xe6\xc0\x05=\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace* tecton/workspace#delete_features\x12\xde\x01\n\x0fGetHiveMetadata\x12\x34.tecton_proto.metadataservice.GetHiveMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetHiveMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-hive-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xde\x01\n\x0fGetFileMetadata\x12\x34.tecton_proto.metadataservice.GetFileMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetFileMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-file-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xda\x01\n\x0cValidateFcos\x12\x31.tecton_proto.metadataservice.ValidateFcosRequest\x1a\x32.tecton_proto.metadataservice.ValidateFcosResponse\"c\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/validate-fcos:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xf7\x01\n\x13GetOnboardingStatus\x12\x38.tecton_proto.metadataservice.GetOnboardingStatusRequest\x1a\x39.tecton_proto.metadataservice.GetOnboardingStatusResponse\"k\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#read_workspace\x12\xcb\x01\n\x13SetOnboardingStatus\x12\x38.tecton_proto.metadataservice.SetOnboardingStatusRequest\x1a\x16.google.protobuf.Empty\"b\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/set-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xe3\x01\n\x1aGetDataPlatformSetupStatus\x12\x16.google.protobuf.Empty\x1a@.tecton_proto.metadataservice.GetDataPlatformSetupStatusResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-data-platform-setup-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xe5\x01\n\x1bGetRetrieveFeaturesNotebook\x12\x16.google.protobuf.Empty\x1a\x41.tecton_proto.metadataservice.GetRetrieveFeaturesNotebookResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-retrieve-features-notebook:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x80\x02\n\x16GetObservabilityConfig\x12;.tecton_proto.metadataservice.GetObservabilityConfigRequest\x1a<.tecton_proto.metadataservice.GetObservabilityConfigResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-observability-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xd3\x01\n\x0bQueryMetric\x12\x30.tecton_proto.metadataservice.QueryMetricRequest\x1a\x31.tecton_proto.metadataservice.QueryMetricResponse\"_\x82\xd3\xe4\x93\x02&\"!/v1/metadata-service/query-metric:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationHistory\x12@.tecton_proto.metadataservice.GetFeatureValidationHistoryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationHistoryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-history:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationSummary\x12@.tecton_proto.metadataservice.GetFeatureValidationSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationSummaryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-summary:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\xfb\x01\n\x16GetFeatureServerConfig\x12;.tecton_proto.metadataservice.GetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"f\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xfe\x01\n\x16SetFeatureServerConfig\x12;.tecton_proto.metadataservice.SetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"i\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/set-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#scale_feature_server\x12\xb5\x01\n\x07GetUser\x12,.tecton_proto.metadataservice.GetUserRequest\x1a-.tecton_proto.metadataservice.GetUserResponse\"M\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-user:\x01*\xa2\xbc\xe6\xc0\x05\x1f*\x1dtecton/organization#list_userBg\n\x1a\x63om.tecton.metadataserviceB\x14MetadataServiceProtoP\x01Z1github.com/tecton-ai/tecton_proto/metadataservice')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3tecton_proto/metadataservice/metadata_service.proto\x12\x1ctecton_proto.metadataservice\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a google/protobuf/field_mask.proto\x1a!tecton_proto/auth/principal.proto\x1a\x1etecton_proto/data/entity.proto\x1a tecton_proto/args/fco_args.proto\x1a\x1ftecton_proto/auth/service.proto\x1a\x1btecton_proto/data/fco.proto\x1a$tecton_proto/data/feature_view.proto\x1a\'tecton_proto/data/feature_service.proto\x1a&tecton_proto/data/hive_metastore.proto\x1a$tecton_proto/data/state_update.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a\x30tecton_proto/data/user_deployment_settings.proto\x1a\x1ctecton_proto/data/user.proto\x1a(tecton_proto/spark_common/clusters.proto\x1a&tecton_proto/dataobs/expectation.proto\x1a*tecton_proto/consumption/consumption.proto\x1a!tecton_proto/dataobs/metric.proto\x1a%tecton_proto/dataobs/validation.proto\x1a\x1ctecton_proto/common/id.proto\x1a%tecton_proto/common/fco_locator.proto\x1a&tecton_proto/common/spark_schema.proto\x1a.tecton_proto/data/materialization_status.proto\x1a(tecton_proto/data/freshness_status.proto\x1a&tecton_proto/data/serving_status.proto\x1a\x35tecton_proto/data/internal_spark_cluster_status.proto\x1a\x1ftecton_proto/data/summary.proto\x1a\x30tecton_proto/data/saved_feature_data_frame.proto\x1a\"tecton_proto/data/onboarding.proto\x1a&tecton_proto/data/transformation.proto\x1a+tecton_proto/data/virtual_data_source.proto\x1a!tecton_proto/data/workspace.proto\x1a+tecton_proto/amplitude/client_logging.proto\x1a&tecton_proto/amplitude/amplitude.proto\x1a\'tecton_proto/validation/validator.proto\x1a\x39tecton_proto/materialization/materialization_states.proto\x1a\x30tecton_proto/materialization/spark_cluster.proto\"p\n\nJobsKeySet\x12\x39\n\nupdated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"\xd0\x01\n\x11PaginationRequest\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x19\n\x08sort_key\x18\x03 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x04 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\x12\x1d\n\npage_token\x18\x05 \x01(\tR\tpageToken\"\xf0\x01\n\x12PaginationResponse\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x14\n\x05total\x18\x03 \x01(\rR\x05total\x12&\n\x0fnext_page_token\x18\x04 \x01(\tR\rnextPageToken\x12\x19\n\x08sort_key\x18\x05 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x06 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\"\x9a\x01\n\x18GetFeatureServiceRequest\x12+\n\x11service_reference\x18\x02 \x01(\tR\x10serviceReference\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02idJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"a\n\x19GetFeatureServiceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"<\n\x1cGetAllFeatureServicesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"m\n\x1dGetAllFeatureServicesResponse\x12L\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32!.tecton_proto.data.FeatureServiceR\x0f\x66\x65\x61tureServices\"\xc7\x01\n\x1fGetFeatureServiceSummaryRequest\x12G\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x32\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tH\x00R\x12\x66\x65\x61tureServiceName\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\t\n\x07locator\"\x8c\x01\n GetFeatureServiceSummaryResponse\x12\x43\n\rgeneral_items\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.SummaryItemR\x0cgeneralItems\x12#\n\rvariant_names\x18\x03 \x03(\tR\x0cvariantNames\"f\n\"GetVirtualDataSourceSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"e\n#GetVirtualDataSourceSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"c\n\x1fGetTransformationSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"b\n GetTransformationSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"[\n\x17GetEntitySummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"Z\n\x18GetEntitySummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"\xd9\x01\n\x17GetServingStatusRequest\x12G\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0e\n\x0crequest_type\"\xd6\x01\n\x1eGetFVServingStatusForFSRequest\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x02 \x02(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12O\n\npagination\x18\x04 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xe7\x01\n\x1fGetFVServingStatusForFSResponse\x12r\n\x1b\x66ull_serving_status_summary\x18\x01 \x01(\x0b\x32\x33.tecton_proto.data.FullFeatureServiceServingSummaryR\x18\x66ullServingStatusSummary\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"y\n\x18GetServingStatusResponse\x12]\n\x16serving_status_summary\x18\x05 \x01(\x0b\x32\'.tecton_proto.data.ServingStatusSummaryR\x14servingStatusSummary\"=\n\x1dGetAllFeatureFreshnessRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"s\n\x1eGetAllFeatureFreshnessResponse\x12Q\n\x12\x66reshness_statuses\x18\x01 \x03(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x11\x66reshnessStatuses\"^\n\x1aGetFeatureFreshnessRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"l\n\x1bGetFeatureFreshnessResponse\x12M\n\x10\x66reshness_status\x18\x01 \x01(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x0f\x66reshnessStatus\"`\n\x1cGetFeatureConsumptionRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"u\n\x1dGetFeatureConsumptionResponse\x12T\n\x10\x63onsumption_info\x18\x01 \x03(\x0b\x32).tecton_proto.consumption.ConsumptionInfoR\x0f\x63onsumptionInfo\"h\n\x1fGetMaterializationStatusRequest\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\"\x83\x01\n GetMaterializationStatusResponse\x12_\n\x16materialization_status\x18\x01 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"V\n2GetAllMaterializationStatusInLiveWorkspacesRequest\x12 \n\x0c\x63ut_off_days\x18\x01 \x01(\x05R\ncutOffDays\"4\n\nCountRange\x12\x14\n\x05start\x18\x01 \x01(\rR\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\rR\x03\x65nd\"m\n\rDurationRange\x12/\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05start\x12+\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03\x65nd\"o\n\rDateTimeRange\x12\x30\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05start\x12,\n\x03\x65nd\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03\x65nd\"\x82\x06\n\x0eGetJobsRequest\x12\x1e\n\nworkspaces\x18\x01 \x03(\tR\nworkspaces\x12#\n\rfeature_views\x18\x02 \x03(\tR\x0c\x66\x65\x61tureViews\x12R\n\x08statuses\x18\x03 \x03(\x0e\x32\x36.tecton_proto.materialization.MaterializationTaskStateR\x08statuses\x12J\n\ncreated_at\x18\x06 \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\tcreatedAt\x12\x43\n\ttask_type\x18\x04 \x03(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12K\n\x0cnum_attempts\x18\x05 \x01(\x0b\x32(.tecton_proto.metadataservice.CountRangeR\x0bnumAttempts\x12-\n\x12manually_triggered\x18\x07 \x01(\x08R\x11manuallyTriggered\x12G\n\x08\x64uration\x18\x08 \x01(\x0b\x32+.tecton_proto.metadataservice.DurationRangeR\x08\x64uration\x12Y\n\x12\x66\x65\x61ture_start_time\x18\n \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x10\x66\x65\x61tureStartTime\x12U\n\x10\x66\x65\x61ture_end_time\x18\x0b \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x0e\x66\x65\x61tureEndTime\x12O\n\npagination\x18\t \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xc5\x01\n FeatureViewMaterializationStatus\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"\xbe\x04\n\x10TaskWithAttempts\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12T\n\ttaskState\x18\x02 \x01(\x0e\x32\x36.tecton_proto.materialization.MaterializationTaskStateR\ttaskState\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\x12\x30\n\x07task_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x08 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12*\n\x11\x66\x65\x61ture_view_name\x18\x05 \x01(\tR\x0f\x66\x65\x61tureViewName\x12H\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\"\xc5\x01\n3GetAllMaterializationStatusInLiveWorkspacesResponse\x12\x8d\x01\n#feature_view_materialization_status\x18\x01 \x03(\x0b\x32>.tecton_proto.metadataservice.FeatureViewMaterializationStatusR featureViewMaterializationStatus\"\xc1\x01\n\x0fGetJobsResponse\x12\\\n\x11tasksWithAttempts\x18\x01 \x03(\x0b\x32..tecton_proto.metadataservice.TaskWithAttemptsR\x11tasksWithAttempts\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xa0\x01\n$ForceRetryMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\x12\'\n\x0f\x61llow_overwrite\x18\x02 \x01(\x08R\x0e\x61llowOverwrite\"L\n%ForceRetryMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\".\n\x0eGetFcosRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"W\n\x0fGetFcosResponse\x12\x44\n\rfco_container\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"a\n\x15GetSparkConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xb0\x01\n\x16GetSparkConfigResponse\x12I\n\x0c\x62\x61tch_config\x18\x01 \x01(\x0b\x32&.tecton_proto.spark_common.ClusterInfoR\x0b\x62\x61tchConfig\x12K\n\rstream_config\x18\x02 \x01(\x0b\x32&.tecton_proto.spark_common.ClusterInfoR\x0cstreamConfig\"t\n(GetMetricAndExpectationDefinitionRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xe4\x02\n)GetMetricAndExpectationDefinitionResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x36\n\x07metrics\x18\x03 \x03(\x0b\x32\x1c.tecton_proto.dataobs.MetricR\x07metrics\x12[\n\x14\x66\x65\x61ture_expectations\x18\x04 \x03(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x13\x66\x65\x61tureExpectations\x12X\n\x13metric_expectations\x18\x05 \x03(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x12metricExpectations\"\x91\x01\n\x15GetFeatureViewRequest\x12+\n\x11version_specifier\x18\x01 \x01(\tR\x10versionSpecifier\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02idJ\x04\x08\x05\x10\x06\"^\n\x16GetFeatureViewResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"`\n\x1cGetFeatureViewSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"_\n\x1dGetFeatureViewSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"R\n\x18QueryFeatureViewsRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceJ\x04\x08\x05\x10\x06\"a\n\x19QueryFeatureViewsResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"{\n4GetMaterializingFeatureViewsInLiveWorkspacesResponse\x12\x43\n\rfeature_views\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.FeatureViewR\x0c\x66\x65\x61tureViews\"\xba\x01\n\x1bGetVirtualDataSourceRequest\x12N\n\x16virtual_data_source_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x13virtualDataSourceId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"d\n\x1cGetVirtualDataSourceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"?\n\x1fGetAllVirtualDataSourcesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n GetAllVirtualDataSourcesResponse\x12V\n\x14virtual_data_sources\x18\x01 \x03(\x0b\x32$.tecton_proto.data.VirtualDataSourceR\x12virtualDataSources\"\x97\x01\n\x10GetEntityRequest\x12\x36\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x08\x65ntityId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"Y\n\x11GetEntityResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"5\n\x15GetAllEntitiesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"O\n\x16GetAllEntitiesResponse\x12\x35\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.tecton_proto.data.EntityR\x08\x65ntities\"\xaf\x01\n\x18GetTransformationRequest\x12\x46\n\x11transformation_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10transformationId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x04 \x01(\tR\tworkspaceB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"g\n\x19GetTransformationResponse\x12\x44\n\rfco_container\x18\x03 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainerJ\x04\x08\x01\x10\x02\"<\n\x1cGetAllTransformationsRequest\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"r\n\x1dGetAllTransformationsResponse\x12K\n\x0ftransformations\x18\x02 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformationsJ\x04\x08\x01\x10\x02\"B\n\x17\x46indFcoWorkspaceRequest\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"8\n\x18\x46indFcoWorkspaceResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n\x17IngestClientLogsRequest\x12_\n\x15sdk_method_invocation\x18\x01 \x01(\x0b\x32+.tecton_proto.amplitude.SDKMethodInvocationR\x13sdkMethodInvocation\"v\n\x16IngestAnalyticsRequest\x12>\n\x06\x65vents\x18\x01 \x03(\x0b\x32&.tecton_proto.amplitude.AmplitudeEventR\x06\x65vents\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xbf\x01\n\x15NewStateUpdateRequest\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\"\xfd\x01\n\x17NewStateUpdateRequestV2\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\x12\x19\n\x08no_color\x18\x04 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x05 \x01(\x08R\njsonOutput\"\xe7\x01\n\x16NewStateUpdateResponse\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12]\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x36.tecton_proto.metadataservice.QueryStateUpdateResponseR\reagerResponse\"\xeb\x01\n\x18NewStateUpdateResponseV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12_\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2R\reagerResponse\"k\n\x17QueryStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xa9\x01\n\x19QueryStateUpdateRequestV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x19\n\x08no_color\x18\x03 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x04 \x01(\x08R\njsonOutput\"\xd4\x02\n\x18QueryStateUpdateResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x31\n\x14recreates_suppressed\x18\x07 \x01(\x08R\x13recreatesSuppressed\x12P\n\x11validation_result\x18\x04 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x39\n\ndiff_items\x18\x05 \x03(\x0b\x32\x1a.tecton_proto.data.FcoDiffR\tdiffItems\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\"\xe9\x02\n\x1aQueryStateUpdateResponseV2\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\x12R\n\x11validation_errors\x18\x08 \x01(\x0b\x32#.tecton_proto.data.ValidationResultH\x00R\x10validationErrors\x12_\n\x16successful_plan_output\x18\t \x01(\x0b\x32\'.tecton_proto.data.SuccessfulPlanOutputH\x00R\x14successfulPlanOutputB\n\n\x08responseJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"T\n GetStateUpdatePlanSummaryRequest\x12\x30\n\x07plan_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06planId\"b\n!GetStateUpdatePlanSummaryResponse\x12=\n\x04plan\x18\x01 \x01(\x0b\x32).tecton_proto.data.StateUpdatePlanSummaryR\x04plan\"p\n\x17\x41pplyStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12!\n\napplied_by\x18\x02 \x01(\tB\x02\x18\x01R\tappliedBy\"\x1a\n\x18\x41pplyStateUpdateResponse\"\xb2\x01\n\x12GetConfigsResponse\x12^\n\nkey_values\x18\x01 \x03(\x0b\x32?.tecton_proto.metadataservice.GetConfigsResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc2\x01\n\x1aGetGlobalsForWebUIResponse\x12\x66\n\nkey_values\x18\x01 \x03(\x0b\x32G.tecton_proto.metadataservice.GetGlobalsForWebUIResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"N\n\x18GetStateUpdateLogRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"Z\n\x19GetStateUpdateLogResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32#.tecton_proto.data.StateUpdateEntryR\x07\x65ntries\"R\n\x15GetRestoreInfoRequest\x12\x1b\n\tcommit_id\x18\x01 \x01(\tR\x08\x63ommitId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\x96\x01\n\x16GetRestoreInfoResponse\x12>\n\x1csigned_url_for_repo_download\x18\x01 \x01(\tR\x18signedUrlForRepoDownload\x12\x1b\n\tcommit_id\x18\x02 \x01(\tR\x08\x63ommitId\x12\x1f\n\x0bsdk_version\x18\x03 \x01(\tR\nsdkVersion\"\x93\x01\n\x16\x43reateWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x02 \x01(\tR\rworkspaceName\x12L\n\x0c\x63\x61pabilities\x18\x03 \x01(\x0b\x32(.tecton_proto.data.WorkspaceCapabilitiesR\x0c\x63\x61pabilitiesJ\x04\x08\x01\x10\x02\"6\n\x16\x44\x65leteWorkspaceRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"2\n\x17IntrospectApiKeyRequest\x12\x17\n\x07\x61pi_key\x18\x01 \x01(\tR\x06\x61piKey\"\xcb\x01\n\x18IntrospectApiKeyResponse\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x03 \x01(\tR\tcreatedBy\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\"R\n\x13\x43reateApiKeyRequest\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x19\n\x08is_admin\x18\x02 \x01(\x08R\x07isAdmin\"Q\n\x14\x43reateApiKeyResponse\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\">\n\x13\x44\x65leteApiKeyRequest\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"?\n\x12ListApiKeysRequest\x12)\n\x10include_archived\x18\x01 \x01(\x08R\x0fincludeArchived\"Q\n\x13ListApiKeysResponse\x12:\n\x08\x61pi_keys\x18\x01 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x07\x61piKeys\"\xe4\x01\n\x0eServiceAccount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12\x36\n\x07\x63reator\x18\x05 \x01(\x0b\x32\x1c.tecton_proto.auth.PrincipalR\x07\x63reator\x12\x37\n\x05owner\x18\x06 \x01(\x0b\x32!.tecton_proto.auth.PrincipalBasicR\x05owner\"S\n\x1b\x43reateServiceAccountRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"\x9a\x01\n\x1c\x43reateServiceAccountResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12\x17\n\x07\x61pi_key\x18\x05 \x01(\tR\x06\x61piKey\"E\n\x19GetServiceAccountsRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\"u\n\x1aGetServiceAccountsResponse\x12W\n\x10service_accounts\x18\x01 \x03(\x0b\x32,.tecton_proto.metadataservice.ServiceAccountR\x0fserviceAccounts\"\x80\x01\n\x1bUpdateServiceAccountRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\"\x81\x01\n\x1cUpdateServiceAccountResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\"-\n\x1b\x44\x65leteServiceAccountRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x1e\n\x1c\x44\x65leteServiceAccountResponse\"\x17\n\x15ListWorkspacesRequest\"V\n\x16ListWorkspacesResponse\x12<\n\nworkspaces\x18\x01 \x03(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\nworkspaces\"<\n\x13GetWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\"R\n\x14GetWorkspaceResponse\x12:\n\tworkspace\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\tworkspace\"\x93\x03\n\"CreateSavedFeatureDataFrameRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x07 \x01(\tR\tworkspace\x12G\n\x12\x66\x65\x61ture_package_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x31\n\x15join_key_column_names\x18\x04 \x03(\tR\x12joinKeyColumnNames\x12\x32\n\x15timestamp_column_name\x18\x05 \x01(\tR\x13timestampColumnName\x12\x38\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x06schemaB\x08\n\x06source\"\x87\x01\n#CreateSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"{\n#ArchiveSavedFeatureDataFrameRequest\x12T\n\x1asaved_feature_dataframe_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x17savedFeatureDataframeId\"&\n$ArchiveSavedFeatureDataFrameResponse\"\xe7\x01\n\x1fGetSavedFeatureDataFrameRequest\x12\x41\n\x1csaved_feature_dataframe_name\x18\x01 \x01(\tH\x00R\x19savedFeatureDataframeName\x12V\n\x1asaved_feature_dataframe_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x17savedFeatureDataframeId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0b\n\treference\"\xa5\x01\n\x1bGetClusterAdminInfoResponse\x12&\n\x0f\x63\x61ller_is_admin\x18\x01 \x01(\x08R\rcallerIsAdmin\x12-\n\x05users\x18\x02 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x05users\x12/\n\x06\x61\x64mins\x18\x03 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x06\x61\x64mins\";\n\x18\x43reateClusterUserRequest\x12\x1f\n\x0blogin_email\x18\x01 \x01(\tR\nloginEmail\"@\n\x19\x43reateClusterUserResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"3\n\x18\x44\x65leteClusterUserRequest\x12\x17\n\x07okta_id\x18\x01 \x01(\tR\x06oktaId\"@\n\x19\x44\x65leteClusterUserResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"\xe2\x01\n\x18\x43lusterUserActionRequest\x12\x17\n\x07okta_id\x18\x01 \x01(\tR\x06oktaId\x12\x38\n\x17resend_activation_email\x18\x02 \x01(\x08H\x00R\x15resendActivationEmail\x12!\n\x0bunlock_user\x18\x03 \x01(\x08H\x00R\nunlockUser\x12!\n\x0bgrant_admin\x18\x04 \x01(\x08H\x00R\ngrantAdmin\x12#\n\x0crevoke_admin\x18\x05 \x01(\x08H\x00R\x0brevokeAdminB\x08\n\x06\x61\x63tion\"@\n\x19\x43lusterUserActionResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"\x84\x01\n GetSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"C\n#GetAllSavedFeatureDataFramesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x8a\x01\n$GetAllSavedFeatureDataFramesResponse\x12\x62\n\x18saved_feature_dataframes\x18\x01 \x03(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x16savedFeatureDataframes\"\x9c\x01\n\x16IngestDataframeRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\x12\x17\n\x07\x64\x66_path\x18\x02 \x01(\tR\x06\x64\x66Path\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\"\x19\n\x17IngestDataframeResponse\"o\n GetNewIngestDataframeInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"t\n!GetNewIngestDataframeInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x36\n\x18signed_url_for_df_upload\x18\x02 \x01(\tR\x14signedUrlForDfUpload\"\x88\x01\n!GetUserDeploymentSettingsResponse\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\"\xc5\x01\n#UpdateUserDeploymentSettingsRequest\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\x12\x39\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\tfieldMask\"e\n$UpdateUserDeploymentSettingsResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\"n\n%GetInternalSparkClusterStatusResponse\x12\x45\n\x06status\x18\x01 \x01(\x0b\x32-.tecton_proto.data.InternalSparkClusterStatusR\x06status\"k\n\x1cGetDeleteEntitiesInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"\xca\x01\n\x1dGetDeleteEntitiesInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x43\n\x1fsigned_url_for_df_upload_online\x18\x03 \x01(\tR\x1asignedUrlForDfUploadOnline\x12\x45\n signed_url_for_df_upload_offline\x18\x04 \x01(\tR\x1bsignedUrlForDfUploadOfflineJ\x04\x08\x02\x10\x03\"\xf3\x01\n\x15\x44\x65leteEntitiesRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12\x31\n\x15online_join_keys_path\x18\x02 \x01(\tR\x12onlineJoinKeysPath\x12\x33\n\x16offline_join_keys_path\x18\x03 \x01(\tR\x13offlineJoinKeysPath\x12\x16\n\x06online\x18\x04 \x01(\x08R\x06online\x12\x18\n\x07offline\x18\x05 \x01(\x08R\x07offline\"\x18\n\x16\x44\x65leteEntitiesResponse\"\xf9\x01\n\x16GetHiveMetadataRequest\x12S\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32;.tecton_proto.metadataservice.GetHiveMetadataRequest.ActionR\x06\x61\x63tion\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x14\n\x05table\x18\x03 \x01(\tR\x05table\"X\n\x06\x41\x63tion\x12\x19\n\x15\x41\x43TION_LIST_DATABASES\x10\x00\x12\x16\n\x12\x41\x43TION_LIST_TABLES\x10\x01\x12\x1b\n\x17\x41\x43TION_GET_TABLE_SCHEMA\x10\x02\"\xd1\x02\n\x17GetHiveMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12\x41\n\tdatabases\x18\x03 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\tdatabases\x12;\n\x06tables\x18\x04 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\x06tables\x12=\n\x07\x63olumns\x18\x05 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\x07\x63olumns\x12.\n\x13\x64\x65\x62ug_error_message\x18\x06 \x01(\tR\x11\x64\x65\x62ugErrorMessageB\x08\n\x06result\"K\n\x16GetFileMetadataRequest\x12\x10\n\x03uri\x18\x01 \x01(\tR\x03uri\x12\x1f\n\x0b\x66ile_format\x18\x02 \x01(\tR\nfileFormat\"\xab\x01\n\x17GetFileMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12!\n\x0c\x63olumn_names\x18\x03 \x03(\tR\x0b\x63olumnNames\x12.\n\x13\x64\x65\x62ug_error_message\x18\x04 \x01(\tR\x11\x64\x65\x62ugErrorMessage\"R\n\x13ValidateFcosRequest\x12\x35\n\x08\x66\x63o_args\x18\x02 \x03(\x0b\x32\x1a.tecton_proto.args.FcoArgsR\x07\x66\x63oArgsJ\x04\x08\x01\x10\x02\"\xe6\x01\n\x14ValidateFcosResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x32\n\x15\x64isplay_error_message\x18\x04 \x01(\tR\x13\x64isplayErrorMessage\x12.\n\x13\x64\x65\x62ug_error_message\x18\x03 \x01(\tR\x11\x64\x65\x62ugErrorMessage\"\x95\x01\n\x17ValidateLocalFcoRequest\x12Y\n\x12validation_request\x18\x01 \x01(\x0b\x32*.tecton_proto.validation.ValidationRequestR\x11validationRequest\x12\x1f\n\x0bsdk_version\x18\x02 \x01(\tR\nsdkVersion\"\x9c\x01\n\x18ValidateLocalFcoResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\":\n\x1aGetOnboardingStatusRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x9c\x02\n\x1bGetOnboardingStatusResponse\x12N\n\x0esetup_platform\x18\x03 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\rsetupPlatform\x12W\n\x13\x63reate_feature_view\x18\x01 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x11\x63reateFeatureView\x12T\n\x11\x66inish_onboarding\x18\x02 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x10\x66inishOnboarding\"]\n\x1aSetOnboardingStatusRequest\x12?\n\x06status\x18\x01 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x06status\"\x92\x01\n\"GetDataPlatformSetupStatusResponse\x12&\n\x0esetupCompleted\x18\x01 \x01(\x08R\x0esetupCompleted\x12\x44\n\x05tasks\x18\x02 \x03(\x0b\x32..tecton_proto.data.DataPlatformSetupTaskStatusR\x05tasks\"7\n#GetRetrieveFeaturesNotebookResponse\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\"i\n\x1dGetObservabilityConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xa5\x01\n\x1eGetObservabilityConfigResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x39\n\x19is_dataobs_metric_enabled\x18\x03 \x01(\x08R\x16isDataobsMetricEnabled\"\x93\x02\n\x12QueryMetricRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12\x39\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x35\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndTime\"\xf5\x03\n\x13QueryMetricResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12V\n\x1ametric_data_point_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17metricDataPointInterval\x12H\n\x12\x61ligned_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x61lignedStartTime\x12\x44\n\x10\x61ligned_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x61lignedEndTime\x12\x46\n\x0bmetric_data\x18\x04 \x03(\x0b\x32%.tecton_proto.dataobs.MetricDataPointR\nmetricData\x12!\n\x0c\x63olumn_names\x18\x06 \x03(\tR\x0b\x63olumnNames\"\x89\x01\n\"GetFeatureValidationHistoryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x19\n\x05limit\x18\x03 \x01(\x05:\x03\x31\x30\x30R\x05limit\"\xb2\x01\n#GetFeatureValidationHistoryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x07results\x18\x03 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\"\x80\x04\n!GetFeatureValidationResultRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12\x39\n\x19\x66ilter_feature_view_names\x18\x04 \x03(\tR\x16\x66ilterFeatureViewNames\x12\x38\n\x18\x66ilter_expectation_names\x18\x05 \x03(\tR\x16\x66ilterExpectationNames\x12[\n\x13\x66ilter_result_types\x18\x06 \x03(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x11\x66ilterResultTypes\x12O\n\npagination\x18\x07 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\x8c\x01\n\"GetFeatureValidationResultResponse\x12#\n\rtotal_results\x18\x01 \x01(\x05R\x0ctotalResults\x12\x41\n\x07results\x18\x02 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\"\xde\x01\n\"GetFeatureValidationSummaryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\"\xba\x02\n#GetFeatureValidationSummaryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12Y\n\x11workspace_summary\x18\x04 \x01(\x0b\x32,.tecton_proto.dataobs.WorkspaceResultSummaryR\x10workspaceSummary\"6\n\x0eGetUserRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\"C\n\x0fGetUserResponse\x12\x30\n\x04user\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.auth.UserBasicR\x04user\"\x1f\n\x1dGetFeatureServerConfigRequest\"\x90\x01\n\x1eGetFeatureServerConfigResponse\x12\"\n\x0c\x63urrentCount\x18\x01 \x01(\rR\x0c\x63urrentCount\x12&\n\x0e\x61vailableCount\x18\x02 \x01(\rR\x0e\x61vailableCount\x12\"\n\x0c\x64\x65siredCount\x18\x03 \x01(\rR\x0c\x64\x65siredCount\"5\n\x1dSetFeatureServerConfigRequest\x12\x14\n\x05\x63ount\x18\x01 \x01(\rR\x05\x63ount*>\n\rSortDirection\x12\x10\n\x0cSORT_UNKNOWN\x10\x00\x12\x0c\n\x08SORT_ASC\x10\x01\x12\r\n\tSORT_DESC\x10\x02\x32\xac\x97\x01\n\x0fMetadataService\x12\xec\x01\n\x11GetFeatureService\x12\x36.tecton_proto.metadataservice.GetFeatureServiceRequest\x1a\x37.tecton_proto.metadataservice.GetFeatureServiceResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-feature-service:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfd\x01\n\x15GetAllFeatureServices\x12:.tecton_proto.metadataservice.GetAllFeatureServicesRequest\x1a;.tecton_proto.metadataservice.GetAllFeatureServicesResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-all-feature-services:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x98\x02\n\x18GetFeatureServiceSummary\x12=.tecton_proto.metadataservice.GetFeatureServiceSummaryRequest\x1a>.tecton_proto.metadataservice.GetFeatureServiceSummaryResponse\"}\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/get-feature-service-summary:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\xf7\x01\n\x10GetServingStatus\x12\x35.tecton_proto.metadataservice.GetServingStatusRequest\x1a\x36.tecton_proto.metadataservice.GetServingStatusResponse\"t\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-serving-status:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x96\x02\n\x17GetFVServingStatusForFS\x12<.tecton_proto.metadataservice.GetFVServingStatusForFSRequest\x1a=.tecton_proto.metadataservice.GetFVServingStatusForFSResponse\"~\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-fv-serving-status-for-fs:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x16GetAllFeatureFreshness\x12;.tecton_proto.metadataservice.GetAllFeatureFreshnessRequest\x1a<.tecton_proto.metadataservice.GetAllFeatureFreshnessResponse\"{\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-all-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x13GetFeatureFreshness\x12\x38.tecton_proto.metadataservice.GetFeatureFreshnessRequest\x1a\x39.tecton_proto.metadataservice.GetFeatureFreshnessResponse\"\x83\x01\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xdd\x01\n\x18GetMaterializationStatus\x12=.tecton_proto.metadataservice.GetMaterializationStatusRequest\x1a>.tecton_proto.metadataservice.GetMaterializationStatusResponse\"B\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-service/get-materialization-status:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xac\x02\n+GetAllMaterializationStatusInLiveWorkspaces\x12P.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesRequest\x1aQ.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesResponse\"X\x82\xd3\xe4\x93\x02J\"E/v1/metadata-service/get-all-materialization-status-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x94\x01\n\x07GetJobs\x12,.tecton_proto.metadataservice.GetJobsRequest\x1a-.tecton_proto.metadataservice.GetJobsResponse\",\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/metadata-service/jobs:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xf2\x01\n\x1d\x46orceRetryMaterializationTask\x12\x42.tecton_proto.metadataservice.ForceRetryMaterializationTaskRequest\x1a\x43.tecton_proto.metadataservice.ForceRetryMaterializationTaskResponse\"H\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/force-retry-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe0\x01\n\x0eGetSparkConfig\x12\x33.tecton_proto.metadataservice.GetSparkConfigRequest\x1a\x34.tecton_proto.metadataservice.GetSparkConfigResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-spark-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xae\x02\n!GetMetricAndExpectationDefinition\x12\x46.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionRequest\x1aG.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionResponse\"x\x82\xd3\xe4\x93\x02?\":/v1/metadata-service/get-metric-and-expectation-definition:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetFeatureView\x12\x33.tecton_proto.metadataservice.GetFeatureViewRequest\x1a\x34.tecton_proto.metadataservice.GetFeatureViewResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-feature-view:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf0\x01\n,GetMaterializingFeatureViewsInLiveWorkspaces\x12\x16.google.protobuf.Empty\x1aR.tecton_proto.metadataservice.GetMaterializingFeatureViewsInLiveWorkspacesResponse\"T\x82\xd3\xe4\x93\x02\x46\"A/v1/metadata-service/get-materializing-features-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xec\x01\n\x11QueryFeatureViews\x12\x36.tecton_proto.metadataservice.QueryFeatureViewsRequest\x1a\x37.tecton_proto.metadataservice.QueryFeatureViewsResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/query-feature-views:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x99\x02\n\x15GetFeatureViewSummary\x12:.tecton_proto.metadataservice.GetFeatureViewSummaryRequest\x1a;.tecton_proto.metadataservice.GetFeatureViewSummaryResponse\"\x86\x01\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-package/get-feature-view-summary:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\x8d\x02\n\x15GetFeatureConsumption\x12:.tecton_proto.metadataservice.GetFeatureConsumptionRequest\x1a;.tecton_proto.metadataservice.GetFeatureConsumptionResponse\"{\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-feature-view-consumption:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xf9\x01\n\x14GetVirtualDataSource\x12\x39.tecton_proto.metadataservice.GetVirtualDataSourceRequest\x1a:.tecton_proto.metadataservice.GetVirtualDataSourceResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-virtual-data-source:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8a\x02\n\x18GetAllVirtualDataSources\x12=.tecton_proto.metadataservice.GetAllVirtualDataSourcesRequest\x1a>.tecton_proto.metadataservice.GetAllVirtualDataSourcesResponse\"o\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-all-virtual-data-sources:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x90\x01\n\x10IngestClientLogs\x12\x35.tecton_proto.metadataservice.IngestClientLogsRequest\x1a\x16.google.protobuf.Empty\"-\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xbe\x01\n\x0fIngestAnalytics\x12\x34.tecton_proto.metadataservice.IngestAnalyticsRequest\x1a\x16.google.protobuf.Empty\"]\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/ingest-analytics:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa2\x02\n\x1bGetVirtualDataSourceSummary\x12@.tecton_proto.metadataservice.GetVirtualDataSourceSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetVirtualDataSourceSummaryResponse\"~\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/get-virtual-data-source-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xc3\x01\n\x07GetFcos\x12,.tecton_proto.metadataservice.GetFcosRequest\x1a-.tecton_proto.metadataservice.GetFcosResponse\"[\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-fcos:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xa1\x01\n\tGetEntity\x12..tecton_proto.metadataservice.GetEntityRequest\x1a/.tecton_proto.metadataservice.GetEntityResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetAllEntities\x12\x33.tecton_proto.metadataservice.GetAllEntitiesRequest\x1a\x34.tecton_proto.metadataservice.GetAllEntitiesResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-all-entities:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf4\x01\n\x10GetEntitySummary\x12\x35.tecton_proto.metadataservice.GetEntitySummaryRequest\x1a\x36.tecton_proto.metadataservice.GetEntitySummaryResponse\"q\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-package/get-entity-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xeb\x01\n\x11GetTransformation\x12\x36.tecton_proto.metadataservice.GetTransformationRequest\x1a\x37.tecton_proto.metadataservice.GetTransformationResponse\"e\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-transformation:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfc\x01\n\x15GetAllTransformations\x12:.tecton_proto.metadataservice.GetAllTransformationsRequest\x1a;.tecton_proto.metadataservice.GetAllTransformationsResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-all-transformations:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x94\x02\n\x18GetTransformationSummary\x12=.tecton_proto.metadataservice.GetTransformationSummaryRequest\x1a>.tecton_proto.metadataservice.GetTransformationSummaryResponse\"y\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-package/get-transformation-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xbd\x01\n\x10\x46indFcoWorkspace\x12\x35.tecton_proto.metadataservice.FindFcoWorkspaceRequest\x1a\x36.tecton_proto.metadataservice.FindFcoWorkspaceResponse\":\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/find-fco-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb8\x01\n\x0eNewStateUpdate\x12\x33.tecton_proto.metadataservice.NewStateUpdateRequest\x1a\x34.tecton_proto.metadataservice.NewStateUpdateResponse\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#read_config\x12\xbe\x01\n\x10NewStateUpdateV2\x12\x35.tecton_proto.metadataservice.NewStateUpdateRequestV2\x1a\x36.tecton_proto.metadataservice.NewStateUpdateResponseV2\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#read_config\x12\xb8\x01\n\x10ValidateLocalFco\x12\x35.tecton_proto.metadataservice.ValidateLocalFcoRequest\x1a\x36.tecton_proto.metadataservice.ValidateLocalFcoResponse\"5\xa2\xbc\xe6\xc0\x05/*-tecton/organization#validate_notebook_objects\x12\xb6\x01\n\x10QueryStateUpdate\x12\x35.tecton_proto.metadataservice.QueryStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.QueryStateUpdateResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xbc\x01\n\x12QueryStateUpdateV2\x12\x37.tecton_proto.metadataservice.QueryStateUpdateRequestV2\x1a\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8b\x01\n\x10\x41pplyStateUpdate\x12\x35.tecton_proto.metadataservice.ApplyStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.ApplyStateUpdateResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb0\x01\n\nGetConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/get-configs:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xcb\x01\n\x12GetGlobalsForWebUI\x12\x16.google.protobuf.Empty\x1a\x38.tecton_proto.metadataservice.GetGlobalsForWebUIResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-globals-for-web-ui:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x98\x01\n\x0fGetLoginConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\";\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-login-configs:\x01*\xa2\xbc\xe6\xc0\x05\x04\x08\x01\x10\x01\x12?\n\x03Nop\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x08\xa2\xbc\xe6\xc0\x05\x02\x10\x01\x12\xe3\x01\n\x19GetStateUpdatePlanSummary\x12>.tecton_proto.metadataservice.GetStateUpdatePlanSummaryRequest\x1a?.tecton_proto.metadataservice.GetStateUpdatePlanSummaryResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-state-update-plan-summary:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xed\x01\n\x11GetStateUpdateLog\x12\x36.tecton_proto.metadataservice.GetStateUpdateLogRequest\x1a\x37.tecton_proto.metadataservice.GetStateUpdateLogResponse\"g\x82\xd3\xe4\x93\x02.\")/v1/metadata-service/get-state-update-log:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x01\n\x0eGetRestoreInfo\x12\x33.tecton_proto.metadataservice.GetRestoreInfoRequest\x1a\x34.tecton_proto.metadataservice.GetRestoreInfoResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8e\x02\n\x0f\x43reateWorkspace\x12\x34.tecton_proto.metadataservice.CreateWorkspaceRequest\x1a\x16.google.protobuf.Empty\"\xac\x01\xa2\xbc\xe6\xc0\x05v*$tecton/organization#create_workspace2N\n\x1b\x63\x61pabilities.materializable\x12\x04true\x1a)tecton/organization#create_workspace_live\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/create-workspace:\x01*\x12\x99\x01\n\x0f\x44\x65leteWorkspace\x12\x34.tecton_proto.metadataservice.DeleteWorkspaceRequest\x1a\x16.google.protobuf.Empty\"8\xa2\xbc\xe6\xc0\x05\x32\x1a\r\x08\x01\x12\tworkspace*!tecton/workspace#delete_workspace\x12\xb4\x01\n\x0eListWorkspaces\x12\x33.tecton_proto.metadataservice.ListWorkspacesRequest\x1a\x34.tecton_proto.metadataservice.ListWorkspacesResponse\"7\x82\xd3\xe4\x93\x02)\"$/v1/metadata-service/list-workspaces:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xdf\x01\n\x0cGetWorkspace\x12\x31.tecton_proto.metadataservice.GetWorkspaceRequest\x1a\x32.tecton_proto.metadataservice.GetWorkspaceResponse\"h\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/get-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x35\x1a\x12\x08\x01\x12\x0eworkspace_name*\x1ftecton/workspace#read_workspace\x12\xe5\x01\n\x10IntrospectApiKey\x12\x35.tecton_proto.metadataservice.IntrospectApiKeyRequest\x1a\x36.tecton_proto.metadataservice.IntrospectApiKeyResponse\"b\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/introspect-api-key:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xf7\x01\n\x14\x43reateServiceAccount\x12\x39.tecton_proto.metadataservice.CreateServiceAccountRequest\x1a:.tecton_proto.metadataservice.CreateServiceAccountResponse\"h\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/create-service-account:\x01*\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\x12\xec\x01\n\x12GetServiceAccounts\x12\x37.tecton_proto.metadataservice.GetServiceAccountsRequest\x1a\x38.tecton_proto.metadataservice.GetServiceAccountsResponse\"c\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-service-account:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\x82\x02\n\x14UpdateServiceAccount\x12\x39.tecton_proto.metadataservice.UpdateServiceAccountRequest\x1a:.tecton_proto.metadataservice.UpdateServiceAccountResponse\"s\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/update-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\x12\x82\x02\n\x14\x44\x65leteServiceAccount\x12\x39.tecton_proto.metadataservice.DeleteServiceAccountRequest\x1a:.tecton_proto.metadataservice.DeleteServiceAccountResponse\"s\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/delete-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\x12\xef\x01\n\x0c\x43reateApiKey\x12\x31.tecton_proto.metadataservice.CreateApiKeyRequest\x1a\x32.tecton_proto.metadataservice.CreateApiKeyResponse\"x\xa2\xbc\xe6\xc0\x05r**tecton/organization#create_service_account2B\n\x08is_admin\x12\x04true\x1a\x30tecton/organization#create_service_account_admin8\x01\x12\x9a\x01\n\x0c\x44\x65leteApiKey\x12\x31.tecton_proto.metadataservice.DeleteApiKeyRequest\x1a\x16.google.protobuf.Empty\"?\xa2\xbc\xe6\xc0\x05\x39\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account8\x01\x12\xa4\x01\n\x0bListApiKeys\x12\x30.tecton_proto.metadataservice.ListApiKeysRequest\x1a\x31.tecton_proto.metadataservice.ListApiKeysResponse\"0\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xda\x01\n\x1b\x43reateSavedFeatureDataFrame\x12@.tecton_proto.metadataservice.CreateSavedFeatureDataFrameRequest\x1a\x41.tecton_proto.metadataservice.CreateSavedFeatureDataFrameResponse\"6\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#update_dataset\x12\xaf\x01\n\x1c\x41rchiveSavedFeatureDataFrame\x12\x41.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameRequest\x1a\x42.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xcf\x01\n\x18GetSavedFeatureDataFrame\x12=.tecton_proto.metadataservice.GetSavedFeatureDataFrameRequest\x1a>.tecton_proto.metadataservice.GetSavedFeatureDataFrameResponse\"4\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\x9b\x02\n\x1cGetAllSavedFeatureDataFrames\x12\x41.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesRequest\x1a\x42.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesResponse\"t\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/get-all-saved-feature-dataframes:\x01*\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\xa6\x01\n\x19GetNewIngestDataframeInfo\x12>.tecton_proto.metadataservice.GetNewIngestDataframeInfoRequest\x1a?.tecton_proto.metadataservice.GetNewIngestDataframeInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb7\x01\n\x0fIngestDataframe\x12\x34.tecton_proto.metadataservice.IngestDataframeRequest\x1a\x35.tecton_proto.metadataservice.IngestDataframeResponse\"7\xa2\xbc\xe6\xc0\x05\x31\x1a\r\x08\x01\x12\tworkspace* tecton/workspace#ingest_features\x12\xcd\x01\n\x13GetClusterAdminInfo\x12\x16.google.protobuf.Empty\x1a\x39.tecton_proto.metadataservice.GetClusterAdminInfoResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-cluster-admin-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xe0\x01\n\x11\x43reateClusterUser\x12\x36.tecton_proto.metadataservice.CreateClusterUserRequest\x1a\x37.tecton_proto.metadataservice.CreateClusterUserResponse\"Z\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/create-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#create_user\x12\xe0\x01\n\x11\x44\x65leteClusterUser\x12\x36.tecton_proto.metadataservice.DeleteClusterUserRequest\x1a\x37.tecton_proto.metadataservice.DeleteClusterUserResponse\"Z\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/delete-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\x12\xe0\x01\n\x11\x43lusterUserAction\x12\x36.tecton_proto.metadataservice.ClusterUserActionRequest\x1a\x37.tecton_proto.metadataservice.ClusterUserActionResponse\"Z\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/cluster-user-action:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\x12\xdf\x01\n\x19GetUserDeploymentSettings\x12\x16.google.protobuf.Empty\x1a?.tecton_proto.metadataservice.GetUserDeploymentSettingsResponse\"i\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9c\x02\n\x1cUpdateUserDeploymentSettings\x12\x41.tecton_proto.metadataservice.UpdateUserDeploymentSettingsRequest\x1a\x42.tecton_proto.metadataservice.UpdateUserDeploymentSettingsResponse\"u\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/update-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xec\x01\n\x1dGetInternalSparkClusterStatus\x12\x16.google.protobuf.Empty\x1a\x43.tecton_proto.metadataservice.GetInternalSparkClusterStatusResponse\"n\x82\xd3\xe4\x93\x02;\"6/v1/metadata-service/get-internal-spark-cluster-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9a\x01\n\x15GetDeleteEntitiesInfo\x12:.tecton_proto.metadataservice.GetDeleteEntitiesInfoRequest\x1a;.tecton_proto.metadataservice.GetDeleteEntitiesInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc0\x01\n\x0e\x44\x65leteEntities\x12\x33.tecton_proto.metadataservice.DeleteEntitiesRequest\x1a\x34.tecton_proto.metadataservice.DeleteEntitiesResponse\"C\xa2\xbc\xe6\xc0\x05=\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace* tecton/workspace#delete_features\x12\xde\x01\n\x0fGetHiveMetadata\x12\x34.tecton_proto.metadataservice.GetHiveMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetHiveMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-hive-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xde\x01\n\x0fGetFileMetadata\x12\x34.tecton_proto.metadataservice.GetFileMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetFileMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-file-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xda\x01\n\x0cValidateFcos\x12\x31.tecton_proto.metadataservice.ValidateFcosRequest\x1a\x32.tecton_proto.metadataservice.ValidateFcosResponse\"c\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/validate-fcos:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xf7\x01\n\x13GetOnboardingStatus\x12\x38.tecton_proto.metadataservice.GetOnboardingStatusRequest\x1a\x39.tecton_proto.metadataservice.GetOnboardingStatusResponse\"k\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#read_workspace\x12\xcb\x01\n\x13SetOnboardingStatus\x12\x38.tecton_proto.metadataservice.SetOnboardingStatusRequest\x1a\x16.google.protobuf.Empty\"b\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/set-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xe3\x01\n\x1aGetDataPlatformSetupStatus\x12\x16.google.protobuf.Empty\x1a@.tecton_proto.metadataservice.GetDataPlatformSetupStatusResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-data-platform-setup-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xe5\x01\n\x1bGetRetrieveFeaturesNotebook\x12\x16.google.protobuf.Empty\x1a\x41.tecton_proto.metadataservice.GetRetrieveFeaturesNotebookResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-retrieve-features-notebook:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x80\x02\n\x16GetObservabilityConfig\x12;.tecton_proto.metadataservice.GetObservabilityConfigRequest\x1a<.tecton_proto.metadataservice.GetObservabilityConfigResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-observability-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xd3\x01\n\x0bQueryMetric\x12\x30.tecton_proto.metadataservice.QueryMetricRequest\x1a\x31.tecton_proto.metadataservice.QueryMetricResponse\"_\x82\xd3\xe4\x93\x02&\"!/v1/metadata-service/query-metric:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationHistory\x12@.tecton_proto.metadataservice.GetFeatureValidationHistoryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationHistoryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-history:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationSummary\x12@.tecton_proto.metadataservice.GetFeatureValidationSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationSummaryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-summary:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\x91\x02\n\x1aGetFeatureValidationResult\x12?.tecton_proto.metadataservice.GetFeatureValidationResultRequest\x1a@.tecton_proto.metadataservice.GetFeatureValidationResultResponse\"p\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-feature-validation-result:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\xfb\x01\n\x16GetFeatureServerConfig\x12;.tecton_proto.metadataservice.GetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"f\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xfe\x01\n\x16SetFeatureServerConfig\x12;.tecton_proto.metadataservice.SetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"i\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/set-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#scale_feature_server\x12\xb5\x01\n\x07GetUser\x12,.tecton_proto.metadataservice.GetUserRequest\x1a-.tecton_proto.metadataservice.GetUserResponse\"M\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-user:\x01*\xa2\xbc\xe6\xc0\x05\x1f*\x1dtecton/organization#list_userBg\n\x1a\x63om.tecton.metadataserviceB\x14MetadataServiceProtoP\x01Z1github.com/tecton-ai/tecton_proto/metadataservice')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.metadataservice.metadata_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032com.tecton.metadataserviceB\024MetadataServiceProtoP\001Z1github.com/tecton-ai/tecton_proto/metadataservice'
@@ -228,22 +228,24 @@
   _METADATASERVICE.methods_by_name['GetObservabilityConfig']._serialized_options = b'\202\323\344\223\0022\"-/v1/metadata-service/get-observability-config:\001*\242\274\346\300\005-\032\r\010\001\022\tworkspace*\034tecton/workspace#read_config'
   _METADATASERVICE.methods_by_name['QueryMetric']._options = None
   _METADATASERVICE.methods_by_name['QueryMetric']._serialized_options = b'\202\323\344\223\002&\"!/v1/metadata-service/query-metric:\001*\242\274\346\300\005-\032\r\010\001\022\tworkspace*\034tecton/workspace#read_config'
   _METADATASERVICE.methods_by_name['GetFeatureValidationHistory']._options = None
   _METADATASERVICE.methods_by_name['GetFeatureValidationHistory']._serialized_options = b'\202\323\344\223\0028\"3/v1/metadata-service/get-feature-validation-history:\001*\242\274\346\300\005-\032\r\010\001\022\tworkspace*\034tecton/workspace#read_config'
   _METADATASERVICE.methods_by_name['GetFeatureValidationSummary']._options = None
   _METADATASERVICE.methods_by_name['GetFeatureValidationSummary']._serialized_options = b'\202\323\344\223\0028\"3/v1/metadata-service/get-feature-validation-summary:\001*\242\274\346\300\005-\032\r\010\001\022\tworkspace*\034tecton/workspace#read_metric'
+  _METADATASERVICE.methods_by_name['GetFeatureValidationResult']._options = None
+  _METADATASERVICE.methods_by_name['GetFeatureValidationResult']._serialized_options = b'\202\323\344\223\0027\"2/v1/metadata-service/get-feature-validation-result:\001*\242\274\346\300\005-\032\r\010\001\022\tworkspace*\034tecton/workspace#read_metric'
   _METADATASERVICE.methods_by_name['GetFeatureServerConfig']._options = None
   _METADATASERVICE.methods_by_name['GetFeatureServerConfig']._serialized_options = b'\202\323\344\223\0023\"./v1/metadata-service/get-feature-server-config:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
   _METADATASERVICE.methods_by_name['SetFeatureServerConfig']._options = None
   _METADATASERVICE.methods_by_name['SetFeatureServerConfig']._serialized_options = b'\202\323\344\223\0023\"./v1/metadata-service/set-feature-server-config:\001*\242\274\346\300\005**(tecton/organization#scale_feature_server'
   _METADATASERVICE.methods_by_name['GetUser']._options = None
   _METADATASERVICE.methods_by_name['GetUser']._serialized_options = b'\202\323\344\223\002\"\"\035/v1/metadata-service/get-user:\001*\242\274\346\300\005\037*\035tecton/organization#list_user'
-  _SORTDIRECTION._serialized_start=24226
-  _SORTDIRECTION._serialized_end=24288
+  _SORTDIRECTION._serialized_start=24884
+  _SORTDIRECTION._serialized_end=24946
   _JOBSKEYSET._serialized_start=1685
   _JOBSKEYSET._serialized_end=1797
   _PAGINATIONREQUEST._serialized_start=1800
   _PAGINATIONREQUEST._serialized_end=2008
   _PAGINATIONRESPONSE._serialized_start=2011
   _PAGINATIONRESPONSE._serialized_end=2251
   _GETFEATURESERVICEREQUEST._serialized_start=2254
@@ -548,24 +550,28 @@
   _QUERYMETRICREQUEST._serialized_end=22497
   _QUERYMETRICRESPONSE._serialized_start=22500
   _QUERYMETRICRESPONSE._serialized_end=23001
   _GETFEATUREVALIDATIONHISTORYREQUEST._serialized_start=23004
   _GETFEATUREVALIDATIONHISTORYREQUEST._serialized_end=23141
   _GETFEATUREVALIDATIONHISTORYRESPONSE._serialized_start=23144
   _GETFEATUREVALIDATIONHISTORYRESPONSE._serialized_end=23322
-  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_start=23325
-  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_end=23547
-  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_start=23550
-  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_end=23864
-  _GETUSERREQUEST._serialized_start=23866
-  _GETUSERREQUEST._serialized_end=23920
-  _GETUSERRESPONSE._serialized_start=23922
-  _GETUSERRESPONSE._serialized_end=23989
-  _GETFEATURESERVERCONFIGREQUEST._serialized_start=23991
-  _GETFEATURESERVERCONFIGREQUEST._serialized_end=24022
-  _GETFEATURESERVERCONFIGRESPONSE._serialized_start=24025
-  _GETFEATURESERVERCONFIGRESPONSE._serialized_end=24169
-  _SETFEATURESERVERCONFIGREQUEST._serialized_start=24171
-  _SETFEATURESERVERCONFIGREQUEST._serialized_end=24224
-  _METADATASERVICE._serialized_start=24292
-  _METADATASERVICE._serialized_end=43388
+  _GETFEATUREVALIDATIONRESULTREQUEST._serialized_start=23325
+  _GETFEATUREVALIDATIONRESULTREQUEST._serialized_end=23837
+  _GETFEATUREVALIDATIONRESULTRESPONSE._serialized_start=23840
+  _GETFEATUREVALIDATIONRESULTRESPONSE._serialized_end=23980
+  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_start=23983
+  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_end=24205
+  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_start=24208
+  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_end=24522
+  _GETUSERREQUEST._serialized_start=24524
+  _GETUSERREQUEST._serialized_end=24578
+  _GETUSERRESPONSE._serialized_start=24580
+  _GETUSERRESPONSE._serialized_end=24647
+  _GETFEATURESERVERCONFIGREQUEST._serialized_start=24649
+  _GETFEATURESERVERCONFIGREQUEST._serialized_end=24680
+  _GETFEATURESERVERCONFIGRESPONSE._serialized_start=24683
+  _GETFEATURESERVERCONFIGRESPONSE._serialized_end=24827
+  _SETFEATURESERVERCONFIGREQUEST._serialized_start=24829
+  _SETFEATURESERVERCONFIGREQUEST._serialized_end=24882
+  _METADATASERVICE._serialized_start=24950
+  _METADATASERVICE._serialized_end=44322
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.7.0b8/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.7.0b9/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.7.0b9/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/spark_api/error_pb2.py` & `tecton-0.7.0b9/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.7.0b9/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.7.0b9/tecton_proto/spark_common/clusters_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,50 +10,50 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(tecton_proto/spark_common/clusters.proto\x12\x19tecton_proto.spark_common\x1a\x1cgoogle/protobuf/struct.proto\"0\n\x0f\x45xistingCluster\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\x9f\x08\n\nNewCluster\x12!\n\x0bnum_workers\x18\x01 \x01(\x05H\x00R\nnumWorkers\x12\x44\n\tautoscale\x18\x02 \x01(\x0b\x32$.tecton_proto.spark_common.AutoScaleH\x00R\tautoscale\x12!\n\x0c\x63luster_name\x18\x03 \x01(\tR\x0b\x63lusterName\x12#\n\rspark_version\x18\x04 \x01(\tR\x0csparkVersion\x12S\n\nspark_conf\x18\x0f \x03(\x0b\x32\x34.tecton_proto.spark_common.NewCluster.SparkConfEntryR\tsparkConf\x12O\n\x0e\x61ws_attributes\x18\x07 \x01(\x0b\x32(.tecton_proto.spark_common.AwsAttributesR\rawsAttributes\x12 \n\x0cnode_type_id\x18\x06 \x01(\tR\nnodeTypeId\x12.\n\x13\x65nable_elastic_disk\x18\x0c \x01(\x08R\x11\x65nableElasticDisk\x12N\n\x0cinit_scripts\x18\t \x03(\x0b\x32+.tecton_proto.spark_common.ResourceLocationR\x0binitScripts\x12U\n\x10\x63luster_log_conf\x18\n \x01(\x0b\x32+.tecton_proto.spark_common.ResourceLocationR\x0e\x63lusterLogConf\x12\x46\n\x0b\x63ustom_tags\x18\x0b \x03(\x0b\x32%.tecton_proto.spark_common.ClusterTagR\ncustomTags\x12\x30\n\x13terminateOnComplete\x18\r \x01(\x08R\x13terminateOnComplete\x12]\n\x0espark_env_vars\x18\x10 \x03(\x0b\x32\x37.tecton_proto.spark_common.NewCluster.SparkEnvVarsEntryR\x0csparkEnvVars\x12G\n\x13json_cluster_config\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructR\x11jsonClusterConfig\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a?\n\x11SparkEnvVarsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0e\n\x0cworkers_typeJ\x04\x08\x05\x10\x06J\x04\x08\x08\x10\tJ\x04\x08\x0e\x10\x0f\"\x90\x01\n\x0b\x43lusterInfo\x12\x46\n\x0bnew_cluster\x18\x01 \x01(\x0b\x32%.tecton_proto.spark_common.NewClusterR\nnewCluster\x12\x1d\n\nfinal_json\x18\x02 \x01(\tR\tfinalJson\x12\x1a\n\x08warnings\x18\x03 \x03(\tR\x08warnings\"M\n\tAutoScale\x12\x1f\n\x0bmin_workers\x18\x01 \x01(\x05R\nminWorkers\x12\x1f\n\x0bmax_workers\x18\x02 \x01(\x05R\nmaxWorkers\"\xab\x03\n\rAwsAttributes\x12&\n\x0f\x66irst_on_demand\x18\x05 \x01(\x05R\rfirstOnDemand\x12N\n\x0c\x61vailability\x18\x06 \x01(\x0e\x32*.tecton_proto.spark_common.AwsAvailabilityR\x0c\x61vailability\x12\x17\n\x07zone_id\x18\x07 \x01(\tR\x06zoneId\x12\x33\n\x16spot_bid_price_percent\x18\x08 \x01(\x05R\x13spotBidPricePercent\x12\x30\n\x14instance_profile_arn\x18\x04 \x01(\tR\x12instanceProfileArn\x12P\n\x0f\x65\x62s_volume_type\x18\x01 \x01(\x0e\x32(.tecton_proto.spark_common.EbsVolumeTypeR\rebsVolumeType\x12(\n\x10\x65\x62s_volume_count\x18\x02 \x01(\x05R\x0e\x65\x62sVolumeCount\x12&\n\x0f\x65\x62s_volume_size\x18\x03 \x01(\x05R\rebsVolumeSize\"\xe1\x01\n\x10ResourceLocation\x12:\n\x02s3\x18\x01 \x01(\x0b\x32(.tecton_proto.spark_common.S3StorageInfoH\x00R\x02s3\x12@\n\x04\x64\x62\x66s\x18\x03 \x01(\x0b\x32*.tecton_proto.spark_common.DbfsStorageInfoH\x00R\x04\x64\x62\x66s\x12\x43\n\x05local\x18\x02 \x01(\x0b\x32+.tecton_proto.spark_common.LocalStorageInfoH\x00R\x05localB\n\n\x08location\"I\n\rS3StorageInfo\x12 \n\x0b\x64\x65stination\x18\x01 \x01(\tR\x0b\x64\x65stination\x12\x16\n\x06region\x18\x02 \x01(\tR\x06region\"3\n\x0f\x44\x62\x66sStorageInfo\x12 \n\x0b\x64\x65stination\x18\x01 \x01(\tR\x0b\x64\x65stination\"&\n\x10LocalStorageInfo\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"J\n\x0e\x43lusterLogConf\x12\x38\n\x02s3\x18\x01 \x01(\x0b\x32(.tecton_proto.spark_common.S3StorageInfoR\x02s3\"4\n\nClusterTag\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value*\x8f\x01\n\x0f\x41wsAvailability\x12\x1c\n\x18UNKNOWN_AWS_AVAILABILITY\x10\x00\x12\x08\n\x04SPOT\x10\x01\x12\r\n\tON_DEMAND\x10\x02\x12\x16\n\x12SPOT_WITH_FALLBACK\x10\x03\x12-\n)INSTANCE_FLEET_FOR_INTEGRATION_TESTS_ONLY\x10\x04*c\n\rEbsVolumeType\x12\x1b\n\x17UNKNOWN_EBS_VOLUME_TYPE\x10\x00\x12\x17\n\x13GENERAL_PURPOSE_SSD\x10\x01\x12\x1c\n\x18THROUGHPUT_OPTIMIZED_HDD\x10\x02\x42\x1b\n\x17\x63om.tecton.spark_commonP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(tecton_proto/spark_common/clusters.proto\x12\x19tecton_proto.spark_common\x1a\x1cgoogle/protobuf/struct.proto\"0\n\x0f\x45xistingCluster\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xbc\x08\n\nNewCluster\x12!\n\x0bnum_workers\x18\x01 \x01(\x05H\x00R\nnumWorkers\x12\x44\n\tautoscale\x18\x02 \x01(\x0b\x32$.tecton_proto.spark_common.AutoScaleH\x00R\tautoscale\x12!\n\x0c\x63luster_name\x18\x03 \x01(\tR\x0b\x63lusterName\x12#\n\rspark_version\x18\x04 \x01(\tR\x0csparkVersion\x12S\n\nspark_conf\x18\x0f \x03(\x0b\x32\x34.tecton_proto.spark_common.NewCluster.SparkConfEntryR\tsparkConf\x12O\n\x0e\x61ws_attributes\x18\x07 \x01(\x0b\x32(.tecton_proto.spark_common.AwsAttributesR\rawsAttributes\x12 \n\x0cnode_type_id\x18\x06 \x01(\tR\nnodeTypeId\x12.\n\x13\x65nable_elastic_disk\x18\x0c \x01(\x08R\x11\x65nableElasticDisk\x12N\n\x0cinit_scripts\x18\t \x03(\x0b\x32+.tecton_proto.spark_common.ResourceLocationR\x0binitScripts\x12U\n\x10\x63luster_log_conf\x18\n \x01(\x0b\x32+.tecton_proto.spark_common.ResourceLocationR\x0e\x63lusterLogConf\x12\x46\n\x0b\x63ustom_tags\x18\x0b \x03(\x0b\x32%.tecton_proto.spark_common.ClusterTagR\ncustomTags\x12\x30\n\x13terminateOnComplete\x18\r \x01(\x08R\x13terminateOnComplete\x12]\n\x0espark_env_vars\x18\x10 \x03(\x0b\x32\x37.tecton_proto.spark_common.NewCluster.SparkEnvVarsEntryR\x0csparkEnvVars\x12G\n\x13json_cluster_config\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructR\x11jsonClusterConfig\x12\x1b\n\tpolicy_id\x18\x12 \x01(\tR\x08policyId\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a?\n\x11SparkEnvVarsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0e\n\x0cworkers_typeJ\x04\x08\x05\x10\x06J\x04\x08\x08\x10\tJ\x04\x08\x0e\x10\x0f\"\x90\x01\n\x0b\x43lusterInfo\x12\x46\n\x0bnew_cluster\x18\x01 \x01(\x0b\x32%.tecton_proto.spark_common.NewClusterR\nnewCluster\x12\x1d\n\nfinal_json\x18\x02 \x01(\tR\tfinalJson\x12\x1a\n\x08warnings\x18\x03 \x03(\tR\x08warnings\"M\n\tAutoScale\x12\x1f\n\x0bmin_workers\x18\x01 \x01(\x05R\nminWorkers\x12\x1f\n\x0bmax_workers\x18\x02 \x01(\x05R\nmaxWorkers\"\xab\x03\n\rAwsAttributes\x12&\n\x0f\x66irst_on_demand\x18\x05 \x01(\x05R\rfirstOnDemand\x12N\n\x0c\x61vailability\x18\x06 \x01(\x0e\x32*.tecton_proto.spark_common.AwsAvailabilityR\x0c\x61vailability\x12\x17\n\x07zone_id\x18\x07 \x01(\tR\x06zoneId\x12\x33\n\x16spot_bid_price_percent\x18\x08 \x01(\x05R\x13spotBidPricePercent\x12\x30\n\x14instance_profile_arn\x18\x04 \x01(\tR\x12instanceProfileArn\x12P\n\x0f\x65\x62s_volume_type\x18\x01 \x01(\x0e\x32(.tecton_proto.spark_common.EbsVolumeTypeR\rebsVolumeType\x12(\n\x10\x65\x62s_volume_count\x18\x02 \x01(\x05R\x0e\x65\x62sVolumeCount\x12&\n\x0f\x65\x62s_volume_size\x18\x03 \x01(\x05R\rebsVolumeSize\"\xe1\x01\n\x10ResourceLocation\x12:\n\x02s3\x18\x01 \x01(\x0b\x32(.tecton_proto.spark_common.S3StorageInfoH\x00R\x02s3\x12@\n\x04\x64\x62\x66s\x18\x03 \x01(\x0b\x32*.tecton_proto.spark_common.DbfsStorageInfoH\x00R\x04\x64\x62\x66s\x12\x43\n\x05local\x18\x02 \x01(\x0b\x32+.tecton_proto.spark_common.LocalStorageInfoH\x00R\x05localB\n\n\x08location\"I\n\rS3StorageInfo\x12 \n\x0b\x64\x65stination\x18\x01 \x01(\tR\x0b\x64\x65stination\x12\x16\n\x06region\x18\x02 \x01(\tR\x06region\"3\n\x0f\x44\x62\x66sStorageInfo\x12 \n\x0b\x64\x65stination\x18\x01 \x01(\tR\x0b\x64\x65stination\"&\n\x10LocalStorageInfo\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"J\n\x0e\x43lusterLogConf\x12\x38\n\x02s3\x18\x01 \x01(\x0b\x32(.tecton_proto.spark_common.S3StorageInfoR\x02s3\"4\n\nClusterTag\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value*\x8f\x01\n\x0f\x41wsAvailability\x12\x1c\n\x18UNKNOWN_AWS_AVAILABILITY\x10\x00\x12\x08\n\x04SPOT\x10\x01\x12\r\n\tON_DEMAND\x10\x02\x12\x16\n\x12SPOT_WITH_FALLBACK\x10\x03\x12-\n)INSTANCE_FLEET_FOR_INTEGRATION_TESTS_ONLY\x10\x04*c\n\rEbsVolumeType\x12\x1b\n\x17UNKNOWN_EBS_VOLUME_TYPE\x10\x00\x12\x17\n\x13GENERAL_PURPOSE_SSD\x10\x01\x12\x1c\n\x18THROUGHPUT_OPTIMIZED_HDD\x10\x02\x42\x1b\n\x17\x63om.tecton.spark_commonP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.spark_common.clusters_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\027com.tecton.spark_commonP\001'
   _NEWCLUSTER_SPARKCONFENTRY._options = None
   _NEWCLUSTER_SPARKCONFENTRY._serialized_options = b'8\001'
   _NEWCLUSTER_SPARKENVVARSENTRY._options = None
   _NEWCLUSTER_SPARKENVVARSENTRY._serialized_options = b'8\001'
-  _AWSAVAILABILITY._serialized_start=2392
-  _AWSAVAILABILITY._serialized_end=2535
-  _EBSVOLUMETYPE._serialized_start=2537
-  _EBSVOLUMETYPE._serialized_end=2636
+  _AWSAVAILABILITY._serialized_start=2421
+  _AWSAVAILABILITY._serialized_end=2564
+  _EBSVOLUMETYPE._serialized_start=2566
+  _EBSVOLUMETYPE._serialized_end=2665
   _EXISTINGCLUSTER._serialized_start=101
   _EXISTINGCLUSTER._serialized_end=149
   _NEWCLUSTER._serialized_start=152
-  _NEWCLUSTER._serialized_end=1207
-  _NEWCLUSTER_SPARKCONFENTRY._serialized_start=1048
-  _NEWCLUSTER_SPARKCONFENTRY._serialized_end=1108
-  _NEWCLUSTER_SPARKENVVARSENTRY._serialized_start=1110
-  _NEWCLUSTER_SPARKENVVARSENTRY._serialized_end=1173
-  _CLUSTERINFO._serialized_start=1210
-  _CLUSTERINFO._serialized_end=1354
-  _AUTOSCALE._serialized_start=1356
-  _AUTOSCALE._serialized_end=1433
-  _AWSATTRIBUTES._serialized_start=1436
-  _AWSATTRIBUTES._serialized_end=1863
-  _RESOURCELOCATION._serialized_start=1866
-  _RESOURCELOCATION._serialized_end=2091
-  _S3STORAGEINFO._serialized_start=2093
-  _S3STORAGEINFO._serialized_end=2166
-  _DBFSSTORAGEINFO._serialized_start=2168
-  _DBFSSTORAGEINFO._serialized_end=2219
-  _LOCALSTORAGEINFO._serialized_start=2221
-  _LOCALSTORAGEINFO._serialized_end=2259
-  _CLUSTERLOGCONF._serialized_start=2261
-  _CLUSTERLOGCONF._serialized_end=2335
-  _CLUSTERTAG._serialized_start=2337
-  _CLUSTERTAG._serialized_end=2389
+  _NEWCLUSTER._serialized_end=1236
+  _NEWCLUSTER_SPARKCONFENTRY._serialized_start=1077
+  _NEWCLUSTER_SPARKCONFENTRY._serialized_end=1137
+  _NEWCLUSTER_SPARKENVVARSENTRY._serialized_start=1139
+  _NEWCLUSTER_SPARKENVVARSENTRY._serialized_end=1202
+  _CLUSTERINFO._serialized_start=1239
+  _CLUSTERINFO._serialized_end=1383
+  _AUTOSCALE._serialized_start=1385
+  _AUTOSCALE._serialized_end=1462
+  _AWSATTRIBUTES._serialized_start=1465
+  _AWSATTRIBUTES._serialized_end=1892
+  _RESOURCELOCATION._serialized_start=1895
+  _RESOURCELOCATION._serialized_end=2120
+  _S3STORAGEINFO._serialized_start=2122
+  _S3STORAGEINFO._serialized_end=2195
+  _DBFSSTORAGEINFO._serialized_start=2197
+  _DBFSSTORAGEINFO._serialized_end=2248
+  _LOCALSTORAGEINFO._serialized_start=2250
+  _LOCALSTORAGEINFO._serialized_end=2288
+  _CLUSTERLOGCONF._serialized_start=2290
+  _CLUSTERLOGCONF._serialized_end=2364
+  _CLUSTERTAG._serialized_start=2366
+  _CLUSTERTAG._serialized_end=2418
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.7.0b8/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.7.0b9/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_proto/validation/validator_pb2.py` & `tecton-0.7.0b9/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/pipeline_helper.py` & `tecton-0.7.0b9/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.7.0b9/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/sql_helper.py` & `tecton-0.7.0b9/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/historical_features.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates/time_limit.sql` & `tecton-0.7.0b9/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_snowflake/templates_utils.py` & `tecton-0.7.0b9/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/aggregation_plans.py` & `tecton-0.7.0b9/tecton_spark/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/data_observability.py` & `tecton-0.7.0b9/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/data_source_credentials.py` & `tecton-0.7.0b9/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/data_source_helper.py` & `tecton-0.7.0b9/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/feature_view_spark_utils.py` & `tecton-0.7.0b9/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/ingest_utils.py` & `tecton-0.7.0b9/tecton_spark/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.7.0b9/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/materialization_plan.py` & `tecton-0.7.0b9/tecton_spark/materialization_plan.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/offline_store.py` & `tecton-0.7.0b9/tecton_spark/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/partial_aggregations.py` & `tecton-0.7.0b9/tecton_spark/partial_aggregations.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/pipeline_helper.py` & `tecton-0.7.0b9/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/data_source.py` & `tecton-0.7.0b9/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/filter.py` & `tecton-0.7.0b9/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/join.py` & `tecton-0.7.0b9/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/node.py` & `tecton-0.7.0b9/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/pipeline.py` & `tecton-0.7.0b9/tecton_spark/query/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/projection.py` & `tecton-0.7.0b9/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/query/translate.py` & `tecton-0.7.0b9/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/request_context.py` & `tecton-0.7.0b9/tecton_spark/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/schema_derivation_utils.py` & `tecton-0.7.0b9/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/schema_spark_utils.py` & `tecton-0.7.0b9/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/spark_helper.py` & `tecton-0.7.0b9/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/spark_schema_wrapper.py` & `tecton-0.7.0b9/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/time_utils.py` & `tecton-0.7.0b9/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0b8/tecton_spark/udfs.py` & `tecton-0.7.0b9/tecton_spark/udfs.py`

 * *Files identical despite different names*


# Comparing `tmp/vwo-python-sdk-1.8.2.tar.gz` & `tmp/vwo-python-sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vwo-python-sdk-1.8.2.tar", last modified: Wed Feb 10 08:52:12 2021, max compression
+gzip compressed data, was "dist/vwo-python-sdk-1.9.0.tar", last modified: Mon Feb 15 10:41:33 2021, max compression
```

## Comparing `vwo-python-sdk-1.8.2.tar` & `vwo-python-sdk-1.9.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5563 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1877 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 varunmalhotra   (502) staff       (20)       56 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/requires.txt
--rw-r--r--   0 varunmalhotra   (502) staff       (20)       10 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 varunmalhotra   (502) staff       (20)        1 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5563 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/PKG-INFO
--rw-r--r--   0 varunmalhotra   (502) staff       (20)    11362 2021-02-10 08:31:38.000000 vwo-python-sdk-1.8.2/LICENSE
--rw-r--r--   0 varunmalhotra   (502) staff       (20)       56 2019-08-08 11:44:43.000000 vwo-python-sdk-1.8.2/requirements.txt
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/core/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)    22699 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/core/variation_decider.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/core/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     6288 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/core/bucketer.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/logger/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/logger/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5072 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/logger/VWOLogger.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/constants/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2300 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/constants/constants.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/constants/__init__.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/enums/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2152 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/file_name_enum.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      738 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/log_level_enum.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      722 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)    12394 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/log_message_enum.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      674 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/operand_types.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      663 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/operator_types.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      660 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/result_status.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      872 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      713 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/operand_value_types_name.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      765 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/operand_value_types.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      667 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/enums/segments/operand_value_boolean_types.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      821 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/__init__.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/schemas/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1104 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/settings_file_schema.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1070 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/variation_schema.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      649 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/empty_object_schema.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1437 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/campaign_schema.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      888 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/variable_schema.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      815 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/schemas/goal_schema.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/storage/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1446 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/storage/user.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/storage/__init__.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/http/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/http/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2004 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/http/connection.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     3294 2021-02-10 08:41:17.000000 vwo-python-sdk-1.8.2/vwo/vwo.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/api/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     9656 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/api/track.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5129 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/api/is_feature_enabled.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      865 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/api/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     3609 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/api/launch.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     3651 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/api/get_variation_name.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5784 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/api/get_feature_variable_value.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     4495 2021-02-10 08:41:15.000000 vwo-python-sdk-1.8.2/vwo/api/activate.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2907 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/api/push.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/event/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2485 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/event/event_dispatcher.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/event/__init__.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/helpers/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     8760 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/helpers/campaign_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     3923 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/helpers/impression_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2070 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/helpers/uuid_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1880 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/helpers/custom_dimensions_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     4647 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/helpers/validate_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/helpers/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2188 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/helpers/feature_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5344 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/helpers/segment_utils.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2518 2021-02-10 08:41:16.000000 vwo-python-sdk-1.8.2/vwo/helpers/generic_util.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2744 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/helpers/settings_file_util.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/services/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     1852 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/services/settings_file_manager.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/services/__init__.py
-drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/vwo/services/segmentor/
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      659 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/services/segmentor/__init__.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     2225 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/services/segmentor/segment_evaluator.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     5904 2021-02-10 08:30:49.000000 vwo-python-sdk-1.8.2/vwo/services/segmentor/operand_evaluator.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)      114 2019-08-07 11:31:17.000000 vwo-python-sdk-1.8.2/MANIFEST.in
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     3624 2021-02-10 08:31:49.000000 vwo-python-sdk-1.8.2/README.md
--rw-r--r--   0 varunmalhotra   (502) staff       (20)     4163 2021-02-10 08:51:57.000000 vwo-python-sdk-1.8.2/setup.py
--rw-r--r--   0 varunmalhotra   (502) staff       (20)       95 2020-07-01 14:11:40.000000 vwo-python-sdk-1.8.2/requirements-dev.txt
--rw-r--r--   0 varunmalhotra   (502) staff       (20)       38 2021-02-10 08:52:12.000000 vwo-python-sdk-1.8.2/setup.cfg
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5563 2021-02-15 10:41:32.000000 vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1877 2021-02-15 10:41:32.000000 vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)       56 2021-02-15 10:41:32.000000 vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)       10 2021-02-15 10:41:32.000000 vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)        1 2021-02-15 10:41:32.000000 vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5563 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/PKG-INFO
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)    11362 2021-02-10 08:31:38.000000 vwo-python-sdk-1.9.0/LICENSE
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)       56 2019-08-08 11:44:43.000000 vwo-python-sdk-1.9.0/requirements.txt
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/core/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)    22699 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/core/variation_decider.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/core/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     6288 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/core/bucketer.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/logger/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/logger/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5072 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/logger/VWOLogger.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/constants/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2300 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/constants/constants.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/constants/__init__.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/enums/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2152 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/enums/file_name_enum.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      738 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/log_level_enum.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      722 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)    12394 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/enums/log_message_enum.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      674 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/operand_types.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      663 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/operator_types.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      660 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/result_status.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      872 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      713 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/operand_value_types_name.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      765 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/operand_value_types.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      667 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/enums/segments/operand_value_boolean_types.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      821 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/__init__.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/schemas/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1104 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/settings_file_schema.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1070 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/variation_schema.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      649 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/empty_object_schema.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1437 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/campaign_schema.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      888 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/variable_schema.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      815 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/schemas/goal_schema.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/storage/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1446 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/storage/user.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/storage/__init__.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/http/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/http/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2004 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/http/connection.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     3294 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/vwo.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/api/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     9656 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/api/track.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5129 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/api/is_feature_enabled.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      865 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/api/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     3609 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/api/launch.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     3651 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/api/get_variation_name.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5784 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/api/get_feature_variable_value.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     4495 2021-02-10 08:41:15.000000 vwo-python-sdk-1.9.0/vwo/api/activate.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2907 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/api/push.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/event/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2485 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/event/event_dispatcher.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/event/__init__.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/helpers/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     8760 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/helpers/campaign_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     3923 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/helpers/impression_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2070 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/helpers/uuid_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1880 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/helpers/custom_dimensions_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     4647 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/helpers/validate_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/helpers/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2188 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/helpers/feature_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5344 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/helpers/segment_utils.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2518 2021-02-10 08:41:16.000000 vwo-python-sdk-1.9.0/vwo/helpers/generic_util.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2744 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/helpers/settings_file_util.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/services/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     1852 2021-02-15 10:40:55.000000 vwo-python-sdk-1.9.0/vwo/services/settings_file_manager.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      594 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/services/__init__.py
+drwxr-xr-x   0 varunmalhotra   (502) staff       (20)        0 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/vwo/services/segmentor/
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      659 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/services/segmentor/__init__.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     2225 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/services/segmentor/segment_evaluator.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     5904 2021-02-10 08:30:49.000000 vwo-python-sdk-1.9.0/vwo/services/segmentor/operand_evaluator.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)      114 2019-08-07 11:31:17.000000 vwo-python-sdk-1.9.0/MANIFEST.in
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     3624 2021-02-10 08:31:49.000000 vwo-python-sdk-1.9.0/README.md
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)     4163 2021-02-15 10:41:09.000000 vwo-python-sdk-1.9.0/setup.py
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)       95 2020-07-01 14:11:40.000000 vwo-python-sdk-1.9.0/requirements-dev.txt
+-rw-r--r--   0 varunmalhotra   (502) staff       (20)       38 2021-02-15 10:41:33.000000 vwo-python-sdk-1.9.0/setup.cfg
```

### Comparing `vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/PKG-INFO` & `vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vwo-python-sdk
-Version: 1.8.2
+Version: 1.9.0
 Summary: Python SDK for VWO server-side A/B Testing
 Home-page: https://github.com/wingify/vwo-python-sdk
 Author: VWO
 Author-email: dev@wingify.com
 License: Apache License 2.0
 Description: # VWO Python SDK
```

### Comparing `vwo-python-sdk-1.8.2/vwo_python_sdk.egg-info/SOURCES.txt` & `vwo-python-sdk-1.9.0/vwo_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/PKG-INFO` & `vwo-python-sdk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vwo-python-sdk
-Version: 1.8.2
+Version: 1.9.0
 Summary: Python SDK for VWO server-side A/B Testing
 Home-page: https://github.com/wingify/vwo-python-sdk
 Author: VWO
 Author-email: dev@wingify.com
 License: Apache License 2.0
 Description: # VWO Python SDK
```

### Comparing `vwo-python-sdk-1.8.2/LICENSE` & `vwo-python-sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/core/variation_decider.py` & `vwo-python-sdk-1.9.0/vwo/core/variation_decider.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/core/__init__.py` & `vwo-python-sdk-1.9.0/vwo/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/core/bucketer.py` & `vwo-python-sdk-1.9.0/vwo/core/bucketer.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/logger/__init__.py` & `vwo-python-sdk-1.9.0/vwo/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/logger/VWOLogger.py` & `vwo-python-sdk-1.9.0/vwo/logger/VWOLogger.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/constants/constants.py` & `vwo-python-sdk-1.9.0/vwo/constants/constants.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/constants/__init__.py` & `vwo-python-sdk-1.9.0/vwo/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/file_name_enum.py` & `vwo-python-sdk-1.9.0/vwo/enums/file_name_enum.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/log_level_enum.py` & `vwo-python-sdk-1.9.0/vwo/enums/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/__init__.py` & `vwo-python-sdk-1.9.0/vwo/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/log_message_enum.py` & `vwo-python-sdk-1.9.0/vwo/enums/log_message_enum.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/operand_types.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/operand_types.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/operator_types.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/operator_types.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/result_status.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/result_status.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/__init__.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/operand_value_types_name.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/operand_value_types_name.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/operand_value_types.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/operand_value_types.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/enums/segments/operand_value_boolean_types.py` & `vwo-python-sdk-1.9.0/vwo/enums/segments/operand_value_boolean_types.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/__init__.py` & `vwo-python-sdk-1.9.0/vwo/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/settings_file_schema.py` & `vwo-python-sdk-1.9.0/vwo/schemas/settings_file_schema.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/variation_schema.py` & `vwo-python-sdk-1.9.0/vwo/schemas/variation_schema.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/__init__.py` & `vwo-python-sdk-1.9.0/vwo/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/empty_object_schema.py` & `vwo-python-sdk-1.9.0/vwo/schemas/empty_object_schema.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/campaign_schema.py` & `vwo-python-sdk-1.9.0/vwo/schemas/campaign_schema.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/variable_schema.py` & `vwo-python-sdk-1.9.0/vwo/schemas/variable_schema.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/schemas/goal_schema.py` & `vwo-python-sdk-1.9.0/vwo/schemas/goal_schema.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/storage/user.py` & `vwo-python-sdk-1.9.0/vwo/storage/user.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/storage/__init__.py` & `vwo-python-sdk-1.9.0/vwo/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/http/__init__.py` & `vwo-python-sdk-1.9.0/vwo/http/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/http/connection.py` & `vwo-python-sdk-1.9.0/vwo/http/connection.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/vwo.py` & `vwo-python-sdk-1.9.0/vwo/vwo.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/track.py` & `vwo-python-sdk-1.9.0/vwo/api/track.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/is_feature_enabled.py` & `vwo-python-sdk-1.9.0/vwo/api/is_feature_enabled.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/__init__.py` & `vwo-python-sdk-1.9.0/vwo/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/launch.py` & `vwo-python-sdk-1.9.0/vwo/api/launch.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/get_variation_name.py` & `vwo-python-sdk-1.9.0/vwo/api/get_variation_name.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/get_feature_variable_value.py` & `vwo-python-sdk-1.9.0/vwo/api/get_feature_variable_value.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/activate.py` & `vwo-python-sdk-1.9.0/vwo/api/activate.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/api/push.py` & `vwo-python-sdk-1.9.0/vwo/api/push.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/event/event_dispatcher.py` & `vwo-python-sdk-1.9.0/vwo/event/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/event/__init__.py` & `vwo-python-sdk-1.9.0/vwo/event/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/campaign_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/campaign_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/impression_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/impression_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/uuid_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/uuid_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/custom_dimensions_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/custom_dimensions_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/validate_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/validate_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/__init__.py` & `vwo-python-sdk-1.9.0/vwo/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/feature_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/feature_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/segment_utils.py` & `vwo-python-sdk-1.9.0/vwo/helpers/segment_utils.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/generic_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/generic_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/helpers/settings_file_util.py` & `vwo-python-sdk-1.9.0/vwo/helpers/settings_file_util.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/services/settings_file_manager.py` & `vwo-python-sdk-1.9.0/vwo/services/settings_file_manager.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/services/__init__.py` & `vwo-python-sdk-1.9.0/vwo/services/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/services/segmentor/__init__.py` & `vwo-python-sdk-1.9.0/vwo/services/segmentor/__init__.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/services/segmentor/segment_evaluator.py` & `vwo-python-sdk-1.9.0/vwo/services/segmentor/segment_evaluator.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/vwo/services/segmentor/operand_evaluator.py` & `vwo-python-sdk-1.9.0/vwo/services/segmentor/operand_evaluator.py`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/README.md` & `vwo-python-sdk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vwo-python-sdk-1.8.2/setup.py` & `vwo-python-sdk-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         print("\nDONE: RUNNING POST INSTALL DEVELOP SCRIPT \n")
 
         develop.run(self)
 
 
 setup(
     name="vwo-python-sdk",
-    version="1.8.2",
+    version="1.9.0",
     description="Python SDK for VWO server-side A/B Testing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="VWO",
     author_email="dev@wingify.com",
     url="https://github.com/wingify/vwo-python-sdk",
     license="Apache License 2.0",
```


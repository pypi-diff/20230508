# Comparing `tmp/omnibenchmark-0.0.8.tar.gz` & `tmp/omnibenchmark-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnibenchmark-0.0.8.tar", last modified: Thu Jul 21 14:19:25 2022, max compression
+gzip compressed data, was "omnibenchmark-0.0.9.tar", last modified: Fri Jul 22 09:41:13 2022, max compression
```

## Comparing `omnibenchmark-0.0.8.tar` & `omnibenchmark-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/
--rw-rw-r--   0 almut     (1000) almut     (1000)    11357 2022-06-27 09:28:17.000000 omnibenchmark-0.0.8/LICENSE
--rw-rw-r--   0 almut     (1000) almut     (1000)     5158 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/PKG-INFO
--rw-rw-r--   0 almut     (1000) almut     (1000)     4357 2022-07-21 14:17:41.000000 omnibenchmark-0.0.8/README.md
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.864268 omnibenchmark-0.0.8/omnibenchmark/
--rw-rw-r--   0 almut     (1000) almut     (1000)      210 2022-07-21 14:17:43.000000 omnibenchmark-0.0.8/omnibenchmark/__init__.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.864268 omnibenchmark-0.0.8/omnibenchmark/core/
--rw-rw-r--   0 almut     (1000) almut     (1000)     6401 2022-07-19 14:12:05.000000 omnibenchmark-0.0.8/omnibenchmark/core/input_classes.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     5961 2022-07-21 11:52:42.000000 omnibenchmark-0.0.8/omnibenchmark/core/omni_object.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     8133 2022-07-21 11:50:34.000000 omnibenchmark-0.0.8/omnibenchmark/core/output_classes.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.864268 omnibenchmark-0.0.8/omnibenchmark/management/
--rw-rw-r--   0 almut     (1000) almut     (1000)     1291 2022-05-16 09:46:26.000000 omnibenchmark-0.0.8/omnibenchmark/management/data_checks.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     9467 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/management/data_commands.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     2066 2022-07-01 13:51:25.000000 omnibenchmark-0.0.8/omnibenchmark/management/general_checks.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     3946 2022-06-28 11:41:19.000000 omnibenchmark-0.0.8/omnibenchmark/management/parameter_checks.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     5907 2022-06-16 11:50:17.000000 omnibenchmark-0.0.8/omnibenchmark/management/run_commands.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     4797 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/management/wflow_checks.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.864268 omnibenchmark-0.0.8/omnibenchmark/renku_commands/
--rw-rw-r--   0 almut     (1000) almut     (1000)     5835 2022-06-24 13:24:51.000000 omnibenchmark-0.0.8/omnibenchmark/renku_commands/datasets.py
--rw-rw-r--   0 almut     (1000) almut     (1000)      623 2022-06-16 11:50:17.000000 omnibenchmark-0.0.8/omnibenchmark/renku_commands/general.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     3019 2022-05-16 15:19:05.000000 omnibenchmark-0.0.8/omnibenchmark/renku_commands/workflows.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.864268 omnibenchmark-0.0.8/omnibenchmark/test/
--rw-rw-r--   0 almut     (1000) almut     (1000)        0 2022-02-24 14:58:08.000000 omnibenchmark-0.0.8/omnibenchmark/test/__init__.py
--rw-rw-r--   0 almut     (1000) almut     (1000)    10265 2022-07-20 06:14:39.000000 omnibenchmark-0.0.8/omnibenchmark/test/conftest.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/omnibenchmark/test/core/
--rw-rw-r--   0 almut     (1000) almut     (1000)      395 2022-03-11 06:55:27.000000 omnibenchmark-0.0.8/omnibenchmark/test/core/conftest.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     1097 2022-07-20 06:17:20.000000 omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_command.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     2349 2022-06-21 15:43:44.000000 omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_input.py
--rw-rw-r--   0 almut     (1000) almut     (1000)        0 2022-02-24 14:58:08.000000 omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_object.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     2370 2022-07-19 13:47:31.000000 omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_output.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     1026 2022-03-21 16:34:30.000000 omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_parameter.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/omnibenchmark/test/managment/
--rw-rw-r--   0 almut     (1000) almut     (1000)      266 2022-06-28 11:41:19.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/conftest.py
--rw-rw-r--   0 almut     (1000) almut     (1000)      628 2022-06-16 12:20:02.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_data_checks.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     9169 2022-06-17 09:34:29.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_data_commands.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     1939 2022-07-01 14:02:26.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_general_checks.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     3883 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_parameter_checks.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     4711 2022-06-28 11:41:19.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_run_commands.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     5350 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/test/managment/test_managment_wflow_checks.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/omnibenchmark/test/renku_commands/
--rw-rw-r--   0 almut     (1000) almut     (1000)     5111 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/test/renku_commands/test_renku_commands_datasets.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/omnibenchmark/test/utils/
--rw-rw-r--   0 almut     (1000) almut     (1000)     1330 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/test/utils/conftest.py
--rw-rw-r--   0 almut     (1000) almut     (1000)    12583 2022-07-19 14:00:29.000000 omnibenchmark-0.0.8/omnibenchmark/test/utils/test_build_omni_object.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     2636 2022-03-22 09:31:28.000000 omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_command.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     4733 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_input.py
--rw-rw-r--   0 almut     (1000) almut     (1000)    12339 2022-07-19 14:16:45.000000 omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_output.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     5797 2022-05-09 07:58:02.000000 omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_run.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/omnibenchmark/utils/
--rw-rw-r--   0 almut     (1000) almut     (1000)     3617 2022-05-06 20:02:23.000000 omnibenchmark-0.0.8/omnibenchmark/utils/auto_command.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     4630 2022-07-14 05:57:14.000000 omnibenchmark-0.0.8/omnibenchmark/utils/auto_input.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     9498 2022-07-19 12:46:20.000000 omnibenchmark-0.0.8/omnibenchmark/utils/auto_output.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     3735 2022-05-16 14:04:16.000000 omnibenchmark-0.0.8/omnibenchmark/utils/auto_run.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     9777 2022-06-20 12:06:26.000000 omnibenchmark-0.0.8/omnibenchmark/utils/build_omni_object.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     1575 2022-05-16 09:51:57.000000 omnibenchmark-0.0.8/omnibenchmark/utils/context_manager.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     1425 2022-04-11 14:18:34.000000 omnibenchmark-0.0.8/omnibenchmark/utils/decorators.py
--rw-rw-r--   0 almut     (1000) almut     (1000)      545 2022-07-01 15:08:30.000000 omnibenchmark-0.0.8/omnibenchmark/utils/default_global_vars.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     1333 2022-06-21 15:43:44.000000 omnibenchmark-0.0.8/omnibenchmark/utils/exceptions.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     3336 2022-04-26 17:44:09.000000 omnibenchmark-0.0.8/omnibenchmark/utils/log.py
--rw-rw-r--   0 almut     (1000) almut     (1000)     2546 2022-07-19 14:08:00.000000 omnibenchmark-0.0.8/omnibenchmark/utils/user_input_checks.py
-drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-21 14:19:25.864268 omnibenchmark-0.0.8/omnibenchmark.egg-info/
--rw-rw-r--   0 almut     (1000) almut     (1000)     5158 2022-07-21 14:19:25.000000 omnibenchmark-0.0.8/omnibenchmark.egg-info/PKG-INFO
--rw-rw-r--   0 almut     (1000) almut     (1000)     2242 2022-07-21 14:19:25.000000 omnibenchmark-0.0.8/omnibenchmark.egg-info/SOURCES.txt
--rw-rw-r--   0 almut     (1000) almut     (1000)        1 2022-07-21 14:19:25.000000 omnibenchmark-0.0.8/omnibenchmark.egg-info/dependency_links.txt
--rw-rw-r--   0 almut     (1000) almut     (1000)      112 2022-07-21 14:19:25.000000 omnibenchmark-0.0.8/omnibenchmark.egg-info/requires.txt
--rw-rw-r--   0 almut     (1000) almut     (1000)       14 2022-07-21 14:19:25.000000 omnibenchmark-0.0.8/omnibenchmark.egg-info/top_level.txt
--rw-rw-r--   0 almut     (1000) almut     (1000)     1420 2022-07-21 14:19:16.000000 omnibenchmark-0.0.8/pyproject.toml
--rw-rw-r--   0 almut     (1000) almut     (1000)       38 2022-07-21 14:19:25.868268 omnibenchmark-0.0.8/setup.cfg
--rw-rw-r--   0 almut     (1000) almut     (1000)       38 2022-07-11 13:48:17.000000 omnibenchmark-0.0.8/setup.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.331738 omnibenchmark-0.0.9/
+-rw-rw-r--   0 almut     (1000) almut     (1000)    11357 2022-06-27 09:28:17.000000 omnibenchmark-0.0.9/LICENSE
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5226 2022-07-22 09:41:13.331738 omnibenchmark-0.0.9/PKG-INFO
+-rw-rw-r--   0 almut     (1000) almut     (1000)     4425 2022-07-22 09:39:35.000000 omnibenchmark-0.0.9/README.md
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/
+-rw-rw-r--   0 almut     (1000) almut     (1000)      210 2022-07-22 09:41:05.000000 omnibenchmark-0.0.9/omnibenchmark/__init__.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/core/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     6401 2022-07-19 14:12:05.000000 omnibenchmark-0.0.9/omnibenchmark/core/input_classes.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5961 2022-07-21 11:52:42.000000 omnibenchmark-0.0.9/omnibenchmark/core/omni_object.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     8133 2022-07-21 11:50:34.000000 omnibenchmark-0.0.9/omnibenchmark/core/output_classes.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/management/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1291 2022-05-16 09:46:26.000000 omnibenchmark-0.0.9/omnibenchmark/management/data_checks.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     9467 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/management/data_commands.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     2066 2022-07-01 13:51:25.000000 omnibenchmark-0.0.9/omnibenchmark/management/general_checks.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     3946 2022-06-28 11:41:19.000000 omnibenchmark-0.0.9/omnibenchmark/management/parameter_checks.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5907 2022-06-16 11:50:17.000000 omnibenchmark-0.0.9/omnibenchmark/management/run_commands.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     4797 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/management/wflow_checks.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/renku_commands/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5835 2022-06-24 13:24:51.000000 omnibenchmark-0.0.9/omnibenchmark/renku_commands/datasets.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)      623 2022-06-16 11:50:17.000000 omnibenchmark-0.0.9/omnibenchmark/renku_commands/general.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     3019 2022-05-16 15:19:05.000000 omnibenchmark-0.0.9/omnibenchmark/renku_commands/workflows.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/test/
+-rw-rw-r--   0 almut     (1000) almut     (1000)        0 2022-02-24 14:58:08.000000 omnibenchmark-0.0.9/omnibenchmark/test/__init__.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)    10265 2022-07-20 06:14:39.000000 omnibenchmark-0.0.9/omnibenchmark/test/conftest.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/test/core/
+-rw-rw-r--   0 almut     (1000) almut     (1000)      395 2022-03-11 06:55:27.000000 omnibenchmark-0.0.9/omnibenchmark/test/core/conftest.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1097 2022-07-20 06:17:20.000000 omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_command.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     2349 2022-06-21 15:43:44.000000 omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_input.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)        0 2022-02-24 14:58:08.000000 omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_object.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     2370 2022-07-19 13:47:31.000000 omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_output.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1026 2022-03-21 16:34:30.000000 omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_parameter.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/test/managment/
+-rw-rw-r--   0 almut     (1000) almut     (1000)      266 2022-06-28 11:41:19.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/conftest.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)      628 2022-06-16 12:20:02.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_data_checks.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     9169 2022-06-17 09:34:29.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_data_commands.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1939 2022-07-01 14:02:26.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_general_checks.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     3883 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_parameter_checks.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     4711 2022-06-28 11:41:19.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_run_commands.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5350 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/test/managment/test_managment_wflow_checks.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/test/renku_commands/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5111 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/test/renku_commands/test_renku_commands_datasets.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark/test/utils/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1330 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/test/utils/conftest.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)    12583 2022-07-19 14:00:29.000000 omnibenchmark-0.0.9/omnibenchmark/test/utils/test_build_omni_object.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     2636 2022-03-22 09:31:28.000000 omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_command.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     4733 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_input.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)    12339 2022-07-19 14:16:45.000000 omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_output.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5797 2022-05-09 07:58:02.000000 omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_run.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.331738 omnibenchmark-0.0.9/omnibenchmark/utils/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     3617 2022-05-06 20:02:23.000000 omnibenchmark-0.0.9/omnibenchmark/utils/auto_command.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5830 2022-07-22 09:37:57.000000 omnibenchmark-0.0.9/omnibenchmark/utils/auto_input.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     9498 2022-07-19 12:46:20.000000 omnibenchmark-0.0.9/omnibenchmark/utils/auto_output.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     3735 2022-05-16 14:04:16.000000 omnibenchmark-0.0.9/omnibenchmark/utils/auto_run.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     9777 2022-06-20 12:06:26.000000 omnibenchmark-0.0.9/omnibenchmark/utils/build_omni_object.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1575 2022-05-16 09:51:57.000000 omnibenchmark-0.0.9/omnibenchmark/utils/context_manager.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1425 2022-04-11 14:18:34.000000 omnibenchmark-0.0.9/omnibenchmark/utils/decorators.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)      545 2022-07-01 15:08:30.000000 omnibenchmark-0.0.9/omnibenchmark/utils/default_global_vars.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1333 2022-06-21 15:43:44.000000 omnibenchmark-0.0.9/omnibenchmark/utils/exceptions.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     3336 2022-04-26 17:44:09.000000 omnibenchmark-0.0.9/omnibenchmark/utils/log.py
+-rw-rw-r--   0 almut     (1000) almut     (1000)     2546 2022-07-19 14:08:00.000000 omnibenchmark-0.0.9/omnibenchmark/utils/user_input_checks.py
+drwxrwxr-x   0 almut     (1000) almut     (1000)        0 2022-07-22 09:41:13.327738 omnibenchmark-0.0.9/omnibenchmark.egg-info/
+-rw-rw-r--   0 almut     (1000) almut     (1000)     5226 2022-07-22 09:41:13.000000 omnibenchmark-0.0.9/omnibenchmark.egg-info/PKG-INFO
+-rw-rw-r--   0 almut     (1000) almut     (1000)     2242 2022-07-22 09:41:13.000000 omnibenchmark-0.0.9/omnibenchmark.egg-info/SOURCES.txt
+-rw-rw-r--   0 almut     (1000) almut     (1000)        1 2022-07-22 09:41:13.000000 omnibenchmark-0.0.9/omnibenchmark.egg-info/dependency_links.txt
+-rw-rw-r--   0 almut     (1000) almut     (1000)      112 2022-07-22 09:41:13.000000 omnibenchmark-0.0.9/omnibenchmark.egg-info/requires.txt
+-rw-rw-r--   0 almut     (1000) almut     (1000)       14 2022-07-22 09:41:13.000000 omnibenchmark-0.0.9/omnibenchmark.egg-info/top_level.txt
+-rw-rw-r--   0 almut     (1000) almut     (1000)     1420 2022-07-22 09:40:57.000000 omnibenchmark-0.0.9/pyproject.toml
+-rw-rw-r--   0 almut     (1000) almut     (1000)       38 2022-07-22 09:41:13.331738 omnibenchmark-0.0.9/setup.cfg
+-rw-rw-r--   0 almut     (1000) almut     (1000)       38 2022-07-11 13:48:17.000000 omnibenchmark-0.0.9/setup.py
```

### Comparing `omnibenchmark-0.0.8/LICENSE` & `omnibenchmark-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/PKG-INFO` & `omnibenchmark-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnibenchmark
-Version: 0.0.8
+Version: 0.0.9
 Summary: Omnibenchmark core utilities: Setup and running of continous benchmarking modules as part of omnibenchmark
 Author-email: Almut Lütge <almut.lue@gmail.com>
 Project-URL: Homepage, https://omnibenchmark.pages.uzh.ch/omni_dash
 Project-URL: Code, https://github.com/almutlue/omnibenchmark-py
 Project-URL: Bug Tracker, https://github.com/almutlue/omnibenchmark-py/issues
 Project-URL: Documentation, https://omnibenchmark.readthedocs.io
 Keywords: benchmark,omnibenchmark,renku
@@ -122,15 +122,17 @@
 
 #### OmniPlan
 
 ### Submit your module
 
 
 ## Release History
-
+* 0.0.9
+    * FIX:
+    * add common sequence to auto file matching  
 * 0.0.8
     * FIX:
     * add update command to omni_obj.update_object()  
 * 0.0.4 - 0.0.7
     * FIX:
     * convert defaults to string to generate plan 
     * adapt output default
```

### Comparing `omnibenchmark-0.0.8/README.md` & `omnibenchmark-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,17 @@
 
 #### OmniPlan
 
 ### Submit your module
 
 
 ## Release History
-
+* 0.0.9
+    * FIX:
+    * add common sequence to auto file matching  
 * 0.0.8
     * FIX:
     * add update command to omni_obj.update_object()  
 * 0.0.4 - 0.0.7
     * FIX:
     * convert defaults to string to generate plan 
     * adapt output default
```

### Comparing `omnibenchmark-0.0.8/omnibenchmark/core/input_classes.py` & `omnibenchmark-0.0.9/omnibenchmark/core/input_classes.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/core/omni_object.py` & `omnibenchmark-0.0.9/omnibenchmark/core/omni_object.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/core/output_classes.py` & `omnibenchmark-0.0.9/omnibenchmark/core/output_classes.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/management/data_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/management/data_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/management/data_commands.py` & `omnibenchmark-0.0.9/omnibenchmark/management/data_commands.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/management/general_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/management/general_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/management/parameter_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/management/parameter_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/management/run_commands.py` & `omnibenchmark-0.0.9/omnibenchmark/management/run_commands.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/management/wflow_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/management/wflow_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/renku_commands/datasets.py` & `omnibenchmark-0.0.9/omnibenchmark/renku_commands/datasets.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/renku_commands/general.py` & `omnibenchmark-0.0.9/omnibenchmark/renku_commands/general.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/renku_commands/workflows.py` & `omnibenchmark-0.0.9/omnibenchmark/renku_commands/workflows.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/conftest.py` & `omnibenchmark-0.0.9/omnibenchmark/test/conftest.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_command.py` & `omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_command.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_input.py` & `omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_input.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_output.py` & `omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_output.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/core/test_core_omni_parameter.py` & `omnibenchmark-0.0.9/omnibenchmark/test/core/test_core_omni_parameter.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_data_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_data_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_data_commands.py` & `omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_data_commands.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_general_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_general_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_parameter_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_parameter_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/managment/test_management_run_commands.py` & `omnibenchmark-0.0.9/omnibenchmark/test/managment/test_management_run_commands.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/managment/test_managment_wflow_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/test/managment/test_managment_wflow_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/renku_commands/test_renku_commands_datasets.py` & `omnibenchmark-0.0.9/omnibenchmark/test/renku_commands/test_renku_commands_datasets.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/utils/conftest.py` & `omnibenchmark-0.0.9/omnibenchmark/test/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/utils/test_build_omni_object.py` & `omnibenchmark-0.0.9/omnibenchmark/test/utils/test_build_omni_object.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_command.py` & `omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_command.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_input.py` & `omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_input.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_output.py` & `omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_output.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/test/utils/test_utils_auto_run.py` & `omnibenchmark-0.0.9/omnibenchmark/test/utils/test_utils_auto_run.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/auto_command.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/auto_command.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/auto_input.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/auto_input.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,52 @@
 from omnibenchmark.utils.exceptions import ParameterError
 from renku.ui.api.models.dataset import Dataset
 from difflib import SequenceMatcher
 import re
 import os
 import json
 
+def find_stem(arr):
+    n = len(arr)
+    # Take first word from array
+    # as reference
+    s = arr[0]
+    l = len(s)
+    res = ""
+    for i in range(l):
+        for j in range(i + 1, l + 1):
+ 
+            # generating all possible substrings
+            # of our reference string arr[0] i.e s
+            stem = s[i:j]
+            k = 1
+            for k in range(1, n):
+ 
+                # Check if the generated stem is
+                # common to all words
+                if stem not in arr[k]:
+                    break
+ 
+            # If current substring is present in
+            # all strings and its length is greater
+            # than current result
+            if (k + 1 == n and len(res) < len(stem)):
+                res = stem
+ 
+    return res
+
+
+def best_match_name_seq(map_dict: Mapping[str, str]) -> str:
+    na_list = [os.path.basename(fi_nam) for fi_nam in map_dict.values()]
+    nam_list = [os.path.splitext(nam)[0] for nam in na_list]
+    name_list = [os.path.splitext(nam)[0] for nam in nam_list]
+    com_sub = find_stem(name_list)
+    return com_sub
+    
+
 def match_files_by_name(file_type_dict: Mapping[str, List[str]]) -> Mapping[str, Mapping]:
     match_dict: Dict = {}
     fi_types = list(file_type_dict.keys())
     fi_start = fi_types[0]
     fil_types = [fi_type for fi_type in fi_types if not fi_type == fi_start]
     for fi_idx, fi in enumerate(file_type_dict[fi_start]):
         group_nam = "inst" + str(fi_idx)
@@ -22,15 +60,16 @@
             for fi_path in file_type_dict[fi_type]:
                 fi_name = os.path.basename(fi_path)
                 seq_match = SequenceMatcher(None, os.path.basename(fi), fi_name).ratio()
                 if seq_match > seq_top:
                     seq_top = seq_match
                     fi_top = fi_path
             match_dict[group_nam][fi_type] = fi_top
-    return(match_dict)
+    com_dict = {m_key + "_" + best_match_name_seq(match_dict[m_key]): match_dict[m_key] for m_key in match_dict.keys()}
+    return(com_dict)
 
 
 def get_input_files_from_prefix(
     input_prefix: Mapping[str, List[str]], keyword: List[str]
 ) -> Mapping[str, Mapping]:
     input_files: Dict = {}
     datasets = Dataset.list()
```

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/auto_output.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/auto_output.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/auto_run.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/auto_run.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/build_omni_object.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/build_omni_object.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/context_manager.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/context_manager.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/decorators.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/default_global_vars.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/default_global_vars.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/exceptions.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/log.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/log.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark/utils/user_input_checks.py` & `omnibenchmark-0.0.9/omnibenchmark/utils/user_input_checks.py`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/omnibenchmark.egg-info/PKG-INFO` & `omnibenchmark-0.0.9/omnibenchmark.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnibenchmark
-Version: 0.0.8
+Version: 0.0.9
 Summary: Omnibenchmark core utilities: Setup and running of continous benchmarking modules as part of omnibenchmark
 Author-email: Almut Lütge <almut.lue@gmail.com>
 Project-URL: Homepage, https://omnibenchmark.pages.uzh.ch/omni_dash
 Project-URL: Code, https://github.com/almutlue/omnibenchmark-py
 Project-URL: Bug Tracker, https://github.com/almutlue/omnibenchmark-py/issues
 Project-URL: Documentation, https://omnibenchmark.readthedocs.io
 Keywords: benchmark,omnibenchmark,renku
@@ -122,15 +122,17 @@
 
 #### OmniPlan
 
 ### Submit your module
 
 
 ## Release History
-
+* 0.0.9
+    * FIX:
+    * add common sequence to auto file matching  
 * 0.0.8
     * FIX:
     * add update command to omni_obj.update_object()  
 * 0.0.4 - 0.0.7
     * FIX:
     * convert defaults to string to generate plan 
     * adapt output default
```

### Comparing `omnibenchmark-0.0.8/omnibenchmark.egg-info/SOURCES.txt` & `omnibenchmark-0.0.9/omnibenchmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omnibenchmark-0.0.8/pyproject.toml` & `omnibenchmark-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omnibenchmark"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Almut Lütge", email="almut.lue@gmail.com" },
 ]
 description = "Omnibenchmark core utilities: Setup and running of continous benchmarking modules as part of omnibenchmark"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -35,15 +35,15 @@
 [project.urls]
 "Homepage" = "https://omnibenchmark.pages.uzh.ch/omni_dash"
 "Code" = "https://github.com/almutlue/omnibenchmark-py"
 "Bug Tracker" = "https://github.com/almutlue/omnibenchmark-py/issues"
 "Documentation" = "https://omnibenchmark.readthedocs.io"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```


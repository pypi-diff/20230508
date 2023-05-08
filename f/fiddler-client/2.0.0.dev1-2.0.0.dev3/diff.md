# Comparing `tmp/fiddler-client-2.0.0.dev1.tar.gz` & `tmp/fiddler-client-2.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-2.0.0.dev1.tar", last modified: Fri Apr 21 22:06:20 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev3.tar", last modified: Mon May  8 21:17:31 2023, max compression
```

## Comparing `fiddler-client-2.0.0.dev1.tar` & `fiddler-client-2.0.0.dev3.tar`

### file list

```diff
@@ -1,99 +1,97 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    19014 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    15514 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)    31118 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-04-21 22:06:14.000000 fiddler-client-2.0.0.dev1/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/api/monitoring.py
--rw-r--r--   0 runner    (1000) docker    (1001)    12340 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/api/publish_event.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/aws_utils.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21386 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   134153 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/experimental.py
--rw-r--r--   0 runner    (1000) docker    (1001)    42915 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5149 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7444 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/model_info_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/monitoring_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/template_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/project.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/logging.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5734 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/pandas.py
--rw-r--r--   0 runner    (1000) docker    (1001)    19454 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v1_v2_compat.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2063 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16074 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14721 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15444 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14627 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/project_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1324 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/constants.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4600 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5948 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/common.py
--rw-r--r--   0 runner    (1000) docker    (1001)      640 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2283 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1527 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/validators/dataset_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    19014 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2317 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      217 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1400 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1757 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/tests/test_fiddler_api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3721 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/tests/test_v1_v2_compat.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    19268 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    15712 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)    30845 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/api/monitoring.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/aws_utils.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21386 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/connection.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   128650 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/experimental.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    26153 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5149 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7444 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/model_info_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/monitoring_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/template_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/project.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/logging.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4996 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/pandas.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    18490 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v1_v2_compat.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/v2/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2063 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15065 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14721 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15444 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14627 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/project_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1203 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/constants.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/v2/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4600 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3135 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/fiddler/v2/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2283 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/fiddler/v2/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1523 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/validators/dataset_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    19268 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2260 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      212 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1395 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1757 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/tests/test_fiddler_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3721 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/tests/test_v1_v2_compat.py
```

### Comparing `fiddler-client-2.0.0.dev1/PKG-INFO` & `fiddler-client-2.0.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev1
+Version: 2.0.0.dev3
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -39,18 +39,25 @@
               - list_teams
               - list_project_roles
               - list_org_roles
               - unshare_project
               - share_project
               - process_avro
               - process_csv
+          - #### **New Features**
+            - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
+        
+        ### 1.8.0
           - #### **Modifications**
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
         
+        ### 1.7.1
+          - #### **Modification**
+            - Relaxed boto3 version constraint
         
         ### 1.7.0
           - #### **Removed**
             - Remove support for initializing fiddler client with version=1
             - Following methods are removed
               - get_segment_info
               - delete_segment
@@ -60,15 +67,15 @@
               - upload_segment
               - add_monitoring_config
               - publish_parquet_s3
               - publish_events_log
         
         ### 1.6.2
           - #### **Modifications**
-            - Made dataset_id a required field in add_model()
+            - Make dataset_id a required field in add_model()
             - Update max_inferred_cardinality to 100
           - #### **New Features**
             - New method for updating a model artifact `update_model_artifact`
         
         ### 1.5.3
           - #### **Modifications**
             - Fix add_model_artifact error for NLP models
```

### Comparing `fiddler-client-2.0.0.dev1/PUBLIC.md` & `fiddler-client-2.0.0.dev3/PUBLIC.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,25 @@
       - list_teams
       - list_project_roles
       - list_org_roles
       - unshare_project
       - share_project
       - process_avro
       - process_csv
+  - #### **New Features**
+    - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
+
+### 1.8.0
   - #### **Modifications**
     - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
       `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
 
+### 1.7.1
+  - #### **Modification**
+    - Relaxed boto3 version constraint
 
 ### 1.7.0
   - #### **Removed**
     - Remove support for initializing fiddler client with version=1
     - Following methods are removed
       - get_segment_info
       - delete_segment
@@ -53,15 +60,15 @@
       - upload_segment
       - add_monitoring_config
       - publish_parquet_s3
       - publish_events_log
 
 ### 1.6.2
   - #### **Modifications**
-    - Made dataset_id a required field in add_model()
+    - Make dataset_id a required field in add_model()
     - Update max_inferred_cardinality to 100
   - #### **New Features**
     - New method for updating a model artifact `update_model_artifact`
 
 ### 1.5.3
   - #### **Modifications**
     - Fix add_model_artifact error for NLP models
```

### Comparing `fiddler-client-2.0.0.dev1/README.md` & `fiddler-client-2.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/__init__.py` & `fiddler-client-2.0.0.dev3/fiddler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,42 +34,36 @@
     ArtifactStatus,
     BaselineType,
     BatchPublishType,
     Column,
     CustomFeature,
     DatasetInfo,
     DataType,
-    DeploymentOptions,
     DeploymentType,
     ExplanationMethod,
     FiddlerPublishSchema,
     FiddlerTimestamp,
-    MLFlowParams,
-    ModelDeploymentParams,
     ModelInfo,
     ModelInputType,
     ModelTask,
+    WeightingParams,
     WindowSize,
 )
 from .fiddler_api import FiddlerApi as FiddlerApiV1
 from .packtools import gem
 from .utils import ColorLogger
 from .v1_v2_compat import V1V2Compat
 from .v2.api.api import Client as FiddlerApiV2
 from .v2.api.explainability_mixin import (
     DatasetDataSource,
     RowDataSource,
     SqlSliceQueryDataSource,
 )
 from .v2.constants import (
     CSV_EXTENSION,
-    PARQUET_COMPRESSION,
-    PARQUET_ENGINE,
-    PARQUET_EXTENSION,
-    PARQUET_ROW_GROUP_SIZE,
     FileType,
 )
 from .v2.schema.job import JobStatus
 from .v2.schema.model_deployment import DeploymentParams, ModelDeployment
 from .v2.utils.exceptions import NotSupported
 from .v2.utils.helpers import match_semvar, raise_not_support
 from .validator import PackageValidator, ValidationChainSettings, ValidationModule
@@ -927,25 +921,20 @@
     'DatasetInfo',
     'DataType',
     'Fiddler',
     'FiddlerApi',
     'FiddlerTimestamp',
     'FiddlerPublishSchema',
     'gem',
-    'MLFlowParams',
-    'ModelDeploymentParams',
     'ModelInfo',
     'ModelInputType',
     'ModelTask',
+    'WeightingParams',
     'ExplanationMethod',
     'PredictionEventBundle',
     'PackageValidator',
     'ValidationChainSettings',
     'ValidationModule',
     'utils',
     # Exposing constants
     'CSV_EXTENSION',
-    'PARQUET_EXTENSION',
-    'PARQUET_ROW_GROUP_SIZE',
-    'PARQUET_ENGINE',
-    'PARQUET_COMPRESSION',
 ]
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/api/monitoring.py` & `fiddler-client-2.0.0.dev3/fiddler/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev3/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/aws_utils.py` & `fiddler-client-2.0.0.dev3/fiddler/aws_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/client.py` & `fiddler-client-2.0.0.dev3/fiddler/client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/connection.py` & `fiddler-client-2.0.0.dev3/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev3/fiddler/core_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     Union,
     cast,
 )
 
 import numpy as np
 import pandas as pd
 import pandas.api.types
-import pyarrow as pa
 from deprecated import deprecated
 
 from ._version import __version__
 from .utils.exceptions import MalformedSchemaException
 from .utils.formatting import prettyprint_number, validate_sanitized_names
 from .utils.general_checks import (
     is_greater_than_max_value,
@@ -46,15 +45,18 @@
 # default for DatasetInfo.data_type_version and ModelInfo.data_type_version
 # Introduced to bypass certain data type conversion functions
 # from both client and server.
 # More details https://fiddlerlabs.atlassian.net/wiki/spaces/FL/pages/1973617158/Introducing+Version+in+DatasetInfo+and+ModelInfo
 
 # v0 means variable is just defined, no change in any logic.
 # v0 is launched in python-client release 1.7.0
-CURRENT_DATA_TYPE_VERSION: str = 'v0'
+
+# v1 ignores typecasting of possible_values of categorical data type
+# v1 is launched in python-client release 2.0.0
+CURRENT_DATA_TYPE_VERSION: str = 'v1'
 
 LOG = logging.getLogger(__name__)
 
 
 class IntegrityViolationStatus(NamedTuple):
     is_nullable_violation: bool
     is_type_violation: bool
@@ -360,75 +362,14 @@
             explanations={
                 label_class: AttributionExplanation.from_dict(explanation_dict)
                 for label_class, explanation_dict in deserialized_json.items()
             },
         )
 
 
-class MLFlowParams:
-    """Holds the configuration information for a model packaged as an MLFlow
-    model."""
-
-    def __init__(
-        self,
-        relative_path_to_saved_model: Union[str, Path],
-        live_endpoint: Optional[str] = None,
-    ):
-        self.relative_path_to_saved_model = Path(relative_path_to_saved_model)
-        self.live_endpoint = live_endpoint
-
-    @classmethod
-    def from_dict(cls, d):
-        return cls(d['relative_path_to_saved_model'], d.get('live_endpoint', None))
-
-    def to_dict(self):
-        res = {
-            'relative_path_to_saved_model': str(self.relative_path_to_saved_model),
-        }
-        if self.live_endpoint is not None:
-            res['live_endpoint'] = self.live_endpoint
-        return res
-
-
-class ModelDeploymentParams:
-    """Holds configuration information for a model packaged as a container."""
-
-    def __init__(
-        self,
-        image: str,
-    ):
-        self.image = image
-
-    @classmethod
-    def from_dict(cls, d):
-        return cls(d['image'])
-
-    def to_dict(self):
-        res = {
-            'image': str(self.image),
-        }
-        return res
-
-
-@dataclass
-class DeploymentOptions:
-    deployment_type: str = DeploymentType.SURROGATE
-    image: str = None  # image to be used for newly uploaded model
-    namespace: Optional[str] = None  # kubernetes namespace
-    port: int = 5100  # port on which model is served
-    replicas: int = 1  # number of replicas
-    cpus: float = 0.25  # number of CPU cores
-    memory: str = '128m'  # amount of memory required.
-    gpus: int = 0  # number of GPU cores
-    await_deployment: bool = True  # wait for deployment
-
-    def to_dict(self):
-        return asdict(self)
-
-
 @dataclass
 class CustomFeature:
     """A class used to define custom features such as complex/vector features
 
     :param name: The name of the custom feature as it will appear in the monitoring tab.
     :param columns: The name of the data column(s) that constitute the custom feature.
     :param transformation: The transformation method applied on the original data.
@@ -582,16 +523,16 @@
 
     def __init__(
         self,
         name: str,
         data_type: DataType,
         possible_values: Optional[List[Any]] = None,
         is_nullable: Optional[bool] = None,
-        value_range_min: Optional[float] = None,
-        value_range_max: Optional[float] = None,
+        value_range_min: Optional[Union[int, float]] = None,
+        value_range_max: Optional[Union[int, float]] = None,
     ):
         self.name = name
         self.data_type = data_type
         self.possible_values = possible_values
         self.is_nullable = is_nullable
         self.value_range_min = value_range_min
         self.value_range_max = value_range_max
@@ -653,34 +594,14 @@
         # Commenting to allow none possible values.
         # self._raise_on_bad_categorical()
 
         if self.data_type.value == DataType.CATEGORY.value:
             return pandas.api.types.CategoricalDtype(self.possible_values)
         return self.data_type.value
 
-    def get_arrow_field(self) -> pa.Field:
-        """Converts the data_type field to a pyarrow field"""
-
-        if self.data_type == DataType.CATEGORY:
-            field_type = pa.dictionary(index_type=pa.int64(), value_type=pa.string())
-        elif self.data_type == DataType.INTEGER:
-            field_type = pa.int64()
-        elif self.data_type == DataType.FLOAT:
-            field_type = pa.float64()
-        elif self.data_type == DataType.BOOLEAN:
-            field_type = pa.bool_()
-        elif self.data_type == DataType.STRING:
-            field_type = pa.string()
-        else:
-            raise ValueError(
-                f'Not able to map data type to arrow field - {self.data_type}'
-            )
-
-        return pa.field(self.name, field_type)
-
     def to_dict(self) -> Dict[str, Any]:
         """Converts this object to a more JSON-friendly form."""
         res = {
             'column-name': self.name,
             'data-type': self.data_type.value,
         }
         if self.possible_values is not None:
@@ -691,70 +612,14 @@
             res['is-nullable'] = self.is_nullable
         if self.value_range_min is not None:
             res['value-range-min'] = self.value_range_min
         if self.value_range_max is not None:
             res['value-range-max'] = self.value_range_max
         return res
 
-    @deprecated(reason='Moved to data_type module in fiddler repo')
-    def violation_of_value(self, value):
-        if Column._value_is_na_or_none(value):
-            return False
-        if self.data_type.is_numeric():
-            is_too_low = self.value_range_min is not None and is_less_than_min_value(
-                value, self.value_range_min
-            )
-            is_too_high = (
-                self.value_range_max is not None
-                and is_greater_than_max_value(value, self.value_range_max)
-            )
-            return is_too_low or is_too_high
-        if self.data_type.value in [DataType.CATEGORY.value, DataType.BOOLEAN.value]:
-            return value not in self.possible_values
-        return False
-
-    @deprecated(reason='Moved to data_type module in fiddler repo')
-    def violation_of_type(self, value):
-        if Column._value_is_na_or_none(value):
-            return False
-        if self.data_type.value == DataType.FLOAT.value:
-            # json loading from string reads non-decimal number always as int
-            return not (isinstance(value, float) or isinstance(value, int))
-        if self.data_type.value == DataType.INTEGER.value:
-            # pandas converts int columns to float columns, will further cause backend to flag it as type violation
-            # e.g: "2" is casted as "2.0" by pandas. And "2.0" will be flagged as type violation. typeof(2.0) != INT
-            if isinstance(value, float):
-                if int(value) == value:
-                    value = int(value)
-            return not isinstance(value, int) and not pandas.api.types.is_int64_dtype(
-                value
-            )
-        if self.data_type.value == DataType.STRING.value:
-            return not isinstance(value, str)
-        if self.data_type.value == DataType.BOOLEAN.value:
-            return not isinstance(value, bool) and value not in (0, 1)
-        if self.data_type.value == DataType.CATEGORY.value:
-            possible_types = tuple(set(type(v) for v in self.possible_values))
-            return not isinstance(value, possible_types)
-
-    @deprecated(reason='Moved to data_type module in fiddler repo')
-    def violation_of_nullable(self, value):
-        if self.is_nullable is not None and self.is_nullable is False:
-            return Column._value_is_na_or_none(value)
-        return False
-
-    @deprecated(reason='Moved to data_type module in fiddler repo')
-    def check_violation(self, value):
-        if self.violation_of_nullable(value):
-            return IntegrityViolationStatus(True, False, False)
-        if self.violation_of_type(value):
-            return IntegrityViolationStatus(False, True, False)
-        if self.violation_of_value(value):
-            return IntegrityViolationStatus(False, False, True)
-        return IntegrityViolationStatus(False, False, False)
 
     @staticmethod
     def _value_is_na_or_none(value):
         if value is None:
             return True
         # This needs to be added because when we add `pandas._libs.missing.NAType` type in rabbitmq.
         # When we read the message, it converts the value to the "<NA>".
@@ -859,50 +724,24 @@
         dtypes = {}
 
         for column in self.columns:
             dtypes[column.name] = column.get_pandas_dtype()
 
         return dtypes
 
-    def get_arrow_schema(self) -> pa.Schema:
-        """
-        Convert dataset info columns data types to pyarrow compatible schema
-        :return: pyarrow compatible schema
-        """
-
-        fields = []
-
-        for column in self.columns:
-            fields.append(column.get_arrow_field())
-
-        return pa.schema(fields)
-
     def get_column_names(self) -> List[str]:
         """Returns a list of column names."""
         return [column.name for column in self.columns]
 
     def get_column_pandas_dtypes(
         self,
     ) -> Dict[str, Union[str, pandas.api.types.CategoricalDtype]]:
         """Get a dictionary describing the pandas datatype of every column."""
         return _get_field_pandas_dtypes(self.columns)
 
-    def get_event_integrity(
-        self, event: Dict[str, Union[str, float, int, bool]]
-    ) -> Tuple[IntegrityViolationStatus, ...]:
-        if not set(event.keys()).issuperset(set(self.get_column_names())):
-            raise ValueError(
-                f'Event feature names {set(event.keys())} not'
-                f'a superset of column names '
-                f'{set(self.get_column_names())}'
-            )
-        return tuple(
-            column.check_violation(event[column.name]) for column in self.columns
-        )
-
     @staticmethod
     def _datatype_check(columns):
         """
         # loop through all columns
         # if the column datatype is numpy datatype, transform to python type
         """
         for column in columns:
@@ -1038,86 +877,104 @@
         columns = []
         if df.index.name is not None:
             # add index column if it is not just an unnamed RangeIndex
             df = df.reset_index(inplace=False)
         name_series_iter = df.items()
         for column_name, column_series in name_series_iter:
             column_info = cls._calculate_stats_for_col(
-                column_name, column_series, max_inferred_cardinality
+                column_name,
+                column_series,
+                max_inferred_cardinality,
+                data_type_version=CURRENT_DATA_TYPE_VERSION
             )
             columns.append(column_info)
         return cls(
             display_name,
             columns,
             dataset_id=dataset_id,
             data_type_version=CURRENT_DATA_TYPE_VERSION,
         )
 
     @staticmethod
-    def _calculate_stats_for_col(column_name, column_series, max_inferred_cardinality):
+    def _calculate_stats_for_col(
+        column_name,
+        column_series,
+        max_inferred_cardinality,
+        data_type_version:Optional[str]='v0'):
         # @TODO Automatically drop the empty column with warning and proceed instead of aborting the upload
         if column_series.isna().all():
             raise ValueError(
                 f'Column {column_name} is empty. '
                 f'Please remove it and re-upload the dataset.'
             )
 
         # if we infer string or categorical, ensure that the underlying data
         # is also string by casting it.
+
+        # FDL-10905: dropna is needed to take care of cases where having None changes
+        # data type of int, float, bool to category. dropna() won't change
+        # is_nullable detection as column_series.dropna() returns a new instance.
+        column_series_dropped_na = column_series.dropna()
         column_dtype = DatasetInfo.datatype_from_pandas_dtype(
-            column_series.infer_objects().dtype
+            column_series_dropped_na.infer_objects().dtype
         )
+        # get nullability before any datatype modifications like 'astype'
+        # which distorts None values.
+        is_nullable = bool(column_series.isna().any())
+
         if column_dtype in [DataType.CATEGORY, DataType.STRING]:
             if 'mixed' in pd.api.types.infer_dtype(column_series):
                 LOG.warning(
                     '***********************************\n'
                     'WARNING: The column passed has mixed datatypes.\n'
                     ' We have casted the column to string to ensure smooth functionality.\n'
                     '***********************************'
                 )
-            column_series = column_series.astype(str)
 
         # infer categorical if configured to do so
         if (
             max_inferred_cardinality
             and column_dtype.value == DataType.STRING.value
             and not is_datetime(column_series)
-            and column_series.nunique() <= max_inferred_cardinality
+            and column_series_dropped_na.nunique() <= max_inferred_cardinality
         ):
             column_dtype = DataType.CATEGORY
 
         # get possible values for categorical type
-        if column_dtype.value in [DataType.CATEGORY.value, DataType.BOOLEAN.value]:
-            possible_values = np.sort(column_series.dropna().unique()).tolist()
-            possible_values_floats = None
-            if column_dtype.value == DataType.CATEGORY.value:
-                try:
-                    possible_values_floats = [
-                        str(float(raw_val)) for raw_val in possible_values
-                    ]
-                except ValueError:
-                    pass
-            if possible_values_floats is not None:
-                possible_values = possible_values_floats
+        if column_dtype.is_bool_or_cat():
+            # Only when data_type_version is 'v0',
+            # categorical column values undergo int/bool -> float -> string conversion.
+            if data_type_version == 'v0':
+                possible_values = np.sort(column_series_dropped_na.astype(str).unique()).tolist()
+                possible_values_floats = None
+                if column_dtype.value == DataType.CATEGORY.value:
+                    try:
+                        possible_values_floats = [
+                            str(float(raw_val)) for raw_val in possible_values
+                        ]
+                    except ValueError:
+                        pass
+                if possible_values_floats is not None:
+                    possible_values = possible_values_floats
+            else:
+                possible_values = np.sort(column_series_dropped_na.unique()).tolist()
         else:
             possible_values = None
 
         # get value range for numerical dtype
         if column_dtype.is_numeric():
             # these are saved as series members.
             value_min, value_max = column_series.min(), column_series.max()
             if np.isnan(value_min):
                 value_min = None
             if np.isnan(value_max):
                 value_max = None
         else:
             value_min, value_max = None, None
 
-        # get nullability
-        is_nullable = bool(column_series.isna().any())
         return Column(
             name=column_name,
             data_type=column_dtype,
             possible_values=possible_values,
             is_nullable=is_nullable,
             value_range_min=value_min,
             value_range_max=value_max,
@@ -1318,22 +1175,15 @@
     :param algorithm: A string providing information about the model type.
     :param framework: A string providing information about the software library
         and version used to train and run this model.
     :param description: A user-facing description of the model.
     :param datasets: A list of dataset names assocated with this model.
     :param weighting_params: [Optional] Weighting parameters to account for class-imbalance. These parameters
         will be used to generate reference and production histograms.
-    :param mlflow_params: [Deprecated in 1.7.0 and will be removed from 2.0.0 version.]
-    MLFlow parameters.
-    :param model_deployment_params: [Deprecated in 1.7.0 and will be removed from 2.0.0 version.]
-    Model Deployment parameters.
-    :param artifact_status: [Deprecated in 1.7.0 and will be removed from 2.0.0 version.]
-    Status of the model artifact
-    :param preferred_explanation_method: [Deprecated in 1.7.0 and will be removed from 2.0.0 version.]
-    [Optional] Specifies a preference
+    :param preferred_explanation_method: [Optional] Specifies a preference
         for the default explanation algorithm.  Front-end will choose
         explanation method if unspecified (typically Fiddler Shapley).
         Must be one of the built-in explanation types (ie an `fdl.core_objects.ExplanationMethod`) or be specified as
         a custom explanation type via `custom_explanation_names` (and in `package.py`).
     :param custom_explanation_names:
     [Optional] List of (string) names that
         can be passed to the explanation_name argument of the optional
@@ -1358,25 +1208,23 @@
     def __init__(
         self,
         display_name: str,
         input_type: ModelInputType,
         model_task: ModelTask,
         inputs: List[Column],
         outputs: List[Column],
+        targets: List[Column],
         target_class_order: Optional[List] = None,
         metadata: Optional[List[Column]] = None,
         decisions: Optional[List[Column]] = None,
-        targets: Optional[List[Column]] = None,
         algorithm: Optional[str] = None,
         framework: Optional[str] = None,
         description: Optional[str] = None,
         datasets: Optional[List[str]] = None,
         weighting_params: Optional[WeightingParams] = None,
-        mlflow_params: Optional[MLFlowParams] = None,
-        model_deployment_params: Optional[ModelDeploymentParams] = None,
         artifact_status: Optional[ArtifactStatus] = None,
         # TODO: smartly set default preferred_explanation_method (ie infer method here, instead of on BE/FE):
         preferred_explanation_method: Optional[str] = None,
         custom_explanation_names: Optional[List[str]] = None,
         binary_classification_threshold: Optional[float] = None,
         ranking_top_k: Optional[int] = None,
         group_by: Optional[str] = None,
@@ -1389,102 +1237,85 @@
         **kwargs,
     ):
         self.display_name = display_name
         self.input_type = input_type
         self.model_task = model_task
         self.inputs = inputs
         self.outputs = outputs
-        self.target_class_order = target_class_order
         self.targets = targets
+        self.target_class_order = target_class_order
         self.metadata = metadata
         self.decisions = decisions
         self.algorithm = algorithm
         self.framework = framework
         self.description = description
         self.datasets = datasets
         self.weighting_params = weighting_params
-        self.mlflow_params = mlflow_params
-        self.model_deployment_params = model_deployment_params
         self.artifact_status = artifact_status
         self.binary_classification_threshold = binary_classification_threshold
         self.ranking_top_k = ranking_top_k
         self.schema_version = CURRENT_MODELINFO_SCHEMA_VERSION
         self.custom_features = custom_features
         self.data_type_version = data_type_version
 
-        # warning for parameters deprecated in version 1.7
-        if mlflow_params is not None:
-            self.warn_deprecated_parameter(
-                param_name='mlflow_params', from_version='1.7'
-            )
-        if display_name is not None:
-            self.warn_deprecated_parameter(
-                param_name='display_name', from_version='1.7'
-            )
-        if model_deployment_params is not None:
-            self.warn_deprecated_parameter(
-                param_name='model_deployment_params', from_version='1.7'
-            )
+        self.is_binary_ranking_model = is_binary_ranking_model
+
+        self._validate_columns()
+
+        self.target_class_order = self.get_target_class_order(
+            self.target_class_order, self.model_task, self.targets[0])
+
+        if model_task == ModelTask.RANKING:
+            if group_by is None:
+                raise ValueError(
+                    'The argument group_by cannot be empty for Ranking models'
+                )
+            self.is_binary_ranking_model = len(self.target_class_order) == 2
+
+        self.group_by = group_by
 
         # artifact_status is set by Model Service
         # POST /v2/models sets  artifact_status to NO_MODEL
         # POST /v2/<model-id>/deploy-artifacts/... sets USER_UPLOADED
         # POST /v2/<model-id>/deploy-surrogate sets SURROGATE
         if artifact_status is not None:
             self.warn_deprecated_parameter(
                 param_name='artifact_status', from_version='1.7'
             )
 
         if custom_explanation_names is None:
             custom_explanation_names = []
 
-        self.is_binary_ranking_model = is_binary_ranking_model
-
-        self.target_class_order = self.get_target_class_order(self.target_class_order, self.model_task, self.targets[0])
-
-        if model_task == ModelTask.RANKING:
-            if group_by is None:
-                raise ValueError(
-                    'The argument group_by cannot be empty for Ranking models'
-                )
-            self.is_binary_ranking_model = len(self.target_class_order) == 2
-
-        self.group_by = group_by
-
         if tree_shap_enabled:
             custom_explanation_names.append('Tree Shap')
             if preferred_explanation_method is None:
                 preferred_explanation_method = 'Tree Shap'
 
         # we only store strings, not enums
         if isinstance(preferred_explanation_method, ExplanationMethod):
             preferred_explanation_method = preferred_explanation_method.value
 
         # Prevent the user from overloading a built-in.
-        if custom_explanation_names is not None:
-            duplicated_names = []
-            for name in custom_explanation_names:
-                if type(name) != str:
-                    raise ValueError(
-                        f'custom_explanation_names for ModelInfo must all be of '
-                        f"type 'str', but '{name}' is of type '{type(name)}'"
-                    )
-                if name in BUILT_IN_EXPLANATION_NAMES:
-                    duplicated_names.append(name)
-            if len(duplicated_names) > 0:
-                raise ValueError(
-                    f'Please select different names for your custom explanations. '
-                    f'The following are reserved built-ins duplicated in your custom '
-                    f'explanation names: {duplicated_names}.'
-                )
+        duplicated_names = []
+        for name in custom_explanation_names:
+            if type(name) != str:
+                raise ValueError(
+                    f'custom_explanation_names for ModelInfo must all be of '
+                    f"type 'str', but '{name}' is of type '{type(name)}'"
+                )
+            if name in BUILT_IN_EXPLANATION_NAMES:
+                duplicated_names.append(name)
+        if len(duplicated_names) > 0:
+            raise ValueError(
+                f'Please select different names for your custom explanations. '
+                f'The following are reserved built-ins duplicated in your custom '
+                f'explanation names: {duplicated_names}.'
+            )
 
         # Prevent the user from defaulting to an explanation that doesn't exist
-        assert (
-            custom_explanation_names is not None
-        ), 'custom_explanation_names is unexpectedly None'
         if (
             preferred_explanation_method is not None
             and preferred_explanation_method not in BUILT_IN_EXPLANATION_NAMES
             and preferred_explanation_method not in custom_explanation_names
         ):
             if len(custom_explanation_names) > 0:
                 raise ValueError(
@@ -1586,35 +1417,30 @@
         res = {
             'name': self.display_name,
             'input-type': self.input_type.value,
             'model-task': self.model_task.value,
             'inputs': [c.to_dict() for c in self.inputs],
             'outputs': [c.to_dict() for c in self.outputs],
             'datasets': self.datasets or [],
+            'targets': [target_col.to_dict() for target_col in self.targets]
         }
         if self.target_class_order is not None:
             res['target-class-order'] = self.target_class_order
         if self.metadata:
             res['metadata'] = [metadata_col.to_dict() for metadata_col in self.metadata]
         if self.decisions:
             res['decisions'] = [
                 decision_col.to_dict() for decision_col in self.decisions
             ]
-        if self.targets:
-            res['targets'] = [target_col.to_dict() for target_col in self.targets]
         if self.description is not None:
             res['description'] = self.description
         if self.algorithm is not None:
             res['algorithm'] = self.algorithm
         if self.framework is not None:
             res['framework'] = self.framework
-        if self.mlflow_params is not None:
-            res['mlflow'] = self.mlflow_params.to_dict()
-        if self.model_deployment_params is not None:
-            res['model_deployment'] = self.model_deployment_params.to_dict()
         if self.artifact_status is not None:
             res['artifact_status'] = self.artifact_status.value
         if self.preferred_explanation_method is not None:
             res['preferred-explanation-method'] = self.preferred_explanation_method
         if self.binary_classification_threshold is not None:
             res[
                 'binary_classification_threshold'
@@ -1694,24 +1520,14 @@
             tree_shap_enabled = deserialized_json.pop('tree_shap_enabled')
         else:
             tree_shap_enabled = False
 
         description = deserialized_json.pop('description', None)
         algorithm = deserialized_json.pop('algorithm', None)
         framework = deserialized_json.pop('framework', None)
-        mlflow_params: Optional[MLFlowParams] = None
-        if 'mlflow' in deserialized_json:
-            mlflow_params = MLFlowParams.from_dict(deserialized_json.pop('mlflow'))
-
-        model_deployment_params: Optional[ModelDeploymentParams] = None
-        if 'model_deployment' in deserialized_json:
-            model_deployment_params = ModelDeploymentParams.from_dict(
-                deserialized_json.pop('model_deployment')
-            )
-
         datasets: Optional[Any] = None
         if 'datasets' in deserialized_json:
             datasets = deserialized_json.pop('datasets')
 
         preferred_explanation_method: Optional[Any] = None
         if 'preferred-explanation-method' in deserialized_json:
             preferred_explanation_method = deserialized_json.pop(
@@ -1784,16 +1600,14 @@
             decisions=decisions,
             targets=targets,
             description=description,
             algorithm=algorithm,
             framework=framework,
             datasets=datasets,
             weighting_params=weighting_params,
-            mlflow_params=mlflow_params,
-            model_deployment_params=model_deployment_params,
             artifact_status=artifact_status,
             preferred_explanation_method=preferred_explanation_method,
             custom_explanation_names=custom_explanation_names,
             binary_classification_threshold=binary_classification_threshold,
             ranking_top_k=ranking_top_k,
             group_by=group_by,
             fall_back=fall_back,
@@ -1804,14 +1618,30 @@
             data_type_version=data_type_version,
             **deserialized_json,
         )
         # Explicitly set the version number
         model_info.schema_version = schema_version
         return model_info
 
+    def _validate_columns(self) -> None:
+        """
+        validate if required columns are provided in constructor and populate target_class_order
+        """
+        if not self.inputs:
+            raise ValueError('Model inputs not specified')
+
+        if not self.outputs:
+            raise ValueError('Model outputs not specified')
+
+        if not self.targets:
+            raise ValueError('Model targets not specified')
+
+        if not isinstance(self.targets, list) or len(self.targets) != 1:
+            raise ValueError('Model target must be a list of Column with length 1')
+
     @staticmethod
     def validate_missing_value_encodings(
         missing_value_encodings: dict, all_columns: List[Column]
     ) -> None:
         unmatched_col = []
         if not isinstance(missing_value_encodings, dict):
             raise ValueError(
@@ -1920,16 +1750,14 @@
         """Returns a list of names for model decisions."""
         if self.decisions is None:
             return []
         return [column.name for column in self.decisions]
 
     def get_target_names(self):
         """Returns a list of names for model targets."""
-        if self.targets is None:
-            return []
         return [column.name for column in self.targets]
 
     def get_input_pandas_dtypes(
         self,
     ) -> Dict[str, Union[str, pandas.api.types.CategoricalDtype]]:
         """Get a dictionary describing the pandas datatype of every input."""
         return _get_field_pandas_dtypes(self.inputs)
@@ -1959,22 +1787,33 @@
     def get_target_pandas_dtypes(
         self,
     ) -> Dict[str, Union[str, pandas.api.types.CategoricalDtype]]:
         """Get a dictionary describing the pandas datatype of every target."""
         assert self.targets is not None
         return _get_field_pandas_dtypes(self.targets)
 
-    def get_non_monitor_components(self):
-        ret = []
-        if self.custom_features is None:
-            return ret
+    def get_non_monitor_components(self) -> set:
+        """
+        return a set of column names which are part of custom_features but are not
+        monitored as individual features.
+        If a column is found in multiple custom_features with different monitor_components
+        value, True overwrites False and it is not a part of non-monitor-components
+        return an empty set if no custom_features
+        """
+        non_monitor = set()
+        if not self.custom_features:
+            return non_monitor
+        monitor = set()
         for cf in self.custom_features:
-            if not getattr(cf, 'monitor_components', False):
-                ret.extend(cf.columns)
-        return ret
+            if getattr(cf, 'monitor_components', False):
+                monitor.update(cf.columns)
+            else:
+                non_monitor.update(cf.columns)
+        non_monitor = non_monitor - monitor
+        return non_monitor
 
     @classmethod  # noqa: C901
     def from_dataset_info(
         cls,
         dataset_info: DatasetInfo,
         target: str,
         dataset_id: Optional[str] = None,
@@ -1988,15 +1827,14 @@
         algorithm: Optional[str] = None,
         framework: Optional[str] = None,
         input_type: ModelInputType = ModelInputType.TABULAR,
         model_task: Optional[ModelTask] = None,
         outputs: Optional[Any] = None,
         categorical_target_class_details: Optional[Any] = None,
         weighting_params: Optional[WeightingParams] = None,
-        model_deployment_params: Optional[ModelDeploymentParams] = None,
         preferred_explanation_method: Optional[str] = None,
         custom_explanation_names: Optional[List[str]] = None,
         binary_classification_threshold: Optional[float] = None,
         ranking_top_k: Optional[int] = None,
         group_by: Optional[str] = None,
         tree_shap_enabled: Optional[bool] = False,
         custom_features: Optional[List[CustomFeature]] = None,
@@ -2021,15 +1859,14 @@
         :param framework: A string providing information about the software library
             and version used to train and run this model.
         :param input_type: Specifies the paradigm (tabular or text) of the
             model.
         :param model_task: Specifies the prediction task addressed by the
             model. If not explicitly provided, this will be inferred from the
             data type of the target variable.
-        :param mlflow_params: MLFlow parameters.
         :param outputs: model output names, if multiclass classification, must be a sequence in the same order as categorical_target_class_details.
             If binary classification, must be a single name signifying the probability of the positive class. # TODO: bulletproofing
             If regression/ranking, must be a dictionary of the form {column_name: (min_value, max_value)}, or a
             dictionary with empty range {column_name:[]} if column_name can be found in the dataset
         :param categorical_target_class_details: specify the output categories of your model (only applicable for classification and ranking models)
             This parameter *must* be provided for multiclass, binary-classification and ranking models where
             the target is of type CATEGORY. It is optional for binary classification with BOOLEAN targets, and ignored for regression.
@@ -2053,15 +1890,14 @@
                 - by default the higher of the two possible values will be considered the positive class.
             In all other cases, one of the two classes will arbitrarily be FIXED as the positive class.
 
             For ranking models, provide a list of all the possible target values in order of relevance. The first element will be considered
             as not relevant, the last element from the list will be considered the most relevant grade.
         :param weighting_params: [Optional] Weighting parameters to account for class-imbalance. These parameters
             will be used to generate reference and production histograms.
-        :param model_deployment_params: Model Deployment parameters.
         :param preferred_explanation_method: [Optional] Specifies a preference
             for the default explanation algorithm.  Front-end will choose
             explanaton method if unspecified (typically Fiddler Shapley).
             Providing ExplanationMethod.CUSTOM will cause the first of the
             custom_explanation_names to be the default (which must be defined
             in that case).
         :param custom_explanation_names: [Optional] List of names that
@@ -2215,16 +2051,14 @@
             inputs=inputs,
             outputs=output_columns,
             target_class_order=target_class_order,
             metadata=metadata,
             decisions=decisions,
             targets=[target_column],
             weighting_params=weighting_params,
-            mlflow_params=None,
-            model_deployment_params=model_deployment_params,
             preferred_explanation_method=preferred_explanation_method,
             custom_explanation_names=custom_explanation_names,
             binary_classification_threshold=binary_classification_threshold,
             ranking_top_k=ranking_top_k,
             group_by=group_by,
             fall_back=fall_back,
             missing_value_encodings=missing_value_encodings,
@@ -2461,48 +2295,67 @@
         dataset_info: DatasetInfo,
         model_task: ModelTask,
     ) -> Optional[List[Column]]:
         if not output_names:
             return None
 
         output_columns = []
+        ds_info_names_columns = {}
+        for ds_column in dataset_info.columns:
+            ds_info_names_columns[ds_column.name] = ds_column
+
 
         if model_task.is_classification():
             if isinstance(output_names, dict):
                 output_names = list(output_names.keys())
             for name in output_names:
-                output_columns.append(
-                    Column(
-                        name=name,
-                        data_type=DataType.FLOAT,
-                        is_nullable=False,
-                        value_range_min=0.0,
-                        value_range_max=1.0,
+                if name in ds_info_names_columns:
+                    output_columns.append(ds_info_names_columns[name])
+                else:
+                    output_columns.append(
+                        Column(
+                            name=name,
+                            data_type=DataType.FLOAT,
+                            is_nullable=False,
+                            value_range_min=0.0,
+                            value_range_max=1.0,
+                        )
                     )
-                )
             return output_columns
 
         if isinstance(output_names, dict):
             for name in output_names.keys():
                 values = output_names[name]
                 if not isinstance(values, (list, tuple)) or len(values) != 2:
                     raise ValueError(
                         f'If outputs is a dictionary, the values should '
                         f'be a tuple of 2 values. Currently passing: '
                         f'{values} for output {name}. Please correct.'
                     )
-                output_columns.append(
-                    Column(
-                        name=name,
-                        data_type=DataType.FLOAT,
-                        is_nullable=False,
-                        value_range_min=float(min(values)),
-                        value_range_max=float(max(values)),
+                if name in ds_info_names_columns:
+                    column = ds_info_names_columns[name]
+                    if not (column.data_type == DataType.FLOAT or column.data_type == DataType.INTEGER):
+                        raise ValueError(
+                            f'Column {name} with type {column.data_type} can not be specified as output.'
+                            f'Output column type has to be either INTEGER or FLOAT.'
+                            f'Please correct.'
+                        )
+                    column.value_range_min = min(values)
+                    column.value_range_max = max(values)
+                    output_columns.append(column)
+                else:
+                    output_columns.append(
+                        Column(
+                            name=name,
+                            data_type=DataType.FLOAT,
+                            is_nullable=False,
+                            value_range_min=float(min(values)),
+                            value_range_max=float(max(values)),
+                        )
                     )
-                )
             return output_columns
 
         if isinstance(output_names, list):
             for name in output_names:
                 col = name
                 if name not in dataset_info.get_column_names():
                     if model_task.value == ModelTask.REGRESSION.value and target_column:
@@ -2510,14 +2363,19 @@
                         col = target_column.name
                     else:
                         raise ValueError(
                             f'Output {name} is not present in the dataset. '
                             f'Please provide a dictionary with the range: '
                             f'{name}: (min_value, max_value).'
                         )
+                if dataset_info[col].value_range_min is None or dataset_info[col].value_range_max is None:
+                    raise ValueError(
+                        f'Column {name} with value_range_min or value_range_max as None can not be specified as output.'
+                        f'Please correct.'
+                    )
                 output_columns.append(
                     Column(
                         name=name,
                         data_type=DataType.FLOAT,
                         is_nullable=False,
                         value_range_min=float(dataset_info[col].value_range_min),
                         value_range_max=float(dataset_info[col].value_range_max),
@@ -2742,15 +2600,15 @@
             if len(target_class_order) > 2:
                 raise ValueError(
                     'Target-class-order(categorical_target_class_details) cannot have '
                     f'more than 2 elements for model task {model_task}.'
                 )
 
             if len(target_class_order) == 2:
-                if not target_column.data_type.is_numeric() and set(
+                if target_column.data_type.is_bool_or_cat() and set(
                     target_column.possible_values
                 ) != set(target_class_order):
                     raise ValueError(
                         'Target-class-order(categorical_target_class_details) does not '
                         f'have the same elements as target column {target_column.name}'
                     )
                 return target_class_order
@@ -2807,19 +2665,14 @@
             else ''
         )
         custom_features = (
             f'<hr>custom features:{summary_dict["custom_features"]._repr_html_()}'
             if self.custom_features is not None
             else ''
         )
-        data_type_version_info = (
-            f'  data_type_version: {self.data_type_version}\n'
-            if self.data_type_version is not None
-            else ''
-        )
         return (
             f'<div style="border: thin solid rgb(41, 57, 141); padding: 10px;">'
             f'<h3 style="text-align: center; margin: auto;">ModelInfo\n</h3><pre>'
             f'  display_name: {self.display_name}\n'
             f'  description: {self.description}\n'
             f'  input_type: {self.input_type}\n'
             f'  model_task: {self.model_task}\n'
@@ -2833,15 +2686,14 @@
             f'  misc: {misc_info}</pre>'
             f'{target_info}'
             f"<hr>inputs:{summary_dict['inputs']._repr_html_()}"
             f"<hr>outputs:{summary_dict['outputs']._repr_html_()}"
             f'{custom_features}'
             f'{decisions_info}'
             f'{metadata_info}'
-            f'{data_type_version_info}'
             f'</div>'
         )
 
     def __repr__(self):
         summary_dict = ModelInfo.get_summary_dataframes_dict(self)
         input_info = textwrap.indent(repr(summary_dict['inputs']), '    ')
         output_info = textwrap.indent(repr(summary_dict['outputs']), '    ')
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/dataset.py` & `fiddler-client-2.0.0.dev3/fiddler/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/experimental.py` & `fiddler-client-2.0.0.dev3/fiddler/experimental.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/fiddler_api.py` & `fiddler-client-2.0.0.dev3/fiddler/fiddler_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 # TODO: Add License
-import copy
 import json
-import tempfile
-import textwrap
 from collections import namedtuple
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
 import pandas as pd
-import yaml
 from deprecated import deprecated
 
-from fiddler.api.publish_event import PublishEvent
 from fiddler.connection import Connection
 from fiddler.experimental import ExperimentalFeatures
 from fiddler.project import Project
 from fiddler.utils import logging
-from fiddler.v2.constants import (
-    CSV_EXTENSION,
-    PARQUET_EXTENSION,
-    SUPPORTABLE_FILE_EXTENSIONS,
-)
 
 from . import constants
 from .core_objects import (
-    BatchPublishType,
     DatasetInfo,
-    DataType,
-    DeploymentOptions,
-    DeploymentType,
     FiddlerTimestamp,
-    MLFlowParams,
     ModelInfo,
-    ModelTask,
     MonitoringViolation,
     MonitoringViolationType,
-    SegmentInfo,
 )
 from .monitoring_validator import MonitoringValidator
 from .utils import cast_input_data
 from .utils.general_checks import do_not_proceed, safe_name_check, type_enforce
-from .utils.pandas import df_size_exceeds, write_dataframe_to_parquet_file
+from .utils.pandas import df_size_exceeds
 
 LOG = logging.getLogger(__name__)
 
 SUCCESS_STATUS = Connection.SUCCESS_STATUS
 FAILURE_STATUS = Connection.FAILURE_STATUS
 FIDDLER_ARGS_KEY = Connection.FIDDLER_ARGS_KEY
 STREAMING_HEADER_KEY = Connection.STREAMING_HEADER_KEY
@@ -418,260 +401,14 @@
 
         LOG.info(f'Uploading the dataset {dataset_id} ...')
 
         result = self._call(path, json_payload=payload, files=file_paths)
 
         return result
 
-    def upload_dataset(
-        self,
-        project_id: str,
-        dataset: Dict[str, pd.DataFrame],
-        dataset_id: str,
-        info: Optional[DatasetInfo] = None,
-        size_check_enabled: bool = True,
-    ):
-        """Uploads a representative dataset to the Fiddler engine.
-
-        :param project_id: The unique identifier of the model's project on the
-            Fiddler engine.
-        :param dataset: A dictionary mapping name -> DataFrame
-            containing data to be uploaded to the Fiddler engine.
-        :param dataset_id: The unique identifier of the dataset on the Fiddler
-            engine. Must be a short string without whitespace.
-        :param info: A DatasetInfo object specifying all the details of the
-            dataset. If not provided, a DatasetInfo will be inferred from the
-            dataset and a warning raised.
-        :param size_check_enabled: Flag to enable the dataframe size check.
-            Default behavior is to raise a warning and present an interactive
-            dialogue if the size of the dataframes exceeds the default limit.
-            Set this flag to False to disable the checks.
-
-        :returns: The server response for the upload.
-        """
-        # Type enforcement
-        # @question: Shouldn't we just throw this as an error from server if we already don't do it?
-        project_id = type_enforce('project_id', project_id, str)
-        dataset_id = type_enforce('dataset_id', dataset_id, str)
-
-        assert (
-            ' ' not in dataset_id
-        ), 'The dataset identifier should not contain whitespace'
-        safe_name_check(dataset_id, constants.MAX_ID_LEN, self.strict_mode)
-
-        # get a dictionary of str -> pd.DataFrame for all data to upload
-        if not isinstance(dataset, dict):
-            raise ValueError('dataset must be a dictionary mapping name -> DataFrame')
-
-        # check if the dataset exceeds size limits
-        # @todo: why is checking for filesize even an option, shouldn't it be default?
-        abort_upload = self._abort_dataset_upload(
-            dataset, size_check_enabled, DATASET_MAX_ROWS
-        )
-        if abort_upload:
-            raise RuntimeError('Dataset upload aborted.')
-
-        if info:
-            # Since we started populating stats recently, some older yamls
-            # dont have it. Or the user might just supply us the basic
-            # schema without stats.
-            # If the user provided the schema/yaml file, ask the user to
-            # re-create dataset info with:
-            # info = DatasetInfo.update_stats_for_existing_schema(dataset,
-            # info, max_inferred_cardinality)
-            # @question: shouldn't these validations be part of DatasetInfo? (high cohesion) and we invoke the method here.
-            for column in info.columns:
-                if (
-                    (column.value_range_min is None) or (column.value_range_max is None)
-                ) and column.data_type.is_numeric():
-                    raise ValueError(
-                        f'Dataset info does not contain min/max values for the numeric feature {column.name}. '
-                        f'Please update using fdl.DatasetInfo.update_stats_for_existing_schema() '
-                        f'and upload dataset with the updated dataset info.'
-                    )
-                if (not column.possible_values) and (
-                    column.data_type.value
-                    in [DataType.CATEGORY.value, DataType.BOOLEAN.value]
-                ):
-                    raise ValueError(
-                        f'Dataset info does not contain possible values for the categorical feature {column.name}. '
-                        f'Please update using fdl.DatasetInfo.update_stats_for_existing_schema() '
-                        f'and upload dataset with the updated dataset info.'
-                    )
-
-            # Validate column names
-            for name, df in dataset.items():
-                for info_column in info.columns:
-                    if info_column.name not in df:
-                        raise RuntimeError(
-                            f'{info_column.name}({name}) column not found in the dataframe, '
-                            f'but passed in the info'
-                        )
-
-        # use inferred info with a warning if not `info` is passed
-        else:
-            inferred_info = DatasetInfo.from_dataframe(
-                df=dataset.values(),
-                display_name=dataset_id,
-                dataset_id=dataset_id,
-                max_inferred_cardinality=1000,
-            )
-            # @question: we only do validation when info is passed and not when it is inferred? Why should this be the case?
-            LOG.warning(
-                f'Heads up! We are inferring the details of your dataset from '
-                f'the dataframe(s) provided. Please take a second to check '
-                f'our work.'
-                f'\n\nIf the following DatasetInfo is an incorrect '
-                f'representation of your data, you can construct a '
-                f'DatasetInfo with the DatasetInfo.from_dataframe() method '
-                f'and modify that object to reflect the correct details of '
-                f'your dataset.'
-                f'\n\nAfter constructing a corrected DatasetInfo, please '
-                f're-upload your dataset with that DatasetInfo object '
-                f'explicitly passed via the `info` parameter of '
-                f'FiddlerApi.upload_dataset().'
-                f'\n\nYou may need to delete the initially uploaded version'
-                f"via FiddlerApi.delete_dataset('{dataset_id}')."
-                f'\n\nInferred DatasetInfo to check:'
-                f'\n{textwrap.indent(repr(inferred_info), "  ")}'
-            )
-            info = inferred_info
-
-        if self.strict_mode:
-            info.validate()
-
-        return self._upload_dataset_with_compression(
-            project_id=project_id,
-            dataset=dataset,
-            dataset_id=dataset_id,
-            dataset_info=info,
-        )
-
-    def upload_dataset_from_dir(
-        self,
-        project_id: str,
-        dataset_id: str,
-        dataset_dir: Path,
-        file_type: str = 'csv',
-        file_schema=None,
-        size_check_enabled: bool = False,
-    ):
-        # Type enforcement
-        project_id = type_enforce('project_id', project_id, str)
-        dataset_id = type_enforce('dataset_id', dataset_id, str)
-        dataset_dir = type_enforce('dataset_dir', dataset_dir, Path)
-
-        if f'.{file_type}' not in SUPPORTABLE_FILE_EXTENSIONS:
-            raise ValueError(
-                f'Invalid file_type :{file_type}. Valid file types are : '
-                f'{SUPPORTABLE_FILE_EXTENSIONS}'
-            )
-
-        if not dataset_dir.is_dir():
-            raise ValueError(f'{dataset_dir} is not a directory')
-
-        dataset_yaml = dataset_dir / f'{dataset_id}.yaml'
-
-        if not dataset_yaml.is_file():
-            raise ValueError(f'YAML file not found: {dataset_yaml}')
-
-        with dataset_yaml.open() as f:
-            dataset_info = DatasetInfo.from_dict(yaml.safe_load(f))
-
-        files = dataset_dir.glob('*.csv')
-        csv_files = [x for x in files if x.is_file()]
-
-        LOG.info(f'Found CSV file {csv_files}')
-
-        # Lets make sure that we add stats if they are not already there.
-        # We need to read the datasets in pandas and create a dataset dictionary
-        dataset = {}
-        csv_paths = []
-        for file in csv_files:
-            csv_name = str(file).split('/')[-1]
-            csv_paths.append(csv_name)
-            name = csv_name[:-4]
-
-            # @TODO Change the flow so that we can read the CSV in chunks
-            dataset[name] = pd.read_csv(file, dtype=dataset_info.get_pandas_dtypes())
-
-        # check if the dataset exceeds size limits
-        abort_upload = self._abort_dataset_upload(
-            dataset, size_check_enabled, DATASET_MAX_ROWS
-        )
-        if abort_upload:
-            raise RuntimeError('Dataset upload aborted.')
-
-        # Update stats
-        dataset_info = DatasetInfo.update_stats_for_existing_schema(
-            dataset, dataset_info
-        )
-        updated_infos = []
-        for item in dataset.values():
-            update_info = DatasetInfo.check_and_update_column_info(dataset_info, item)
-            updated_infos.append(update_info)
-
-        dataset_info = DatasetInfo.as_combination(
-            updated_infos, display_name=dataset_info.display_name
-        )
-
-        return self._upload_dataset_with_compression(
-            project_id=project_id,
-            dataset=dataset,
-            dataset_id=dataset_id,
-            dataset_info=dataset_info,
-        )
-
-    def _upload_dataset_with_compression(
-        self,
-        project_id: str,
-        dataset: Dict[str, pd.DataFrame],
-        dataset_id: str,
-        dataset_info: DatasetInfo,
-    ):
-        schema = dataset_info.get_arrow_schema()
-
-        # dump the data to named parquet temp file
-        with tempfile.TemporaryDirectory() as tmp:
-            file_paths = []
-            for name, df in dataset.items():
-                # Adding .csv to support legacy way of converting everything to CSV
-                filename = f'{name}.{CSV_EXTENSION}.{PARQUET_EXTENSION}'
-                file_path = Path(tmp) / filename
-                file_paths.append(file_path)
-
-                # Data type conversion as per dataset_info
-                # Data types like date/time/datetime should be converted to string before creating parquet file
-                df = df.astype(dtype=dataset_info.get_pandas_dtypes())
-
-                write_dataframe_to_parquet_file(
-                    df=df, file_path=file_path, schema=schema
-                )
-
-            # add files to the DatasetInfo on the fly
-            dataset_info = copy.deepcopy(dataset_info)
-            dataset_info.files = [
-                fp.name.replace(f'.{PARQUET_EXTENSION}', '') for fp in file_paths
-            ]
-
-            # upload the parquet files
-            LOG.info(f'[{dataset_id}] dataset upload: upload and import dataset files')
-
-            res = self._upload_dataset_files(
-                project_id=project_id,
-                dataset_id=dataset_id,
-                file_paths=file_paths,
-                dataset_info=dataset_info,
-            )
-
-            LOG.info(f'Dataset uploaded {res}')
-            return res
-
-    ##### End: Methods related to uploading dataset #####
-
     def get_mutual_information(
         self,
         project_id: str,
         dataset_id: str,
         features: list,
         normalized: Optional[bool] = False,
         slice_query: Optional[str] = None,
@@ -885,120 +622,14 @@
         except RuntimeError:
             msg = f'Error: Dataset:{model_info.datasets[0]} does not exist'
             violations.append(MonitoringViolation(MonitoringViolationType.FATAL, msg))
             return violations
 
         return violations
 
-    def publish_events_batch(  # noqa
-        self,
-        project_id: str,
-        model_id: str,
-        batch_source: Union[pd.DataFrame, str],
-        id_field: Optional[str] = None,
-        update_event: Optional[bool] = False,
-        timestamp_field: Optional[str] = None,
-        timestamp_format: FiddlerTimestamp = FiddlerTimestamp.INFER,
-        data_source: Optional[BatchPublishType] = None,
-        casting_type: Optional[bool] = False,
-        credentials: Optional[dict] = None,
-        group_by: Optional[str] = None,
-    ):
-        """
-        Publishes a batch events object to Fiddler Service.
-        :param project_id:    The project to which the model whose events are being published belongs.
-        :param model_id:      The model whose events are being published.
-        :param batch_source:  Batch object to be published. Can be one of: Pandas DataFrame, CSV file, PKL Pandas DataFrame, or Parquet file.
-        :param id_field:  Column to extract id value from.
-        :param update_event: Bool indicating if the events are updates to previously published rows
-        :param timestamp_field:     Column to extract timestamp value from.
-                              Timestamp must match the specified format in `timestamp_format`.
-        :param timestamp_format:   Format of timestamp within batch object. Can be one of:
-                                - FiddlerTimestamp.INFER
-                                - FiddlerTimestamp.EPOCH_MILLISECONDS
-                                - FiddlerTimestamp.EPOCH_SECONDS
-                                - FiddlerTimestamp.ISO_8601
-        :param data_source:   Source of batch object. In case of failed inference, can be one of:
-                                - BatchPublishType.DATAFRAME
-                                - BatchPublishType.LOCAL_DISK
-                                - BatchPublishType.AWS_S3
-                                - BatchPublishType.GCP_STORAGE
-        :param casting_type: Bool indicating if fiddler should try to cast the data in the event with
-                             the type referenced in model info. Default to False.
-        :param credentials:  Dictionary containing authorization for AWS or GCP.
-
-                             For AWS S3, list of expected keys are
-                              ['aws_access_key_id', 'aws_secret_access_key', 'aws_session_token']
-                              with 'aws_session_token' being applicable to the AWS account being used.
-
-                             For GCP, list of expected keys are
-                              ['gcs_access_key_id', 'gcs_secret_access_key', 'gcs_session_token']
-                              with 'gcs_session_token' being applicable to the GCP account being used.
-        :param group_by: Column to group events together for Model Performance metrics. For example,
-                         in ranking models that column should be query_id or session_id, used to
-                         compute NDCG and MAP. Be aware that the batch_source file/dataset provided should have
-                         events belonging to the SAME query_id/session_id TOGETHER and cannot be mixed
-                         in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
-                         would not work. Please sort the file by group_by group first to have rows with
-                         the following order: query_id 31,31,31,31,31,31,2,2.
-        """
-        return PublishEvent(self.connection).publish_events_batch(
-            project_id,
-            model_id,
-            batch_source,
-            id_field,
-            update_event,
-            timestamp_field,
-            timestamp_format,
-            data_source,
-            casting_type,
-            credentials,
-            group_by,
-        )
-
-    def publish_events_batch_schema(  # noqa
-        self,
-        batch_source: Union[pd.DataFrame, str],
-        publish_schema: Dict[str, Any],
-        data_source: Optional[BatchPublishType] = None,
-        credentials: Optional[dict] = None,
-        group_by: Optional[str] = None,
-    ):
-        """
-        Publishes a batch events object to Fiddler Service.
-        :param batch_source:  Batch object to be published. Can be one of: Pandas DataFrame, CSV file, PKL Pandas DataFrame, or Parquet file.
-        :param publish_schema: Dict object specifying layout of data.
-        :param data_source:   Source of batch object. In case of failed inference, can be one of:
-                                - BatchPublishType.DATAFRAME
-                                - BatchPublishType.LOCAL_DISK
-                                - BatchPublishType.AWS_S3
-                                - BatchPublishType.GCP_STORAGE
-        :param credentials:  Dictionary containing authorization for AWS or GCP.
-
-                             For AWS S3, list of expected keys are
-                              ['aws_access_key_id', 'aws_secret_access_key', 'aws_session_token']
-                              with 'aws_session_token' being applicable to the AWS account being used.
-
-                             For GCP, list of expected keys are
-                              ['gcs_access_key_id', 'gcs_secret_access_key', 'gcs_session_token']
-                              with 'gcs_session_token' being applicable to the GCP account being used.
-        :param group_by: Column to group events together for Model Performance metrics. For example,
-                         in ranking models that column should be query_id or session_id, used to
-                         compute NDCG and MAP.
-        """
-        return PublishEvent(self.connection).publish_events_batch_schema(
-            batch_source,
-            publish_schema,
-            data_source,
-            credentials,
-            group_by,
-        )
-
-    ##### End: Methods related to publishing event #####
-
     def get_model(self, project_id: str, model_id: str, output_dir: Path):
         """
         download the model binary, package.py and model.yaml to the given
         output dir.
 
         :param project_id: project id
         :param model_id: model id
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/libs/http_client.py` & `fiddler-client-2.0.0.dev3/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/model.py` & `fiddler-client-2.0.0.dev3/fiddler/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/model_info_validator.py` & `fiddler-client-2.0.0.dev3/fiddler/model_info_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/monitoring_validator.py` & `fiddler-client-2.0.0.dev3/fiddler/monitoring_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev3/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev3/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev3/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev3/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/project.py` & `fiddler-client-2.0.0.dev3/fiddler/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev3/fiddler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev3/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev3/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev3/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/utils/helper.py` & `fiddler-client-2.0.0.dev3/fiddler/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/utils/pandas.py` & `fiddler-client-2.0.0.dev3/fiddler/utils/pandas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import logging
 from datetime import datetime
-from pathlib import Path
 from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
-import pyarrow as pa
-import pyarrow.parquet as pq
-
-from fiddler.v2.constants import PARQUET_COMPRESSION, PARQUET_ROW_GROUP_SIZE
 
 from .. import constants
 
 LOG = logging.getLogger(__name__)
 TIMESTAMP = 'TIMESTAMP'
 
 
@@ -36,37 +31,42 @@
     - Convert datetime to string
 
     TODO: Expand to all other datatypes
     """
     for ind, col_type in enumerate(df.dtypes):
         col = df.columns[ind]
         if col_type is not None and 'datetime64' in str(col_type):
-            df[col] = pd.to_datetime(df[col], utc=True).dt.tz_localize(
-                None
-            )  # Skipping timezone information from the column. REF: https://fiddlerlabs.atlassian.net/browse/FDL-2592
+            # Skipping timezone information from the column.
+            # REF: https://fiddlerlabs.atlassian.net/browse/FDL-2592
+            df[col] = pd.to_datetime(df[col], utc=True).dt.tz_localize(None)
             df[col] = df[col].dt.strftime(constants.TIMESTAMP_FORMAT)
             df[col] = df[col].astype('string')
 
-        # pandas considers the datatype as an object, if it finds multiple datatypes in a column
-        # If such columns are consists of timestamp values, and those values are less than
-        # specified 'max_inferred_cardinality' value. System infers the timestamp variable as a categorical
-        # variable. To avoid that, we added a check where we check the object is a datetime object
-        # or not. If yes, we convert the datetime object into string.
+        # pandas considers the datatype as an object, if it finds multiple datatypes
+        # in a column. If such columns are consists of timestamp values, and those
+        # values are less than specified 'max_inferred_cardinality' value. System
+        # infers the timestamp variable as a categorical variable. To avoid that,
+        # we added a check where we check the object is a datetime object or not.
+        # If yes, we convert the datetime object into string.
         elif col_type == object:
             if df[col].astype('string') is not None and is_datetime(
                 df[col].astype('string')
             ):
                 df[col] = pd.to_datetime(
                     df[col], format=constants.TIMESTAMP_FORMAT, utc=True
                 ).dt.tz_localize(None)
                 df[col] = df[col].astype('string')
     return df
 
 
 def try_series_retype(series: pd.Series, new_type) -> Union[pd.DataFrame, pd.Series]:
+    if new_type == 'unknown':
+        # Do not retype data
+        return series
+
     try:
         return series.astype(new_type)
     except (TypeError, ValueError) as e:
         if new_type == 'int':
             LOG.warning(
                 f'"{series.name}" cannot be loaded as int '
                 f'(likely because it contains missing values, and '
@@ -80,24 +80,27 @@
                     lambda x: datetime.strptime(x, constants.TIMESTAMP_FORMAT)
                 )
             # if timestamp str doesn't contain millisec.
             # @NOTE: This can be a makeshift fix.
             except ValueError:
                 # @TODO: Should such cases be
                 # 1. handled by client OR
-                # 2. should server apped 00 milliseconds if not present during ingestion OR
+                # 2. should server apped 00 ms if not present during ingestion OR
                 # 3. should it break if timestamp format does not match while ingestion?
                 return series.apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S'))
         else:
             raise e
 
 
 def df_to_dict(df: pd.DataFrame):
-    data_array = [y.iloc[0, :].to_dict() for x, y in df.groupby(level=0)]  # type: ignore
-    # convert numpy type values to python type: some numpy types are not JSON serializable
+    data_array = [
+        y.iloc[0, :].to_dict() for x, y in df.groupby(level=0)  # type: ignore
+    ]
+    # convert numpy type values to python type: some numpy types are not
+    # JSON serializable
     for data in data_array:
         for key, val in data.items():
             if isinstance(val, np.bool_):
                 data[key] = bool(val)
             if isinstance(val, np.integer):
                 data[key] = int(val)
             if isinstance(val, np.floating):
@@ -112,44 +115,22 @@
     """
     for name, df in dataset.items():
         if df.shape[0] > max_len:
             return True
     return False
 
 
-def write_dataframe_to_parquet_file(
-    df: pd.DataFrame, file_path: Path, schema: Optional[pa.Schema] = None
-):
-    """
-    Write the given dataframe to parquet file
-
-    :param df: Pandas dataframe
-    :param file_path: Path where the parquet file should be written
-    :param schema: Arrow schema
-    :return: NA
-    """
-    LOG.info(f'Writing df with shape {df.shape} to {file_path}')
-
-    table = pa.Table.from_pandas(df, schema=schema, preserve_index=False)
-
-    schema = schema or table.schema
-
-    with pq.ParquetWriter(
-        file_path, schema=schema, compression=PARQUET_COMPRESSION
-    ) as pq_writer:
-        pq_writer.write_table(table, row_group_size=PARQUET_ROW_GROUP_SIZE)
-
-
 def convert_flat_csv_data_to_grouped(
     input_data: pd.DataFrame, group_by_col: str, output_path: Optional[str] = None
 ) -> pd.DataFrame:
     """
     :param input_data: The dataframe with flat data.
     :param group_by_col: The column to group the data by.
-    :param output_path: Optional argument, the path to write the grouped data to. If not specified, data won't be written anywhere.
+    :param output_path: Optional argument, the path to write the grouped data to.
+           If not specified, data won't be written anywhere.
     :return grouped_df: dataframe in grouped format
     """
     grouped_df = input_data.groupby(by=group_by_col, sort=False)
     grouped_df = grouped_df.aggregate(lambda x: x.tolist())
 
     if output_path is not None:
         grouped_df.to_csv(output_path)
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v1_v2_compat.py` & `fiddler-client-2.0.0.dev3/fiddler/v1_v2_compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     FiddlerTimestamp,
     ModelInfo,
 )
 from fiddler.utils import logging
 from fiddler.v2.api.api import Client
 from fiddler.v2.constants import FiddlerTimestamp as V2FiddlerTimestamp
 from fiddler.v2.constants import FileType
-from fiddler.v2.schema.common import Column as V2Column
-from fiddler.v2.schema.common import DatasetInfo as V2DatasetInfo
 from fiddler.v2.schema.dataset import Dataset
 
 DATASET_MAX_ROWS = 50_000
 
 
 logger = logging.getLogger(__name__)
 
@@ -94,23 +92,15 @@
         :param project_id: The unique identifier of the project on Fiddler
         :param dataset_id: The unique identifier of the dataset on the Fiddler
             engine.
 
         :returns: A fiddler.DatasetInfo object describing the dataset.
         """
         dataset = self.get_dataset(project_id, dataset_id)
-        dataset_info = DatasetInfo(
-            display_name=dataset.name,
-            columns=[
-                Column.from_dict(col.dict(by_alias=True))
-                for col in dataset.info.columns
-            ],
-            dataset_id=dataset_id,
-        )
-        return dataset_info
+        return dataset.info
 
     def delete_dataset(self, project_id: str, dataset_id: str) -> None:
         """Permanently delete a dataset.
 
         :param project_id: The unique identifier of the project on the Fiddler
             engine.
         :param dataset_id: The unique identifier of the dataset on the Fiddler
@@ -167,25 +157,19 @@
             engine. Must be a short string without whitespace.
         :param info: A DatasetInfo object specifying all the details of the
             dataset.
         :param size_check_enabled: Unused argument to maintain compatibility
 
         :returns: The server response for the upload.
         """
-        v2_info = None
-        if info:
-            v2_info = V2DatasetInfo(
-                columns=[V2Column.from_dict(col.to_dict()) for col in info.columns]
-            )
-
         return self.client_v2.upload_dataset_dataframe(
             project_name=project_id,
             dataset_name=dataset_id,
             datasets=dataset,
-            info=v2_info,
+            info=info,
             is_sync=True,
         )
 
     def upload_dataset(
         self,
         project_id: str,
         dataset_id: str,
@@ -208,26 +192,20 @@
             dataset.
         :param size_check_enabled: Unused argument to maintain compatibility
 
         :returns: The server response for the upload.
         """
         file_name = file_path.split('/')[-1]
         files = {file_name: Path(file_path)}
-        # @todo as we only support csv on server side for now, throw an error saying the same.
-        v2_info = None
-        if info:
-            v2_info = V2DatasetInfo(
-                columns=[V2Column.from_dict(col.to_dict()) for col in info.columns]
-            )
         if file_type == 'csv':
             return self.client_v2.upload_dataset(
                 project_name=project_id,
                 dataset_name=dataset_id,
                 files=files,
-                info=v2_info,
+                info=info,
                 file_type=FileType.CSV,
                 file_schema=file_schema,
             )
         else:
             raise NotImplementedError('Only csv is supported in current implementation')
 
     def upload_dataset_dir(
@@ -315,23 +293,19 @@
 
         if not info_yaml.exists():
             raise ValueError(f'DatasetInfo yaml ({info_yaml}) not found.')
 
         with open(info_yaml) as f:
             dataset_info = DatasetInfo.from_dict(yaml.safe_load(f))
 
-        v2_info = V2DatasetInfo(
-            columns=[V2Column.from_dict(col.to_dict()) for col in dataset_info.columns]
-        )
-
         return self.client_v2.upload_dataset_from_dir(
             project_id,
             dataset_id,
             dataset_dir,
-            v2_info,
+            dataset_info,
             FileType.CSV,
             file_schema,
             is_sync=True,
         )
 
     def publish_events_batch_schema(
         self,
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/alert_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/alert_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/api.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/baseline_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/baseline_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/dataset_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/dataset_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 from typing import Dict, List, Optional
 
 import numpy as np
 import pandas as pd
 from pydantic import parse_obj_as
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
-from fiddler.core_objects import DEFAULT_MAX_INFERRED_CARDINALITY
+from fiddler.core_objects import Column, DataType, DatasetInfo, DEFAULT_MAX_INFERRED_CARDINALITY
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.api.helpers import multipart_upload
 from fiddler.v2.constants import FileType, UploadType
-from fiddler.v2.schema.common import Column, DatasetInfo, DataType
 from fiddler.v2.schema.dataset import Dataset, DatasetIngest
 from fiddler.v2.utils.exceptions import FiddlerAPIException, handle_api_error_response
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 from fiddler.v2.validators.dataset_validator import (
     validate_dataset_columns,
     validate_dataset_info,
     validate_dataset_shape,
 )
 
+DEFAULT_NROWS_PER_CHUNK = 100000
 DEFAULT_SAMPLE_SIZE = 20000
 logger = logging.getLogger(__name__)
 
 
 class DatasetMixin:
     client: RequestClient
     organization_name: str
@@ -47,17 +47,28 @@
         """
         response = self.client.get(
             url='datasets',
             params={
                 'organization_name': self.organization_name,
                 'project_name': project_name,
             },
-        )
+        )        
         _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
-        return parse_obj_as(List[Dataset], items)
+        datasets:List[Dataset] = []
+        for item in items:
+            try :
+                datasets.append(Dataset.from_dict(item))
+            except KeyError as ke:
+                raise FiddlerAPIException(
+                    status_code=response.status_code,
+                    error_code=response.status_code,
+                    message=f'Invalid response content. {str(ke)} in the response.',
+                    errors=[],
+                )   
+        return datasets
 
     @handle_api_error_response
     def get_dataset(self, project_name: str, dataset_name: str) -> Dataset:
         """
         Get all the details for a given dataset
 
         :param project_name:    The project to which the dataset belongs to
@@ -157,17 +168,15 @@
 
         request_body = DatasetIngest(
             name=dataset_name,
             file_name=file_names,
             info=info,
             file_type=file_type,
             file_schema=file_schema,
-        ).dict(
-            by_alias=True
-        )  # setting by_alias bc Columns fields are aliased
+        ).to_dict()
         response = self.client.post(
             url=f'datasets/{self.organization_name}:{project_name}:{dataset_name}/ingest',
             data=json.dumps(request_body),
         )
         # @TODO: Handle invalid file path exception
         if response.status_code == HTTPStatus.ACCEPTED:
             resp = APIResponseHandler(response).get_data()
@@ -313,122 +322,70 @@
             is_sync=is_sync,
         )
 
     @handle_api_error_response
     def infer_dataset_info(
         self,
         file_path: str,
+        display_name: str,
+        dataset_id: Optional[str],
         max_inferred_cardinality: Optional[int] = DEFAULT_MAX_INFERRED_CARDINALITY,
         sample_size: Optional[int] = DEFAULT_SAMPLE_SIZE,
+        chunk_size: Optional[int] = DEFAULT_NROWS_PER_CHUNK,
     ) -> DatasetInfo:
         """
         Derives DatasetInfo from the given csv file
 
         :param file_path:       Relative or absolute path of the file in string format, for example, 'datasets/train.csv'
+        :param display_name:    A name for user-facing display (different from an id). 
+        :param dataset_id:      Dataset Id
 
         :returns:               DatasetInfo derived from the input file_path
         """
         if not file_path:
             raise ValueError('`file_path` is empty. Please enter a valid input.')
 
         file_path = Path(file_path)
 
         if not file_path.exists():
             raise ValueError('`file_path` does not exist. Please enter a valid input.')
 
-        # TODO (pradhuman)
-        # Read from dir
-        # Read chunks if input size is large and merge multiple DatasetInfo
-
+        # TODO (pradhuman): Read from dir
+        
+        dataset_infos:List[DatasetInfo] = []
         # 1. read file
-        df = pd.read_csv(file_path)
-        # 2. take random sample
-        if df.shape[0] > sample_size:
-            random_sample = df.sample(sample_size)
-            temp_dir = tempfile.TemporaryDirectory()
-            sample_file_path = os.path.join(temp_dir.name, file_path.name)
-            random_sample.save(sample_file_path)
-            file_path_server_inference = Path(sample_file_path)
-        else:
-            file_path_server_inference = file_path
-
-        # 3. detect type
-        files_encoders: Dict[str, MultipartEncoder] = {
-            'file': MultipartEncoder(
-                fields={
-                    'file': (
-                        file_path_server_inference.name,
-                        open(file_path_server_inference, 'rb'),
-                        'text/plain',
-                    ),
+        with pd.read_csv(file_path, chunksize=chunk_size) as reader:
+            for df in reader:
+                logger.info(f'Read a chunk from input {df.shape}')
+                # 2. take random sample
+                if df.shape[0] > sample_size:
+                    random_sample = df.sample(sample_size)
+                    temp_dir = tempfile.TemporaryDirectory()
+                    sample_file_path = os.path.join(temp_dir.name, file_path.name)
+                    random_sample.to_csv(sample_file_path, index=False)
+                    file_path_server_inference = Path(sample_file_path)
+                else:
+                    file_path_server_inference = file_path
+
+                # 3. detect type
+                files_encoders: Dict[str, MultipartEncoder] = {
+                    'file': MultipartEncoder(
+                        fields={
+                            'file': (
+                                file_path_server_inference.name,
+                                open(file_path_server_inference, 'rb'),
+                                'text/plain',
+                            ),
+                        }
+                    )
                 }
-            )
-        }
-        response = self.client.post(
-            url='infer-data-types', files_encoders=files_encoders
-        )
-        api_response = APIResponseHandler(response)
-
-        column_datatypes_response = api_response.get_data().get('column_datatypes')
-        column_name_datatype: Dict[str, str] = {}
-        for column_datatype_response in column_datatypes_response:
-            if (
-                'column_name' in column_datatype_response
-                and 'data_type' in column_datatype_response
-            ):
-                column_name_datatype[
-                    column_datatype_response['column_name']
-                ] = column_datatype_response['data_type']
-
-        columns: List[Column] = []
-
-        # 4. calculate the rest of the column level stats
-        for column_name, column_series in df.items():
-            column_info = _calculate_stats_for_col(
-                column_name, column_series, column_name_datatype.get(column_name, None)
-            )
-            columns.append(column_info)
-
-        return DatasetInfo(columns=columns)
-
-
-def _calculate_stats_for_col(
-    column_name: str, column_series: pd.Series, column_dtype: str
-) -> Column:
-    # @TODO Automatically drop the empty column with warning and proceed instead of aborting the upload
-    if column_series.isna().all():
-        raise ValueError(
-            f'Column {column_name} is empty. '
-            f'Please remove it and re-upload the dataset.'
-        )
-    if column_dtype is None:
-        raise ValueError(f'Data type for Column {column_name} is not detected.')
-
-    # get possible values for categorical type
-    if column_dtype in [DataType.CATEGORY.value, DataType.BOOLEAN.value]:
-        possible_values = np.sort(column_series.dropna().unique()).tolist()
-    else:
-        possible_values = None
-
-    # get value range for numerical dtype
-    if column_dtype in [DataType.INTEGER.value, DataType.FLOAT.value]:
-        value_min, value_max = column_series.astype(column_dtype, errors='ignore').agg(
-            ['min', 'max']
-        )
-        if np.isnan(value_min):
-            value_min = None
-        if np.isnan(value_max):
-            value_max = None
-    else:
-        value_min, value_max = None, None
-
-    # get nullability
-    is_nullable = bool(column_series.isna().any())
-
-    return Column(
-        name=column_name,
-        data_type=column_dtype,
-        possible_values=possible_values,
-        is_nullable=is_nullable,
-        value_range_min=value_min,
-        value_range_max=value_max,
-    )
+                request_body = dict(
+                    name=display_name
+                )
+                response = self.client.post(
+                    url='infer-data-types', data=request_body, files_encoders=files_encoders
+                )
+                api_response = APIResponseHandler(response)
+                logger.info(api_response.get_status_code)
+                dataset_infos.append(DatasetInfo.from_dict(api_response.get_data()))
+        logger.info(f'combining {len(dataset_infos)} DatasetInfo objects')
+        return DatasetInfo.as_combination(infos=dataset_infos, display_name=display_name)
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/events_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/events_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/explainability_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/helpers.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/job_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/job_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/model_artifact_deploy.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/model_deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/model_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/model_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/api/project_mixin.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/api/project_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/schema/alert.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/schema/alert.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/schema/events.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/schema/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/schema/model_deployment.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/schema/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/utils/decorators.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/utils/exceptions.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/utils/helpers.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/utils/response_handler.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev3/fiddler/v2/validators/dataset_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from pathlib import Path
 from typing import Dict
 
 import pandas as pd
 import pandas.errors
 
-from fiddler.v2.schema.common import DatasetInfo
+from fiddler.core_objects import DatasetInfo
 
 LOG = logging.getLogger(__name__)
 
 NUM_ROWS = 1
 JUST_THE_HEADER = 0
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler/validator.py` & `fiddler-client-2.0.0.dev3/fiddler/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev3/fiddler_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev1
+Version: 2.0.0.dev3
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -39,18 +39,25 @@
               - list_teams
               - list_project_roles
               - list_org_roles
               - unshare_project
               - share_project
               - process_avro
               - process_csv
+          - #### **New Features**
+            - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
+        
+        ### 1.8.0
           - #### **Modifications**
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
         
+        ### 1.7.1
+          - #### **Modification**
+            - Relaxed boto3 version constraint
         
         ### 1.7.0
           - #### **Removed**
             - Remove support for initializing fiddler client with version=1
             - Following methods are removed
               - get_segment_info
               - delete_segment
@@ -60,15 +67,15 @@
               - upload_segment
               - add_monitoring_config
               - publish_parquet_s3
               - publish_events_log
         
         ### 1.6.2
           - #### **Modifications**
-            - Made dataset_id a required field in add_model()
+            - Make dataset_id a required field in add_model()
             - Update max_inferred_cardinality to 100
           - #### **New Features**
             - New method for updating a model artifact `update_model_artifact`
         
         ### 1.5.3
           - #### **Modifications**
             - Fix add_model_artifact error for NLP models
```

### Comparing `fiddler-client-2.0.0.dev1/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev3/fiddler_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 fiddler/model_info_validator.py
 fiddler/monitoring_validator.py
 fiddler/project.py
 fiddler/v1_v2_compat.py
 fiddler/validator.py
 fiddler/api/__init__.py
 fiddler/api/monitoring.py
-fiddler/api/publish_event.py
 fiddler/assets/__init__.py
 fiddler/assets/pg_reserved_words.py
 fiddler/libs/__init__.py
 fiddler/libs/http_client.py
 fiddler/packtools/__init__.py
 fiddler/packtools/gem.py
 fiddler/packtools/keras_ig_helpers.py
@@ -52,15 +51,14 @@
 fiddler/v2/api/model_deployment_mixin.py
 fiddler/v2/api/model_mixin.py
 fiddler/v2/api/project_mixin.py
 fiddler/v2/schema/__init__.py
 fiddler/v2/schema/alert.py
 fiddler/v2/schema/base.py
 fiddler/v2/schema/baseline.py
-fiddler/v2/schema/common.py
 fiddler/v2/schema/dataset.py
 fiddler/v2/schema/events.py
 fiddler/v2/schema/job.py
 fiddler/v2/schema/model.py
 fiddler/v2/schema/model_deployment.py
 fiddler/v2/schema/project.py
 fiddler/v2/schema/server_info.py
```

### Comparing `fiddler-client-2.0.0.dev1/setup.py` & `fiddler-client-2.0.0.dev3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         'pandas>=1.2.5,<=1.5.3',
         'pyyaml',
         'packaging',
         'deepdiff',
         'boto3',
         'importlib-resources',
         'Werkzeug',
-        'pyarrow>=3.0.0',
         'deprecation==2.1.0',
         'pydantic>=1.9.0',
+        'urllib3<2',
         'deprecated==1.2.13',
         'semver>=2,<3',
         'tqdm==4.64.1',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `fiddler-client-2.0.0.dev1/tests/test_fiddler_api.py` & `fiddler-client-2.0.0.dev3/tests/test_fiddler_api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev1/tests/test_v1_v2_compat.py` & `fiddler-client-2.0.0.dev3/tests/test_v1_v2_compat.py`

 * *Files identical despite different names*


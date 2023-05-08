# Comparing `tmp/wds-client-0.2.8.tar.gz` & `tmp/wds-client-0.2.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/terra-workspace-data-service/terra-workspace-data-service/wds-client/dist/.tmp-v6dee5fu/wds-client-0.2.8.tar", last modified: Tue Nov 29 15:21:47 2022, max compression
+gzip compressed data, was "wds-client-0.2.80.tar", last modified: Mon May  8 19:30:41 2023, max compression
```

## Comparing `wds-client-0.2.8.tar` & `wds-client-0.2.80.tar`

### file list

```diff
@@ -1,64 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:21:47.000000 wds-client-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)      689 2022-11-29 15:21:47.000000 wds-client-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6604 2022-11-29 15:21:34.000000 wds-client-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-11-29 15:21:47.000000 wds-client-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2022-11-29 15:21:35.000000 wds-client-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:21:47.000000 wds-client-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     1983 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (122)     3375 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1818 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1805 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     1748 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2022-11-29 15:21:34.000000 wds-client-0.2.8/test/test_tsv_upload_response.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:21:47.000000 wds-client-0.2.8/wds_client/
--rw-r--r--   0 runner    (1001) docker     (122)     2429 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:21:47.000000 wds-client-0.2.8/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9623 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    12814 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    61202 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    49447 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    26549 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    12775 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4114 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:21:47.000000 wds-client-0.2.8/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1789 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6580 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5040 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5419 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4792 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     7280 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     3893 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     3913 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (122)     6056 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     3911 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     7055 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6551 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (122)     4840 2022-11-29 15:21:34.000000 wds-client-0.2.8/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (122)    12642 2022-11-29 15:21:35.000000 wds-client-0.2.8/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:21:47.000000 wds-client-0.2.8/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      689 2022-11-29 15:21:46.000000 wds-client-0.2.8/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2022-11-29 15:21:46.000000 wds-client-0.2.8/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 15:21:46.000000 wds-client-0.2.8/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-11-29 15:21:46.000000 wds-client-0.2.8/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-29 15:21:46.000000 wds-client-0.2.8/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.491436 wds-client-0.2.80/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 19:30:41.491436 wds-client-0.2.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-08 19:29:34.000000 wds-client-0.2.80/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 19:30:41.491436 wds-client-0.2.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 19:29:34.000000 wds-client-0.2.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.483436 wds-client-0.2.80/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-08 19:29:34.000000 wds-client-0.2.80/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-08 19:29:33.000000 wds-client-0.2.80/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.487436 wds-client-0.2.80/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.487436 wds-client-0.2.80/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61563 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19355 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26218 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.491436 wds-client-0.2.80/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-08 19:29:33.000000 wds-client-0.2.80/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-08 19:29:34.000000 wds-client-0.2.80/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:30:41.487436 wds-client-0.2.80/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 19:30:41.000000 wds-client-0.2.80/wds_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wds-client-0.2.8/README.md` & `wds-client-0.2.80/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # wds-client
-This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented
-are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force
-swagger-ui to display those endpoints differently.
-
-Error codes and responses for proposed APIs are likely to change as we gain more clarity on their
-implementation.
+This page lists current APIs.
 
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.8
+- Package version: 0.2.80
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -71,15 +66,16 @@
 # Enter a context with an instance of the API client
 with wds_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = wds_client.GeneralWDSInformationApi(api_client)
     
     try:
         # Gets health status for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#health for details)
-        api_instance.status_get()
+        api_response = api_instance.status_get()
+        pprint(api_response)
     except ApiException as e:
         print("Exception when calling GeneralWDSInformationApi->status_get: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
@@ -87,54 +83,63 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *GeneralWDSInformationApi* | [**status_get**](docs/GeneralWDSInformationApi.md#status_get) | **GET** /status | Gets health status for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#health for details)
 *GeneralWDSInformationApi* | [**version_get**](docs/GeneralWDSInformationApi.md#version_get) | **GET** /version | Gets related git and build version info for WDS -- generated via Spring Boot Actuator (see https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/#info for details)
 *InstancesApi* | [**create_wds_instance**](docs/InstancesApi.md#create_wds_instance) | **POST** /instances/{v}/{instanceid} | Create an instance
 *InstancesApi* | [**delete_wds_instance**](docs/InstancesApi.md#delete_wds_instance) | **DELETE** /instances/{v}/{instanceid} | Delete an instance
+*InstancesApi* | [**list_wds_instances**](docs/InstancesApi.md#list_wds_instances) | **GET** /instances/{v} | List instances
 *RecordsApi* | [**batch_write_records**](docs/RecordsApi.md#batch_write_records) | **POST** /{instanceid}/batch/{v}/{type} | Batch write records
 *RecordsApi* | [**create_or_replace_record**](docs/RecordsApi.md#create_or_replace_record) | **PUT** /{instanceid}/records/{v}/{type}/{id} | Create or replace record
 *RecordsApi* | [**delete_record**](docs/RecordsApi.md#delete_record) | **DELETE** /{instanceid}/records/{v}/{type}/{id} | Delete record
 *RecordsApi* | [**get_record**](docs/RecordsApi.md#get_record) | **GET** /{instanceid}/records/{v}/{type}/{id} | Get record
 *RecordsApi* | [**get_records_as_tsv**](docs/RecordsApi.md#get_records_as_tsv) | **GET** /{instanceid}/tsv/{v}/{type} | Retrieve all records in record type as tsv.
 *RecordsApi* | [**query_records**](docs/RecordsApi.md#query_records) | **POST** /{instanceid}/search/{v}/{type} | Query records
 *RecordsApi* | [**update_record**](docs/RecordsApi.md#update_record) | **PATCH** /{instanceid}/records/{v}/{type}/{id} | Update record
 *RecordsApi* | [**upload_tsv**](docs/RecordsApi.md#upload_tsv) | **POST** /{instanceid}/tsv/{v}/{type} | Import records to a record type from a tsv file
-*SchemaApi* | [**delete_attribute**](docs/SchemaApi.md#delete_attribute) | **DELETE** /{instanceid}/types/{type}/attributes/{v}/{attribute} | Delete attribute (pending)
 *SchemaApi* | [**delete_record_type**](docs/SchemaApi.md#delete_record_type) | **DELETE** /{instanceid}/types/{v}/{type} | Delete record type
 *SchemaApi* | [**describe_all_record_types**](docs/SchemaApi.md#describe_all_record_types) | **GET** /{instanceid}/types/{v} | Describe all record types
-*SchemaApi* | [**describe_attribute**](docs/SchemaApi.md#describe_attribute) | **GET** /{instanceid}/types/{type}/attributes/{v}/{attribute} | Describe attribute (pending)
 *SchemaApi* | [**describe_record_type**](docs/SchemaApi.md#describe_record_type) | **GET** /{instanceid}/types/{v}/{type} | Describe record type
-*SchemaApi* | [**update_attribute**](docs/SchemaApi.md#update_attribute) | **PATCH** /{instanceid}/types/{type}/attributes/{v}/{attribute} | Update attribute (pending)
-*SchemaApi* | [**update_record_type**](docs/SchemaApi.md#update_record_type) | **PATCH** /{instanceid}/types/{v}/{type} | Update record type (pending)
 
 
 ## Documentation For Models
 
  - [AttributeSchema](docs/AttributeSchema.md)
  - [BatchOperation](docs/BatchOperation.md)
  - [BatchRecordRequest](docs/BatchRecordRequest.md)
  - [BatchResponse](docs/BatchResponse.md)
+ - [Build](docs/Build.md)
+ - [Commit](docs/Commit.md)
+ - [Component](docs/Component.md)
+ - [Components](docs/Components.md)
+ - [DbComponent](docs/DbComponent.md)
  - [ErrorResponse](docs/ErrorResponse.md)
+ - [Git](docs/Git.md)
  - [InlineObject](docs/InlineObject.md)
  - [RecordAttributeDefinition](docs/RecordAttributeDefinition.md)
  - [RecordQueryResponse](docs/RecordQueryResponse.md)
  - [RecordRequest](docs/RecordRequest.md)
  - [RecordResponse](docs/RecordResponse.md)
  - [RecordTypeSchema](docs/RecordTypeSchema.md)
  - [RequestBodySearch](docs/RequestBodySearch.md)
  - [SearchOperator](docs/SearchOperator.md)
  - [SearchRequest](docs/SearchRequest.md)
  - [SearchSortDirection](docs/SearchSortDirection.md)
  - [StackTraceElement](docs/StackTraceElement.md)
+ - [StatusResponse](docs/StatusResponse.md)
  - [TsvUploadResponse](docs/TsvUploadResponse.md)
+ - [VersionResponse](docs/VersionResponse.md)
 
 
 ## Documentation For Authorization
 
- All endpoints do not require authorization.
+
+## bearerAuth
+
+- **Type**: Bearer authentication
+
 
 ## Author
```

### Comparing `wds-client-0.2.8/test/test_attribute_schema.py` & `wds-client-0.2.80/test/test_build.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.attribute_schema import AttributeSchema  # noqa: E501
+from wds_client.models.build import Build  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestAttributeSchema(unittest.TestCase):
-    """AttributeSchema unit test stubs"""
+class TestBuild(unittest.TestCase):
+    """Build unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AttributeSchema
+        """Test Build
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.attribute_schema.AttributeSchema()  # noqa: E501
+        # model = wds_client.models.build.Build()  # noqa: E501
         if include_optional :
-            return AttributeSchema(
+            return Build(
+                artifact = '0', 
                 name = '0', 
-                datatype = 'boolean', 
-                relates_to = '0'
+                time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                version = '0', 
+                group = '0'
             )
         else :
-            return AttributeSchema(
-                name = '0',
-                datatype = 'boolean',
+            return Build(
         )
 
-    def testAttributeSchema(self):
-        """Test AttributeSchema"""
+    def testBuild(self):
+        """Test Build"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/test/test_batch_operation.py` & `wds-client-0.2.80/test/test_batch_operation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -41,38 +41,44 @@
                     id = '0', 
                     type = '0', 
                     attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 , )
             )
         else :
             return BatchOperation(
                 operation = 'upsert',
                 record = wds_client.models.batch_record_request.BatchRecordRequest(
                     id = '0', 
                     type = '0', 
                     attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 , ),
         )
 
     def testBatchOperation(self):
         """Test BatchOperation"""
         inst_req_only = self.make_instance(include_optional=False)
```

### Comparing `wds-client-0.2.8/test/test_batch_record_request.py` & `wds-client-0.2.80/test/test_batch_record_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -39,36 +39,42 @@
                 id = '0', 
                 type = '0', 
                 attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 
             )
         else :
             return BatchRecordRequest(
                 id = '0',
                 type = '0',
                 attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 ,
         )
 
     def testBatchRecordRequest(self):
         """Test BatchRecordRequest"""
         inst_req_only = self.make_instance(include_optional=False)
```

### Comparing `wds-client-0.2.8/test/test_general_wds_information_api.py` & `wds-client-0.2.80/test/test_general_wds_information_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.8/test/test_inline_object.py` & `wds-client-0.2.80/test/test_inline_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.8/test/test_instances_api.py` & `wds-client-0.2.80/test/test_instances_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -38,10 +38,17 @@
     def test_delete_wds_instance(self):
         """Test case for delete_wds_instance
 
         Delete an instance  # noqa: E501
         """
         pass
 
+    def test_list_wds_instances(self):
+        """Test case for list_wds_instances
+
+        List instances  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/test/test_record_attribute_definition.py` & `wds-client-0.2.80/test/test_commit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.record_attribute_definition import RecordAttributeDefinition  # noqa: E501
+from wds_client.models.commit import Commit  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestRecordAttributeDefinition(unittest.TestCase):
-    """RecordAttributeDefinition unit test stubs"""
+class TestCommit(unittest.TestCase):
+    """Commit unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test RecordAttributeDefinition
+        """Test Commit
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.record_attribute_definition.RecordAttributeDefinition()  # noqa: E501
+        # model = wds_client.models.commit.Commit()  # noqa: E501
         if include_optional :
-            return RecordAttributeDefinition(
-                name = '0'
+            return Commit(
+                id = '0', 
+                time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
-            return RecordAttributeDefinition(
-                name = '0',
+            return Commit(
         )
 
-    def testRecordAttributeDefinition(self):
-        """Test RecordAttributeDefinition"""
+    def testCommit(self):
+        """Test Commit"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/test/test_record_query_response.py` & `wds-client-0.2.80/test/test_record_query_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -47,19 +47,22 @@
                         id = '0', 
                         type = '0', 
                         attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 , )
                     ]
             )
         else :
             return RecordQueryResponse(
                 search_request = wds_client.models.search_request.SearchRequest(
@@ -73,19 +76,22 @@
                         id = '0', 
                         type = '0', 
                         attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 , )
                     ],
         )
 
     def testRecordQueryResponse(self):
         """Test RecordQueryResponse"""
```

### Comparing `wds-client-0.2.8/test/test_record_response.py` & `wds-client-0.2.80/test/test_record_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.record_response import RecordResponse  # noqa: E501
+from wds_client.models.record_request import RecordRequest  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestRecordResponse(unittest.TestCase):
-    """RecordResponse unit test stubs"""
+class TestRecordRequest(unittest.TestCase):
+    """RecordRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test RecordResponse
+        """Test RecordRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.record_response.RecordResponse()  # noqa: E501
+        # model = wds_client.models.record_request.RecordRequest()  # noqa: E501
         if include_optional :
-            return RecordResponse(
-                id = '0', 
-                type = '0', 
+            return RecordRequest(
                 attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 
             )
         else :
-            return RecordResponse(
-                id = '0',
-                type = '0',
+            return RecordRequest(
                 attributes = {
   "stringAttr": "string",
   "numericAttr": 123,
   "booleanAttr": true,
   "relationAttr": "terra-wds:/target-type/target-id",
+  "fileAttr": "https://account_name.blob.core.windows.net/container-1/blob1",
   "arrayString": ["green", "red"],
   "arrayBoolean": [true, false],
   "arrayNumber": [12821.112, 0.12121211, 11],
   "arrayDate": ["2022-11-03"],
-  "arrayDateTime": ["2022-11-03T04:36:20"]
+  "arrayDateTime": ["2022-11-03T04:36:20"],
+  "arrayRelation": ["terra-wds:/target-type/target-id-1", "terra-wds:/target-type/target-id-2"],
+  "arrayFile": ["drs://drs.example.org/file_id_1", "https://account_name.blob.core.windows.net/container-2/blob2"]
 }
 ,
         )
 
-    def testRecordResponse(self):
-        """Test RecordResponse"""
+    def testRecordRequest(self):
+        """Test RecordRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/test/test_records_api.py` & `wds-client-0.2.80/test/test_records_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.8/test/test_search_operator.py` & `wds-client-0.2.80/test/test_request_body_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.search_operator import SearchOperator  # noqa: E501
+from wds_client.models.request_body_search import RequestBodySearch  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestSearchOperator(unittest.TestCase):
-    """SearchOperator unit test stubs"""
+class TestRequestBodySearch(unittest.TestCase):
+    """RequestBodySearch unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SearchOperator
+        """Test RequestBodySearch
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.search_operator.SearchOperator()  # noqa: E501
+        # model = wds_client.models.request_body_search.RequestBodySearch()  # noqa: E501
         if include_optional :
-            return SearchOperator(
+            return RequestBodySearch(
+                terms = '0', 
+                operator = 'and'
             )
         else :
-            return SearchOperator(
+            return RequestBodySearch(
+                terms = '0',
         )
 
-    def testSearchOperator(self):
-        """Test SearchOperator"""
+    def testRequestBodySearch(self):
+        """Test RequestBodySearch"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/test/test_search_request.py` & `wds-client-0.2.80/test/test_version_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.search_request import SearchRequest  # noqa: E501
+from wds_client.models.version_response import VersionResponse  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestSearchRequest(unittest.TestCase):
-    """SearchRequest unit test stubs"""
+class TestVersionResponse(unittest.TestCase):
+    """VersionResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SearchRequest
+        """Test VersionResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.search_request.SearchRequest()  # noqa: E501
+        # model = wds_client.models.version_response.VersionResponse()  # noqa: E501
         if include_optional :
-            return SearchRequest(
-                offset = 0, 
-                limit = 0, 
-                sort = 'asc', 
-                sort_attribute = '0'
+            return VersionResponse(
+                git = wds_client.models.git.git(
+                    branch = '0', 
+                    commit = wds_client.models.commit.commit(
+                        id = '0', 
+                        time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), ), 
+                build = wds_client.models.build.build(
+                    artifact = '0', 
+                    name = '0', 
+                    time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    version = '0', 
+                    group = '0', )
             )
         else :
-            return SearchRequest(
+            return VersionResponse(
         )
 
-    def testSearchRequest(self):
-        """Test SearchRequest"""
+    def testVersionResponse(self):
+        """Test VersionResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/test/test_search_sort_direction.py` & `wds-client-0.2.80/test/test_search_sort_direction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.8/test/test_stack_trace_element.py` & `wds-client-0.2.80/test/test_stack_trace_element.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.8/test/test_tsv_upload_response.py` & `wds-client-0.2.80/test/test_error_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import wds_client
-from wds_client.models.tsv_upload_response import TsvUploadResponse  # noqa: E501
+from wds_client.models.error_response import ErrorResponse  # noqa: E501
 from wds_client.rest import ApiException
 
-class TestTsvUploadResponse(unittest.TestCase):
-    """TsvUploadResponse unit test stubs"""
+class TestErrorResponse(unittest.TestCase):
+    """ErrorResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test TsvUploadResponse
+        """Test ErrorResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = wds_client.models.tsv_upload_response.TsvUploadResponse()  # noqa: E501
+        # model = wds_client.models.error_response.ErrorResponse()  # noqa: E501
         if include_optional :
-            return TsvUploadResponse(
+            return ErrorResponse(
+                status = 56, 
+                error = '0', 
                 message = '0', 
-                records_modified = 56
+                path = '0', 
+                timestamp = '0'
             )
         else :
-            return TsvUploadResponse(
+            return ErrorResponse(
+                status = 56,
+                error = '0',
                 message = '0',
-                records_modified = 56,
+                path = '0',
+                timestamp = '0',
         )
 
-    def testTsvUploadResponse(self):
-        """Test TsvUploadResponse"""
+    def testErrorResponse(self):
+        """Test ErrorResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wds-client-0.2.8/wds_client/api/general_wds_information_api.py` & `wds-client-0.2.80/wds_client/api/general_wds_information_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -48,15 +48,15 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: None
+        :return: StatusResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.status_get_with_http_info(**kwargs)  # noqa: E501
 
     def status_get_with_http_info(self, **kwargs):  # noqa: E501
@@ -73,15 +73,15 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: None
+        :return: tuple(StatusResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -112,26 +112,30 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
             '/status', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type=None,  # noqa: E501
+            response_type='StatusResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -147,15 +151,15 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: None
+        :return: VersionResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.version_get_with_http_info(**kwargs)  # noqa: E501
 
     def version_get_with_http_info(self, **kwargs):  # noqa: E501
@@ -172,15 +176,15 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: None
+        :return: tuple(VersionResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -211,25 +215,29 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
             '/version', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type=None,  # noqa: E501
+            response_type='VersionResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `wds-client-0.2.8/wds_client/api/instances_api.py` & `wds-client-0.2.80/wds_client/api/instances_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -35,15 +35,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def create_wds_instance(self, instanceid, v, **kwargs):  # noqa: E501
         """Create an instance  # noqa: E501
 
-        Create an instance with the given UUID. This API is liable to change.  # noqa: E501
+        Create an instance with the given UUID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_wds_instance(instanceid, v, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
@@ -61,15 +61,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.create_wds_instance_with_http_info(instanceid, v, **kwargs)  # noqa: E501
 
     def create_wds_instance_with_http_info(self, instanceid, v, **kwargs):  # noqa: E501
         """Create an instance  # noqa: E501
 
-        Create an instance with the given UUID. This API is liable to change.  # noqa: E501
+        Create an instance with the given UUID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_wds_instance_with_http_info(instanceid, v, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
@@ -137,15 +137,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/instances/{v}/{instanceid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -260,15 +260,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/instances/{v}/{instanceid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -277,7 +277,121 @@
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def list_wds_instances(self, v, **kwargs):  # noqa: E501
+        """List instances  # noqa: E501
+
+        List all instances in this server.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_wds_instances(v, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str v: API version (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: list[str]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.list_wds_instances_with_http_info(v, **kwargs)  # noqa: E501
+
+    def list_wds_instances_with_http_info(self, v, **kwargs):  # noqa: E501
+        """List instances  # noqa: E501
+
+        List all instances in this server.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_wds_instances_with_http_info(v, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str v: API version (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(list[str], status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'v'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_wds_instances" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'v' is set
+        if self.api_client.client_side_validation and ('v' not in local_var_params or  # noqa: E501
+                                                        local_var_params['v'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `v` when calling `list_wds_instances`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'v' in local_var_params:
+            path_params['v'] = local_var_params['v']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/instances/{v}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[str]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `wds-client-0.2.8/wds_client/api/records_api.py` & `wds-client-0.2.80/wds_client/api/records_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -46,14 +46,15 @@
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
         :param str v: API version (required)
         :param str type: Record type (required)
         :param list[BatchOperation] batch_operation: A list of batch operations to perform on records (required)
+        :param str primary_key: the column to uniquely identify a record
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -74,14 +75,15 @@
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
         :param str v: API version (required)
         :param str type: Record type (required)
         :param list[BatchOperation] batch_operation: A list of batch operations to perform on records (required)
+        :param str primary_key: the column to uniquely identify a record
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -94,15 +96,16 @@
 
         local_var_params = locals()
 
         all_params = [
             'instanceid',
             'v',
             'type',
-            'batch_operation'
+            'batch_operation',
+            'primary_key'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -141,14 +144,16 @@
             path_params['instanceid'] = local_var_params['instanceid']  # noqa: E501
         if 'v' in local_var_params:
             path_params['v'] = local_var_params['v']  # noqa: E501
         if 'type' in local_var_params:
             path_params['type'] = local_var_params['type']  # noqa: E501
 
         query_params = []
+        if 'primary_key' in local_var_params and local_var_params['primary_key'] is not None:  # noqa: E501
+            query_params.append(('primaryKey', local_var_params['primary_key']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -159,15 +164,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/{instanceid}/batch/{v}/{type}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -180,26 +185,27 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_or_replace_record(self, instanceid, v, type, id, record_request, **kwargs):  # noqa: E501
         """Create or replace record  # noqa: E501
 
-        Creates or replaces the record using the specified type and id. If the record already exists, its entire set of attributes will be overwritten by the attributes in the request body.  TODO: add a query parameter to allow/disallow overwriting existing records?   # noqa: E501
+        Creates or replaces the record using the specified type and id. If the record already exists, its entire set of attributes will be overwritten by the attributes in the request body. TODO: add a query parameter to allow/disallow overwriting existing records?   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_or_replace_record(instanceid, v, type, id, record_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
         :param str v: API version (required)
         :param str type: Record type (required)
         :param str id: Record id (required)
         :param RecordRequest record_request: A record's attributes to upload (required)
+        :param str primary_key: the column to uniquely identify a record
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -209,26 +215,27 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.create_or_replace_record_with_http_info(instanceid, v, type, id, record_request, **kwargs)  # noqa: E501
 
     def create_or_replace_record_with_http_info(self, instanceid, v, type, id, record_request, **kwargs):  # noqa: E501
         """Create or replace record  # noqa: E501
 
-        Creates or replaces the record using the specified type and id. If the record already exists, its entire set of attributes will be overwritten by the attributes in the request body.  TODO: add a query parameter to allow/disallow overwriting existing records?   # noqa: E501
+        Creates or replaces the record using the specified type and id. If the record already exists, its entire set of attributes will be overwritten by the attributes in the request body. TODO: add a query parameter to allow/disallow overwriting existing records?   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_or_replace_record_with_http_info(instanceid, v, type, id, record_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
         :param str v: API version (required)
         :param str type: Record type (required)
         :param str id: Record id (required)
         :param RecordRequest record_request: A record's attributes to upload (required)
+        :param str primary_key: the column to uniquely identify a record
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -242,15 +249,16 @@
         local_var_params = locals()
 
         all_params = [
             'instanceid',
             'v',
             'type',
             'id',
-            'record_request'
+            'record_request',
+            'primary_key'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -295,14 +303,16 @@
             path_params['v'] = local_var_params['v']  # noqa: E501
         if 'type' in local_var_params:
             path_params['type'] = local_var_params['type']  # noqa: E501
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
+        if 'primary_key' in local_var_params and local_var_params['primary_key'] is not None:  # noqa: E501
+            query_params.append(('primaryKey', local_var_params['primary_key']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -313,15 +323,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/{instanceid}/records/{v}/{type}/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -454,15 +464,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/{instanceid}/records/{v}/{type}/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1026,15 +1036,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/{instanceid}/records/{v}/{type}/{id}', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1058,15 +1068,15 @@
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
         :param str v: API version (required)
         :param str type: Record type (required)
         :param file records: A valid TSV import file (required)
-        :param str unique_row_identifier_column: the column to uniquely identify a record
+        :param str primary_key: the column to uniquely identify a record
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1087,15 +1097,15 @@
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str instanceid: WDS instance id; by convention equal to workspace id (required)
         :param str v: API version (required)
         :param str type: Record type (required)
         :param file records: A valid TSV import file (required)
-        :param str unique_row_identifier_column: the column to uniquely identify a record
+        :param str primary_key: the column to uniquely identify a record
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1109,15 +1119,15 @@
         local_var_params = locals()
 
         all_params = [
             'instanceid',
             'v',
             'type',
             'records',
-            'unique_row_identifier_column'
+            'primary_key'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -1156,16 +1166,16 @@
             path_params['instanceid'] = local_var_params['instanceid']  # noqa: E501
         if 'v' in local_var_params:
             path_params['v'] = local_var_params['v']  # noqa: E501
         if 'type' in local_var_params:
             path_params['type'] = local_var_params['type']  # noqa: E501
 
         query_params = []
-        if 'unique_row_identifier_column' in local_var_params and local_var_params['unique_row_identifier_column'] is not None:  # noqa: E501
-            query_params.append(('uniqueRowIdentifierColumn', local_var_params['unique_row_identifier_column']))  # noqa: E501
+        if 'primary_key' in local_var_params and local_var_params['primary_key'] is not None:  # noqa: E501
+            query_params.append(('primaryKey', local_var_params['primary_key']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
         if 'records' in local_var_params:
             local_var_files['records'] = local_var_params['records']  # noqa: E501
@@ -1176,15 +1186,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['multipart/form-data'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/{instanceid}/tsv/{v}/{type}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `wds-client-0.2.8/wds_client/api_client.py` & `wds-client-0.2.80/wds_client/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.2.8/python'
+        self.user_agent = 'OpenAPI-Generator/0.2.80/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.8/wds_client/configuration.py` & `wds-client-0.2.80/wds_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
@@ -46,14 +46,15 @@
       2. The client was generated using an older version of the OpenAPI document
          and the server has been upgraded since then.
       If a schema in the OpenAPI document defines the additionalProperties attribute,
       then all undeclared properties received by the server are injected into the
       additional properties map. In that case, there are undeclared properties, and
       nothing to discard.
 
+    :Example:
     """
 
     _default = None
 
     def __init__(self, host="http://..",
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -84,14 +85,17 @@
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
+        self.access_token = None
+        """access token for OAuth/Bearer
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("wds_client")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -310,26 +314,33 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if self.access_token is not None:
+            auth['bearerAuth'] = {
+                'type': 'bearer',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
+            }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.8".\
+               "SDK Package Version: 0.2.80".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.8/wds_client/exceptions.py` & `wds-client-0.2.80/wds_client/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `wds-client-0.2.8/wds_client/models/attribute_schema.py` & `wds-client-0.2.80/wds_client/models/attribute_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -103,15 +103,15 @@
         Datatype of this attribute. The enum of datatypes is in flux and will change. Please comment at https://docs.google.com/document/d/1d352ZoN5kEYWPjy0NqqWGxdf7HEu5VEdrLmiAv7dMmQ/edit#heading=h.naxag0augkgf.   # noqa: E501
 
         :param datatype: The datatype of this AttributeSchema.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and datatype is None:  # noqa: E501
             raise ValueError("Invalid value for `datatype`, must not be `None`")  # noqa: E501
-        allowed_values = ["boolean", "date", "datetime", "string", "json", "long", "double", "relation", "array_of_boolean", "array_of_string", "array_of_number", "array_of_date", "array_of_datetime"]  # noqa: E501
+        allowed_values = ["BOOLEAN", "NUMBER", "DATE", "DATE_TIME", "STRING", "JSON", "RELATION", "FILE", "ARRAY_OF_BOOLEAN", "ARRAY_OF_STRING", "ARRAY_OF_NUMBER", "ARRAY_OF_DATE", "ARRAY_OF_DATE_TIME", "ARRAY_OF_RELATION", "ARRAY_OF_FILE"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and datatype not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `datatype` ({0}), must be one of {1}"  # noqa: E501
                 .format(datatype, allowed_values)
             )
 
         self._datatype = datatype
```

### Comparing `wds-client-0.2.8/wds_client/models/batch_operation.py` & `wds-client-0.2.80/wds_client/models/batch_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/batch_record_request.py` & `wds-client-0.2.80/wds_client/models/batch_record_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -59,70 +59,76 @@
         self.type = type
         self.attributes = attributes
 
     @property
     def id(self):
         """Gets the id of this BatchRecordRequest.  # noqa: E501
 
+        Record id  # noqa: E501
 
         :return: The id of this BatchRecordRequest.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this BatchRecordRequest.
 
+        Record id  # noqa: E501
 
         :param id: The id of this BatchRecordRequest.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this BatchRecordRequest.  # noqa: E501
 
+        Record type  # noqa: E501
 
         :return: The type of this BatchRecordRequest.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this BatchRecordRequest.
 
+        Record type  # noqa: E501
 
         :param type: The type of this BatchRecordRequest.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
         self._type = type
 
     @property
     def attributes(self):
         """Gets the attributes of this BatchRecordRequest.  # noqa: E501
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
         :return: The attributes of this BatchRecordRequest.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._attributes
 
     @attributes.setter
     def attributes(self, attributes):
         """Sets the attributes of this BatchRecordRequest.
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
         :param attributes: The attributes of this BatchRecordRequest.  # noqa: E501
         :type: dict(str, object)
         """
         if self.local_vars_configuration.client_side_validation and attributes is None:  # noqa: E501
             raise ValueError("Invalid value for `attributes`, must not be `None`")  # noqa: E501
```

### Comparing `wds-client-0.2.8/wds_client/models/batch_response.py` & `wds-client-0.2.80/wds_client/models/batch_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/error_response.py` & `wds-client-0.2.80/wds_client/models/error_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/inline_object.py` & `wds-client-0.2.80/wds_client/models/inline_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/record_attribute_definition.py` & `wds-client-0.2.80/wds_client/models/record_attribute_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/record_query_response.py` & `wds-client-0.2.80/wds_client/models/record_query_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/record_request.py` & `wds-client-0.2.80/wds_client/models/record_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -51,24 +51,26 @@
 
         self.attributes = attributes
 
     @property
     def attributes(self):
         """Gets the attributes of this RecordRequest.  # noqa: E501
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
         :return: The attributes of this RecordRequest.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._attributes
 
     @attributes.setter
     def attributes(self, attributes):
         """Sets the attributes of this RecordRequest.
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
         :param attributes: The attributes of this RecordRequest.  # noqa: E501
         :type: dict(str, object)
         """
         if self.local_vars_configuration.client_side_validation and attributes is None:  # noqa: E501
             raise ValueError("Invalid value for `attributes`, must not be `None`")  # noqa: E501
```

### Comparing `wds-client-0.2.8/wds_client/models/record_response.py` & `wds-client-0.2.80/wds_client/models/record_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
@@ -59,70 +59,76 @@
         self.type = type
         self.attributes = attributes
 
     @property
     def id(self):
         """Gets the id of this RecordResponse.  # noqa: E501
 
+        Record id  # noqa: E501
 
         :return: The id of this RecordResponse.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """Sets the id of this RecordResponse.
 
+        Record id  # noqa: E501
 
         :param id: The id of this RecordResponse.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def type(self):
         """Gets the type of this RecordResponse.  # noqa: E501
 
+        Record type  # noqa: E501
 
         :return: The type of this RecordResponse.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this RecordResponse.
 
+        Record type  # noqa: E501
 
         :param type: The type of this RecordResponse.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
         self._type = type
 
     @property
     def attributes(self):
         """Gets the attributes of this RecordResponse.  # noqa: E501
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
         :return: The attributes of this RecordResponse.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._attributes
 
     @attributes.setter
     def attributes(self, attributes):
         """Sets the attributes of this RecordResponse.
 
+        KVPs of record attributes, valid characters for attribute names are limited to letters, numbers, spaces, dashes, and underscores.  # noqa: E501
 
         :param attributes: The attributes of this RecordResponse.  # noqa: E501
         :type: dict(str, object)
         """
         if self.local_vars_configuration.client_side_validation and attributes is None:  # noqa: E501
             raise ValueError("Invalid value for `attributes`, must not be `None`")  # noqa: E501
```

### Comparing `wds-client-0.2.8/wds_client/models/record_type_schema.py` & `wds-client-0.2.80/wds_client/models/record_type_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/request_body_search.py` & `wds-client-0.2.80/wds_client/models/request_body_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/search_operator.py` & `wds-client-0.2.80/wds_client/models/search_operator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/search_request.py` & `wds-client-0.2.80/wds_client/models/search_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/search_sort_direction.py` & `wds-client-0.2.80/wds_client/models/search_sort_direction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/stack_trace_element.py` & `wds-client-0.2.80/wds_client/models/stack_trace_element.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/models/tsv_upload_response.py` & `wds-client-0.2.80/wds_client/models/tsv_upload_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
```

### Comparing `wds-client-0.2.8/wds_client/rest.py` & `wds-client-0.2.80/wds_client/rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Workspace Data Service
 
-    This page lists both current and proposed APIs. The proposed APIs which have not yet been implemented are marked as deprecated. This is incongruous, but by using the deprecated flag, we can force swagger-ui to display those endpoints differently.  Error codes and responses for proposed APIs are likely to change as we gain more clarity on their implementation.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
+    This page lists current APIs.  As of v0.2, all APIs are subject to change without notice.   # noqa: E501
 
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `wds-client-0.2.8/wds_client.egg-info/SOURCES.txt` & `wds-client-0.2.80/wds_client.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 README.md
 setup.cfg
 setup.py
 test/test_attribute_schema.py
 test/test_batch_operation.py
 test/test_batch_record_request.py
 test/test_batch_response.py
+test/test_build.py
+test/test_commit.py
+test/test_component.py
+test/test_components.py
+test/test_db_component.py
 test/test_error_response.py
 test/test_general_wds_information_api.py
+test/test_git.py
 test/test_inline_object.py
 test/test_instances_api.py
 test/test_record_attribute_definition.py
 test/test_record_query_response.py
 test/test_record_request.py
 test/test_record_response.py
 test/test_record_type_schema.py
 test/test_records_api.py
 test/test_request_body_search.py
 test/test_schema_api.py
 test/test_search_operator.py
 test/test_search_request.py
 test/test_search_sort_direction.py
 test/test_stack_trace_element.py
+test/test_status_response.py
 test/test_tsv_upload_response.py
+test/test_version_response.py
 wds_client/__init__.py
 wds_client/api_client.py
 wds_client/configuration.py
 wds_client/exceptions.py
 wds_client/rest.py
 wds_client.egg-info/PKG-INFO
 wds_client.egg-info/SOURCES.txt
@@ -38,20 +46,28 @@
 wds_client/api/records_api.py
 wds_client/api/schema_api.py
 wds_client/models/__init__.py
 wds_client/models/attribute_schema.py
 wds_client/models/batch_operation.py
 wds_client/models/batch_record_request.py
 wds_client/models/batch_response.py
+wds_client/models/build.py
+wds_client/models/commit.py
+wds_client/models/component.py
+wds_client/models/components.py
+wds_client/models/db_component.py
 wds_client/models/error_response.py
+wds_client/models/git.py
 wds_client/models/inline_object.py
 wds_client/models/record_attribute_definition.py
 wds_client/models/record_query_response.py
 wds_client/models/record_request.py
 wds_client/models/record_response.py
 wds_client/models/record_type_schema.py
 wds_client/models/request_body_search.py
 wds_client/models/search_operator.py
 wds_client/models/search_request.py
 wds_client/models/search_sort_direction.py
 wds_client/models/stack_trace_element.py
-wds_client/models/tsv_upload_response.py
+wds_client/models/status_response.py
+wds_client/models/tsv_upload_response.py
+wds_client/models/version_response.py
```


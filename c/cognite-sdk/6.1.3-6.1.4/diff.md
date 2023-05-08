# Comparing `tmp/cognite_sdk-6.1.3.tar.gz` & `tmp/cognite_sdk-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.1.3.tar", max compression
+gzip compressed data, was "cognite_sdk-6.1.4.tar", max compression
```

## Comparing `cognite_sdk-6.1.3.tar` & `cognite_sdk-6.1.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/LICENSE
--rw-r--r--   0        0        0     3945 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/README.md
--rw-r--r--   0        0        0      503 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87464 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44656 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49922 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/config.py
--rw-r--r--   0        0        0    16261 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    22565 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2132 2023-05-08 13:08:14.315463 cognite_sdk-6.1.3/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/LICENSE
+-rw-r--r--   0        0        0     3945 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/README.md
+-rw-r--r--   0        0        0      503 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87464 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17436 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44656 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49922 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/config.py
+-rw-r--r--   0        0        0    18062 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14287 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    22565 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-05-08 14:13:34.978338 cognite_sdk-6.1.4/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2132 2023-05-08 14:13:34.978338 cognite_sdk-6.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.4/PKG-INFO
```

### Comparing `cognite_sdk-6.1.3/LICENSE` & `cognite_sdk-6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/README.md` & `cognite_sdk-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/annotations.py` & `cognite_sdk-6.1.4/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/assets.py` & `cognite_sdk-6.1.4/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/data_sets.py` & `cognite_sdk-6.1.4/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.1.4/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/datapoints.py` & `cognite_sdk-6.1.4/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/diagrams.py` & `cognite_sdk-6.1.4/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.1.4/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/events.py` & `cognite_sdk-6.1.4/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.1.4/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/files.py` & `cognite_sdk-6.1.4/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/functions.py` & `cognite_sdk-6.1.4/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/geospatial.py` & `cognite_sdk-6.1.4/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/iam.py` & `cognite_sdk-6.1.4/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/labels.py` & `cognite_sdk-6.1.4/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/raw.py` & `cognite_sdk-6.1.4/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/relationships.py` & `cognite_sdk-6.1.4/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/sequences.py` & `cognite_sdk-6.1.4/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.1.4/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/templates.py` & `cognite_sdk-6.1.4/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/three_d.py` & `cognite_sdk-6.1.4/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/time_series.py` & `cognite_sdk-6.1.4/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.1.4/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.1.4/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.1.4/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.1.4/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.1.4/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api/vision.py` & `cognite_sdk-6.1.4/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_api_client.py` & `cognite_sdk-6.1.4/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_cognite_client.py` & `cognite_sdk-6.1.4/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_http_client.py` & `cognite_sdk-6.1.4/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.1.4/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/config.py` & `cognite_sdk-6.1.4/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/credentials.py` & `cognite_sdk-6.1.4/cognite/client/credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,25 @@
     __TOKEN_EXPIRY_LEEWAY_SECONDS = 3
 
     def __init__(self) -> None:
         self.__token_refresh_lock = threading.Lock()
         self.__access_token: Optional[str] = None
         self.__access_token_expires_at: Optional[float] = None
 
+    def __getstate__(self) -> dict[str, Any]:
+        # threading.Lock is not picklable, temporarily remove:
+        lock_tmp, self.__token_refresh_lock = self.__token_refresh_lock, None  # type: ignore [assignment]
+        state = self.__dict__.copy()
+        self.__token_refresh_lock = lock_tmp
+        return state
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        self.__dict__ = state
+        self.__token_refresh_lock = threading.Lock()
+
     @abstractmethod
     def _refresh_access_token(self) -> Tuple[str, float]:
         """This method should return the access_token and expiry time"""
         raise NotImplementedError
 
     @classmethod
     def __should_refresh_token(cls, token: Optional[str], expires_at: Optional[float]) -> bool:
@@ -114,14 +125,30 @@
             if token_cache.has_state_changed:
                 with open(cache_path, "w+") as fh:
                     fh.write(token_cache.serialize())
 
         atexit.register(__at_exit)
         return token_cache
 
+    @staticmethod
+    def _resolve_token_cache_path(token_cache_path: Optional[Path], client_id: str) -> Path:
+        return token_cache_path or Path(tempfile.gettempdir()) / f"cognitetokencache.{client_id}.bin"
+
+    def _create_client_app(self, token_cache_path: Path, client_id: str, authority_url: str) -> PublicClientApplication:
+        from cognite.client.config import global_config
+
+        # In addition to caching in memory, we also cache the token on disk so it can be reused across processes:
+        serializable_token_cache = self._create_serializable_token_cache(token_cache_path)
+        return PublicClientApplication(
+            client_id=client_id,
+            authority=authority_url,
+            token_cache=serializable_token_cache,
+            verify=not global_config.disable_ssl,
+        )
+
 
 class OAuthDeviceCode(_OAuthCredentialProviderWithTokenRefresh, _WithMsalSerializableTokenCache):
     """OAuth credential provider for the device code login flow.
 
     Args:
         authority_url (str): OAuth authority url
         client_id (str): Your application's client id.
@@ -142,30 +169,32 @@
     def __init__(
         self,
         authority_url: str,
         client_id: str,
         scopes: List[str],
         token_cache_path: Path = None,
     ) -> None:
-        from cognite.client.config import global_config
-
         super().__init__()
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__scopes = scopes
 
-        # In addition to caching in memory, we also cache the token on disk so it can be reused across processes.
-        token_cache_path = token_cache_path or Path(tempfile.gettempdir()) / f"cognitetokencache.{self.__client_id}.bin"
-        serializable_token_cache = self._create_serializable_token_cache(token_cache_path)
-        self.__app = PublicClientApplication(
-            client_id=self.__client_id,
-            authority=self.__authority_url,
-            token_cache=serializable_token_cache,
-            verify=not global_config.disable_ssl,
-        )
+        self._token_cache_path = self._resolve_token_cache_path(token_cache_path, client_id)
+        self.__app = self._create_client_app(self._token_cache_path, client_id, authority_url)
+
+    def __getstate__(self) -> dict[str, Any]:
+        # PublicClientApplication is not picklable, temporarily remove:
+        app_tmp, self.__app = self.__app, None
+        state = super().__getstate__()
+        self.__app = app_tmp
+        return state
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        super().__setstate__(state)
+        self.__app = self._create_client_app(self._token_cache_path, self.__client_id, self.__authority_url)
 
     @property
     def authority_url(self) -> str:
         return self.__authority_url
 
     @property
     def client_id(self) -> str:
@@ -173,19 +202,18 @@
 
     @property
     def scopes(self) -> List[str]:
         return self.__scopes
 
     def _refresh_access_token(self) -> Tuple[str, float]:
         # First check if there is a serialized token cached on disk.
-        accounts = self.__app.get_accounts()
-        credentials = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0]) if accounts else None
-
-        # If not, we acquire a new token interactively
-        if credentials is None:
+        if accounts := self.__app.get_accounts():
+            credentials = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0])
+        # If not, we acquire a new token using device code auth flow:
+        else:
             device_flow = self.__app.initiate_device_flow(scopes=self.__scopes)
             # print device code user instructions to screen
             print(f"Device code: {device_flow['message']}")  # noqa: T201
             credentials = self.__app.acquire_token_by_device_flow(flow=device_flow)
 
         self._verify_credentials(credentials)
         return credentials["access_token"], time.time() + credentials["expires_in"]
@@ -218,31 +246,34 @@
         self,
         authority_url: str,
         client_id: str,
         scopes: List[str],
         redirect_port: int = 53000,
         token_cache_path: Path = None,
     ) -> None:
-        from cognite.client.config import global_config
 
         super().__init__()
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__scopes = scopes
         self.__redirect_port = redirect_port
 
-        # In addition to caching in memory, we also cache the token on disk so it can be reused across processes.
-        token_cache_path = token_cache_path or Path(tempfile.gettempdir()) / f"cognitetokencache.{self.__client_id}.bin"
-        serializable_token_cache = self._create_serializable_token_cache(token_cache_path)
-        self.__app = PublicClientApplication(
-            client_id=self.__client_id,
-            authority=self.__authority_url,
-            token_cache=serializable_token_cache,
-            verify=not global_config.disable_ssl,
-        )
+        self._token_cache_path = self._resolve_token_cache_path(token_cache_path, client_id)
+        self.__app = self._create_client_app(self._token_cache_path, client_id, authority_url)
+
+    def __getstate__(self) -> dict[str, Any]:
+        # PublicClientApplication is not picklable, temporarily remove:
+        app_tmp, self.__app = self.__app, None
+        state = super().__getstate__()
+        self.__app = app_tmp
+        return state
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        super().__setstate__(state)
+        self.__app = self._create_client_app(self._token_cache_path, self.__client_id, self.__authority_url)
 
     @property
     def authority_url(self) -> str:
         return self.__authority_url
 
     @property
     def client_id(self) -> str:
@@ -250,19 +281,18 @@
 
     @property
     def scopes(self) -> List[str]:
         return self.__scopes
 
     def _refresh_access_token(self) -> Tuple[str, float]:
         # First check if there is a serialized token cached on disk.
-        accounts = self.__app.get_accounts()
-        credentials = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0]) if accounts else None
-
+        if accounts := self.__app.get_accounts():
+            credentials = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0])
         # If not, we acquire a new token interactively
-        if credentials is None:
+        else:
             credentials = self.__app.acquire_token_interactive(scopes=self.__scopes, port=self.__redirect_port)
 
         self._verify_credentials(credentials)
         return credentials["access_token"], time.time() + credentials["expires_in"]
 
 
 class OAuthClientCredentials(_OAuthCredentialProviderWithTokenRefresh):
@@ -299,27 +329,41 @@
     ):
         super().__init__()
         self.__token_url = token_url
         self.__client_id = client_id
         self.__client_secret = client_secret
         self.__scopes = scopes
         self.__token_custom_args: Dict[str, Any] = token_custom_args
-        self.__oauth = OAuth2Session(client=BackendApplicationClient(client_id=self.__client_id, scope=self.__scopes))
+        self.__oauth = self._create_oauth_session()
         self._validate_token_custom_args()
 
+    def _create_oauth_session(self) -> OAuth2Session:
+        return OAuth2Session(client=BackendApplicationClient(client_id=self.__client_id, scope=self.__scopes))
+
     def _validate_token_custom_args(self) -> None:
         # We make sure that whatever is passed as part of 'token_custom_args' can't set or override any of the
         # named parameters that 'fetch_token' accepts:
         reserved = set(inspect.signature(self.__oauth.fetch_token).parameters) - {"kwargs"}
         if bad_args := reserved.intersection(self.__token_custom_args):
             raise TypeError(
                 f"The following reserved token custom arg(s) were passed: {sorted(bad_args)}. The full list of "
                 f"reserved custom args is: {sorted(reserved)}."
             )
 
+    def __getstate__(self) -> dict[str, Any]:
+        # OAuth2Session is not picklable, temporarily remove:
+        oauth_session_tmp, self.__oauth = self.__oauth, None
+        state = super().__getstate__()
+        self.__oauth = oauth_session_tmp
+        return state
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        super().__setstate__(state)
+        self.__oauth = self._create_oauth_session()
+
     @property
     def token_url(self) -> str:
         return self.__token_url
 
     @property
     def client_id(self) -> str:
         return self.__client_id
```

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/_base.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/assets.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/events.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/files.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/functions.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/iam.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/labels.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/raw.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/shared.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/templates.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/exceptions.py` & `cognite_sdk-6.1.4/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/testing.py` & `cognite_sdk-6.1.4/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/__init__.py` & `cognite_sdk-6.1.4/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.1.4/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.1.4/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_graph.py` & `cognite_sdk-6.1.4/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_identifier.py` & `cognite_sdk-6.1.4/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_logging.py` & `cognite_sdk-6.1.4/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.1.4/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.1.4/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.1.4/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_text.py` & `cognite_sdk-6.1.4/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_time.py` & `cognite_sdk-6.1.4/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_validation.py` & `cognite_sdk-6.1.4/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.1.4/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.3/pyproject.toml` & `cognite_sdk-6.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.1.3"
+version = "6.1.4"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.1.3/PKG-INFO` & `cognite_sdk-6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.1.3
+Version: 6.1.4
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.3 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.4 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```


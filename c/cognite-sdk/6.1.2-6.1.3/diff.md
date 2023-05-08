# Comparing `tmp/cognite_sdk-6.1.2.tar.gz` & `tmp/cognite_sdk-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.1.2.tar", max compression
+gzip compressed data, was "cognite_sdk-6.1.3.tar", max compression
```

## Comparing `cognite_sdk-6.1.2.tar` & `cognite_sdk-6.1.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/LICENSE
--rw-r--r--   0        0        0     3945 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/README.md
--rw-r--r--   0        0        0      503 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87464 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-05-04 08:19:33.654246 cognite_sdk-6.1.2/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44656 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49922 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/config.py
--rw-r--r--   0        0        0    16261 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-05-04 08:19:33.658246 cognite_sdk-6.1.2/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    22565 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24907 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-05-04 08:19:33.662246 cognite_sdk-6.1.2/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2109 2023-05-04 08:19:33.666246 cognite_sdk-6.1.2/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 cognite_sdk-6.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/LICENSE
+-rw-r--r--   0        0        0     3945 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/README.md
+-rw-r--r--   0        0        0      503 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-05-08 13:08:14.303463 cognite_sdk-6.1.3/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87464 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17436 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44656 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49922 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/config.py
+-rw-r--r--   0        0        0    16261 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-05-08 13:08:14.307463 cognite_sdk-6.1.3/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14287 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    22565 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-05-08 13:08:14.311463 cognite_sdk-6.1.3/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2132 2023-05-08 13:08:14.315463 cognite_sdk-6.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.3/PKG-INFO
```

### Comparing `cognite_sdk-6.1.2/LICENSE` & `cognite_sdk-6.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/README.md` & `cognite_sdk-6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/annotations.py` & `cognite_sdk-6.1.3/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/assets.py` & `cognite_sdk-6.1.3/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/data_sets.py` & `cognite_sdk-6.1.3/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.1.3/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/datapoints.py` & `cognite_sdk-6.1.3/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/diagrams.py` & `cognite_sdk-6.1.3/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.1.3/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/events.py` & `cognite_sdk-6.1.3/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.1.3/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/files.py` & `cognite_sdk-6.1.3/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/functions.py` & `cognite_sdk-6.1.3/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/geospatial.py` & `cognite_sdk-6.1.3/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/iam.py` & `cognite_sdk-6.1.3/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/labels.py` & `cognite_sdk-6.1.3/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/raw.py` & `cognite_sdk-6.1.3/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/relationships.py` & `cognite_sdk-6.1.3/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/sequences.py` & `cognite_sdk-6.1.3/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.1.3/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/templates.py` & `cognite_sdk-6.1.3/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/three_d.py` & `cognite_sdk-6.1.3/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/time_series.py` & `cognite_sdk-6.1.3/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.1.3/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.1.3/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.1.3/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.1.3/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.1.3/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api/vision.py` & `cognite_sdk-6.1.3/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_api_client.py` & `cognite_sdk-6.1.3/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_cognite_client.py` & `cognite_sdk-6.1.3/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_http_client.py` & `cognite_sdk-6.1.3/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.3/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.1.3/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.1.3/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.1.3/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/config.py` & `cognite_sdk-6.1.3/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/credentials.py` & `cognite_sdk-6.1.3/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/_base.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/assets.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/events.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/files.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/functions.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/iam.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/labels.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/raw.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/shared.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/templates.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.1.3/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/exceptions.py` & `cognite_sdk-6.1.3/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/testing.py` & `cognite_sdk-6.1.3/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/__init__.py` & `cognite_sdk-6.1.3/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.1.3/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.1.3/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_graph.py` & `cognite_sdk-6.1.3/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_identifier.py` & `cognite_sdk-6.1.3/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_logging.py` & `cognite_sdk-6.1.3/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.1.3/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.1.3/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.1.3/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_text.py` & `cognite_sdk-6.1.3/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_time.py` & `cognite_sdk-6.1.3/cognite/client/utils/_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 def import_zoneinfo() -> type[ZoneInfo]:
     try:
         if sys.version_info >= (3, 9):
             from zoneinfo import ZoneInfo
         else:
             from backports.zoneinfo import ZoneInfo
-        return ZoneInfo  # type: ignore [return-value]
+        return ZoneInfo
 
     except ImportError as e:
         raise CogniteImportError(
             "ZoneInfo is part of the standard library starting with Python >=3.9. In earlier versions "
             "you need to install a backport. This is done automatically for you when installing with the pandas "
             "group: 'cognite-sdk[pandas]', or with poetry: 'poetry install -E pandas'"
         ) from e
@@ -54,15 +54,15 @@
         from zoneinfo import ZoneInfoNotFoundError
     else:
         from backports.zoneinfo import ZoneInfoNotFoundError
     return ZoneInfoNotFoundError
 
 
 def get_utc_zoneinfo() -> ZoneInfo:
-    return import_zoneinfo()("UTC")  # type: ignore [operator]
+    return import_zoneinfo()("UTC")
 
 
 def datetime_to_ms(dt: datetime) -> int:
     """Converts a datetime object to milliseconds since epoch.
 
     Args:
         dt (datetime): Naive or aware datetime object. Naive datetimes are interpreted as local time.
@@ -214,15 +214,17 @@
     if remainder := (end - start) % gms:
         # Ceil `end` when not exactly at boundary decided by `start + N * granularity`
         end += gms - remainder
     return start, end
 
 
 class DateTimeAligner(ABC):
-    _zeros_upto_hour = dict(hour=0, minute=0, second=0, microsecond=0)
+    @staticmethod
+    def normalize(date: datetime) -> datetime:
+        return date.replace(hour=0, minute=0, second=0, microsecond=0)
 
     @classmethod
     @abstractmethod
     def ceil(cls, date: datetime) -> datetime:
         ...
 
     @classmethod
@@ -240,19 +242,19 @@
     def add_units(cls, date: datetime, units: int) -> datetime:
         ...
 
 
 class DayAligner(DateTimeAligner):
     @classmethod
     def floor(cls, date: datetime) -> datetime:
-        return date.replace(**cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date)
 
     @classmethod
     def ceil(cls, date: datetime) -> datetime:
-        return date.replace(**cls._zeros_upto_hour) + timedelta(days=1)  # type: ignore [arg-type]
+        return cls.normalize(date) + timedelta(days=1)
 
     @classmethod
     def units_between(cls, start: datetime, end: datetime) -> int:
         return math.floor((end - start) / timedelta(days=1))
 
     @classmethod
     def add_units(cls, date: datetime, units: int) -> datetime:
@@ -263,27 +265,27 @@
     @classmethod
     def ceil(cls, date: datetime) -> datetime:
         """
         Ceils the date to the next monday
         >>> WeekAligner.ceil(datetime(2023, 4, 9 ))
         datetime.datetime(2023, 4, 10, 0, 0)
         """
-        date = date.replace(**cls._zeros_upto_hour)  # type: ignore [arg-type]
+        date = cls.normalize(date)
         if (weekday := date.weekday()) != 0:
             return date + timedelta(days=7 - weekday)
         return date
 
     @classmethod
     def floor(cls, date: datetime) -> datetime:
         """
         Floors the date to the nearest monday
         >>> WeekAligner.floor(datetime(2023, 4, 9))
         datetime.datetime(2023, 4, 3, 0, 0)
         """
-        date = date.replace(**cls._zeros_upto_hour)  # type: ignore [arg-type]
+        date = cls.normalize(date)
         if (weekday := date.weekday()) != 0:
             return date - timedelta(days=weekday)
         return date
 
     @classmethod
     def units_between(cls, start: datetime, end: datetime) -> int:
         return math.floor((end - start) / timedelta(days=7))
@@ -307,19 +309,19 @@
         datetime.datetime(2024, 1, 1, 0, 0)
         >>> MonthAligner.ceil(datetime(2024, 1, 10))
         datetime.datetime(2024, 2, 1, 0, 0)
         """
         if date == datetime(year=date.year, month=date.month, day=1, tzinfo=date.tzinfo):
             return date
         extra, month = divmod(date.month + 1, 12)
-        return date.replace(year=date.year + extra, month=month, day=1, **cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date.replace(year=date.year + extra, month=month, day=1))
 
     @classmethod
     def floor(cls, date: datetime) -> datetime:
-        return date.replace(day=1, **cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date.replace(day=1))
 
     @classmethod
     def units_between(cls, start: datetime, end: datetime) -> int:
         return (end.year - start.year) * 12 + end.month - start.month
 
     @classmethod
     def add_units(cls, date: datetime, units: int) -> datetime:
@@ -340,29 +342,29 @@
         >>> QuarterAligner.ceil(datetime(2023, 1, 1))
         datetime.datetime(2023, 1, 1, 0, 0)
         """
         if any(date == datetime(date.year, month, 1, tzinfo=date.tzinfo) for month in [1, 4, 7, 10]):
             return date
         month = 3 * ((date.month - 1) // 3 + 1) + 1
         add_years, month = divmod(month, 12)
-        return date.replace(year=date.year + add_years, month=month, day=1, **cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date.replace(year=date.year + add_years, month=month, day=1))
 
     @classmethod
     def floor(cls, date: datetime) -> datetime:
         """
         Floors the months to start of quarter.
         >>> QuarterAligner.floor(datetime(2023, 3, 1))
         datetime.datetime(2023, 1, 1, 0, 0)
         >>> QuarterAligner.floor(datetime(2023, 8, 1))
         datetime.datetime(2023, 7, 1, 0, 0)
         >>> QuarterAligner.floor(datetime(2023, 12, 1))
         datetime.datetime(2023, 10, 1, 0, 0)
         """
         month = 3 * ((date.month - 1) // 3) + 1
-        return date.replace(month=month, day=1, **cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date.replace(month=month, day=1))
 
     @classmethod
     def units_between(cls, start: datetime, end: datetime) -> int:
         return (end.year - start.year) * 4 + (end.month - start.month) // 3
 
     @classmethod
     def add_units(cls, date: datetime, units: int) -> datetime:
@@ -371,19 +373,19 @@
 
 
 class YearAligner(DateTimeAligner):
     @classmethod
     def ceil(cls, date: datetime) -> datetime:
         if date == datetime(date.year, 1, 1, tzinfo=date.tzinfo):
             return date
-        return date.replace(year=date.year + 1, month=1, day=1, **cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date.replace(year=date.year + 1, month=1, day=1))
 
     @classmethod
     def floor(cls, date: datetime) -> datetime:
-        return date.replace(month=1, day=1, **cls._zeros_upto_hour)  # type: ignore [arg-type]
+        return cls.normalize(date.replace(month=1, day=1))
 
     @classmethod
     def units_between(cls, start: datetime, end: datetime) -> int:
         return end.year - start.year
 
     @classmethod
     def add_units(cls, date: datetime, units: int) -> datetime:
@@ -505,55 +507,55 @@
     freq = multiplier * GRANULARITY_IN_HOURS[unit]
     index = pandas_date_range_tz(start, end, to_pandas_freq(f"{multiplier}{unit}", start))
     utc_offsets = pd.Series([t.utcoffset() for t in index], index=index)
     transition_raw = index[(utc_offsets != utc_offsets.shift(-1)) | (utc_offsets != utc_offsets.shift(1))]
 
     hour, zero = pd.Timedelta(hours=1), pd.Timedelta(0)
     transitions = []
-    for start, end in zip(transition_raw[:-1], transition_raw[1:]):
-        if start.dst() == end.dst():
+    for t_start, t_end in zip(transition_raw[:-1], transition_raw[1:]):
+        if t_start.dst() == t_end.dst():
             dst_adjustment = 0
-        elif start.dst() == hour and end.dst() == zero:
-            # Fall, going away from summer.
+        elif t_start.dst() == hour and t_end.dst() == zero:
+            # Fall, going away from summer (above the equator).
             dst_adjustment = 1
-        elif start.dst() == zero and end.dst() == hour:
-            # Spring, going to summer.
+        elif t_start.dst() == zero and t_end.dst() == hour:
+            # Spring, going to summer (above the equator).
             dst_adjustment = -1
         else:
-            raise ValueError(f"Invalid dst, {start} and {end}")
+            raise ValueError(f"Invalid dst, {t_start} and {t_end}")
 
         transitions.append(
             {
-                "start": start.to_pydatetime().astimezone(utc),  # type: ignore
-                "end": end.to_pydatetime().astimezone(utc),  # type: ignore
+                "start": t_start.to_pydatetime().astimezone(utc),
+                "end": t_end.to_pydatetime().astimezone(utc),
                 "granularity": f"{freq+dst_adjustment}h",
             }
         )
     return transitions
 
 
 def pandas_date_range_tz(start: datetime, end: datetime, freq: str, inclusive: str = "both") -> pandas.DatetimeIndex:
     """
     Pandas date_range struggles with time zone aware datetimes.
     This function overcomes that limitation.
 
     Assumes that start and end have the same timezone.
     """
-    pd = local_import("pandas")
+    pd = cast(Any, local_import("pandas"))
     # There is a bug in date_range which makes it fail to handle ambiguous timestamps when you use time zone aware
     # datetimes. This is a workaround by passing the time zone as an argument to the function.
     # In addition, pandas struggle with ZoneInfo objects, so we convert them to string so that pandas can use its own
     # tzdata implementation.
 
     # An ambiguous timestamp is for example 1916-10-01 00:00:00 Europe/Oslo, as this corresponds to two different points in time,
     # 1916-10-01 00:00:00+02:00 and 1916-10-01 00:00:00+01:00; before and after the DST transition.
     # (Back in 1916 they did not consider the needs of software engineers in 2023 :P).
     # Setting ambiguous=True will make pandas ignore the ambiguity and use the DST timestamp. This is what we want;
     # for a user requesting monthly aggregates, we don't want to miss the first hour of the month.
-    return pd.date_range(  # type: ignore [union-attr]
+    return pd.date_range(
         start.replace(tzinfo=None),
         end.replace(tzinfo=None),
         tz=str(start.tzinfo),
         freq=freq,
         inclusive=inclusive,
         nonexistent="shift_forward",
         ambiguous=True,
```

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_validation.py` & `cognite_sdk-6.1.3/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.1.3/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.2/pyproject.toml` & `cognite_sdk-6.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.1.2"
+version = "6.1.3"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
+license = "Apache-2.0"
 
 packages = [{ include="cognite", from="." }]
 
 [tool.ruff.pyupgrade]
 keep-runtime-typing = true
 
 [tool.ruff.per-file-ignores]
```

### Comparing `cognite_sdk-6.1.2/PKG-INFO` & `cognite_sdk-6.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.1.2
+Version: 6.1.3
 Summary: Cognite Python SDK
+License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: functions
```

#### html2text {}

```diff
@@ -1,71 +1,72 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.2 Summary: Cognite Python
-SDK Author: Erlend Vollset Author-email: erlend.vollset@cognite.com Requires-
-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
-functions Provides-Extra: geo Provides-Extra: numpy Provides-Extra: pandas
-Provides-Extra: pyodide Provides-Extra: sympy Requires-Dist: backports-zoneinfo
-[tzdata] (>=0.2.1) ; (python_version < "3.9") and (extra == "pandas" or extra
-== "all") Requires-Dist: geopandas (>=0.10.0) ; extra == "geo" or extra ==
-"all" Requires-Dist: graphlib-backport (>=1.0.0,<2.0.0) ; python_version <
-"3.9" Requires-Dist: msal (>=1,<2) Requires-Dist: numpy (>=1.20,<2.0) ; extra
-== "numpy" Requires-Dist: pandas (>=1.4) ; extra == "pandas" or extra == "all"
-Requires-Dist: pip (>=20.0.0) ; extra == "functions" or extra == "all"
-Requires-Dist: protobuf (>=3.16.0) Requires-Dist: pyodide-http (>=0.2.0,<0.3.0)
-; extra == "pyodide" Requires-Dist: requests (>=2,<3) Requires-Dist:
-requests_oauthlib (>=1,<2) Requires-Dist: shapely (>=1.7.0) ; extra == "geo" or
-extra == "all" Requires-Dist: sortedcontainers (>=2.2,<3.0) Requires-Dist:
-sympy ; extra == "sympy" or extra == "all" Requires-Dist: tzdata (>=2023.3) ;
-sys_platform == "win32" Project-URL: Documentation, https://cognite-sdk-
-python.readthedocs-hosted.com Description-Content-Type: text/markdown [Cognite
-logo] Cognite Python SDK ========================== [![build](https://
-github.com/cognitedata/cognite-sdk-python/workflows/release/badge.svg)](https:/
-/github.com/cognitedata/cognite-sdk-python/actions?query=workflow:release) [!
-[Downloads](https://img.shields.io/pypi/dm/cognite-sdk)](https://pypistats.org/
-packages/cognite-sdk) [![GitHub](https://img.shields.io/github/license/
-cognitedata/cognite-sdk-python)](https://github.com/cognitedata/cognite-sdk-
-python/blob/master/LICENSE) [![codecov](https://codecov.io/gh/cognitedata/
-cognite-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/
-cognitedata/cognite-sdk-python) [![Documentation Status](https://
-readthedocs.com/projects/cognite-sdk-python/badge/?version=latest)](https://
-cognite-sdk-python.readthedocs-hosted.com/en/latest/) [![PyPI version](https://
-badge.fury.io/py/cognite-sdk.svg)](https://pypi.org/project/cognite-sdk/) [!
-[mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/ambv/black) This is the Cognite Python SDK for
-developers and data scientists working with Cognite Data Fusion (CDF). The
-package is tightly integrated with pandas, and helps you work easily and
-efficiently with data in Cognite Data Fusion (CDF). ## Refererence
-documentation * [SDK Documentation](https://cognite-sdk-python.readthedocs-
-hosted.com/en/latest/) * [CDF API Documentation](https://doc.cognitedata.com/
-) * [Cognite Developer Documentation](https://docs.cognite.com/dev/) ##
-Installation ### Without any optional dependencies To install this package
-without pandas and geopandas support: ```bash $ pip install cognite-sdk ``` ###
-With optional dependencies A number of optional dependencies may be specified
-in order to support a wider set of features. The available extras (along with
-the libraries they include) are: - numpy `[numpy]` - pandas `[pandas]` - geo `
-[geopandas, shapely]` - sympy `[sympy]` - functions `[pip]` - all `[numpy,
-pandas, geopandas, shapely, sympy, pip]` To include optional dependencies,
-specify them like this with pip: ```bash $ pip install "cognite-sdk[pandas,
-geo]" ``` or like this if you are using poetry: ```bash $ poetry add cognite-
-sdk -E pandas -E geo ``` ### Performance notes If you regularly need to fetch
-large amounts of datapoints, consider installing with `numpy` (or with
-`pandas`, as it depends on `numpy`) for best performance, then use the
-`retrieve_arrays` (or `retrieve_dataframe`) endpoint(s). This avoids building
-large pure Python data structures, and instead reads data directly into memory-
-efficient `numpy.ndarrays`. ### Windows specific On Windows, it is recommended
-to install `geopandas` and its dependencies using `conda` package manager, see
-[geopandas installation page](https://geopandas.org/en/stable/getting_started/
-install.html#installation). The following commands create a new environment,
-install `geopandas` and `cognite-sdk`. ```bash conda create -n geo_env conda
-activate geo_env conda install --channel conda-forge geopandas pip install
-cognite-sdk ``` ## Changelog Wondering about upcoming or previous changes to
-the SDK? Take a look at the [CHANGELOG](https://github.com/cognitedata/cognite-
-sdk-python/blob/master/CHANGELOG.md). ## Migration Guide To help you upgrade
-your code(base) quickly and safely to a newer major version of the SDK, check
-out our migration guide. It is a more focused guide based on the detailed
-change log. [MIGRATION GUIDE](https://github.com/cognitedata/cognite-sdk-
-python/blob/master/MIGRATION_GUIDE.md). ## Contributing Want to contribute?
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.3 Summary: Cognite Python
+SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
+erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
+Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
+Provides-Extra: pandas Provides-Extra: pyodide Provides-Extra: sympy Requires-
+Dist: backports-zoneinfo[tzdata] (>=0.2.1) ; (python_version < "3.9") and
+(extra == "pandas" or extra == "all") Requires-Dist: geopandas (>=0.10.0) ;
+extra == "geo" or extra == "all" Requires-Dist: graphlib-backport
+(>=1.0.0,<2.0.0) ; python_version < "3.9" Requires-Dist: msal (>=1,<2)
+Requires-Dist: numpy (>=1.20,<2.0) ; extra == "numpy" Requires-Dist: pandas
+(>=1.4) ; extra == "pandas" or extra == "all" Requires-Dist: pip (>=20.0.0) ;
+extra == "functions" or extra == "all" Requires-Dist: protobuf (>=3.16.0)
+Requires-Dist: pyodide-http (>=0.2.0,<0.3.0) ; extra == "pyodide" Requires-
+Dist: requests (>=2,<3) Requires-Dist: requests_oauthlib (>=1,<2) Requires-
+Dist: shapely (>=1.7.0) ; extra == "geo" or extra == "all" Requires-Dist:
+sortedcontainers (>=2.2,<3.0) Requires-Dist: sympy ; extra == "sympy" or extra
+== "all" Requires-Dist: tzdata (>=2023.3) ; sys_platform == "win32" Project-
+URL: Documentation, https://cognite-sdk-python.readthedocs-hosted.com
+Description-Content-Type: text/markdown [Cognite_logo] Cognite Python SDK
+========================== [![build](https://github.com/cognitedata/cognite-
+sdk-python/workflows/release/badge.svg)](https://github.com/cognitedata/
+cognite-sdk-python/actions?query=workflow:release) [![Downloads](https://
+img.shields.io/pypi/dm/cognite-sdk)](https://pypistats.org/packages/cognite-
+sdk) [![GitHub](https://img.shields.io/github/license/cognitedata/cognite-sdk-
+python)](https://github.com/cognitedata/cognite-sdk-python/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/cognitedata/cognite-sdk-python/branch/master/
+graph/badge.svg)](https://codecov.io/gh/cognitedata/cognite-sdk-python) [!
+[Documentation Status](https://readthedocs.com/projects/cognite-sdk-python/
+badge/?version=latest)](https://cognite-sdk-python.readthedocs-hosted.com/en/
+latest/) [![PyPI version](https://badge.fury.io/py/cognite-sdk.svg)](https://
+pypi.org/project/cognite-sdk/) [![mypy](http://www.mypy-lang.org/static/
+mypy_badge.svg)](http://mypy-lang.org) [![Code style: black](https://
+img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
+black) This is the Cognite Python SDK for developers and data scientists
+working with Cognite Data Fusion (CDF). The package is tightly integrated with
+pandas, and helps you work easily and efficiently with data in Cognite Data
+Fusion (CDF). ## Refererence documentation * [SDK Documentation](https://
+cognite-sdk-python.readthedocs-hosted.com/en/latest/) * [CDF API Documentation]
+(https://doc.cognitedata.com/) * [Cognite Developer Documentation](https://
+docs.cognite.com/dev/) ## Installation ### Without any optional dependencies To
+install this package without pandas and geopandas support: ```bash $ pip
+install cognite-sdk ``` ### With optional dependencies A number of optional
+dependencies may be specified in order to support a wider set of features. The
+available extras (along with the libraries they include) are: - numpy `[numpy]`
+- pandas `[pandas]` - geo `[geopandas, shapely]` - sympy `[sympy]` - functions
+`[pip]` - all `[numpy, pandas, geopandas, shapely, sympy, pip]` To include
+optional dependencies, specify them like this with pip: ```bash $ pip install
+"cognite-sdk[pandas, geo]" ``` or like this if you are using poetry: ```bash $
+poetry add cognite-sdk -E pandas -E geo ``` ### Performance notes If you
+regularly need to fetch large amounts of datapoints, consider installing with
+`numpy` (or with `pandas`, as it depends on `numpy`) for best performance, then
+use the `retrieve_arrays` (or `retrieve_dataframe`) endpoint(s). This avoids
+building large pure Python data structures, and instead reads data directly
+into memory-efficient `numpy.ndarrays`. ### Windows specific On Windows, it is
+recommended to install `geopandas` and its dependencies using `conda` package
+manager, see [geopandas installation page](https://geopandas.org/en/stable/
+getting_started/install.html#installation). The following commands create a new
+environment, install `geopandas` and `cognite-sdk`. ```bash conda create -
+n geo_env conda activate geo_env conda install --channel conda-forge geopandas
+pip install cognite-sdk ``` ## Changelog Wondering about upcoming or previous
+changes to the SDK? Take a look at the [CHANGELOG](https://github.com/
+cognitedata/cognite-sdk-python/blob/master/CHANGELOG.md). ## Migration Guide To
+help you upgrade your code(base) quickly and safely to a newer major version of
+the SDK, check out our migration guide. It is a more focused guide based on the
+detailed change log. [MIGRATION GUIDE](https://github.com/cognitedata/cognite-
+sdk-python/blob/master/MIGRATION_GUIDE.md). ## Contributing Want to contribute?
 Check out [CONTRIBUTING](https://github.com/cognitedata/cognite-sdk-python/
 blob/master/CONTRIBUTING.md).
```


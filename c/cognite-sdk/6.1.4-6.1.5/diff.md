# Comparing `tmp/cognite_sdk-6.1.4.tar.gz` & `tmp/cognite_sdk-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.1.4.tar", max compression
+gzip compressed data, was "cognite_sdk-6.1.5.tar", max compression
```

## Comparing `cognite_sdk-6.1.4.tar` & `cognite_sdk-6.1.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/LICENSE
--rw-r--r--   0        0        0     3945 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/README.md
--rw-r--r--   0        0        0      503 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87464 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44656 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49922 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-05-08 14:13:34.970338 cognite_sdk-6.1.4/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/config.py
--rw-r--r--   0        0        0    18062 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    22565 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-05-08 14:13:34.974338 cognite_sdk-6.1.4/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-05-08 14:13:34.978338 cognite_sdk-6.1.4/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2132 2023-05-08 14:13:34.978338 cognite_sdk-6.1.4/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-10 11:35:00.714193 cognite_sdk-6.1.5/LICENSE
+-rw-r--r--   0        0        0     3945 2023-05-10 11:35:00.714193 cognite_sdk-6.1.5/README.md
+-rw-r--r--   0        0        0      503 2023-05-10 11:35:00.714193 cognite_sdk-6.1.5/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:35:00.714193 cognite_sdk-6.1.5/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-10 11:35:00.714193 cognite_sdk-6.1.5/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87464 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17436 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44656 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49922 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/config.py
+-rw-r--r--   0        0        0    18062 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-10 11:35:00.718193 cognite_sdk-6.1.5/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14287 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-05-10 11:35:00.722193 cognite_sdk-6.1.5/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2132 2023-05-10 11:35:00.726193 cognite_sdk-6.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.5/PKG-INFO
```

### Comparing `cognite_sdk-6.1.4/LICENSE` & `cognite_sdk-6.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/README.md` & `cognite_sdk-6.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/annotations.py` & `cognite_sdk-6.1.5/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/assets.py` & `cognite_sdk-6.1.5/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/data_sets.py` & `cognite_sdk-6.1.5/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.1.5/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/datapoints.py` & `cognite_sdk-6.1.5/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/diagrams.py` & `cognite_sdk-6.1.5/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.1.5/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/events.py` & `cognite_sdk-6.1.5/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.1.5/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/files.py` & `cognite_sdk-6.1.5/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/functions.py` & `cognite_sdk-6.1.5/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/geospatial.py` & `cognite_sdk-6.1.5/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/iam.py` & `cognite_sdk-6.1.5/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/labels.py` & `cognite_sdk-6.1.5/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/raw.py` & `cognite_sdk-6.1.5/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/relationships.py` & `cognite_sdk-6.1.5/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/sequences.py` & `cognite_sdk-6.1.5/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.1.5/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/templates.py` & `cognite_sdk-6.1.5/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/three_d.py` & `cognite_sdk-6.1.5/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/time_series.py` & `cognite_sdk-6.1.5/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.1.5/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.1.5/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.1.5/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.1.5/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.1.5/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api/vision.py` & `cognite_sdk-6.1.5/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_api_client.py` & `cognite_sdk-6.1.5/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_cognite_client.py` & `cognite_sdk-6.1.5/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_http_client.py` & `cognite_sdk-6.1.5/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.1.5/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.1.5/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.5/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.1.5/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.1.5/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.1.5/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.1.5/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/config.py` & `cognite_sdk-6.1.5/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/credentials.py` & `cognite_sdk-6.1.5/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/_base.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/assets.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/events.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/files.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/functions.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/iam.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/labels.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/raw.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/shared.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/templates.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/transformations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 from cognite.client.utils._text import convert_all_keys_to_camel_case, convert_all_keys_to_snake_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
 
 class SessionDetails:
-    """Details of a session which provid.
+    """Details of a source session which provid.
 
     Args:
-        session_id (int): CDF session ID
-        client_id (str): Idp client ID
-        project_name (str): CDF project name
+        session_id (int): CDF source session ID
+        client_id (str): Idp source client ID
+        project_name (str): CDF source project name
     """
 
     def __init__(
         self,
         session_id: int = None,
         client_id: str = None,
         project_name: str = None,
@@ -186,48 +186,52 @@
             self.tags,
         )
 
     def _process_credentials(self, sessions_cache: Dict[str, NonceCredentials] = None, keep_none: bool = False) -> None:
         if sessions_cache is None:
             sessions_cache = {}
 
-        def try_get_or_create_nonce(oidc_credentials: Optional[OidcCredentials]) -> Optional[NonceCredentials]:
+        def try_get_or_create_nonce(
+            oidc_credentials: Optional[OidcCredentials], project: str
+        ) -> Optional[NonceCredentials]:
             if keep_none and oidc_credentials is None:
                 return None
 
             # MyPy requires this to make sure it's not changed to None after inner declaration
             assert sessions_cache is not None
 
             key = (
-                f"{oidc_credentials.client_id}:{hash(oidc_credentials.client_secret)}"
+                f"{oidc_credentials.client_id}:{hash(oidc_credentials.client_secret)}:{project}"
                 if oidc_credentials
                 else "DEFAULT"
             )
 
             ret = sessions_cache.get(key)
             if not ret:
                 if oidc_credentials and oidc_credentials.client_id and oidc_credentials.client_secret:
                     credentials = ClientCredentials(oidc_credentials.client_id, oidc_credentials.client_secret)
                 else:
                     credentials = None
                 try:
-                    session = self._cognite_client.iam.sessions.create(credentials)
-                    ret = NonceCredentials(session.id, session.nonce, self._cognite_client._config.project)
+                    session = self._cognite_client.iam.sessions.create(credentials, project=project)
+                    ret = NonceCredentials(session.id, session.nonce, project)
                     sessions_cache[key] = ret
                 except Exception:
                     ret = None
             return ret
 
-        if self.source_nonce is None:
-            self.source_nonce = try_get_or_create_nonce(self.source_oidc_credentials)
+        if self.source_nonce is None and self.source_oidc_credentials:
+            project = self.source_oidc_credentials.cdf_project_name or self._cognite_client.project
+            self.source_nonce = try_get_or_create_nonce(self.source_oidc_credentials, project)
             if self.source_nonce:
                 self.source_oidc_credentials = None
 
-        if self.destination_nonce is None:
-            self.destination_nonce = try_get_or_create_nonce(self.destination_oidc_credentials)
+        if self.destination_nonce is None and self.destination_oidc_credentials:
+            project = self.destination_oidc_credentials.cdf_project_name or self._cognite_client.project
+            self.destination_nonce = try_get_or_create_nonce(self.destination_oidc_credentials, project)
             if self.destination_nonce:
                 self.destination_oidc_credentials = None
 
     def run(self, wait: bool = True, timeout: Optional[float] = None) -> TransformationJob:
         return self._cognite_client.transformations.run(transformation_id=self.id, wait=wait, timeout=timeout)
 
     def cancel(self) -> None:
@@ -285,15 +289,21 @@
         """
 
         ret = super().dump(camel_case=camel_case)
 
         for name, prop in ret.items():
             if isinstance(
                 prop,
-                (OidcCredentials, NonceCredentials, TransformationDestination, SessionDetails, TransformationSchedule),
+                (
+                    OidcCredentials,
+                    NonceCredentials,
+                    TransformationDestination,
+                    SessionDetails,
+                    TransformationSchedule,
+                ),
             ):
                 ret[name] = prop.dump(camel_case=camel_case)
         return ret
 
     def __hash__(self) -> int:
         return hash(self.external_id)
```

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.1.5/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/exceptions.py` & `cognite_sdk-6.1.5/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/testing.py` & `cognite_sdk-6.1.5/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/__init__.py` & `cognite_sdk-6.1.5/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.1.5/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.1.5/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_graph.py` & `cognite_sdk-6.1.5/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_identifier.py` & `cognite_sdk-6.1.5/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_logging.py` & `cognite_sdk-6.1.5/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.1.5/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.1.5/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.1.5/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_text.py` & `cognite_sdk-6.1.5/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_time.py` & `cognite_sdk-6.1.5/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_validation.py` & `cognite_sdk-6.1.5/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.1.5/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.4/pyproject.toml` & `cognite_sdk-6.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.1.4"
+version = "6.1.5"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.1.4/PKG-INFO` & `cognite_sdk-6.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.1.4
+Version: 6.1.5
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.4 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.5 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```


# Comparing `tmp/unify-sdk-4.1.0.tar.gz` & `tmp/unify-sdk-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-sdk-4.1.0.tar", last modified: Thu May  4 21:28:41 2023, max compression
+gzip compressed data, was "dist/unify-sdk-4.1.1.tar", last modified: Thu May 11 16:30:06 2023, max compression
```

## Comparing `unify-sdk-4.1.0.tar` & `unify-sdk-4.1.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2331 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1774 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2581 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3881 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/disable_test_connectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/disable_test_connectors_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7017 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_aa_permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4821 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_api_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4416 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_api_manager_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_asset_access.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_graph_v2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_graph_v2_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_hierarchies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_hierarchies_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_org_admin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_org_admin_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8643 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_pipelines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8064 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_pipelines_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2388 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10038 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6669 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_sources_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_templates_default_org.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/Unify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4376 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/WaitingLibrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44927 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/apimanager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8167 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/apirequestsmng.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/apiutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3609 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/assetaccess.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/clusters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11459 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/connectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3057 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/generalutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5142 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/graph.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/Permissions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/Permissions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/SingleOrg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/datasets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/datasets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/datasets/column.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/dataset_gql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10009 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/graphql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5401 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/pipeline_gql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/pipeline/flow_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/pipeline/schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/staticsql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/unify_objects/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/unify_objects/Template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/unify_objects/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/hierarchies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16874 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/orgadmin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8738 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30555 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/pipelines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14043 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    52295 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21586 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3803 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify_sdk.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2331 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1897 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2581 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3881 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/disable_test_connectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/disable_test_connectors_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7017 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_aa_permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4821 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_api_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4416 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_api_manager_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_asset_access.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_graph_v2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_graph_v2_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_hierarchies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_hierarchies_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_org_admin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_org_admin_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8643 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_pipelines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8064 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_pipelines_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2388 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10038 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6669 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_sources_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/tests/test_templates_default_org.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/Unify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4376 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/WaitingLibrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    44927 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/apimanager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8167 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/apirequestsmng.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/apiutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3609 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/assetaccess.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/clusters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11459 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/connectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3057 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/generalutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5142 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/graph.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/Permissions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/Permissions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/SingleOrg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/datasets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/datasets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/datasets/column.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/dataset_gql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10009 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/graphql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5401 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/graph_ql/pipeline_gql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/pipeline/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/pipeline/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/pipeline/flow_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/pipeline/schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/staticsql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify/helpers/unify_objects/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/unify_objects/Template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/helpers/unify_objects/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/hierarchies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17684 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/orgadmin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8738 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30555 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/pipelines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14043 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52295 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21586 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3803 2023-05-11 16:30:00.000000 unify-sdk-4.1.1/unify/users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-05-11 16:30:06.000000 unify-sdk-4.1.1/unify_sdk.egg-info/top_level.txt
```

### Comparing `unify-sdk-4.1.0/LICENSE` & `unify-sdk-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/PKG-INFO` & `unify-sdk-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-sdk
-Version: 4.1.0
+Version: 4.1.1
 Summary: Unify Python SDK
 Home-page: https://github.com/ElementAnalytics/unify-python-sdk
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-sdk-4.1.0/README.md` & `unify-sdk-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/setup.py` & `unify-sdk-4.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text().strip()
 
-version = os.popen('git describe --dirty').read()
+version = os.popen('git describe').read().strip()
+version = version if version != '' else '0.0.0'
+version = re.sub(r'(\d+\.\d+\.\d+)-(\d+)-(.*)', r'\g<1>.dev\g<2>+git\g<3>', version)
 
 setup(
     name='unify-sdk',
     version=str(version),
     description="Unify Python SDK",
     long_description=README,
     long_description_content_type='text/markdown',
@@ -40,24 +42,24 @@
     include_package_data=True,
     hiddenimports=[
         'keyring',
         'setuptools',
         'tabulate',
         'requests',
         'json-lines',
-        'gql[all]',
+        'gql',
         'gql-query-builder'
     ],
     install_requires=[
         'keyring',
         'setuptools',
         'tabulate',
         'requests',
         'json-lines',
-        'gql[all]',
+        'gql',
         'gql-query-builder'
     ],
     url='https://github.com/ElementAnalytics/unify-python-sdk',
     author='Element Analytics',
     author_email='platform@ean.io',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `unify-sdk-4.1.0/tests/__init__.py` & `unify-sdk-4.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/disable_test_connectors.py` & `unify-sdk-4.1.1/tests/disable_test_connectors.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/disable_test_connectors_default_org.py` & `unify-sdk-4.1.1/tests/disable_test_connectors_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_aa_permissions.py` & `unify-sdk-4.1.1/tests/test_aa_permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_api_manager.py` & `unify-sdk-4.1.1/tests/test_api_manager.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_api_manager_default_org.py` & `unify-sdk-4.1.1/tests/test_api_manager_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_asset_access.py` & `unify-sdk-4.1.1/tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_graph_v2.py` & `unify-sdk-4.1.1/tests/test_graph_v2.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_graph_v2_default_org.py` & `unify-sdk-4.1.1/tests/test_graph_v2_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_hierarchies.py` & `unify-sdk-4.1.1/tests/test_hierarchies.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_hierarchies_default_org.py` & `unify-sdk-4.1.1/tests/test_hierarchies_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_org_admin.py` & `unify-sdk-4.1.1/tests/test_org_admin.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_org_admin_default_org.py` & `unify-sdk-4.1.1/tests/test_org_admin_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_pipelines.py` & `unify-sdk-4.1.1/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_pipelines_default_org.py` & `unify-sdk-4.1.1/tests/test_pipelines_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_properties.py` & `unify-sdk-4.1.1/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_sources.py` & `unify-sdk-4.1.1/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_sources_default_org.py` & `unify-sdk-4.1.1/tests/test_sources_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_templates.py` & `unify-sdk-4.1.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/tests/test_templates_default_org.py` & `unify-sdk-4.1.1/tests/test_templates_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/WaitingLibrary.py` & `unify-sdk-4.1.1/unify/WaitingLibrary.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/apimanager.py` & `unify-sdk-4.1.1/unify/apimanager.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/apirequestsmng.py` & `unify-sdk-4.1.1/unify/apirequestsmng.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/apiutils.py` & `unify-sdk-4.1.1/unify/apiutils.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/assetaccess.py` & `unify-sdk-4.1.1/unify/assetaccess.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/clusters.py` & `unify-sdk-4.1.1/unify/clusters.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/connectors.py` & `unify-sdk-4.1.1/unify/connectors.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/generalutils.py` & `unify-sdk-4.1.1/unify/generalutils.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/graph.py` & `unify-sdk-4.1.1/unify/graph.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/Permissions/__init__.py` & `unify-sdk-4.1.1/unify/helpers/Permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/datasets/column.py` & `unify-sdk-4.1.1/unify/helpers/datasets/column.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/graph_ql/dataset_gql.py` & `unify-sdk-4.1.1/unify/helpers/graph_ql/dataset_gql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/graph_ql/graphql.py` & `unify-sdk-4.1.1/unify/helpers/graph_ql/graphql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/graph_ql/permissions.py` & `unify-sdk-4.1.1/unify/helpers/graph_ql/permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/graph_ql/pipeline_gql.py` & `unify-sdk-4.1.1/unify/helpers/graph_ql/pipeline_gql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/pipeline/schema.py` & `unify-sdk-4.1.1/unify/helpers/pipeline/schema.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/staticsql.py` & `unify-sdk-4.1.1/unify/helpers/staticsql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/helpers/unify_objects/Template.py` & `unify-sdk-4.1.1/unify/helpers/unify_objects/Template.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/hierarchies.py` & `unify-sdk-4.1.1/unify/hierarchies.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/orgadmin.py` & `unify-sdk-4.1.1/unify/orgadmin.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             self.orgs_api_url = remote + 'api/management/v1/orgs'
             self.org_api_url = remote + 'api/management/v1/orgs/{}'
             self.org_info_url = remote + 'api/v1/orgs/{}'
             self.who_ami_url = remote + 'api/whoami'
             self.org_sensor_analytics = remote + "api/v1/orgs/{}/sensor_diagnostics"
             self.change_group_url = remote + "api/authz/v1/groups/{}/users"
             self.all_users_url = remote + "api/v1/users"
+            self.machine_user_password_url = remote + "api/v1/users/{}/machine-user-password"
             self.all_users_on_org = remote + "api/v1/orgs/{}/users"
             self.all_groups_url = remote + "api/authz/v1/groups"
 
         except Exception as error:
             raise error
 
     @single_org
@@ -277,14 +278,37 @@
                 return json.loads(invite_user_post.content)
 
             raise Exception(json.loads(invite_user_post.content))
 
         except Exception as error:
             raise error
 
+    def change_machine_user_password(self, id, password):
+        change_password_url = self.machine_user_password_url.format(id)
+
+        header = self.build_header(
+            aut_token=self.props.get_auth_token(cluster=self.cluster),
+            others=self.content_type_header
+        )
+
+        payload = {
+            "newPassword": password,
+        }
+
+        change_password_put = self.session.put(
+            change_password_url,
+            headers=header,
+            data=json.dumps(payload)
+        )
+
+        if change_password_put.status_code == 200:
+                return json.loads(change_password_put.content)
+        else:
+            raise Exception(json.loads(change_password_put.content))
+
     def get_org_list(self):
         """
         Retrieves the org list of the current cluster, only the ones whos users has logged in
 
         :return: List of organizations
         """
         try:
```

### Comparing `unify-sdk-4.1.0/unify/permissions.py` & `unify-sdk-4.1.1/unify/permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/pipelines.py` & `unify-sdk-4.1.1/unify/pipelines.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/properties.py` & `unify-sdk-4.1.1/unify/properties.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/sources.py` & `unify-sdk-4.1.1/unify/sources.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/templates.py` & `unify-sdk-4.1.1/unify/templates.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify/users.py` & `unify-sdk-4.1.1/unify/users.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.1.0/unify_sdk.egg-info/PKG-INFO` & `unify-sdk-4.1.1/unify_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-sdk
-Version: 4.1.0
+Version: 4.1.1
 Summary: Unify Python SDK
 Home-page: https://github.com/ElementAnalytics/unify-python-sdk
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-sdk-4.1.0/unify_sdk.egg-info/SOURCES.txt` & `unify-sdk-4.1.1/unify_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


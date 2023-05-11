# Comparing `tmp/infoworkssdk-3.0a0.tar.gz` & `tmp/infoworkssdk-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoworkssdk-3.0a0.tar", last modified: Thu May 11 08:05:24 2023, max compression
+gzip compressed data, was "infoworkssdk-3.0b0.tar", last modified: Thu Apr 13 12:48:00 2023, max compression
```

## Comparing `infoworkssdk-3.0a0.tar` & `infoworkssdk-3.0b0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.511680 infoworkssdk-3.0a0/
--rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-3.0a0/LICENSE
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-05-11 08:05:24.511474 infoworkssdk-3.0a0/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-3.0a0/README.md
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.481508 infoworkssdk-3.0a0/infoworks/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/__init__.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.482191 infoworkssdk-3.0a0/infoworks/core/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/core/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/core/iw_authentication.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1080 2023-01-09 10:04:48.000000 infoworkssdk-3.0a0/infoworks/error.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.497697 infoworkssdk-3.0a0/infoworks/sdk/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    89421 2023-04-08 13:06:20.000000 infoworkssdk-3.0a0/infoworks/sdk/admin_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/sdk/base_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.498376 infoworkssdk-3.0a0/infoworks/sdk/cicd/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-08 16:36:18.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/cicd_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.502043 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-02-07 06:46:50.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-02-07 06:47:32.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2979 2023-05-11 08:03:43.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1929 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1986 2023-02-07 06:52:34.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)    29459 2023-05-11 08:03:43.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/utils.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.509365 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    12629 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/cdata_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    18649 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/csv_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13421 2022-12-08 16:37:10.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/domains.py
--rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/misc.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7881 2023-04-13 12:30:16.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
--rw-r--r--   0 infoworks   (501) staff       (20)    16611 2023-04-13 12:30:16.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/pipelines.py
--rw-r--r--   0 infoworks   (501) staff       (20)    18556 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    10283 2023-04-11 06:44:19.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)      963 2022-12-19 09:42:17.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/update_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    12796 2023-04-13 12:30:16.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/workflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)    21402 2023-04-13 04:12:24.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
--rw-r--r--   0 infoworks   (501) staff       (20)    26668 2023-04-25 04:08:43.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/wrappersource.py
--rw-r--r--   0 infoworks   (501) staff       (20)    11434 2023-04-13 04:12:24.000000 infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1729 2023-05-08 06:11:43.000000 infoworkssdk-3.0a0/infoworks/sdk/client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    31762 2023-04-10 04:34:31.000000 infoworkssdk-3.0a0/infoworks/sdk/domain_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.509750 infoworkssdk-3.0a0/infoworks/sdk/ejson/
--rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-3.0a0/infoworks/sdk/ejson/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-3.0a0/infoworks/sdk/generic_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-3.0a0/infoworks/sdk/jobmetrics.py
--rw-r--r--   0 infoworks   (501) staff       (20)    32432 2023-04-11 04:32:34.000000 infoworkssdk-3.0a0/infoworks/sdk/jobs_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-3.0a0/infoworks/sdk/jobs_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2216 2023-05-08 06:08:31.000000 infoworkssdk-3.0a0/infoworks/sdk/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    46328 2023-05-11 04:41:44.000000 infoworkssdk-3.0a0/infoworks/sdk/pipeline_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    47562 2023-04-13 12:30:16.000000 infoworkssdk-3.0a0/infoworks/sdk/pipeline_group_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/pipeline_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)      495 2023-05-08 06:13:24.000000 infoworkssdk-3.0a0/infoworks/sdk/replicator_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)   177768 2023-05-08 06:08:31.000000 infoworkssdk-3.0a0/infoworks/sdk/source_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/source_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    61773 2023-05-11 04:40:52.000000 infoworkssdk-3.0a0/infoworks/sdk/url_builder.py
--rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/utils.py
--rw-r--r--   0 infoworks   (501) staff       (20)    65766 2023-04-13 12:30:16.000000 infoworkssdk-3.0a0/infoworks/sdk/workflow_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-3.0a0/infoworks/sdk/workflow_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-05-11 08:05:24.511135 infoworkssdk-3.0a0/infoworkssdk.egg-info/
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-05-11 08:05:24.000000 infoworkssdk-3.0a0/infoworkssdk.egg-info/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     2360 2023-05-11 08:05:24.000000 infoworkssdk-3.0a0/infoworkssdk.egg-info/SOURCES.txt
--rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-05-11 08:05:24.000000 infoworkssdk-3.0a0/infoworkssdk.egg-info/dependency_links.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-05-11 08:05:24.000000 infoworkssdk-3.0a0/infoworkssdk.egg-info/requires.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-05-11 08:05:24.000000 infoworkssdk-3.0a0/infoworkssdk.egg-info/top_level.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-05-11 08:05:24.511762 infoworkssdk-3.0a0/setup.cfg
--rw-r--r--   0 infoworks   (501) staff       (20)      897 2023-05-11 08:04:24.000000 infoworkssdk-3.0a0/setup.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.619391 infoworkssdk-3.0b0/
+-rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/LICENSE
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-04-13 12:48:00.619240 infoworkssdk-3.0b0/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-3.0b0/README.md
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.599722 infoworkssdk-3.0b0/infoworks/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/__init__.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.600163 infoworkssdk-3.0b0/infoworks/core/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/core/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/core/iw_authentication.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1080 2023-01-09 10:04:48.000000 infoworkssdk-3.0b0/infoworks/error.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.610072 infoworkssdk-3.0b0/infoworks/sdk/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    89421 2023-04-08 13:06:20.000000 infoworkssdk-3.0b0/infoworks/sdk/admin_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/base_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.610480 infoworkssdk-3.0b0/infoworks/sdk/cicd/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/cicd_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.612923 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-02-07 06:46:50.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-02-07 06:47:32.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2784 2023-04-12 13:53:13.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1929 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1986 2023-02-07 06:52:34.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    28608 2023-04-12 13:53:13.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/utils.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.617829 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12629 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/cdata_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    18649 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/csv_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    13421 2022-12-08 16:37:10.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/domains.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/misc.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7881 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    16611 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipelines.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    18556 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    10283 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      963 2022-12-19 09:42:17.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/update_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12796 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/workflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    21402 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    26631 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrappersource.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11434 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1650 2023-04-04 12:20:53.000000 infoworkssdk-3.0b0/infoworks/sdk/client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    31762 2023-04-10 04:34:31.000000 infoworkssdk-3.0b0/infoworks/sdk/domain_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.618051 infoworkssdk-3.0b0/infoworks/sdk/ejson/
+-rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/infoworks/sdk/ejson/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-3.0b0/infoworks/sdk/generic_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-3.0b0/infoworks/sdk/jobmetrics.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    32432 2023-04-11 04:32:34.000000 infoworkssdk-3.0b0/infoworks/sdk/jobs_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-3.0b0/infoworks/sdk/jobs_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1911 2023-01-27 06:24:03.000000 infoworkssdk-3.0b0/infoworks/sdk/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    36765 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    47562 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_group_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   176960 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/source_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/source_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    60128 2023-04-11 06:45:26.000000 infoworkssdk-3.0b0/infoworks/sdk/url_builder.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/utils.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    65766 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/workflow_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/workflow_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.619020 infoworkssdk-3.0b0/infoworkssdk.egg-info/
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     2325 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/requires.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/top_level.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-04-13 12:48:00.619438 infoworkssdk-3.0b0/setup.cfg
+-rw-r--r--   0 infoworks   (501) staff       (20)      896 2023-04-13 12:47:53.000000 infoworkssdk-3.0b0/setup.py
```

### Comparing `infoworkssdk-3.0a0/LICENSE` & `infoworkssdk-3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/PKG-INFO` & `infoworkssdk-3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 3.0a0
+Version: 3.0b0
 Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infoworkssdk-3.0a0/README.md` & `infoworkssdk-3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/core/iw_authentication.py` & `infoworkssdk-3.0b0/infoworks/core/iw_authentication.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/error.py` & `infoworkssdk-3.0b0/infoworks/error.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/admin_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/admin_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/base_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/base_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/cicd_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/cicd_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,14 @@
                         f.write(filename)
                         f.write("\n")
             except Exception as e:
                 self.logger.error(f"Unable to export configurations for pipeline {pipeline_id} due to {str(e)}")
                 print(f"Unable to export configurations for pipeline {pipeline_id} due to {str(e)}")
         if pipeline_grp_config is not None:
             pipeline_group_id = pipeline_grp_config["id"]
-            json_obj = {"entity_id": pipeline_group_id, "entity_type": "pipeline_group"}
-            domain_id = utils_obj.get_domain_id(self, json_obj)
-            if domain_id:
-                filename, configuration_obj = utils_obj.dump_to_file(self, "pipeline_group", domain_id, pipeline_group_id,
+            filename, configuration_obj = utils_obj.dump_to_file(self, "pipeline_group", domain_id, pipeline_group_id,
                                                                  replace_words, config_file_dump_path)
-                if filename is not None:
-                    f_pipeline_group.write(filename)
-                    f_pipeline_group.write("\n")
+            if filename is not None:
+                f_pipeline_group.write(filename)
+                f_pipeline_group.write("\n")
         f.close()
         f_pipeline_group.close()
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/lineage.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/download_configurations/utils.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import copy
 import os
-import traceback
-
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import get_parent_entity_url, list_domains_url, configure_pipeline_url, \
     configure_workflow_url, \
     configure_source_url, get_environment_details, get_environment_storage_details, get_environment_compute_details, \
     get_environment_interactive_compute_details, get_source_configurations_url, get_pipeline_url, \
     get_data_connection, source_info, list_users_url, list_secrets_url, get_pipeline_group_base_url,list_pipelines_url
 from infoworks.sdk.cicd.cicd_response import CICDResponse
@@ -300,15 +298,14 @@
                                                                 cicd_client.client_config['bearer_token']))
                             parsed_response = IWUtils.ejson_deserialize(response.content)
                             if response.status_code == 200:
                                 status = "SUCCESS"
                             else:
                                 status = "FAILED"
                                 print("Get Data Connection Details failed " + json.dumps(response))
-                                cicd_client.logger.error("Get Data Connection Details failed " + json.dumps(response))
 
                             response_to_return["get_data_connection_details_response"] = CICDResponse.parse_result(
                                 status=status,
                                 entity_id=entity_id,
                                 response=parsed_response)
                             if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
                                 result = parsed_response.get("result", [])
@@ -317,26 +314,19 @@
                                                                                               result["properties"])
                                 for key in ['name', 'type', 'sub_type', 'properties']:
                                     dataconnection_obj[key] = result[key]
                                 configuration_obj["dataconnection_configurations"].append(
                                     copy.deepcopy(dataconnection_obj))
                 elif entity_type == "pipeline_group":
                     list_pipelines_under_domain_url = list_pipelines_url(cicd_client.client_config,domain_id=domain_id)
-                    cicd_client.logger.info(f"Calling the api: {list_pipelines_under_domain_url}")
                     pipeline_name_lookup={}
                     pipelines_under_domain_response = cicd_client.call_api("GET", list_pipelines_under_domain_url, IWUtils.get_default_header_for_v3(
             cicd_client.client_config[
                 'bearer_token']))
                     pipelines_under_domain_parsed_response = IWUtils.ejson_deserialize(pipelines_under_domain_response.content)
-                    if pipelines_under_domain_parsed_response.get("result","")=="":
-                        cicd_client.logger.error(f"Failed to list the pipelines under domain {domain_id}")
-                        cicd_client.logger.error(pipelines_under_domain_parsed_response)
-                        print(f"Failed to list the pipelines under domain {domain_id}")
-                        print(pipelines_under_domain_parsed_response)
-                        raise Exception(f"Failed to list the pipelines under domain {domain_id}")
                     for pipeline in pipelines_under_domain_parsed_response["result"]:
                         pipeline_name_lookup[pipeline["id"]]=pipeline["name"]
                     for index,pipeline in enumerate(configuration_obj["pipelines"]):
                         pipeline["name"]=pipeline_name_lookup.get(pipeline["pipeline_id"],None)
                     environment_id = configuration_obj["environment_id"]
                 domains_url_base = list_domains_url(cicd_client.client_config)
                 filter_condition = IWUtils.ejson_serialize({"_id": domain_id})
@@ -344,15 +334,14 @@
                     filter_condition=filter_condition)
                 response = cicd_client.call_api("GET", domains_url,
                                                 IWUtils.get_default_header_for_v3(
                                                     cicd_client.client_config['bearer_token']))
                 parsed_response = IWUtils.ejson_deserialize(response.content)
                 if response.status_code == 200:
                     status = "SUCCESS"
-                    cicd_client.logger.info("Got domain details successfully")
                 else:
                     status = "FAILED"
                     print("Get Domains Details failed " + json.dumps(response))
                 response_to_return["get_domain_details_response"] = CICDResponse.parse_result(status=status,
                                                                                               entity_id=entity_id,
                                                                                               response=parsed_response)
                 existing_domain_name = None
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/cdata_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/cdata_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/csv_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/csv_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/domains.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/domains.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/misc.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/misc.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/pipelines.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipelines.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/update_configurations.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/update_configurations.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/workflow.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/workflow.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/wrappersource.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrappersource.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                         mapping["recommendation"]["compute_name"]=compute_mappings_from_config.get(mapping["recommendation"]["compute_name"],mapping["recommendation"]["compute_name"])
             if env_id is None or storage_id is None:
                 print("No env id or storage id found")
                 raise Exception("No env id or storage id found")
 
             source_type = configuration_obj["configuration"]["source_configs"]["type"]
             source_sub_type = configuration_obj["configuration"]["source_configs"]["sub_type"]
-            if source_type == "file" and (source_sub_type == "structured" or source_sub_type == "fixedwidth"):
+            if source_type == "file" and source_sub_type == "structured":
                 source_obj = CSVSource(env_id, storage_id, configuration_file_path, self.secrets_config, replace_words)
                 source_obj.update_mappings_for_configurations(self.mappings)
                 create_source_response = source_obj.create_csv_source(self)
                 source_id=create_source_response["result"]["source_id"]
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     source_connection_configurations_response = source_obj.configure_csv_source(self, source_id, self.mappings,
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/client.py` & `infoworkssdk-3.0b0/infoworks/sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from infoworks.sdk.pipeline_client import PipelineClient
 from infoworks.sdk.workflow_client import WorkflowClient
 from infoworks.sdk.domain_client import DomainClient
 from infoworks.sdk.jobmetrics import JobMetricsClient
 from infoworks.sdk.admin_client import AdminClient
 from infoworks.sdk.jobs_client import JobsClient
 from infoworks.sdk.pipeline_group_client import PipelineGroupClient
-from infoworks.sdk.replicator_client import ReplicatorClient
 
 
 class InfoworksClientSDK(SourceClient, PipelineClient, WorkflowClient, DomainClient, AdminClient, JobMetricsClient,
                          DownloadSource, DownloadPipeline, DownloadWorkflow, DownloadEntityWithLineage,
                          DownloadAllEntitiesFromDomain, WrapperSource, WrapperPipeline, WrapperWorkflow, JobsClient,
-                         PipelineGroupClient, ReplicatorClient):
+                         PipelineGroupClient):
     def __init__(self):
         super().__init__()
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/domain_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/domain_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/ejson/__init__.py` & `infoworkssdk-3.0b0/infoworks/sdk/ejson/__init__.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/generic_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/generic_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/jobmetrics.py` & `infoworkssdk-3.0b0/infoworks/sdk/jobmetrics.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/jobs_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/jobs_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/pipeline_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import time
 
 from infoworks.error import PipelineError
 from infoworks.sdk import url_builder, local_configurations
 from infoworks.sdk.base_client import BaseClient
-from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.local_configurations import Response, ErrorCode
 from infoworks.sdk.pipeline_response import PipelineResponse
 from infoworks.sdk.utils import IWUtils
 
 
 class PipelineClient(BaseClient):
     def __init__(self):
@@ -640,167 +639,7 @@
                                                      error_code=ErrorCode.USER_ERROR,
                                                      response=response)
         except Exception as e:
             self.logger.error(
                 f"Failed to get pipeline lineage for pipeline {pipeline_id} and column {column_name} " + str(e))
             raise PipelineError(
                 f"Failed to get pipeline lineage for pipeline {pipeline_id} and column {column_name} " + str(e))
-
-    def create_pipeline_version(self, domain_id, pipeline_id, body=None):
-        """
-        Create a new Pipeline Version
-        :param body: a JSON object containing pipeline version
-        :type body: JSON Object
-        :param domain_id: Entity identifier of domain
-        :param pipeline_id: Entity identifier of pipeline_id
-        :return: response dict
-        """
-        try:
-            response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.pipeline_version_base_url(
-                self.client_config, domain_id, pipeline_id), IWUtils.get_default_header_for_v3(
-                self.client_config['bearer_token']),
-                                                               body).content)
-            result = response.get('result', {})
-            pipeline_version_id = result.get('id', None)
-            if pipeline_version_id is None:
-                self.logger.error('Pipeline version failed to create.')
-                return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                     error_code=ErrorCode.USER_ERROR,
-                                                     error_desc='Pipeline version failed to create.',
-                                                     response=response)
-
-            pipeline_version_id = str(pipeline_version_id)
-            self.logger.info(
-                'Pipeline version {id} has been created under domain {domain_id}.'.format(id=pipeline_version_id,
-                                                                                          domain_id=domain_id))
-            return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=pipeline_version_id,
-                                                response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to create a new pipeline version.')
-            raise PipelineError('Error occurred while trying to create a new pipeline version.')
-
-    def update_pipeline_version(self, domain_id, pipeline_id, pipeline_version_id, body=None):
-        """
-        Updates the Pipeline Version
-        :param body: a JSON object containing pipeline version
-        :type body: JSON Object
-        :param domain_id: Entity identifier of domain
-        :param pipeline_id: Entity identifier of pipeline_id
-        :param pipeline_version_id: Entity identifier of pipeline_version_id
-        :return: response dict
-        """
-        try:
-            response = IWUtils.ejson_deserialize(self.call_api("PATCH", url_builder.pipeline_version_base_url(
-                self.client_config, domain_id, pipeline_id) + f"/{pipeline_version_id}",
-                                                               IWUtils.get_default_header_for_v3(
-                                                                   self.client_config['bearer_token']), body).content)
-            message = response.get('message', "")
-            if message != "Pipeline Version Updated Successfully":
-                self.logger.error('Pipeline version failed to update.')
-                return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                     error_code=ErrorCode.USER_ERROR,
-                                                     error_desc='Pipeline version failed to update.',
-                                                     response=response)
-
-            else:
-                self.logger.info(
-                    'Pipeline version {id} has been updated.'.format(id=pipeline_version_id))
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=pipeline_version_id,
-                                                    response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to update a pipeline version.')
-            raise PipelineError('Error occurred while trying to update a pipeline version.')
-
-    def set_pipeline_version_as_active(self, domain_id, pipeline_id, pipeline_version_id):
-        """
-        Sets the pipeline version as active
-        :param domain_id: Entity identifier of domain
-        :param pipeline_id: Entity identifier of pipeline_id
-        :param pipeline_version_id: Entity identifier of pipeline_version_id
-        :return: response dict
-        """
-        try:
-            response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.pipeline_version_base_url(
-                self.client_config, domain_id, pipeline_id) + f"/{pipeline_version_id}/set-active",
-                                                               IWUtils.get_default_header_for_v3(
-                                                                   self.client_config['bearer_token'])).content)
-            message = response.get('message', "")
-            if message != "Successfully set active version":
-                self.logger.error('Pipeline version failed to be set active.')
-                return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                     error_code=ErrorCode.USER_ERROR,
-                                                     error_desc='Pipeline version failed to be set active.',
-                                                     response=response)
-
-            else:
-                self.logger.info(
-                    'Pipeline version {id} has been set as active.'.format(id=pipeline_version_id))
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=pipeline_version_id,
-                                                    response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to set a pipeline version as active.')
-            raise PipelineError('Error occurred while trying to set a pipeline version as active.')
-
-    def modify_advanced_config_for_pipeline(self, domain_id, pipeline_id, adv_config_body,
-                                            action_type="update", key=None):
-        """
-        Function to add/update the adv config for the pipeline
-        :param pipeline_id: id of the pipeline
-        :type pipeline_id: String
-        :param domain_id: Domain id to which the pipeline belongs to
-        :type domain_id: String
-        :param action_type: values can be either create/update. default update
-        :type action_type: String
-        :param adv_config_body: JSON dict
-        adv_config_body_example = {
-            "key" : "",
-            "value": "",
-            "description": "",
-            "is_active": True
-            }
-        :param key: In case of update, name of the adv config to update
-        :return: response dict
-        """
-        if None in {pipeline_id, domain_id} or adv_config_body is None:
-            raise Exception(f"pipeline_id, domain_id and adv_config_body cannot be None")
-        try:
-            if action_type.lower() == "create":
-                request_type = "POST"
-                request_url = url_builder.advanced_config_pipeline_url(self.client_config, domain_id,
-                                                                       pipeline_id)
-            else:
-                request_type = "PUT"
-                request_url = url_builder.advanced_config_pipeline_url(self.client_config, domain_id,
-                                                                       pipeline_id) + f"{key}"
-            response = IWUtils.ejson_deserialize(
-                self.call_api(request_type, request_url,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                              adv_config_body).content)
-            result = response.get('result', {})
-            message = response.get('message', "")
-            adv_config_id = result.get('id', None)
-            if adv_config_id is not None:
-                adv_config_id = str(adv_config_id)
-                self.logger.info(
-                    'Advanced Config has been created {id}.'.format(id=adv_config_id))
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=adv_config_id,
-                                                    response=response)
-            elif message == "Successfully updated Advance configuration":
-                self.logger.info('Advanced Config has been updated')
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-            else:
-                self.logger.error(f'Failed to {action_type} advanced config for pipeline.')
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    error_desc=f'Failed to {action_type} advanced config for pipeline',
-                                                    response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to add/update adv config pipeline.')
-            raise PipelineError('Error occurred while trying to add/update adv config pipeline.')
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/pipeline_group_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_group_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/pipeline_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/source_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/source_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1637,33 +1637,22 @@
             return None
         if src_type.lower() == "oracle":
             sub_type = SourceMappings.oracle.get("sub_type")
             driver_name = SourceMappings.oracle.get("driver_name")
             driver_version = SourceMappings.oracle.get("driver_version")
             database = SourceMappings.oracle.get("database")
         elif src_type.lower() == "sqlserver":
-            sub_type = SourceMappings.sqlserver.get("sub_type")
-            driver_name = SourceMappings.sqlserver.get("driver_name")
-            driver_version = SourceMappings.sqlserver.get("driver_version")
-            database = SourceMappings.sqlserver.get("database")
+            pass
         elif src_type.lower() == "teradata":
             sub_type = SourceMappings.teradata.get("sub_type")
             driver_name = SourceMappings.teradata.get("driver_name")
             driver_version = SourceMappings.teradata.get("driver_version")
             database = SourceMappings.teradata.get("database")
         elif src_type.lower() == "mysql":
-            sub_type = SourceMappings.mysql.get("sub_type")
-            driver_name = SourceMappings.mysql.get("driver_name")
-            driver_version = SourceMappings.mysql.get("driver_version")
-            database = SourceMappings.mysql.get("database")
-        elif src_type.lower() == "netezza":
-            sub_type = SourceMappings.netezza.get("sub_type")
-            driver_name = SourceMappings.netezza.get("driver_name")
-            driver_version = SourceMappings.netezza.get("driver_version")
-            database = SourceMappings.netezza.get("database")
+            pass
         else:
             sub_type = SourceMappings.oracle.get("sub_type")
             driver_name = SourceMappings.oracle.get("driver_name")
             driver_version = SourceMappings.oracle.get("driver_version")
             database = SourceMappings.oracle.get("database")
         src_create_response = self.create_source(source_config={
             "name": src_name,
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/source_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/source_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/url_builder.py` & `infoworkssdk-3.0b0/infoworks/sdk/url_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1538,32 +1538,21 @@
     return request
 
 
 def advanced_config_domain_url(config, domain_id):
     """
     returns url to work with adv config of the domain
     """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/configurations/advance'.format(
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-pipeline-extensions'.format(
         domain_id=domain_id,
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
 
 
-def advanced_config_pipeline_url(config, domain_id, pipeline_id):
-    """
-    returns url to work with adv config of the pipeline
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipelines/{pipeline_id}/configurations/advance'.format(
-        domain_id=domain_id, pipeline_id=pipeline_id,
-        ip=config['ip'], port=config['port'],
-        protocol=config['protocol'])
-    return request
-
-
 def table_advanced_base_url(config, source_id, table_id):
     """
     returns url to work with table level advanced configuration
     """
     request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/configurations/advance'.format(
         source_id=source_id,
         table_id=table_id,
@@ -1620,27 +1609,7 @@
     """
         returns url to get secret details in Infoworks
         """
     request = '{protocol}://{ip}:{port}/v3/admin/manage-secrets/secrets'.format(
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
-
-
-def pipeline_version_base_url(config, domain_id, pipeline_id):
-    """
-    returns URL to work on pipeline versions using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :param pipeline_id: Identifier for pipeline
-    :return: url to work on pipeline version
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipelines/{pipeline_id}/versions'.format(ip=config['ip'],
-                                                                                                        port=config[
-                                                                                                            'port'],
-                                                                                                        protocol=config[
-                                                                                                            'protocol'],
-                                                                                                        domain_id=domain_id,
-                                                                                                        pipeline_id=pipeline_id)
-    return request
```

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/utils.py` & `infoworkssdk-3.0b0/infoworks/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/workflow_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/workflow_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworks/sdk/workflow_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/workflow_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a0/infoworkssdk.egg-info/PKG-INFO` & `infoworkssdk-3.0b0/infoworkssdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 3.0a0
+Version: 3.0b0
 Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infoworkssdk-3.0a0/infoworkssdk.egg-info/SOURCES.txt` & `infoworkssdk-3.0b0/infoworkssdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 infoworks/sdk/jobmetrics.py
 infoworks/sdk/jobs_client.py
 infoworks/sdk/jobs_response.py
 infoworks/sdk/local_configurations.py
 infoworks/sdk/pipeline_client.py
 infoworks/sdk/pipeline_group_client.py
 infoworks/sdk/pipeline_response.py
-infoworks/sdk/replicator_client.py
 infoworks/sdk/source_client.py
 infoworks/sdk/source_response.py
 infoworks/sdk/url_builder.py
 infoworks/sdk/utils.py
 infoworks/sdk/workflow_client.py
 infoworks/sdk/workflow_response.py
 infoworks/sdk/cicd/__init__.py
```

### Comparing `infoworkssdk-3.0a0/setup.py` & `infoworkssdk-3.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="infoworkssdk",
-    version="3.0-alpha",
+    version="3.0-beta",
     author="Infoworks CE Team",
     author_email="abhishek.raviprasad@infoworks.io",
     description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Infoworks/InfoworksPythonSDK",
     packages=setuptools.find_packages(),
```


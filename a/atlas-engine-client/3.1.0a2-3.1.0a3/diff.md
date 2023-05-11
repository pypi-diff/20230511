# Comparing `tmp/atlas_engine_client-3.1.0a2.tar.gz` & `tmp/atlas_engine_client-3.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas_engine_client-3.1.0a2.tar", last modified: Thu May 11 18:22:09 2023, max compression
+gzip compressed data, was "atlas_engine_client-3.1.0a3.tar", last modified: Thu May 11 18:41:06 2023, max compression
```

## Comparing `atlas_engine_client-3.1.0a2.tar` & `atlas_engine_client-3.1.0a3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.938357 atlas_engine_client-3.1.0a2/atlas_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.938357 atlas_engine_client-3.1.0a2/atlas_engine_client/app_info/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/app_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/app_info/app_info_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.938357 atlas_engine_client-3.1.0a2/atlas_engine_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/application_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/data_object_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/empty_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/external_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/flow_node_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/manual_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/process_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/process_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/process_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/user_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/core/loop_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/event/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/event/event_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/client_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/external_task_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/external_task_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/functional_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/flow_node_instance/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/flow_node_instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/flow_node_instance/flow_node_instance_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/notification/notification_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.942357 atlas_engine_client-3.1.0a2/atlas_engine_client/process_definition/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/process_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/process_definition/process_definition_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/process_definition/start_callback_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/atlas_engine_client/process_instance/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/process_instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/process_instance/process_instance_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/atlas_engine_client/user_task/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/user_task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/atlas_engine_client/user_task/user_task_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.938357 atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-11 18:22:09.000000 atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-11 18:22:09.000000 atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:22:09.000000 atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 18:22:09.000000 atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 18:22:09.000000 atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-11 18:22:09.000000 atlas_engine_client-3.1.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/core/test_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/core/test_loop_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/helper_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:09.946357 atlas_engine_client-3.1.0a2/tests/process_control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-11 18:22:03.000000 atlas_engine_client-3.1.0a2/tests/process_control/test_process_control_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.154278 atlas_engine_client-3.1.0a3/atlas_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/app_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/app_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/app_info/app_info_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/application_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/data_object_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/empty_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/external_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/flow_node_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/manual_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/process_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/process_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/process_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/user_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/core/loop_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/event/event_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/external_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/external_task_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/functional_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.158278 atlas_engine_client-3.1.0a3/atlas_engine_client/flow_node_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/flow_node_instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/flow_node_instance/flow_node_instance_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/atlas_engine_client/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/notification/notification_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/atlas_engine_client/process_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/process_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/process_definition/process_definition_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/process_definition/start_callback_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/atlas_engine_client/process_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/process_instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/process_instance/process_instance_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/atlas_engine_client/user_task/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/user_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/atlas_engine_client/user_task/user_task_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.154278 atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-11 18:41:06.000000 atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-11 18:41:06.000000 atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:41:06.000000 atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 18:41:06.000000 atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 18:41:06.000000 atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-11 18:41:05.000000 atlas_engine_client-3.1.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/core/test_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/core/test_loop_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/helper_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:41:06.162278 atlas_engine_client-3.1.0a3/tests/process_control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-11 18:40:56.000000 atlas_engine_client-3.1.0a3/tests/process_control/test_process_control_client.py
```

### Comparing `atlas_engine_client-3.1.0a2/PKG-INFO` & `atlas_engine_client-3.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas_engine_client
-Version: 3.1.0a2
+Version: 3.1.0a3
 Summary: A Client for the workflow engine of the ProcessCube platform.
 Home-page: https://github.com/atlas-engine/Client.py
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: ProcessCube@5Minds.de
 Keywords: workflow-engine atlas-engine client bpmn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atlas_engine_client-3.1.0a2/README.md` & `atlas_engine_client-3.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/__init__.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/app_info/app_info_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/app_info/app_info_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/client_factory.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/client_factory.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/__init__.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/base_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/base_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/application_info.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/application_info.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/data_object_instances.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/data_object_instances.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/empty_tasks.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/empty_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/events.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/events.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/external_tasks.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/external_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/flow_node_instances.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/flow_node_instances.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/manual_tasks.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/manual_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/process_definitions.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/process_definitions.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/process_instances.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/process_instances.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/process_models.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/process_models.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/api/helpers/user_tasks.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/api/helpers/user_tasks.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/base_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/base_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/core/loop_helper.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/core/loop_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.on_shutdown = kwargs.get('on_shutdown', self.__internal_on_shutdown)
 
     def create_task(self, task_callback):
         task = asyncio.run_coroutine_threadsafe(task_callback(), self._loop)
         self._tasks.append(task)
 
     def register_delayed_task(self, task_func, **options):
-        logger.info(f"create delayed tasks with options ({options}).")
+        logger.info(f"Create delayed tasks with options ({options}).")
         task = asyncio.run_coroutine_threadsafe(self.__create_delayed_task(task_func, **options), self._loop)
         self._tasks.append(task)
 
         return task
 
     def unregister_delayed_task(self, delayed_task, msg=""):
         return self.__unregister_task(delayed_task, msg)
@@ -66,15 +66,15 @@
             logger.warning('delay is deprecated, please use delay_in_ms')
             options['delay_in_ms'] = options['delay']
 
         delay = options.get('delay_in_ms', _DEFAULT_DELAY)
         return await _worker(delay)
 
     def register_background_task(self, task_func, **options):
-        logger.info(f"create background worker with options ({options}).")
+        logger.info(f"Create background worker with options ({options}).")
 
         task = asyncio.run_coroutine_threadsafe(self.__create_background_task(task_func, **options), self._loop)
         self._tasks.append(task)
 
         return task
 
     def unregister_background_task(self, background_task, msg=""):
```

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/event/event_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/event/event_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/client_wrapper.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/external_task_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/external_task_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,20 +71,20 @@
     def __start_subscription(self, topic, handler, task_options):
         async def bg_job_handle_external_tasks():
             try:
                 await self.handle_external_tasks(topic, handler, task_options)
             except Exception as e:
                 if type(e) is errno.EPIPE:
                     # Raised while long polling finished, that the reason for only log as info.
-                    logger.info(f"expected long pollng error: {e}")
+                    logger.info(f"Expected long polling error: {e}")
                 else:
                     import traceback
                     import sys
                     traceback.print_exc(file=sys.stdout)
-                    logger.warn(f"exception on handle_external_task: {e}")
+                    logger.warn(f"Exception on handle_external_task: {e}")
 
         async_bg_task = self.__loop_helper.register_background_task(bg_job_handle_external_tasks)
         self._topic_for_handler[topic] = async_bg_task
 
     def subscribe_to_external_tasks_for_topics(self, topics_for_handlers):
         for topic in topics_for_handlers.keys():
             handler = topics_for_handlers[topic] # TODO: Options sollten auch hier zu setzen sein
@@ -97,15 +97,15 @@
         self.__loop_helper.start(run_forever=run_forever)
 
     async def handle_external_tasks(self, topic, handler, task_options):
         external_tasks = await self.__fetch_and_lock(topic, handler, task_options)
 
         len_external_tasks = len(external_tasks)
         if len_external_tasks >= 1:
-            logger.info(f"receive {len_external_tasks} tasks for topic '{topic}'.")
+            logger.info(f"Receive {len_external_tasks} tasks for topic '{topic}'.")
 
             external_task_tasks = []
 
             external_task_options = {
                 'long_polling_timeout_in_ms': task_options.get('long_polling_timeout_in_ms'),
                 'lock_duration_in_ms': task_options.get('lock_duration_in_ms'),
             }
```

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/external_task/external_task_worker.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/external_task/external_task_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self._payload = self._external_task.get('payload', {})
         self._options = options
 
     def __get_lock_duration_in_ms(self):
         lock_duration_in_ms = self._options.get("lock_duration_in_ms", ExternalTaskWorker.LOCK_DURATION_IN_MS)
 
         if lock_duration_in_ms is None:
-            logger.info(f"lock_duration_in_ms is not given, set to default {ExternalTaskWorker.LOCK_DURATION_IN_MS}")
+            logger.info(f":ock_duration_in_ms is not given, set to default {ExternalTaskWorker.LOCK_DURATION_IN_MS}")
             lock_duration_in_ms = ExternalTaskWorker.LOCK_DURATION_IN_MS
 
         return lock_duration_in_ms
 
     def __lock_timeout_in_ms(self):
         lock_duration_in_ms = self.__get_lock_duration_in_ms()
         lock_timeout_in_ms = lock_duration_in_ms * 0.9
@@ -85,15 +85,15 @@
 
         delay_in_seconds = self.__delay_in_seconds()
 
         options = {'delay_in_seconds': delay_in_seconds}
         extend_lock = self._loop_helper.register_background_task(extend_lock_task_wrapper, **options)
         
         external_task_id = self._external_task['id']
-        logger.info(f"starting external task '{external_task_id}' for topic '{self._topic}'")
+        logger.info(f"Starting external task '{external_task_id}' for topic '{self._topic}'")
 
         try:
             result = None
             
             if is_async_handler(self._handler):
                 def handler_wrapper():
                     async def async_handler():
@@ -139,15 +139,15 @@
             
         except FunctionalError as fe:
             logger.warning(f"Finish external task with functional error (code: {fe.get_code()}, message: {fe.get_message()})")
             await self.__finish_task_with_functional_errors(fe.get_code(), fe.get_message(), fe.get_details())
 
         except Exception as e:
             formatted_lines = traceback.format_exc().splitlines()
-            logger.error(f"Finish external task with technial error ({str(e)} -> {formatted_lines})")
+            logger.error(f"Finish external task with technical error ({str(e)} -> {formatted_lines})")
             await self.__finish_task_with_technical_errors(str(e), str(formatted_lines))
         finally:
             self._loop_helper.unregister_background_task(extend_lock, "extend_lock background task")
 
     async def extend_lock(self, worker_id, external_task_id, additional_duration):
         path = f"/atlas_engine/api/v1/external_tasks/{external_task_id}/extend_lock"
         
@@ -162,42 +162,42 @@
         except Exception as e:
             logger.error(f"Error on extend lock for worker {worker_id} for {additional_duration}ms with error {e}")
 
     async def __finish_task_successfully(self, result):
         external_task_id = self._external_task['id']
         worker_id = self._external_task['workerId']
 
-        logger.info(f"finish external task '{external_task_id}' for worker '{worker_id}' and topic '{self._topic}' with result '{result}'")
+        logger.info(f"Finish external task '{external_task_id}' for worker '{worker_id}' and topic '{self._topic}' with result '{result}'")
         path = f"/atlas_engine/api/v1/external_tasks/{external_task_id}/finish"
 
         payload = {
             "workerId": worker_id,
             "result": result
         }
 
         result = await self.do_put(path, payload)
-        logger.info(f"finished external task '{external_task_id}' successfully.")
+        logger.info(f"Finished external task '{external_task_id}' successfully.")
 
     async def __finish_task_with_functional_errors(self, error_code, error_message, error_details=""):
-        logger.warn(f"finished external task_with functional errors '{self._external_task}', '{error_code}', '{error_message}'.")
+        logger.warn(f"Finished external task_with functional errors '{self._external_task}', '{error_code}', '{error_message}'.")
         path = f"/atlas_engine/api/v1/external_tasks/{self._external_task['id']}/handle_bpmn_error"
 
         payload = {
             "workerId": self._external_task['workerId'],
             "bpmnError": {
                 "errorCode": error_code,
                 "errorMessage": error_message,
                 "errorDetails": error_details
             }
         }
 
         await self.do_put(path, payload)
 
     async def __finish_task_with_technical_errors(self, error_message, error_details, error_code=500):
-        logger.warn(f"finished task with technical errors '{self._external_task}', '{error_message}', '{error_details}'.")
+        logger.warn(f"Finished task with technical errors '{self._external_task}', '{error_message}', '{error_details}'.")
         path = f"/atlas_engine/api/v1/external_tasks/{self._external_task['id']}/handle_service_error"
 
         payload = {
             "workerId": self._external_task['workerId'],
             "error": {
                 "errorCode": error_code,
                 "errorMessage": error_message,
```

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/flow_node_instance/flow_node_instance_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/flow_node_instance/flow_node_instance_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/notification/notification_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/notification/notification_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/process_definition/process_definition_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/process_definition/process_definition_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
         payload = {
             "returnOn": int(start_callback_type),
             "processModelId": process_model_id,
             "initialToken": initial_token
         }
 
-        logger.info(f"start process with uri '{path}' and payload '{payload}'")
+        logger.info(f"Start process with uri '{path}' and payload '{payload}'")
 
         result = await self.do_post(path, payload)
 
         return result
 
     async def __start_process_instance_by_start_event(self, process_model_id, start_event_id, end_event_id, **options):
         start_callback_type = options.get('start_callback', StartCallbackType.ON_PROCESSINSTANCE_CREATED)
@@ -42,15 +42,15 @@
             "startEventId": start_event_id,
             "initialToken": initial_token
         }
 
         if end_event_id is not None:
             payload["endEventId"] = end_event_id
 
-        logger.info(f"start process with uri '{path}' and payload '{payload}'")
+        logger.info(f"Start process with uri '{path}' and payload '{payload}'")
 
         result = await self.do_post(path, payload)
 
         return result
 
     def __start_process_instance_wrapper(self, process_model_id, start_event_id=None, end_event_id=None, **options):
```

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/process_instance/process_instance_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/process_instance/process_instance_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client/user_task/user_task_client.py` & `atlas_engine_client-3.1.0a3/atlas_engine_client/user_task/user_task_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/PKG-INFO` & `atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-engine-client
-Version: 3.1.0a2
+Version: 3.1.0a3
 Summary: A Client for the workflow engine of the ProcessCube platform.
 Home-page: https://github.com/atlas-engine/Client.py
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: ProcessCube@5Minds.de
 Keywords: workflow-engine atlas-engine client bpmn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `atlas_engine_client-3.1.0a2/atlas_engine_client.egg-info/SOURCES.txt` & `atlas_engine_client-3.1.0a3/atlas_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/setup.py` & `atlas_engine_client-3.1.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='atlas_engine_client',
-    version=setuptools.sic('3.1.0-alpha.2'),
+    version=setuptools.sic('3.1.0-alpha.3'),
     author="5Minds IT-Solutions GmbH & Co. KG",
     author_email="ProcessCube@5Minds.de",
     description="A Client for the workflow engine of the ProcessCube platform.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="workflow-engine atlas-engine client bpmn",
     url="https://github.com/atlas-engine/Client.py",
```

### Comparing `atlas_engine_client-3.1.0a2/tests/core/test_base_client.py` & `atlas_engine_client-3.1.0a3/tests/core/test_base_client.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/tests/helper_aiohttp.py` & `atlas_engine_client-3.1.0a3/tests/helper_aiohttp.py`

 * *Files identical despite different names*

### Comparing `atlas_engine_client-3.1.0a2/tests/process_control/test_process_control_client.py` & `atlas_engine_client-3.1.0a3/tests/process_control/test_process_control_client.py`

 * *Files identical despite different names*


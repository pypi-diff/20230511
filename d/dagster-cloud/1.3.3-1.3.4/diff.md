# Comparing `tmp/dagster_cloud-1.3.3.tar.gz` & `tmp/dagster_cloud-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.3.3.tar", last modified: Thu May  4 17:55:39 2023, max compression
+gzip compressed data, was "dagster_cloud-1.3.4.tar", last modified: Thu May 11 17:10:42 2023, max compression
```

## Comparing `dagster_cloud-1.3.3.tar` & `dagster_cloud-1.3.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.233870 dagster_cloud-1.3.3/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.237870 dagster_cloud-1.3.3/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.237870 dagster_cloud-1.3.3/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43075 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.241870 dagster_cloud-1.3.3/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.241870 dagster_cloud-1.3.3/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.241870 dagster_cloud-1.3.3/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14188 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.249870 dagster_cloud-1.3.3/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.249870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.253870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.253870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.261870 dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.261870 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26757 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.265870 dagster_cloud-1.3.3/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19041 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     6552 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.273870 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.273870 dagster_cloud-1.3.3/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.277870 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22459 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.281870 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74040 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.237870 dagster_cloud-1.3.3/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.827479 dagster_cloud-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-11 17:10:42.827479 dagster_cloud-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.735480 dagster_cloud-1.3.4/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.739480 dagster_cloud-1.3.4/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.739480 dagster_cloud-1.3.4/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43075 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.743480 dagster_cloud-1.3.4/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.743480 dagster_cloud-1.3.4/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.743480 dagster_cloud-1.3.4/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.747480 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.751480 dagster_cloud-1.3.4/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.755480 dagster_cloud-1.3.4/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.759480 dagster_cloud-1.3.4/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.759480 dagster_cloud-1.3.4/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.771480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.779480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.787480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.787480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.791480 dagster_cloud-1.3.4/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.791480 dagster_cloud-1.3.4/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.795480 dagster_cloud-1.3.4/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.795480 dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.799480 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    26932 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.803480 dagster_cloud-1.3.4/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19041 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.803480 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.803480 dagster_cloud-1.3.4/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.807479 dagster_cloud-1.3.4/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.807479 dagster_cloud-1.3.4/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.811480 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.815480 dagster_cloud-1.3.4/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.819480 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23263 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    21621 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.819480 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.823480 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74026 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.739480 dagster_cloud-1.3.4/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 17:10:42.827479 dagster_cloud-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/setup.py
```

### Comparing `dagster_cloud-1.3.3/PKG-INFO` & `dagster_cloud-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.3.3
+Version: 1.3.4
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.3/README.md` & `dagster_cloud-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.3.4/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/agent/queries.py` & `dagster_cloud-1.3.4/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.3.4/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/auth/constants.py` & `dagster_cloud-1.3.4/dagster_cloud/auth/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,22 @@
     return f"agent:{organization_name}:hardcoded"
 
 
 def get_hardcoded_test_user_token(organization_name, user_name) -> str:
     return f"user:{organization_name}:{user_name}"
 
 
+def get_organization_public_id_from_api_token(api_token: str) -> Optional[str]:
+    split_token = api_token.split(":")
+    if len(split_token) != 4:
+        raise Exception("Could not derive organization from api token")
+
+    return split_token[2]
+
+
 def get_organization_name_from_agent_token(agent_token: str) -> Optional[str]:
     split_token = agent_token.split(":")
 
     # Legacy agent token format - organization must be specified in dagster.yaml
     if len(split_token) == 1:
         return None
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         return check_on_process(pid) == TaskStatus.RUNNING
 
     def terminate(self, run_id):
         run = self._instance.get_run_by_id(run_id)
         if not run:
             return False
 
+        self._instance.report_run_canceling(run)
+
         pid = self._get_pid(run)
         if not pid:
             return False
 
-        self._instance.report_run_canceling(run)
-
         kill_process(pid)
 
         return True
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.3.4/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.3.4/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.3.4/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/client.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,15 @@
 
     def get_records_for_run(
         self,
         run_id: str,
         cursor: Optional[str] = None,
         of_type: Optional[Union[DagsterEventType, Set[DagsterEventType]]] = None,
         limit: Optional[int] = None,
+        ascending: bool = True,
     ) -> EventLogConnection:
         check.invariant(not of_type or isinstance(of_type, (DagsterEventType, frozenset, set)))
 
         is_of_type_set = isinstance(of_type, (set, frozenset))
 
         res = self._execute_query(
             GET_RECORDS_FOR_RUN_QUERY,
@@ -304,14 +305,16 @@
                 ),
                 "ofTypes": (
                     [dagster_type.value for dagster_type in cast(set, of_type)]
                     if of_type and is_of_type_set
                     else None
                 ),
                 "limit": limit,
+                # only send False for back-compat since True is the default
+                **({"ascending": False} if not ascending else {}),
             },
         )
         connection_data = res["data"]["eventLogs"]["getRecordsForRun"]
         return EventLogConnection(
             records=[_event_record_from_graphql(record) for record in connection_data["records"]],
             cursor=connection_data["cursor"],
             has_more=connection_data["hasMore"],
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.3.4/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/util/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,31 @@
 DEFAULT_ECS_GRACE_PERIOD = 30
 
 STOPPED_TASK_GRACE_PERIOD = 30
 
 config = Config(retries={"max_attempts": 50, "mode": "standard"})
 
 
+def get_debug_ecs_prompt(cluster: str, task_arn: str) -> str:
+    return (
+        "For more information about the failure, check the ECS console for logs for task"
+        f" {task_arn} in cluster {cluster}."
+    )
+
+
 class EcsServiceError(Exception):
-    def __init__(self, task_arn, stopped_reason, logs):
-        log_str = "Task logs:\n" + "\n".join(logs) if logs else ""
-        message = f"ECS service failed because task {task_arn} failed: {stopped_reason}\n{log_str}"
+    def __init__(self, cluster, task_arn, stopped_reason, logs, show_debug_prompt: bool):
+        log_str = "Task logs:\n" + "\n".join(logs) if logs else "No task logs."
+
+        message = (
+            f"ECS service failed because task {task_arn} failed: {stopped_reason}\n\n{log_str}"
+        )
+
+        if show_debug_prompt:
+            message = message + f"\n\n{get_debug_ecs_prompt(cluster, task_arn)}"
         super().__init__(message)
 
 
 class Client:
     def __init__(
         self,
         cluster_name: str,
@@ -35,27 +48,31 @@
         log_group: str,
         subnet_ids: Optional[List[str]] = None,
         security_group_ids: Optional[List[str]] = None,
         ecs_client=None,
         timeout: int = DEFAULT_ECS_TIMEOUT,
         grace_period: int = DEFAULT_ECS_GRACE_PERIOD,
         launch_type: str = "FARGATE",
+        show_debug_cluster_info: bool = True,
     ):
         self.ecs = ecs_client if ecs_client else boto3.client("ecs", config=config)
         self.logs = boto3.client("logs", config=config)
         self.service_discovery = boto3.client("servicediscovery", config=config)
         self.ec2 = boto3.resource("ec2", config=config)
 
         self.cluster_name = cluster_name.split("/")[-1]
         self.subnet_ids = check.opt_list_param(subnet_ids, "subnet_ids")
         self.security_group_ids = check.opt_list_param(security_group_ids, "security_group_ids")
         self.service_discovery_namespace_id = check.str_param(
             service_discovery_namespace_id, "service_discovery_namespace_id"
         )
         self.log_group = check.str_param(log_group, "log_group")
+
+        self.show_debug_cluster_info = show_debug_cluster_info
+
         self.timeout = check.int_param(timeout, "timeout")
         self.grace_period = check.int_param(grace_period, "grace_period")
         self.launch_type = check.str_param(launch_type, "launch_type")
         self._namespace: Optional[str] = None
 
     @property
     def namespace(self):
@@ -311,15 +328,18 @@
         for page in paginator.paginate(cluster=self.cluster_name):
             for arn in page.get("serviceArns"):
                 service = Service(client=self, arn=arn)
                 services.append(service)
 
         return services
 
-    def run_task(self, name, image, command, execution_role_arn):
+    def _run_task(self, name, image, command, execution_role_arn):
+        """This is no longer used except as an integration test util
+        for testing various network configurations.
+        """
         task_definition_arn = self.register_task_definition(
             family=name,
             image=image,
             command=command,
             execution_role_arn=execution_role_arn,
         )
 
@@ -445,15 +465,21 @@
         logs = None
 
         try:
             logs = self.get_task_logs(task_arn, container_name=container_name)
         except:
             logger.exception(f"Error trying to get logs for failed task {task_arn}")
 
-        raise EcsServiceError(task_arn=task_arn, stopped_reason=stopped_reason, logs=logs)
+        raise EcsServiceError(
+            cluster=self.cluster_name,
+            task_arn=task_arn,
+            stopped_reason=stopped_reason,
+            logs=logs,
+            show_debug_prompt=self.show_debug_cluster_info,
+        )
 
     def assert_task_not_stopped(self, task_arn, container_name, logger=None):
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
         task = self.ecs.describe_tasks(cluster=self.cluster_name, tasks=[task_arn]).get("tasks")[0]
         if task.get("lastStatus") == "STOPPED":
             self._raise_failed_task(task, container_name, logger)
@@ -461,15 +487,15 @@
     def check_service_has_running_task(self, service_name, container_name, logger=None) -> str:
         # return the ARN of the task if it starts
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
         start_time = time.time()
 
         task_to_track = None
 
-        while start_time + 300 > time.time():
+        while start_time + self.timeout > time.time():
             # Check for a running task to track
             if not task_to_track:
                 running = self.ecs.list_tasks(
                     cluster=self.cluster_name,
                     serviceName=service_name,
                     desiredStatus="RUNNING",
                 ).get("taskArns")
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     SHARED_USER_CODE_LAUNCHER_CONFIG,
     DagsterCloudGrpcServer,
     DagsterCloudUserCodeLauncher,
     ServerEndpoint,
 )
 from dagster_cloud.workspace.user_code_launcher.utils import deterministic_label_for_location
 
+from .client import get_debug_ecs_prompt
 from .run_launcher import CloudEcsRunLauncher
 from .utils import get_task_definition_family
 
 EcsServerHandleType = Service
 
 CONTAINER_NAME = "dagster"
 PORT = 4000
@@ -115,21 +116,26 @@
 
         self.client = Client(
             cluster_name=self.cluster,
             subnet_ids=self.subnets,
             security_group_ids=security_group_ids,
             service_discovery_namespace_id=self.service_discovery_namespace_id,
             log_group=self.log_group,
+            show_debug_cluster_info=self.show_debug_cluster_info,
             timeout=self._ecs_timeout,
             grace_period=self._ecs_grace_period,
             launch_type=self.launch_type,
         )
         super(EcsUserCodeLauncher, self).__init__(**kwargs)
 
     @property
+    def show_debug_cluster_info(self) -> bool:
+        return True
+
+    @property
     def requires_images(self):
         return True
 
     @classmethod
     def config_type(cls):
         return merge_dicts(
             {
@@ -172,22 +178,27 @@
                     ),
                 ),
                 "server_process_startup_timeout": Field(
                     IntSource,
                     is_required=False,
                     default_value=DEFAULT_SERVER_PROCESS_STARTUP_TIMEOUT,
                     description=(
-                        "Timeout when waiting for a code server to be ready after it is created"
+                        "Timeout when waiting for a code server to be ready after it is created."
+                        " You might want to increase this if your ECS tasks are successfully"
+                        " starting but your gRPC server is timing out."
                     ),
                 ),
                 "ecs_timeout": Field(
                     IntSource,
                     is_required=False,
                     default_value=DEFAULT_ECS_TIMEOUT,
-                    description="How long (in seconds) to poll against ECS API endpoints",
+                    description=(
+                        "How long (in seconds) to poll against ECS API endpoints. You might want to"
+                        " increase this if your ECS tasks are taking too long to start up."
+                    ),
                 ),
                 "ecs_grace_period": Field(
                     IntSource,
                     is_required=False,
                     default_value=DEFAULT_ECS_GRACE_PERIOD,
                     description=(
                         "How long (in seconds) to continue polling if an ECS API endpoint fails "
@@ -364,14 +375,32 @@
             multipex_endpoint.create_multipex_client(),
             timeout=self._server_process_startup_timeout,
             additional_check=lambda: self.client.assert_task_not_stopped(
                 task_arn, CONTAINER_NAME, self._logger
             ),
         )
 
+    def _get_timeout_debug_info(
+        self,
+        task_arn,
+    ):
+        sections = []
+
+        try:
+            logs = self.client.get_task_logs(task_arn, container_name=CONTAINER_NAME)
+            task_logs = "Task logs:\n" + "\n".join(logs) if logs else "No logs in task."
+            sections.append(task_logs)
+        except:
+            self._logger.exception("Error trying to get logs for failed task", task_arn=task_arn)
+
+        if self.show_debug_cluster_info:
+            sections.append(get_debug_ecs_prompt(self.cluster, task_arn))
+
+        return "\n\n".join(sections)
+
     def _wait_for_new_server_ready(
         self,
         _deployment_name: str,
         _location_name: str,
         _metadata: CodeDeploymentMetadata,
         server_handle: Service,
         server_endpoint: ServerEndpoint,
@@ -384,14 +413,15 @@
         )
         self._wait_for_dagster_server_process(
             client=server_endpoint.create_client(),
             timeout=self._server_process_startup_timeout,
             additional_check=lambda: self.client.assert_task_not_stopped(
                 task_arn, CONTAINER_NAME, self._logger
             ),
+            get_timeout_debug_info=lambda: self._get_timeout_debug_info(task_arn),
         )
 
     def _remove_server_handle(self, server_handle: EcsServerHandleType) -> None:
         self._logger.info(
             "Deleting service {} at hostname {}...".format(
                 server_handle.name, server_handle.hostname
             )
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 "location_hash": deterministic_label_for_location(deployment_name, location_name),
                 "location_name": get_k8s_human_readable_label(location_name),
                 "deployment_name": get_k8s_human_readable_label(deployment_name),
             },
         ),
         spec=client.V1ServiceSpec(
             selector={"user-deployment": service_name},
-            ports=[client.V1ServicePort(name="http", protocol="TCP", port=SERVICE_PORT)],
+            ports=[client.V1ServicePort(name="grpc", protocol="TCP", port=SERVICE_PORT)],
         ),
     )
 
 
 def construct_code_location_deployment(
     instance,
     deployment_name,
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1746,17 +1746,16 @@
                         timeout_debug_info = get_timeout_debug_info()
                     except Exception:
                         self._logger.exception("Failure fetching debug info after a timeout")
 
                 raise Exception(
                     f"Timed out after waiting {timeout}s for server"
                     f" {client.host}:{client.port or client.socket}."
-                    + f"\n{timeout_debug_info}"
-                    if timeout_debug_info
-                    else "" + f"\nMost recent connection error: {str(last_error)}"
+                    + (f"\n\n{timeout_debug_info}" if timeout_debug_info else "")
+                    + f"\n\nMost recent connection error: {str(last_error)}"
                 )
 
             time.sleep(1)
 
             if additional_check and (
                 not last_additional_check_time
                 or time.time() - last_additional_check_time > additional_check_interval
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.3.4/dagster_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.3.3
+Version: 1.3.4
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.3/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.3.4/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.3/setup.py` & `dagster_cloud-1.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.3",
-        "dagster-cloud-cli==1.3.3",
+        "dagster==1.3.4",
+        "dagster-cloud-cli==1.3.4",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.19.3",
+            "dagster_k8s==0.19.4",
         ],
-        "docker": ["docker", "dagster_docker==0.19.3"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.19.3"],
-        "ecs": ["dagster_aws==0.19.3", "boto3"],
+        "docker": ["docker", "dagster_docker==0.19.4"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.19.4"],
+        "ecs": ["dagster_aws==0.19.4", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```


# Comparing `tmp/dagster-graphql-1.3.3.tar.gz` & `tmp/dagster-graphql-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.3.tar", last modified: Thu May  4 17:50:47 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.4.tar", last modified: Thu May 11 17:05:47 2023, max compression
```

## Comparing `dagster-graphql-1.3.3.tar` & `dagster-graphql-1.3.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.663851 dagster-graphql-1.3.3/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.667851 dagster-graphql-1.3.3/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21544 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.679851 dagster-graphql-1.3.3/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.683851 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11506 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4404 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12609 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15110 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10796 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8081 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.703851 dagster-graphql-1.3.3/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40446 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16333 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    25158 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.707851 dagster-graphql-1.3.3/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17489 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.715851 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11062 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39461 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.719851 dagster-graphql-1.3.3/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25580 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    36191 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4113 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8309 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7986 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.723851 dagster-graphql-1.3.3/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6376 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:50:47.663851 dagster-graphql-1.3.3/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4150 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-04 17:50:47.000000 dagster-graphql-1.3.3/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-04 17:50:47.727851 dagster-graphql-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-04 17:42:13.000000 dagster-graphql-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.131948 dagster-graphql-1.3.4/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.135948 dagster-graphql-1.3.4/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21544 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.151948 dagster-graphql-1.3.4/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.155948 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11506 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8930 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12609 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15110 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8081 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.187948 dagster-graphql-1.3.4/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40498 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16767 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.191948 dagster-graphql-1.3.4/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17489 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.199948 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39461 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25580 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    36191 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8309 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.131948 dagster-graphql-1.3.4/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-11 17:05:47.211948 dagster-graphql-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/setup.py
```

### Comparing `dagster-graphql-1.3.3/LICENSE` & `dagster-graphql-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/PKG-INFO` & `dagster-graphql-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.3
+Version: 1.3.4
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/cli.py` & `dagster-graphql-1.3.4/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/client/client.py` & `dagster-graphql-1.3.4/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.4/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/client/query.py` & `dagster-graphql-1.3.4/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.4/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dagster._core.errors import DagsterError, DagsterUserCodeProcessError
 from dagster._core.events import AssetKey
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
 from dagster._core.execution.job_backfill import submit_backfill_runs
 from dagster._core.host_representation.external_data import ExternalPartitionExecutionErrorData
 from dagster._core.utils import make_new_backfill_id
 from dagster._core.workspace.permissions import Permissions
+from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
 from ..utils import BackfillParams, assert_permission, assert_permission_for_location, capture_error
 
 BACKFILL_CHUNK_SIZE = 25
 
 
@@ -155,15 +156,17 @@
         backfill = PartitionBackfill.from_asset_partitions(
             asset_graph=asset_graph,
             backfill_id=backfill_id,
             tags=tags,
             backfill_timestamp=backfill_timestamp,
             asset_selection=asset_selection,
             partition_names=backfill_params.get("partitionNames"),
-            dynamic_partitions_store=CachingInstanceQueryer(graphene_info.context.instance),
+            dynamic_partitions_store=CachingInstanceQueryer(
+                graphene_info.context.instance, utc_datetime_from_timestamp(backfill_timestamp)
+            ),
             all_partitions=backfill_params.get("allPartitions", False),
         )
     else:
         raise DagsterError(
             "Backfill requested without specifying partition set selector or asset selection"
         )
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_backfills.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import TYPE_CHECKING, Optional
 
-import dagster._check as check
 from dagster._core.execution.backfill import BulkActionStatus
 
 from .utils import capture_error
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.util import ResolveInfo
 
@@ -12,18 +11,20 @@
         GraphenePartitionBackfill,
         GraphenePartitionBackfills,
     )
 
 
 @capture_error
 def get_backfill(graphene_info: "ResolveInfo", backfill_id: str) -> "GraphenePartitionBackfill":
-    from ..schema.backfill import GraphenePartitionBackfill
+    from ..schema.backfill import GrapheneBackfillNotFoundError, GraphenePartitionBackfill
+
+    backfill_job = graphene_info.context.instance.get_backfill(backfill_id)
+    if backfill_job is None:
+        return GrapheneBackfillNotFoundError(backfill_id)
 
-    # get_backfill can return None but this resolver assumes that the backfill exists
-    backfill_job = check.not_none(graphene_info.context.instance.get_backfill(backfill_id))
     return GraphenePartitionBackfill(backfill_job)
 
 
 @capture_error
 def get_backfills(
     graphene_info: "ResolveInfo",
     status: Optional[BulkActionStatus] = None,
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.4/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -842,36 +842,37 @@
             if (
                 materialized_partition_subset is None
                 or failed_partition_subset is None
                 or in_progress_subset is None
             ):
                 check.failed("Expected partitions subset for a partitioned asset")
 
-            num_materialized = len(materialized_partition_subset)
-            num_materialized_and_not_failed = num_materialized - len(
-                [
-                    k
-                    for k in failed_partition_subset.get_partition_keys()
-                    if k in materialized_partition_subset
-                ]
+            failed_keys = failed_partition_subset.get_partition_keys()
+
+            num_materialized_and_not_failed = len(materialized_partition_subset) - len(
+                [k for k in failed_keys if k in materialized_partition_subset]
             )
             num_materialized_and_not_failed_or_in_progress = num_materialized_and_not_failed - len(
                 [
                     k
                     for k in in_progress_subset.get_partition_keys()
                     if k in materialized_partition_subset
                 ]
             )
 
+            num_failed_and_not_in_progress = len(
+                [k for k in failed_keys if k not in in_progress_subset]
+            )
+
             return GraphenePartitionStats(
                 numMaterialized=num_materialized_and_not_failed_or_in_progress,
                 numPartitions=partitions_def_data.get_partitions_definition().get_num_partitions(
                     dynamic_partitions_store=self._dynamic_partitions_loader
                 ),
-                numFailed=len(failed_partition_subset),
+                numFailed=num_failed_and_not_in_progress,
                 numMaterializing=len(in_progress_subset),
             )
         else:
             return None
 
     def resolve_metadata_entries(
         self, _graphene_info: ResolveInfo
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from ..implementation.fetch_partition_sets import (
     partition_status_counts_from_run_partition_data,
     partition_statuses_from_run_partition_data,
 )
 from .asset_key import GrapheneAssetKey
 from .errors import (
+    GrapheneError,
     GrapheneInvalidOutputError,
     GrapheneInvalidStepError,
     GrapheneInvalidSubsetError,
     GraphenePartitionSetNotFoundError,
     GraphenePipelineNotFoundError,
     GraphenePythonError,
     GrapheneRunConflict,
@@ -392,17 +393,30 @@
             Permissions.LAUNCH_PARTITION_BACKFILL, location_name
         )
 
     def resolve_user(self, _graphene_info: ResolveInfo) -> Optional[str]:
         return self._backfill_job.user
 
 
+class GrapheneBackfillNotFoundError(graphene.ObjectType):
+    class Meta:
+        interfaces = (GrapheneError,)
+        name = "BackfillNotFoundError"
+
+    backfill_id = graphene.NonNull(graphene.String)
+
+    def __init__(self, backfill_id: str):
+        super().__init__()
+        self.backfill_id = backfill_id
+        self.message = f"Backfill {backfill_id} could not be found."
+
+
 class GraphenePartitionBackfillOrError(graphene.Union):
     class Meta:
-        types = (GraphenePartitionBackfill, GraphenePythonError)
+        types = (GraphenePartitionBackfill, GrapheneBackfillNotFoundError, GraphenePythonError)
         name = "PartitionBackfillOrError"
 
 
 class GraphenePartitionBackfills(graphene.ObjectType):
     results = non_null_list(GraphenePartitionBackfill)
 
     class Meta:
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/instigation.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     DeleteDynamicPartitionsRequest,
     RunRequest,
 )
 from dagster._core.definitions.schedule_definition import ScheduleExecutionData
 from dagster._core.definitions.selector import ScheduleSelector, SensorSelector
 from dagster._core.definitions.sensor_definition import SensorExecutionData
 from dagster._core.scheduler.instigation import (
+    DynamicPartitionsRequestResult,
     InstigatorState,
     InstigatorTick,
     InstigatorType,
     ScheduleInstigatorData,
     SensorInstigatorData,
     TickStatus,
 )
@@ -135,35 +136,97 @@
     ADD_PARTITIONS = "ADD_PARTITIONS"
     DELETE_PARTITIONS = "DELETE_PARTITIONS"
 
     class Meta:
         name = "DynamicPartitionsRequestType"
 
 
-class GrapheneDynamicPartitionsRequest(graphene.ObjectType):
+class DynamicPartitionsRequestMixin:
+    # Mixin this class to implement DynamicPartitionsRequest
+    #
+    # Graphene has some strange properties that make it so that you cannot
+    # implement ABCs nor use properties in an overridable way. So the way
+    # the mixin works is that the target classes have to have a method
+    # get_dynamic_partitions_request()
     partitionKeys = graphene.List(graphene.NonNull(graphene.String))
     partitionsDefName = graphene.NonNull(graphene.String)
     type = graphene.NonNull(GrapheneDynamicPartitionsRequestType)
 
     class Meta:
+        name = "DynamicPartitionRequestMixin"
+
+    def get_dynamic_partitions_request(
+        self,
+    ) -> Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest,]:
+        raise NotImplementedError()
+
+    def resolve_partitionKeys(self, _graphene_info: ResolveInfo):
+        return self.get_dynamic_partitions_request().partition_keys
+
+    def resolve_partitionsDefName(self, _graphene_info: ResolveInfo):
+        return self.get_dynamic_partitions_request().partitions_def_name
+
+    def resolve_type(self, _graphene_info: ResolveInfo):
+        return (
+            GrapheneDynamicPartitionsRequestType.ADD_PARTITIONS
+            if isinstance(self.get_dynamic_partitions_request(), AddDynamicPartitionsRequest)
+            else GrapheneDynamicPartitionsRequestType.DELETE_PARTITIONS
+        )
+
+
+class GrapheneDynamicPartitionsRequest(DynamicPartitionsRequestMixin, graphene.ObjectType):
+    class Meta:
         name = "DynamicPartitionRequest"
 
     def __init__(
         self,
         dynamic_partition_request: Union[
             AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest
         ],
     ):
-        super().__init__(
-            type=GrapheneDynamicPartitionsRequestType.ADD_PARTITIONS
-            if isinstance(dynamic_partition_request, AddDynamicPartitionsRequest)
-            else GrapheneDynamicPartitionsRequestType.DELETE_PARTITIONS,
-            partitionKeys=dynamic_partition_request.partition_keys,
-            partitionsDefName=dynamic_partition_request.partitions_def_name,
-        )
+        super().__init__()
+        self._dynamic_partitions_request = dynamic_partition_request
+
+    def get_dynamic_partitions_request(
+        self,
+    ) -> Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest,]:
+        return self._dynamic_partitions_request
+
+
+class GrapheneDynamicPartitionsRequestResult(DynamicPartitionsRequestMixin, graphene.ObjectType):
+    class Meta:
+        name = "DynamicPartitionsRequestResult"
+
+    skippedPartitionKeys = non_null_list(graphene.String)
+
+    def __init__(self, dynamic_partitions_request_result: DynamicPartitionsRequestResult):
+        super().__init__()
+        self._dynamic_partitions_request_result = dynamic_partitions_request_result
+
+    def get_dynamic_partitions_request(
+        self,
+    ) -> Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]:
+        if self._dynamic_partitions_request_result.added_partitions is not None:
+            return AddDynamicPartitionsRequest(
+                partition_keys=self._dynamic_partitions_request_result.added_partitions,
+                partitions_def_name=self._dynamic_partitions_request_result.partitions_def_name,
+            )
+        elif self._dynamic_partitions_request_result.deleted_partitions is not None:
+            return DeleteDynamicPartitionsRequest(
+                partition_keys=self._dynamic_partitions_request_result.deleted_partitions,
+                partitions_def_name=self._dynamic_partitions_request_result.partitions_def_name,
+            )
+        else:
+            check.failed(
+                "Unexpected dynamic_partitions_request_result"
+                f" {self._dynamic_partitions_request_result}"
+            )
+
+    def resolve_skippedPartitionKeys(self, _graphene_info: ResolveInfo):
+        return self._dynamic_partitions_request_result.skipped_partitions
 
 
 class GrapheneInstigationTick(graphene.ObjectType):
     id = graphene.NonNull(graphene.ID)
     status = graphene.NonNull(GrapheneInstigationTickStatus)
     timestamp = graphene.NonNull(graphene.Float)
     runIds = non_null_list(graphene.String)
@@ -171,14 +234,15 @@
     error = graphene.Field(GraphenePythonError)
     skipReason = graphene.String()
     cursor = graphene.String()
     runs = non_null_list("dagster_graphql.schema.pipelines.pipeline.GrapheneRun")
     originRunIds = non_null_list(graphene.String)
     logKey = graphene.List(graphene.NonNull(graphene.String))
     logEvents = graphene.Field(graphene.NonNull(GrapheneInstigationEventConnection))
+    dynamicPartitionsRequestResults = non_null_list(GrapheneDynamicPartitionsRequestResult)
 
     class Meta:
         name = "InstigationTick"
 
     def __init__(self, _, tick):
         self._tick = check.inst_param(tick, "tick", InstigatorTick)
 
@@ -211,14 +275,20 @@
         }
 
         return [GrapheneRun(records_by_id[run_id]) for run_id in run_ids if run_id in records_by_id]
 
     def resolve_logEvents(self, graphene_info: ResolveInfo):
         return get_tick_log_events(graphene_info, self._tick)
 
+    def resolve_dynamicPartitionsRequestResults(self, _):
+        return [
+            GrapheneDynamicPartitionsRequestResult(request_result)
+            for request_result in self._tick.dynamic_partitions_request_results
+        ]
+
 
 class GrapheneDryRunInstigationTick(graphene.ObjectType):
     timestamp = graphene.Float()
     evaluationResult = graphene.Field(lambda: GrapheneTickEvaluation)
 
     class Meta:
         name = "DryRunInstigationTick"
@@ -309,15 +379,18 @@
     cursor = graphene.String()
 
     _execution_data: Union[ScheduleExecutionData, SensorExecutionData, SerializableErrorInfo]
 
     class Meta:
         name = "TickEvaluation"
 
-    def __init__(self, execution_data):
+    def __init__(
+        self,
+        execution_data: Union[ScheduleExecutionData, SensorExecutionData, SerializableErrorInfo],
+    ):
         check.inst_param(
             execution_data,
             "execution_data",
             (ScheduleExecutionData, SensorExecutionData, SerializableErrorInfo),
         )
         error = (
             GraphenePythonError(execution_data)
@@ -331,34 +404,43 @@
         )
         self._execution_data = execution_data
         self._run_requests = (
             execution_data.run_requests
             if not isinstance(execution_data, SerializableErrorInfo)
             else None
         )
-        dynamicPartitionsRequests = None
-        if isinstance(execution_data, SensorExecutionData):
-            dynamicPartitionsRequests = [
-                GrapheneDynamicPartitionsRequest(request)
-                for request in execution_data.dynamic_partitions_requests
-            ]
+
+        self._dynamic_partitions_requests = (
+            execution_data.dynamic_partitions_requests
+            if isinstance(execution_data, SensorExecutionData)
+            else None
+        )
+
         cursor = execution_data.cursor if isinstance(execution_data, SensorExecutionData) else None
         super().__init__(
             skipReason=skip_reason,
             error=error,
             cursor=cursor,
-            dynamicPartitionsRequests=dynamicPartitionsRequests,
         )
 
     def resolve_runRequests(self, _graphene_info: ResolveInfo):
         if not self._run_requests:
             return self._run_requests
 
         return [GrapheneRunRequest(run_request) for run_request in self._run_requests]
 
+    def resolve_dynamicPartitionsRequests(self, _graphene_info: ResolveInfo):
+        if not self._dynamic_partitions_requests:
+            return self._dynamic_partitions_requests
+
+        return [
+            GrapheneDynamicPartitionsRequest(request)
+            for request in self._dynamic_partitions_requests
+        ]
+
 
 class GrapheneRunRequest(graphene.ObjectType):
     runKey = graphene.String()
     tags = non_null_list(GraphenePipelineTag)
     runConfigYaml = graphene.NonNull(graphene.String)
     assetSelection = graphene.List(graphene.NonNull(GrapheneAssetKey))
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/run_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Any, Optional
 
 import dagster._check as check
 import graphene
+from dagster._config.snap import ConfigSchemaSnapshot
 from dagster._core.host_representation import RepresentedJob
 from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
+from dagster._core.snap.snap_to_yaml import default_values_yaml_from_type_snap
 
 from ..implementation.run_config_schema import resolve_is_run_config_valid
 from .config_types import GrapheneConfigType, to_config_type
 from .errors import (
     GrapheneInvalidSubsetError,
     GrapheneModeNotFoundError,
     GraphenePipelineNotFoundError,
@@ -39,14 +41,21 @@
         description="""Parse a particular run config result. The return value
         either indicates that the validation succeeded by returning
         `PipelineConfigValidationValid` or that there are configuration errors
         by returning `RunConfigValidationInvalid' which containers a list errors
         so that can be rendered for the user""",
     )
 
+    rootDefaultYaml = graphene.Field(
+        graphene.NonNull(graphene.String),
+        description="""The default configuration for this run in yaml. This is
+        so that the client does not have to parse JSON client side and assemble
+        it into a single yaml document.""",
+    )
+
     class Meta:
         description = """The run config schema represents the all the config type
         information given a certain execution selection and mode of execution of that
         selection. All config interactions (e.g. checking config validity, fetching
         all config types, fetching in a particular config type) should be done
         through this type """
         name = "RunConfigSchema"
@@ -83,14 +92,25 @@
         return resolve_is_run_config_valid(
             graphene_info,
             self._represented_job,
             self._mode,
             parse_run_config_input(runConfigData or {}, raise_on_error=False),  # type: ignore
         )
 
+    def resolve_rootDefaultYaml(self, _graphene_info) -> str:
+        config_schema_snapshot: ConfigSchemaSnapshot = self._represented_job.config_schema_snapshot
+
+        root_key = check.not_none(
+            self._represented_job.get_mode_def_snap(self._mode).root_config_key
+        )
+
+        root_type = config_schema_snapshot.get_config_snap(root_key)
+
+        return default_values_yaml_from_type_snap(config_schema_snapshot, root_type)
+
 
 class GrapheneRunConfigSchemaOrError(graphene.Union):
     class Meta:
         types = (
             GrapheneRunConfigSchema,
             GraphenePipelineNotFoundError,
             GrapheneInvalidSubsetError,
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.4/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.4/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.4/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.3
+Version: 1.3.4
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.3/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.4/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.3/setup.py` & `dagster-graphql-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.3",
+        "dagster==1.3.4",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```


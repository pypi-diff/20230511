# Comparing `tmp/ob-metaflow-2.8.4.1.tar.gz` & `tmp/ob-metaflow-2.8.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-2.8.4.1.tar", last modified: Fri May  5 18:19:33 2023, max compression
+gzip compressed data, was "ob-metaflow-2.8.4.2.tar", last modified: Thu May 11 15:55:54 2023, max compression
```

## Comparing `ob-metaflow-2.8.4.1.tar` & `ob-metaflow-2.8.4.2.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.709185 ob-metaflow-2.8.4.1/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.709185 ob-metaflow-2.8.4.1/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68712 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31074 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.713185 ob-metaflow-2.8.4.1/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.717185 ob-metaflow-2.8.4.1/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.717185 ob-metaflow-2.8.4.1/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18335 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.717185 ob-metaflow-2.8.4.1/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.717185 ob-metaflow-2.8.4.1/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.717185 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.717185 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    96242 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42423 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.721185 ob-metaflow-2.8.4.1/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.725185 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26463 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55864 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tracing_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tracing_otel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tracing_propagator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.705185 ob-metaflow-2.8.4.1/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.729185 ob-metaflow-2.8.4.1/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-05 18:19:33.000000 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-05 18:19:33.000000 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:19:33.000000 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 18:19:33.000000 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 18:19:33.000000 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 18:19:33.000000 ob-metaflow-2.8.4.1/ob_metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 18:19:33.733185 ob-metaflow-2.8.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-05 18:19:22.000000 ob-metaflow-2.8.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.092694 ob-metaflow-2.8.4.2/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68712 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31074 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18335 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96242 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42423 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26463 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55864 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing_otel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing_propagator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.088694 ob-metaflow-2.8.4.2/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/setup.py
```

### Comparing `ob-metaflow-2.8.4.1/LICENSE` & `ob-metaflow-2.8.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/PKG-INFO` & `ob-metaflow-2.8.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow
-Version: 2.8.4.1
+Version: 2.8.4.2
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ob-metaflow-2.8.4.1/README.md` & `ob-metaflow-2.8.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/R.py` & `ob-metaflow-2.8.4.2/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/_bashcomplete.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/_compat.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/_termui_impl.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/_textwrap.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/_unicodefun.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/_winconsole.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/core.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/decorators.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/exceptions.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/formatting.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/globals.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/parser.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/termui.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/testing.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/types.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/click/utils.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_5/zipp.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/typing_extensions.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/_vendor/v3_6/zipp.py` & `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/cli.py` & `ob-metaflow-2.8.4.2/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/cli_args.py` & `ob-metaflow-2.8.4.2/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/client/core.py` & `ob-metaflow-2.8.4.2/metaflow/client/core.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/client/filecache.py` & `ob-metaflow-2.8.4.2/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/cmd/configure_cmd.py` & `ob-metaflow-2.8.4.2/metaflow/cmd/configure_cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/cmd/main_cli.py` & `ob-metaflow-2.8.4.2/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/cmd/tutorials_cmd.py` & `ob-metaflow-2.8.4.2/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/cmd_with_io.py` & `ob-metaflow-2.8.4.2/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/current.py` & `ob-metaflow-2.8.4.2/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/datastore/content_addressed_store.py` & `ob-metaflow-2.8.4.2/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/datastore/datastore_set.py` & `ob-metaflow-2.8.4.2/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/datastore/datastore_storage.py` & `ob-metaflow-2.8.4.2/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/datastore/flow_datastore.py` & `ob-metaflow-2.8.4.2/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/datastore/task_datastore.py` & `ob-metaflow-2.8.4.2/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/debug.py` & `ob-metaflow-2.8.4.2/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/decorators.py` & `ob-metaflow-2.8.4.2/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/event_logger.py` & `ob-metaflow-2.8.4.2/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/events.py` & `ob-metaflow-2.8.4.2/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/exception.py` & `ob-metaflow-2.8.4.2/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/extension_support/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/extension_support/cmd.py` & `ob-metaflow-2.8.4.2/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/extension_support/integrations.py` & `ob-metaflow-2.8.4.2/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/extension_support/plugins.py` & `ob-metaflow-2.8.4.2/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/flowspec.py` & `ob-metaflow-2.8.4.2/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/graph.py` & `ob-metaflow-2.8.4.2/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/includefile.py` & `ob-metaflow-2.8.4.2/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/integrations.py` & `ob-metaflow-2.8.4.2/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/lint.py` & `ob-metaflow-2.8.4.2/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metadata/heartbeat.py` & `ob-metaflow-2.8.4.2/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metadata/metadata.py` & `ob-metaflow-2.8.4.2/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metadata/util.py` & `ob-metaflow-2.8.4.2/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metaflow_config.py` & `ob-metaflow-2.8.4.2/metaflow/metaflow_config.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metaflow_config_funcs.py` & `ob-metaflow-2.8.4.2/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metaflow_environment.py` & `ob-metaflow-2.8.4.2/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/metaflow_version.py` & `ob-metaflow-2.8.4.2/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/mflog/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/mflog/mflog.py` & `ob-metaflow-2.8.4.2/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/mflog/save_logs.py` & `ob-metaflow-2.8.4.2/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/mflog/save_logs_periodically.py` & `ob-metaflow-2.8.4.2/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/mflog/tee.py` & `ob-metaflow-2.8.4.2/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/monitor.py` & `ob-metaflow-2.8.4.2/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/multicore_utils.py` & `ob-metaflow-2.8.4.2/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/package.py` & `ob-metaflow-2.8.4.2/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/parameters.py` & `ob-metaflow-2.8.4.2/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/airflow_utils.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/plumbing/set_parameters.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/base_sensor.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/airflow/sensors/s3_sensor.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_events.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_events.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_workflows.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_workflows_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/argo/argo_workflows_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/argo/process_input_paths.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/aws_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/aws_utils.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/batch/batch_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/production_token.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/azure/azure_tail.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/azure/azure_utils.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/azure/blob_service_client_factory.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/azure/includefile_support.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_datastore.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/base.html` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/basic.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/bundle.css` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/card.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/main.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/components.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/main.js` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/renderer_tools.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_modules/test_cards.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/card_resolver.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/component_serializer.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/cards/exception.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/catch_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/conda/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/conda/batch_bootstrap.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda_environment.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda_flow_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/conda/conda_step_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datastores/azure_storage.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datastores/gs_storage.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datastores/local_storage.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datastores/s3_storage.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datatools/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datatools/local.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3op.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3tail.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/datatools/s3/s3util.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/debug_logger.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/debug_monitor.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/__init__.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/client_modules.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/bytestream.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/channel.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/communication/utils.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/consts.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/data_transferer.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/exception_transferer.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/override_decorators.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/server.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/stub.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/env_escape/utils.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/environment_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/events_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/frameworks/pytorch.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_storage_client_factory.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_tail.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/gcp/gs_utils.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/gcp/includefile_support.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_client.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/kubernetes/kubernetes_job.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/metadata/local.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/metadata/service.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/package_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/parallel_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/project_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/resources_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/retry_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/secrets/secrets_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/storage_executor.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/tag_cli.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/test_unbounded_foreach_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/plugins/timeout_decorator.py` & `ob-metaflow-2.8.4.2/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/procpoll.py` & `ob-metaflow-2.8.4.2/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/pylint_wrapper.py` & `ob-metaflow-2.8.4.2/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/runtime.py` & `ob-metaflow-2.8.4.2/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar.py` & `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar_messages.py` & `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar_subprocess.py` & `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/sidecar/sidecar_worker.py` & `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tagging_util.py` & `ob-metaflow-2.8.4.2/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/task.py` & `ob-metaflow-2.8.4.2/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tracing.py` & `ob-metaflow-2.8.4.2/metaflow/tracing.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tracing_noop.py` & `ob-metaflow-2.8.4.2/metaflow/tracing_noop.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tracing_otel.py` & `ob-metaflow-2.8.4.2/metaflow/tracing_otel.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 
     set_global_textmap(EnvPropagator(None))
 
     if SERVICE_AUTH_KEY:
         span_exporter = OTLPSpanExporter(
             endpoint=OTEL_ENDPOINT,
             headers={"x-api-key": SERVICE_AUTH_KEY},
-            timeout=1,
+            timeout=10,
         )
     elif SERVICE_HEADERS:
         span_exporter = OTLPSpanExporter(
             endpoint=OTEL_ENDPOINT,
             headers=SERVICE_HEADERS,
-            timeout=1,
+            timeout=10,
         )
     else:
         print("WARNING: no auth settings for Opentelemetry", file=sys.stderr)
         return
 
     if "METAFLOW_KUBERNETES_POD_NAMESPACE" in os.environ:
         service_name = "metaflow-kubernetes"
```

### Comparing `ob-metaflow-2.8.4.1/metaflow/tracing_propagator.py` & `ob-metaflow-2.8.4.2/metaflow/tracing_propagator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/00-helloworld/helloworld.py` & `ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/movies.csv` & `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/playlist.ipynb` & `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/01-playlist/playlist.py` & `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/movies.csv` & `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/stats.ipynb` & `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/02-statistics/stats.py` & `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/03-playlist-redux/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/03-playlist-redux/playlist.py` & `ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/04-playlist-plus/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/04-playlist-plus/playlist.py` & `ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/06-statistics-redux/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/07-worldview/worldview.ipynb` & `ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/08-autopilot/README.md` & `ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/util.py` & `ob-metaflow-2.8.4.2/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/metaflow/vendor.py` & `ob-metaflow-2.8.4.2/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/ob_metaflow.egg-info/PKG-INFO` & `ob-metaflow-2.8.4.2/ob_metaflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow
-Version: 2.8.4.1
+Version: 2.8.4.2
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ob-metaflow-2.8.4.1/ob_metaflow.egg-info/SOURCES.txt` & `ob-metaflow-2.8.4.2/ob_metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.1/setup.py` & `ob-metaflow-2.8.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.8.4.1"
+version = "2.8.4.2"
 
 setup(
     include_package_data=True,
     name="ob-metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```


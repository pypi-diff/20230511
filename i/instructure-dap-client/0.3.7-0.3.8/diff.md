# Comparing `tmp/instructure-dap-client-0.3.7.tar.gz` & `tmp/instructure-dap-client-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructure-dap-client-0.3.7.tar", last modified: Wed Apr 19 18:01:45 2023, max compression
+gzip compressed data, was "instructure-dap-client-0.3.8.tar", last modified: Thu May 11 13:18:16 2023, max compression
```

## Comparing `instructure-dap-client-0.3.7.tar` & `instructure-dap-client-0.3.8.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.378236 instructure-dap-client-0.3.7/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.7/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18505 2023-04-19 18:01:45.378531 instructure-dap-client-0.3.7/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    17706 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.344117 instructure-dap-client-0.3.7/dap/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       22 2023-04-19 07:04:39.000000 instructure-dap-client-0.3.7/dap/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4382 2023-04-04 13:12:06.000000 instructure-dap-client-0.3.7/dap/__main__.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.346893 instructure-dap-client-0.3.7/dap/actions/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/actions/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/actions/drop_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/actions/init_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/actions/sync_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    20570 2023-04-04 13:08:40.000000 instructure-dap-client-0.3.7/dap/api.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2980 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.7/dap/arguments.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.359203 instructure-dap-client-0.3.7/dap/commands/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.7/dap/commands/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      457 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/commands/abstract_db_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/base.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.7/dap/commands/commands.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2611 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.7/dap/commands/commonargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/dbargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/dropdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1361 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/initdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/queryargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1695 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/syncdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/timestampargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/concurrency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2920 2023-04-14 16:20:35.000000 instructure-dap-client-0.3.7/dap/dap_error.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18455 2023-04-04 13:07:56.000000 instructure-dap-client-0.3.7/dap/dap_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.367048 instructure-dap-client-0.3.7/dap/database/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/database/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2316 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/database/base_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/database/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/database/database_errors.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3835 2023-04-19 07:03:02.000000 instructure-dap-client-0.3.7/dap/database/database_operations.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2720 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/database/init_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3661 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/database/sync_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5759 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/downloader.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      669 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/log.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.369231 instructure-dap-client-0.3.7/dap/model/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.7/dap/model/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8026 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/model/meta_table.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6184 2023-04-04 12:03:12.000000 instructure-dap-client-0.3.7/dap/model/metadata.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      850 2023-04-04 12:03:12.000000 instructure-dap-client-0.3.7/dap/networking.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.7/dap/payload.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.371003 instructure-dap-client-0.3.7/dap/replicator/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.7/dap/replicator/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2550 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/replicator/sql.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/timer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1450 2023-03-27 20:20:03.000000 instructure-dap-client-0.3.7/dap/timestamp.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6740 2023-04-19 16:25:38.000000 instructure-dap-client-0.3.7/dap/type_conversion.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.377575 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18505 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1327 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/entry_points.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      151 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-19 18:01:44.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.7/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1170 2023-04-19 18:01:45.379676 instructure-dap-client-0.3.7/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.7/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.039677 instructure-dap-client-0.3.8/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19535 2023-05-11 13:18:16.039974 instructure-dap-client-0.3.8/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18685 2023-04-29 10:55:22.000000 instructure-dap-client-0.3.8/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.011392 instructure-dap-client-0.3.8/dap/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      524 2023-05-11 13:17:51.000000 instructure-dap-client-0.3.8/dap/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4416 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/__main__.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.014308 instructure-dap-client-0.3.8/dap/actions/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/actions/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/actions/drop_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/actions/init_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/actions/sync_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21450 2023-05-11 13:12:25.000000 instructure-dap-client-0.3.8/dap/api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2980 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8/dap/arguments.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.022678 instructure-dap-client-0.3.8/dap/commands/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8/dap/commands/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      491 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/commands/abstract_db_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/base.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8/dap/commands/commands.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2611 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8/dap/commands/commonargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/dbargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/dropdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1361 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/initdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/queryargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1695 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/syncdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/commands/timestampargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8/dap/concurrency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6428 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/conversion_common.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      635 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/conversion_nonperf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      701 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/conversion_perf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3261 2023-05-11 13:12:25.000000 instructure-dap-client-0.3.8/dap/dap_error.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18466 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/dap_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.028488 instructure-dap-client-0.3.8/dap/database/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8/dap/database/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2318 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/database/base_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.8/dap/database/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.8/dap/database/database_errors.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3835 2023-04-19 07:03:02.000000 instructure-dap-client-0.3.8/dap/database/database_operations.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2751 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/database/init_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3671 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/database/sync_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5861 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/downloader.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      684 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/log.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.031249 instructure-dap-client-0.3.8/dap/model/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8/dap/model/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      987 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/model/ddl.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16280 2023-05-07 19:02:41.000000 instructure-dap-client-0.3.8/dap/model/meta_table.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7091 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8/dap/model/metadata.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      932 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/networking.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.8/dap/payload.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:15:30.000000 instructure-dap-client-0.3.8/dap/py.typed
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.032922 instructure-dap-client-0.3.8/dap/replicator/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.8/dap/replicator/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2571 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8/dap/replicator/sql.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1355 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8/dap/timer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1450 2023-03-27 20:20:03.000000 instructure-dap-client-0.3.8/dap/timestamp.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-05-11 13:18:16.039004 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19535 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1408 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/entry_points.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      153 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-05-11 13:18:15.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-05-11 13:17:30.000000 instructure-dap-client-0.3.8/instructure_dap_client.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-25 19:13:58.000000 instructure-dap-client-0.3.8/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1254 2023-05-11 13:18:16.041196 instructure-dap-client-0.3.8/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.8/setup.py
```

### Comparing `instructure-dap-client-0.3.7/LICENSE` & `instructure-dap-client-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/PKG-INFO` & `instructure-dap-client-0.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.7
+Version: 0.3.8
 Summary: Data Access Platform client library
 Author: Levente Hunyadi
 Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Access Platform Client Library
 
 Data Access Platform (DAP) acts as a single source of data for analytics at Instructure. It provides efficient access to data collected across various educational products in bulk with high fidelity and low latency, adhering to a canonical data model.
 
@@ -86,14 +88,16 @@
 dap initdb --help
 dap syncdb --help
 dap dropdb --help
 ```
 
 ## Common use cases
 
+If you are a first-time user of DAP client library, it's best to start with two high-level commands of the CLI (command-line interface): `initdb` and `syncdb`. `initdb` fetches the data stored in DAP and replicates them in a (local) database table. It takes care of authenticating with DAP, fetching data schema, creating a database table, starting a snapshot query, monitoring job progress, downloading data, and inserting records into the table. Subsequently, `syncdb` helps keep the database table up-to-date with the data in DAP. As in the case of `initdb`, `syncdb` manages all the details of verifying the data schema, altering database table structure (if necessary), getting the right data and inserting, updating or deleting the corresponding database table records.
+
 ### Obtain a full snapshot of a table in a database or data warehouse
 
 The command-line utility is capable of automatically copying a full table snapshot to a (local) database with the `initdb` command. Along with the parameters `--table` and `--namespace`, you have to specify your target database with a connection string using the `--connection-string` parameter.
 
 Typically, the connection string looks as follows:
 
 ```sh
@@ -189,22 +193,23 @@
 ## Code examples
 
 While basic functionality of the DAP client library is exposed over its command-line interface (CLI), more advanced functionality requires interacting with classes and functions defined in the module `dap.api`. This enables seamless integration into workflow management platforms like Apache Airflow.
 
 First, we need to instantiate the `DAPClient` class:
 
 ```python
+import os
 from dap.api import DAPClient
 from dap.dap_types import Credentials
 
 base_url: str = os.environ["DAP_API_URL"]
 client_id: str = os.environ["DAP_CLIENT_ID"]
 client_secret: str = os.environ["DAP_CLIENT_SECRET"]
 
-credentials = Credentials.create(client_id, client_secret)
+credentials = Credentials.create(client_id=client_id, client_secret=client_secret)
 async with DAPClient(base_url, credentials) as session:
     ...
 ```
 
 However, `DAPClient` can automatically extract the value of these parameters from the above environment variables, allowing us to write:
 
 ```python
@@ -217,39 +222,43 @@
 Let's explore a few common use cases with `DAPClient`.
 
 ### Obtaining the latest schema
 
 Before we obtain data, we need to get the latest schema of a table. The following example retrieves the JSON schema of the table `accounts` in the namespace `canvas` as a JSON schema object. A JSON object is a recursive Python data structure whose outermost layer is a Python `dict` whose keys are strings (type `str`) and values are JSON objects. We can use the Python package [jsonschema](https://python-jsonschema.readthedocs.io/en/stable/) to validate data against this JSON schema.
 
 ```python
+from dap.api import DAPClient
+
 async with DAPClient() as session:
     schema = await session.get_table_schema("canvas", "accounts")
 ```
 
 We can also save the schema to a file. 
 
 ```python
-output_directory: str = os.getcwd()
+import os
+from dap.api import DAPClient
 
+output_directory: str = os.getcwd()
 async with DAPClient() as session:
     tables = await session.get_tables("canvas")
     for table in tables:
         await session.download_table_schema("canvas", table, output_directory)
 ```
 
 ### Fetching table data with a snapshot query
 
 In order to get an initial copy of the full table contents, we need to perform a snapshot query. The parameter `format` determines the output data format, including CSV, TSV, JSONL and Parquet. We recommend JSONL or Parquet. For JSONL, each line in the output can be parsed into a JSON object, conforming to the JSON schema returned above.
 
 ```python
+import os
 from dap.api import DAPClient
 from dap.dap_types import Format, SnapshotQuery
 
 output_directory = os.getcwd()
-
 async with DAPClient() as session:
     query = SnapshotQuery(format=Format.JSONL, filter=None)
     await session.download_table_data("canvas", "accounts", query, output_directory)
 ```
 
 ### Getting latest changes with an incremental query
 
@@ -297,30 +306,33 @@
 
 1. initialize a database, and
 2. synchronize a database with the data in DAP.
 
 In order to replicate data in DAP locally, we must first initialize a database:
 
 ```python
-connection_string: str = "postgresql://scott:password@localhost/testdb"
+from dap.api import DAPClient
+from dap.database.connection import DatabaseConnection
+from dap.replicator.sql import SQLReplicator
 
+connection_string: str = "postgresql://scott:password@localhost/testdb"
 async with DatabaseConnection(connection_string).open() as db_connection:
-    async with DAPClient(base_url, credentials) as session:
+    async with DAPClient() as session:
         await SQLReplicator(session, db_connection).initialize(namespace, table_name)
 ```
 
 Initialization creates a database schema for the DAP namespace, and  a corresponding database table for each DAP table. In addition, it creates a *meta-table*, which is a special database table that holds synchronization information, e.g. the last time the data was synchronized with DAP, and the schema version that the locally stored data conforms to. Finally, it issues a snapshot query to DAP API, and populates the database table with output returned by the snapshot query.
 
 ### Synchronizing data in a local database
 
 Once the table has been initialized, it can be kept up to date using the synchronize operation:
 
 ```python
 async with DatabaseConnection(connection_string).open() as db_connection:
-    async with DAPClient(base_url, credentials) as session:
+    async with DAPClient() as session:
         await SQLReplicator(session, db_connection).synchronize(namespace, table_name)
 ```
 
 This inspects the information in the meta-table, and issues an incremental query to DAP API with a `since` timestamp corresponding to the last synchronization time. Based on the results of the incremental query, it inserts new records, updates existing records, and deletes records that have been added to, updated in, or removed from the DAP service.
 
 If the local schema version in the meta-table is identical to the remote schema version in DAP, inserting, updating and deleting records proceeds normally. However, if there is a mismatch, the table structure of the local database has to evolve to match the current structure of the data in DAP. This includes the following schema changes in the back-end:
```

### Comparing `instructure-dap-client-0.3.7/README.md` & `instructure-dap-client-0.3.8/instructure_dap_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: instructure-dap-client
+Version: 0.3.8
+Summary: Data Access Platform client library
+Author: Levente Hunyadi
+Author-email: levente.hunyadi@instructure.com
+Maintainer: Edina Tipter
+Maintainer-email: edina.tipter@instructure.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Data Access Platform Client Library
 
 Data Access Platform (DAP) acts as a single source of data for analytics at Instructure. It provides efficient access to data collected across various educational products in bulk with high fidelity and low latency, adhering to a canonical data model.
 
 The outgoing interface for DAP is the [Query API](https://data-access-platform-api.s3.amazonaws.com/index.html), which is an HTTP REST service. Users initiate asynchronous queries to retrieve data associated with their account. The client library is a Python wrapper around the DAP API, allowing users to fetch an initial snapshot and incremental changes, or initialize a database and keep it synchronized with data in DAP.
 
 Each DAP user acts as a data administrator for the organization they represent. They have full read access to the top-level account and all descendant sub-accounts. For example, in Canvas, the top of the organization hierarchy is uniquely identified by a root account ID, and each data record is associated with a root account ID. A DAP user with Canvas access can query data that are assigned the user's root account ID.
@@ -64,14 +88,16 @@
 dap initdb --help
 dap syncdb --help
 dap dropdb --help
 ```
 
 ## Common use cases
 
+If you are a first-time user of DAP client library, it's best to start with two high-level commands of the CLI (command-line interface): `initdb` and `syncdb`. `initdb` fetches the data stored in DAP and replicates them in a (local) database table. It takes care of authenticating with DAP, fetching data schema, creating a database table, starting a snapshot query, monitoring job progress, downloading data, and inserting records into the table. Subsequently, `syncdb` helps keep the database table up-to-date with the data in DAP. As in the case of `initdb`, `syncdb` manages all the details of verifying the data schema, altering database table structure (if necessary), getting the right data and inserting, updating or deleting the corresponding database table records.
+
 ### Obtain a full snapshot of a table in a database or data warehouse
 
 The command-line utility is capable of automatically copying a full table snapshot to a (local) database with the `initdb` command. Along with the parameters `--table` and `--namespace`, you have to specify your target database with a connection string using the `--connection-string` parameter.
 
 Typically, the connection string looks as follows:
 
 ```sh
@@ -167,22 +193,23 @@
 ## Code examples
 
 While basic functionality of the DAP client library is exposed over its command-line interface (CLI), more advanced functionality requires interacting with classes and functions defined in the module `dap.api`. This enables seamless integration into workflow management platforms like Apache Airflow.
 
 First, we need to instantiate the `DAPClient` class:
 
 ```python
+import os
 from dap.api import DAPClient
 from dap.dap_types import Credentials
 
 base_url: str = os.environ["DAP_API_URL"]
 client_id: str = os.environ["DAP_CLIENT_ID"]
 client_secret: str = os.environ["DAP_CLIENT_SECRET"]
 
-credentials = Credentials.create(client_id, client_secret)
+credentials = Credentials.create(client_id=client_id, client_secret=client_secret)
 async with DAPClient(base_url, credentials) as session:
     ...
 ```
 
 However, `DAPClient` can automatically extract the value of these parameters from the above environment variables, allowing us to write:
 
 ```python
@@ -195,39 +222,43 @@
 Let's explore a few common use cases with `DAPClient`.
 
 ### Obtaining the latest schema
 
 Before we obtain data, we need to get the latest schema of a table. The following example retrieves the JSON schema of the table `accounts` in the namespace `canvas` as a JSON schema object. A JSON object is a recursive Python data structure whose outermost layer is a Python `dict` whose keys are strings (type `str`) and values are JSON objects. We can use the Python package [jsonschema](https://python-jsonschema.readthedocs.io/en/stable/) to validate data against this JSON schema.
 
 ```python
+from dap.api import DAPClient
+
 async with DAPClient() as session:
     schema = await session.get_table_schema("canvas", "accounts")
 ```
 
 We can also save the schema to a file. 
 
 ```python
-output_directory: str = os.getcwd()
+import os
+from dap.api import DAPClient
 
+output_directory: str = os.getcwd()
 async with DAPClient() as session:
     tables = await session.get_tables("canvas")
     for table in tables:
         await session.download_table_schema("canvas", table, output_directory)
 ```
 
 ### Fetching table data with a snapshot query
 
 In order to get an initial copy of the full table contents, we need to perform a snapshot query. The parameter `format` determines the output data format, including CSV, TSV, JSONL and Parquet. We recommend JSONL or Parquet. For JSONL, each line in the output can be parsed into a JSON object, conforming to the JSON schema returned above.
 
 ```python
+import os
 from dap.api import DAPClient
 from dap.dap_types import Format, SnapshotQuery
 
 output_directory = os.getcwd()
-
 async with DAPClient() as session:
     query = SnapshotQuery(format=Format.JSONL, filter=None)
     await session.download_table_data("canvas", "accounts", query, output_directory)
 ```
 
 ### Getting latest changes with an incremental query
 
@@ -275,30 +306,33 @@
 
 1. initialize a database, and
 2. synchronize a database with the data in DAP.
 
 In order to replicate data in DAP locally, we must first initialize a database:
 
 ```python
-connection_string: str = "postgresql://scott:password@localhost/testdb"
+from dap.api import DAPClient
+from dap.database.connection import DatabaseConnection
+from dap.replicator.sql import SQLReplicator
 
+connection_string: str = "postgresql://scott:password@localhost/testdb"
 async with DatabaseConnection(connection_string).open() as db_connection:
-    async with DAPClient(base_url, credentials) as session:
+    async with DAPClient() as session:
         await SQLReplicator(session, db_connection).initialize(namespace, table_name)
 ```
 
 Initialization creates a database schema for the DAP namespace, and  a corresponding database table for each DAP table. In addition, it creates a *meta-table*, which is a special database table that holds synchronization information, e.g. the last time the data was synchronized with DAP, and the schema version that the locally stored data conforms to. Finally, it issues a snapshot query to DAP API, and populates the database table with output returned by the snapshot query.
 
 ### Synchronizing data in a local database
 
 Once the table has been initialized, it can be kept up to date using the synchronize operation:
 
 ```python
 async with DatabaseConnection(connection_string).open() as db_connection:
-    async with DAPClient(base_url, credentials) as session:
+    async with DAPClient() as session:
         await SQLReplicator(session, db_connection).synchronize(namespace, table_name)
 ```
 
 This inspects the information in the meta-table, and issues an incremental query to DAP API with a `since` timestamp corresponding to the last synchronization time. Based on the results of the incremental query, it inserts new records, updates existing records, and deletes records that have been added to, updated in, or removed from the DAP service.
 
 If the local schema version in the meta-table is identical to the remote schema version in DAP, inserting, updating and deleting records proceeds normally. However, if there is a mismatch, the table structure of the local database has to evolve to match the current structure of the data in DAP. This includes the following schema changes in the back-end:
```

### Comparing `instructure-dap-client-0.3.7/dap/__main__.py` & `instructure-dap-client-0.3.8/dap/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import asyncio
 import errno
 import logging
-import os
 import sys
-import traceback
 
 from .arguments import Arguments
 from .commands.commands import (
     DapCommandRegistrar,
     IncrementalCommandRegistrar,
     ListCommandRegistrar,
     SchemaCommandRegistrar,
@@ -27,15 +25,15 @@
     NamespaceArgumentRegistrar,
     OutputDirectoryArgumentRegistrar,
     TableArgumentRegistrar,
 )
 from .commands.syncdb_command import SyncDBCommandRegistrar
 from .commands.timestampargs import SinceArgumentRegistrar, UntilArgumentRegistrar
 from .dap_error import OperationError
-from .log import LogFormatter
+from .log import LevelFormatter
 
 dapCommand = DapCommandRegistrar(
     arguments=[
         BaseUrlArgumentRegistrar(),
         OAuthCredentialsArgumentRegistrar(),
         LogLevelArgumentRegistrar(),
         HelpArgumentRegistrar(),
@@ -102,45 +100,45 @@
 def main() -> None:
     parser = dapCommand.register()
 
     args = Arguments()
     if parser:
         parser.parse_args(namespace=args)
 
-    logging.basicConfig(
-        level=getattr(logging, args.loglevel.upper(), logging.INFO),
+    logging.basicConfig(level=getattr(logging, args.loglevel.upper(), logging.INFO))
+    logger = logging.getLogger("dap")
+    logger.propagate = False
+    handler = logging.StreamHandler()
+    default_format = "%(asctime)s - %(levelname)s - %(message)s"
+    debug_format = default_format + " (%(filename)s:%(lineno)d)"
+    handler.setFormatter(
+        LevelFormatter({logging.DEBUG: debug_format, logging.INFO: default_format})
     )
-    loglevel = logging.root.getEffectiveLevel()
-    logging.root.handlers[0].setFormatter(LogFormatter(loglevel))
+    logger.addHandler(handler)
 
     asyncio.run(dapCommand.execute(args))
 
 
 def console_entry() -> None:
-    # propagate exceptions to interactive development environment
-    if os.getenv("TERM_PROGRAM") == "vscode":
-        main()
-        return
+    logger = logging.getLogger("dap")
 
     # handle exceptions for production deployments
     try:
         main()
     except OperationError as e:
-        logging.error(
+        logger.error(
             f"An exception occurred while executing the command: {e.message} ({e.uuid})"
         )
-        logging.exception(e)
+        logger.exception(e)
         sys.exit(errno.EIO)
     except NotImplementedError as e:
-        logging.error(e)
+        logger.exception(e)
         sys.exit(errno.ENOSYS)
     except (asyncio.exceptions.CancelledError, KeyboardInterrupt):
-        sys.exit(errno.EINTR)
+        sys.exit(errno.ECANCELED)
     except Exception as e:
-        # Handle any other exception in similar way
-        logging.debug(traceback.format_exc())
-        logging.error(e)
+        logger.exception(e)
         sys.exit(errno.EIO)
 
 
 if __name__ == "__main__":
     console_entry()
```

### Comparing `instructure-dap-client-0.3.7/dap/actions/drop_db.py` & `instructure-dap-client-0.3.8/dap/actions/drop_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/actions/init_db.py` & `instructure-dap-client-0.3.8/dap/actions/init_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/actions/sync_db.py` & `instructure-dap-client-0.3.8/dap/actions/sync_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/api.py` & `instructure-dap-client-0.3.8/dap/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 import aiofiles
 import aiohttp
 import jwt
 from strong_typing.serialization import json_dump_string, json_to_object, object_to_json
 
 from . import __version__
 from .dap_error import (
+    AccountNotOnboardedError,
     AuthenticationError,
     NotFoundError,
     OutOfRangeError,
     ProcessingError,
     ServerError,
+    AccountDisabledError,
     ValidationError,
 )
 from .dap_types import (
     CompleteIncrementalJob,
     CompleteSnapshotJob,
     Credentials,
     DownloadTableDataResult,
@@ -40,14 +42,16 @@
     SnapshotQuery,
     TableList,
     TokenProperties,
     VersionedSchema,
 )
 from .networking import get_content_type
 
+logger = logging.getLogger("dap")
+
 T = TypeVar("T")
 
 
 class DAPClientError(RuntimeError):
     pass
 
 
@@ -65,21 +69,36 @@
 
     _base_url: str
     _credentials: Credentials
     _session: Optional["DAPSession"]
 
     def __init__(
         self,
-        base_url: str,
-        credentials: Credentials,
+        base_url: Optional[str] = None,
+        credentials: Optional[Credentials] = None,
     ) -> None:
+        if base_url is None:
+            base_url = os.getenv("DAP_API_URL")
+            if not base_url:
+                raise DAPClientError("missing base URL")
+
+        if credentials is None:
+            client_id = os.getenv("DAP_CLIENT_ID")
+            client_secret = os.getenv("DAP_CLIENT_SECRET")
+            if not client_id or not client_secret:
+                raise DAPClientError("missing credentials")
+
+            credentials = Credentials.create(
+                client_id=client_id, client_secret=client_secret
+            )
+
         self._base_url = base_url.rstrip("/")
         self._credentials = credentials
 
-        logging.debug(f"Client region: {self._credentials.client_region}")
+        logger.debug(f"Client region: {self._credentials.client_region}")
 
     async def __aenter__(self) -> "DAPSession":
         session = aiohttp.ClientSession(
             headers={"User-Agent": f"DataAccessPlatform/{__version__}"},
             timeout=aiohttp.ClientTimeout(total=30 * 60, connect=30),
         )
         self._session = DAPSession(session, self._base_url, self._credentials)
@@ -171,34 +190,38 @@
     def _map_to_error_type(
         self, status_code: int, response_body: Any
     ) -> Union[
         ValidationError,
         NotFoundError,
         OutOfRangeError,
         AuthenticationError,
+        AccountDisabledError,
+        AccountNotOnboardedError,
         ProcessingError,
         ServerError,
     ]:
         """
         Maps error body and status to Python error object.
         """
 
         if "error" not in response_body:
             return ServerError(response_body)
 
         response_body_error = response_body["error"]
         try:
-            if (
-                status_code == HTTPStatus.UNAUTHORIZED.value
-                or status_code == HTTPStatus.FORBIDDEN.value
-            ):
+            if status_code == HTTPStatus.UNAUTHORIZED.value:
                 return json_to_object(AuthenticationError, response_body_error)
+            elif status_code == HTTPStatus.FORBIDDEN.value:
+                return json_to_object(
+                    Union[AccountDisabledError, AccountNotOnboardedError],  # type: ignore
+                    response_body_error,
+                )
             else:
                 return json_to_object(
-                    Union[
+                    Union[  # type: ignore
                         ValidationError,
                         NotFoundError,
                         OutOfRangeError,
                         ProcessingError,
                     ],
                     response_body_error,
                 )
@@ -215,15 +238,15 @@
         :returns: The object returned on success.
         :raises Exception: The object returned on failure.
         """
 
         await self.authenticate()
 
         request_payload = object_to_json(request_data)
-        logging.debug(f"POST request payload:\n{repr(request_payload)}")
+        logger.debug(f"POST request payload:\n{repr(request_payload)}")
 
         async with self._session.post(
             f"{self._base_url}{path}",
             data=json_dump_string(request_payload),
             headers={"Content-Type": "application/json"},
         ) as response:
             return await self._process(response, response_type)
@@ -257,40 +280,40 @@
 
         content_type = get_content_type(response.headers.get("Content-Type", ""))
         if content_type == "application/json":
             response_payload = await response.json()
         else:
             response_text = await response.text()
             if response_text:
-                logging.error(f"malformed HTTP response:\n{response_text}")
+                logger.error(f"malformed HTTP response:\n{response_text}")
 
             raise DAPClientError("malformed HTTP response")
 
         if not suppress_output:
-            logging.debug(f"GET/POST response payload:\n{repr(response_payload)}")
+            logger.debug(f"GET/POST response payload:\n{repr(response_payload)}")
 
         # HTTP status codes between 400 (inclusive) and 600 (exclusive) indicate an error
         # (includes non-standard 5xx server-side error codes)
         if HTTPStatus.BAD_REQUEST.value <= response.status < 600:
             error_object = self._map_to_error_type(response.status, response_payload)
-            logging.warning(f"Received error in response: {error_object}")
+            logger.warning(f"Received error in response: {error_object}")
             raise error_object
         else:
             response_object = json_to_object(response_type, response_payload)
             return response_object
 
     async def authenticate(self) -> None:
         """
         Authenticates with API key to receive a JWT.
         """
 
         if self._access_token is not None and not self._access_token.is_expiring():
             return
 
-        logging.debug(
+        logger.debug(
             f"Authenticating to DAP in region {self._credentials.client_region}"
         )
 
         # drop expired auth header, re-authentication will set new one
         self._session.headers.pop("X-InstAuth", None)
 
         properties = await self._post_auth_request(self._credentials.basic_credentials)
@@ -300,51 +323,51 @@
     async def query_snapshot(
         self, namespace: str, table: str, query: SnapshotQuery
     ) -> Job:
         """
         Starts a snapshot query.
         """
 
-        logging.debug(f"Query snapshot of table: {table}")
+        logger.debug(f"Query snapshot of table: {table}")
         job = await self._post(f"/dap/query/{namespace}/table/{table}/data", query, Job)  # type: ignore
         return job
 
     async def query_incremental(
         self, namespace: str, table: str, query: IncrementalQuery
     ) -> Job:
         """
         Starts an incremental query.
         """
 
-        logging.debug(f"Query updates for table: {table}")
+        logger.debug(f"Query updates for table: {table}")
         job = await self._post(f"/dap/query/{namespace}/table/{table}/data", query, Job)  # type: ignore
         return job
 
     async def get_tables(self, namespace: str) -> List[str]:
         """
         Retrieves the list of tables available for querying.
 
         :param namespace: A namespace identifier such as `canvas` or `mastery`.
         :returns: A list of tables available for querying in the given namespace.
         """
 
-        logging.debug(f"Get list of tables from namespace: {namespace}")
+        logger.debug(f"Get list of tables from namespace: {namespace}")
         table_list = await self._get(f"/dap/query/{namespace}/table", TableList)
         return table_list.tables
 
     async def get_table_schema(self, namespace: str, table: str) -> VersionedSchema:
         """
         Retrieves the versioned schema of a table.
 
         :param namespace: A namespace identifier such as `canvas` or `mastery`.
         :param table: A table identifier such as `submissions`, `quizzes`, or `users`.
         :returns: The schema of the table as exposed by DAP API.
         """
 
-        logging.debug(f"Get schema of table: {table}")
+        logger.debug(f"Get schema of table: {table}")
         versioned_schema = await self._get(
             f"/dap/query/{namespace}/table/{table}/schema", VersionedSchema
         )
         return versioned_schema
 
     async def download_table_schema(
         self, namespace: str, table: str, output_directory: str
@@ -362,22 +385,22 @@
         json_object = object_to_json(versioned_schema)
 
         os.makedirs(output_directory, exist_ok=True)
         file_name = f"{table}_schema_version_{schema_version}.json"
         file_path = os.path.join(output_directory, file_name)
         with open(file_path, "w") as file:
             json.dump(json_object, file, indent=4)
-        logging.info(f"JSON schema downloaded to folder: {output_directory}")
+        logger.info(f"JSON schema downloaded to folder: {output_directory}")
 
     async def get_job(self, job_id: JobID) -> Job:
         """
         Retrieve job status.
         """
 
-        logging.debug(f"Retrieving job state for job {job_id}")
+        logger.debug(f"Retrieving job state for job {job_id}")
         job = await self._get(f"/dap/job/{job_id}", Job)  # type: ignore
         return job
 
     async def get_job_status(self, job_id: JobID) -> JobStatus:
         """
         Retrieve job status.
         """
@@ -386,25 +409,25 @@
         return job.status
 
     async def get_objects(self, job_id: JobID) -> List[Object]:
         """
         Retrieve object IDs once the query is completed successfully.
         """
 
-        logging.debug(f"Retrieving object IDs for job {job_id}")
+        logger.debug(f"Retrieving object IDs for job {job_id}")
         job = await self._get(f"/dap/job/{job_id}", Job)  # type: ignore
         return job.objects
 
     async def get_resources(self, objects: List[Object]) -> List[Resource]:
         """
         Retrieve URLs to data stored remotely.
         """
 
-        logging.debug("Retrieve resource URLs for objects:")
-        logging.debug([o.id for o in objects])
+        logger.debug("Retrieve resource URLs for objects:")
+        logger.debug([o.id for o in objects])
 
         response = await self._post("/dap/object/url", objects, ResourceResult)
         resource_list = [response.urls[resource_id] for resource_id in response.urls]
         return resource_list
 
     async def download_resources(
         self, resources: List[Resource], output_directory: str
@@ -420,26 +443,26 @@
         local_files: List[str] = []
         os.makedirs(output_directory, exist_ok=True)
         for resource in resources:
             url = str(resource.url)
             url_path = urlparse(url).path
             file_base_name = os.path.basename(url_path)
             file_path = os.path.join(output_directory, file_base_name)
-            logging.debug(f"Downloading: {url} to {file_path}")
+            logger.debug(f"Downloading: {url} to {file_path}")
 
             async with self.stream_resource(resource) as stream:
                 async with aiofiles.open(file_path, "wb") as file:
                     # save gzip data to file without decompressing
                     async for chunk in stream.iter_chunked(64 * 1024):
                         await file.write(chunk)
 
-                logging.debug(f"Download complete of {url} to {file_path}")
+                logger.debug(f"Download complete of {url} to {file_path}")
 
             local_files.append(file_path)
-        logging.info(f"Files from server downloaded to folder: {output_directory}")
+        logger.info(f"Files from server downloaded to folder: {output_directory}")
         return local_files
 
     @asynccontextmanager
     async def stream_resource(
         self, resource: Resource
     ) -> AsyncIterator[aiohttp.StreamReader]:
         """
@@ -462,22 +485,22 @@
 
         :param job: A job that might be still running.
         :returns: A job that has completed with success or terminated with failure.
         """
 
         while not job.status.isTerminal():
             delay = 5
-            logging.info(
+            logger.info(
                 f"Query job still in status: {job.status.value}. Checking again in {delay} seconds..."
             )
             await asyncio.sleep(delay)
 
             job = await self.get_job(job.id)
 
-        logging.debug(f"Query job finished with status: {job.status.value}")
+        logger.debug(f"Query job finished with status: {job.status.value}")
         return job
 
     async def execute_job(
         self,
         namespace: str,
         table: str,
         query: Query,
@@ -489,15 +512,15 @@
         if isinstance(query, SnapshotQuery):
             job = await self.query_snapshot(namespace, table, query)
         elif isinstance(query, IncrementalQuery):
             job = await self.query_incremental(namespace, table, query)
         else:
             raise TypeError(f"type mismatch for parameter `query`: {type(query)}")
 
-        logging.info(f"Query started with job ID: {job.id}")
+        logger.info(f"Query started with job ID: {job.id}")
 
         job = await self.await_job(job)
         return job
 
     async def download_table_data(
         self, namespace: str, table: str, query: Query, output_directory: str
     ) -> DownloadTableDataResult:
@@ -520,20 +543,20 @@
         if job.status is JobStatus.Complete:
             objects = await self.get_objects(job.id)
             resources = await self.get_resources(objects)
             dir = os.path.join(output_directory, f"job_{job.id}")
             downloaded_files = await self.download_resources(resources, dir)
 
             if isinstance(job, CompleteSnapshotJob):
-                logging.info(f"Data has been successfully retrieved:\n{job.json()}")
+                logger.info(f"Data has been successfully retrieved:\n{job.json()}")
                 return DownloadTableDataResult(
                     job.schema_version, job.at, job.id, downloaded_files
                 )
             elif isinstance(job, CompleteIncrementalJob):
-                logging.info(f"Data has been successfully retrieved:\n{job.json()}")
+                logger.info(f"Data has been successfully retrieved:\n{job.json()}")
                 return DownloadTableDataResult(
                     job.schema_version, job.until, job.id, downloaded_files
                 )
             else:
                 raise DAPClientError(f"unexpected job type: {type(job)}")
 
         else:
@@ -554,19 +577,19 @@
 
         job = await self.execute_job(namespace, table, query)
 
         if job.status is JobStatus.Complete:
             objects = await self.get_objects(job.id)
 
             if isinstance(job, CompleteSnapshotJob):
-                logging.info(f"Data has been successfully retrieved:\n{job.json()}")
+                logger.info(f"Data has been successfully retrieved:\n{job.json()}")
                 return GetTableDataResult(job.schema_version, job.at, job.id, objects)
 
             elif isinstance(job, CompleteIncrementalJob):
-                logging.info(f"Data has been successfully retrieved:\n{job.json()}")
+                logger.info(f"Data has been successfully retrieved:\n{job.json()}")
                 return GetTableDataResult(
                     job.schema_version, job.until, job.id, objects
                 )
 
             else:
                 raise DAPClientError(f"unexpected job type: {type(job)}")
```

### Comparing `instructure-dap-client-0.3.7/dap/arguments.py` & `instructure-dap-client-0.3.8/dap/arguments.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/base.py` & `instructure-dap-client-0.3.8/dap/commands/base.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/commands.py` & `instructure-dap-client-0.3.8/dap/commands/commands.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/commonargs.py` & `instructure-dap-client-0.3.8/dap/commands/commonargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/dropdb_command.py` & `instructure-dap-client-0.3.8/dap/commands/dropdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/initdb_command.py` & `instructure-dap-client-0.3.8/dap/commands/initdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/queryargs.py` & `instructure-dap-client-0.3.8/dap/commands/queryargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/syncdb_command.py` & `instructure-dap-client-0.3.8/dap/commands/syncdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/commands/timestampargs.py` & `instructure-dap-client-0.3.8/dap/commands/timestampargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/concurrency.py` & `instructure-dap-client-0.3.8/dap/concurrency.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/dap_error.py` & `instructure-dap-client-0.3.8/dap/dap_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import typing
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any
+from typing import Any, Literal
 
 from strong_typing.schema import json_schema_type
 
 
 @json_schema_type
 @dataclass
 class ServerError(Exception):
@@ -34,14 +35,30 @@
 
 class AuthenticationError(OperationError):
     """
     Raised when the client fails to provide valid authentication credentials.
     """
 
 
+class AccountNotOnboardedError(OperationError):
+    """
+    Raised when the client is not onboarded.
+    """
+
+    type: Literal["AccountNotOnboarded"]
+
+
+class AccountDisabledError(OperationError):
+    """
+    Raised when the client is onboarded but access is forbidden.
+    """
+
+    type: Literal["AccountDisabled"]
+
+
 @dataclass(frozen=True)
 class Location:
     """
     Refers to a location in parsable text input (e.g. JSON, YAML or structured text).
 
     :param line: Line number (1-based).
     :param column: Column number w.r.t. the beginning of the line (1-based).
```

### Comparing `instructure-dap-client-0.3.7/dap/dap_types.py` & `instructure-dap-client-0.3.8/dap/dap_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     Schemas are backwards compatible. They receive strictly monotonically increasing version numbers as schema
     evolution takes place.
 
     :param schema: The JSON Schema object to validate against.
     :param version: The version of the schema.
     """
 
-    schema: JsonType
+    schema: Dict[str, JsonType]
     version: int
 
 
 @json_schema_type
 @dataclass(frozen=True)
 class Object:
     """
```

### Comparing `instructure-dap-client-0.3.7/dap/database/base_processor.py` & `instructure-dap-client-0.3.8/dap/database/base_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 from dataclasses import dataclass
 from types import TracebackType
 from typing import Optional, Type
 
+from ..conversion_common import JsonRecord
 from ..dap_types import JobID, ObjectID
-from ..type_conversion import JsonRecord
 
 
 @dataclass(frozen=True)
 class ContextAwareObject:
     "Provides information about the context in which the records are processed."
 
     id: ObjectID
```

### Comparing `instructure-dap-client-0.3.7/dap/database/connection.py` & `instructure-dap-client-0.3.8/dap/database/connection.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/database/database_errors.py` & `instructure-dap-client-0.3.8/dap/database/database_errors.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/database/database_operations.py` & `instructure-dap-client-0.3.8/dap/database/database_operations.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/database/init_processor.py` & `instructure-dap-client-0.3.8/dap/database/init_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from types import TracebackType
 from typing import Optional, Tuple, Type
 
 from sqlalchemy import Connection, Inspector, Table, inspect
 from sqlalchemy.sql.ddl import CreateSchema
 
+from ..conversion_common import JsonRecord
+from ..conversion_perf import create_copy_converters
 from ..dap_types import VersionedSchema
 from ..model.metadata import create_table_definition
-from ..type_conversion import JsonRecord, create_copy_converters
 from .base_processor import BaseBatch, BaseInitProcessor, ContextAwareObject
 from .connection import DatabaseSession
 from .database_errors import TableAlreadyExistsError
 from .database_operations import DatabaseCopy
 
 
 def _create_tables(db_conn: Connection, table_def: Table) -> None:
```

### Comparing `instructure-dap-client-0.3.7/dap/database/sync_processor.py` & `instructure-dap-client-0.3.8/dap/database/sync_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from types import TracebackType
 from typing import Optional, Type
 
 from sqlalchemy import Connection, Inspector, Table, inspect
 
+from ..conversion_common import ConverterDict, JsonRecord
+from ..conversion_perf import create_delete_converters, create_upsert_converters
 from ..dap_types import VersionedSchema
 from ..model.metadata import create_table_definition
-from ..type_conversion import (
-    ConverterDict,
-    JsonRecord,
-    create_delete_converters,
-    create_upsert_converters,
-)
 from .base_processor import BaseBatch, BaseSyncProcessor, ContextAwareObject
 from .connection import DatabaseSession
 from .database_errors import NonExistingTableError
 from .database_operations import DatabaseDelete, DatabaseUpsert
 
 
 def _check_table(db_conn: Connection, table_def: Table) -> None:
```

### Comparing `instructure-dap-client-0.3.7/dap/downloader.py` & `instructure-dap-client-0.3.8/dap/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import typing
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Awaitable, Callable
 
 from .api import DAPSession, DownloadError
 from .concurrency import wait_n
 from .dap_types import (
@@ -13,17 +14,20 @@
     SnapshotQuery,
     VersionedSchema,
 )
 from .database.base_processor import (
     BaseInitProcessor,
     BaseSyncProcessor,
     ContextAwareObject,
+    JsonRecord,
 )
-from .payload import get_json_lines_from_gzip_stream
 from .database.database_errors import SchemaVersionMismatchError
+from .payload import get_json_lines_from_gzip_stream
+
+logger = logging.getLogger("dap")
 
 CONCURRENCY: int = 4
 
 SnapshotDownloader = Callable[[BaseInitProcessor], Awaitable[None]]
 
 
 @dataclass(frozen=True)
@@ -89,21 +93,21 @@
         obj: ContextAwareObject,
         processor: BaseInitProcessor,
     ) -> None:
         resource_array = await self._session.get_resources([Object(id=obj.id)])
         if len(resource_array) != 1:
             raise DownloadError("unable to get resource URLs for objects")
 
-        logging.info(f"Downloading {obj}")
+        logger.info(f"Downloading {obj}")
 
         resource = resource_array[0]
         async with self._session.stream_resource(resource) as stream:
             async with processor.batch(obj) as batch:
                 async for record in get_json_lines_from_gzip_stream(stream):
-                    await batch.process(record)
+                    await batch.process(typing.cast(JsonRecord, record))
 
 
 IncrementalDownloader = Callable[[BaseSyncProcessor], Awaitable[None]]
 
 
 @dataclass(frozen=True)
 class IncrementalClient:
@@ -168,9 +172,9 @@
         resource_array = await self._session.get_resources([Object(id=obj.id)])
         if len(resource_array) != 1:
             raise DownloadError("unable to get resource URLs for objects")
 
         resource = resource_array[0]
         async with self._session.stream_resource(resource) as stream:
             async with processor.batch(obj) as batch:
-                async for json_content in get_json_lines_from_gzip_stream(stream):
-                    await batch.process(json_content)
+                async for record in get_json_lines_from_gzip_stream(stream):
+                    await batch.process(typing.cast(JsonRecord, record))
```

### Comparing `instructure-dap-client-0.3.7/dap/model/metadata.py` & `instructure-dap-client-0.3.8/dap/model/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Any, List, Optional, Union
+import typing
+from typing import Any, Dict, List, Optional, Union
 
 import sqlalchemy
 from sqlalchemy.sql.type_api import TypeEngine
-from strong_typing.schema import JsonType
+from strong_typing.core import JsonType, Schema
 
 from ..api import DAPClientError
+from ..conversion_nonperf import create_value_converter
 from ..dap_types import VersionedSchema
 
 SqlAlchemyType = Union[
     sqlalchemy.BigInteger,
     sqlalchemy.Integer,
     sqlalchemy.SmallInteger,
     sqlalchemy.Float,
@@ -19,21 +21,23 @@
     sqlalchemy.JSON,
     sqlalchemy.Boolean,
     sqlalchemy.ARRAY,
 ]
 
 
 def match_type(
-    schema: JsonType, namespace: str, table_name: str, prop_name: str
+    schema: Schema, namespace: str, table_name: str, prop_name: str
 ) -> TypeEngine[Any]:
     detected_type: Optional[SqlAlchemyType] = None
 
     if "oneOf" in schema:
-        for oneOfTypes in schema["oneOf"]:
-            if oneOfTypes["type"] != "string":
+        oneOfSchema = typing.cast(List[JsonType], schema["oneOf"])
+        for item in oneOfSchema:
+            oneOfElement = typing.cast(Dict[str, JsonType], item)
+            if oneOfElement["type"] != "string":
                 raise OneOfTypeSchemaError(table_name)
 
         return sqlalchemy.String()
 
     if "type" not in schema:
         raise NoTypeSpecifiedError(table_name, prop_name)
 
@@ -61,47 +65,55 @@
                 *schema["enum"], name=enum_name, create_type=True, schema=namespace
             )
 
         elif "format" in schema and schema["format"] == "date-time":
             detected_type = sqlalchemy.TIMESTAMP(timezone=False)
 
         elif "maxLength" in schema:
-            detected_type = sqlalchemy.String(length=schema["maxLength"])
+            max_length = typing.cast(int, schema["maxLength"])
+            detected_type = sqlalchemy.String(length=max_length)
         else:
             detected_type = sqlalchemy.String()
 
     elif type_name == "object":
         detected_type = sqlalchemy.JSON()
 
     elif type_name == "boolean":
         detected_type = sqlalchemy.Boolean()
 
     elif type_name == "array":
         if "items" not in schema:
             raise NoArrayItemTypeSpecifiedError(table_name, prop_name)
 
-        items_schema = schema["items"]
+        items_schema = typing.cast(Schema, schema["items"])
         detected_type = sqlalchemy.ARRAY(
             match_type(items_schema, namespace, table_name, prop_name)
         )
 
     if detected_type is None:
         raise UnrecognizedTypeError(table_name, prop_name)
 
     return detected_type
 
 
-def get_comment(schema: JsonType) -> str:
-    comm = schema["description"] if "description" in schema else ""
+def get_comment(schema: Schema) -> str:
+    comm = schema.get("description", "")
     if type(comm) != str:
         raise NoStringDescriptionError
 
     return comm
 
 
+def get_default(schema: Schema, namespace: str, table_name: str, prop_name: str) -> Any:
+    raw_default_value = schema.get("default")
+    value_type = match_type(schema, namespace, table_name, prop_name)
+    converter = create_value_converter(value_type)
+    return converter(raw_default_value)
+
+
 class DAPSchemaParsingError(DAPClientError):
     pass
 
 
 class NoStringDescriptionError(DAPSchemaParsingError):
     def __init__(self) -> None:
         super().__init__("`description` of property in schema must be a string")
@@ -147,51 +159,52 @@
     :param namespace: Namespace that table belongs to.
     :param table_name: Identifier of the table.
     :param versioned_schema: Schema that the table conforms to.
     :returns: Table definition.
     :raises CompositeKeyError: The table has a composite primary key.
     """
 
-    schema = versioned_schema.schema["properties"]
-    key_schema = schema["key"]
-    key_schema_props = key_schema["properties"]
+    schema = typing.cast(Dict[str, JsonType], versioned_schema.schema["properties"])
+    key_schema = typing.cast(Dict[str, JsonType], schema["key"])
+    key_schema_props = typing.cast(Dict[str, JsonType], key_schema["properties"])
 
     if len(key_schema_props) != 1:
         raise CompositeKeyError(table_name)
 
-    value_schema = schema["value"]
-    value_schema_props = value_schema["properties"]
+    value_schema = typing.cast(Dict[str, JsonType], schema["value"])
+    value_schema_props = typing.cast(Dict[str, JsonType], value_schema["properties"])
     columns: List[sqlalchemy.Column] = []
 
-    required_keys = key_schema.get("required", [])
-    for id_prop_name in key_schema_props:
-        id_schema = key_schema_props[id_prop_name]
+    required_keys = typing.cast(List[str], key_schema.get("required", []))
+    for id_prop_name in key_schema_props.keys():
+        id_schema = typing.cast(Schema, key_schema_props[id_prop_name])
 
         column_type = match_type(id_schema, namespace, table_name, id_prop_name)
 
         columns.append(
             sqlalchemy.Column(
                 id_prop_name,
                 column_type,
                 primary_key=True,
                 nullable=(id_prop_name not in required_keys),
                 comment=get_comment(id_schema),
             )
         )
 
-    required_values = value_schema.get("required", [])
-    for prop_name in value_schema_props:
-        prop_schema = value_schema_props[prop_name]
+    required_values = typing.cast(List[str], value_schema.get("required", []))
+    for prop_name in value_schema_props.keys():
+        prop_schema = typing.cast(Schema, value_schema_props[prop_name])
         column_type = match_type(prop_schema, namespace, table_name, prop_name)
 
         columns.append(
             sqlalchemy.Column(
                 prop_name,
                 column_type,
                 nullable=(prop_name not in required_values),
                 comment=get_comment(prop_schema),
+                default=get_default(prop_schema, namespace, table_name, prop_name),
             )
         )
 
     # create table model
     metadata = sqlalchemy.MetaData(schema=namespace)
     return sqlalchemy.Table(table_name, metadata, *columns)
```

### Comparing `instructure-dap-client-0.3.7/dap/networking.py` & `instructure-dap-client-0.3.8/dap/networking.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from email.message import Message
-from typing import Dict, Optional
+from typing import Dict, List, Tuple
 
 
 @dataclass
 class ParseContentResult:
     """
     Results of parsing an HTTP `Content-Type` header.
 
@@ -17,14 +17,16 @@
 
 
 def parse_content_type(content_type_header: str) -> ParseContentResult:
     "Parses an HTTP `Content-Type` header."
 
     email = Message()
     email["Content-Type"] = content_type_header
-    params = email.get_params()
+    params: List[Tuple[str, str]] = email.get_params(
+        failobj=[("application/octet-stream", "")]
+    )
     return ParseContentResult(params[0][0], dict(params[1:]))
 
 
 def get_content_type(content_type_header: str) -> str:
     result = parse_content_type(content_type_header)
     return result.content_type
```

### Comparing `instructure-dap-client-0.3.7/dap/payload.py` & `instructure-dap-client-0.3.8/dap/payload.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/replicator/sql.py` & `instructure-dap-client-0.3.8/dap/replicator/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,12 +70,12 @@
                 namespace=namespace,
                 table_name=table_name,
                 schema=client.table_schema,
             )
 
         await processor.prepare()
 
-        await meta_table_manager.synchronize(client.table_data)
+        await meta_table_manager.synchronize(client.table_schema, client.table_data)
         await client.download(processor)
 
         async with self._connection.context() as conn:
             await conn.commit()
```

### Comparing `instructure-dap-client-0.3.7/dap/timer.py` & `instructure-dap-client-0.3.8/dap/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import time
 from types import TracebackType
 from typing import Optional, Type
 
+logger = logging.getLogger("dap")
+
 
 class TimerError(Exception):
     """An exception used to report errors in use of the `Timer` class."""
 
 
 class Timer:
     _name: str
@@ -18,26 +20,26 @@
 
     async def start(self) -> None:
         """Starts a new timer."""
 
         if self._start_time is not None:
             raise TimerError(f"timer is running; use `stop()` to stop it")
 
-        logging.debug(f"start {self._name}")
+        logger.debug(f"start {self._name}")
         self._start_time = time.perf_counter()
 
     async def stop(self) -> None:
         """Stops the timer, and reports the elapsed time."""
 
         if self._start_time is None:
             raise TimerError(f"timer is not running; use `start()` to start it")
 
         elapsed_time = time.perf_counter() - self._start_time
         self._start_time = None
-        logging.debug(f"{self._name} took {elapsed_time:0.3f}s")
+        logger.debug(f"{self._name} took {elapsed_time:0.3f}s")
 
     async def __aenter__(self) -> "Timer":
         await self.start()
         return self
 
     async def __aexit__(
         self,
```

### Comparing `instructure-dap-client-0.3.7/dap/timestamp.py` & `instructure-dap-client-0.3.8/dap/timestamp.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.7/dap/type_conversion.py` & `instructure-dap-client-0.3.8/dap/conversion_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 import orjson
 from sqlalchemy import ARRAY, JSON, TIMESTAMP, BigInteger, Boolean, Column, Double
 from sqlalchemy import Enum as SqlEnum
-from sqlalchemy import Float, Integer, SmallInteger, String, Table
+from sqlalchemy import Float, Integer, SmallInteger, String
+from sqlalchemy.sql.type_api import TypeEngine
 from strong_typing.core import JsonType
 
 from .timestamp import valid_naive_datetime
 
 T = TypeVar("T")
 
-JsonRecord = Dict[str, JsonType]
+JsonRecord = Dict[str, Dict[str, JsonType]]
 JsonTypeCast = Callable[[JsonType], Any]
 RecordExtractor = Callable[[JsonRecord], Any]
 
 
 def _get_primary_extractor(
     column_name: str, type_cast: Optional[JsonTypeCast]
 ) -> RecordExtractor:
@@ -72,15 +73,15 @@
 
 def _json_dump(value: Any) -> str:
     return orjson.dumps(value, option=orjson.OPT_NAIVE_UTC | orjson.OPT_UTC_Z).decode(
         "utf-8"
     )
 
 
-def _get_column_converter(col: Column) -> RecordExtractor:
+def get_column_converter(col: Column) -> RecordExtractor:
     """
     Returns a lambda function that extracts a column value from the deserialized JSON representation of a record.
 
     The input to the returned lambda function is a deserialized JSON representation obtained by `orjson.loads`, which
     deserializes (recursively) to `dict`, `list`, `int`, `float`, `str`, `bool`, and `None` objects. For example,
 
     ```json
@@ -92,15 +93,28 @@
     such as `int` or `str` don't require any mutation. However, `datetime` needs to be converted into a naive
     (timezone-unaware) representation for `asyncpg` to pass it on as a database `timestamp without time zone`.
 
     :returns: A lambda function that extracts the value from a JSON record in the right format and as the right type.
     """
 
     column_type = type(col.type)
+    type_cast: Optional[JsonTypeCast] = get_type_cast(column_type)
 
+    # make sure to return a single lambda that takes a record and returns the value directly
+    # perform as much pre-processing outside the lambda as possible, avoid expensive computations within the lambda
+    column_name = col.name
+    if col.primary_key:
+        return _get_primary_extractor(column_name, type_cast)
+    elif col.nullable:
+        return _get_optional_extractor(column_name, type_cast)
+    else:
+        return _get_required_extractor(column_name, type_cast)
+
+
+def get_type_cast(column_type: Type[TypeEngine]) -> Optional[JsonTypeCast]:
     type_cast: Optional[JsonTypeCast]
     if (
         column_type is Integer
         or column_type is SmallInteger
         or column_type is BigInteger
     ):
         # original JSON type: `integer` (a specialization of `number`)
@@ -108,15 +122,15 @@
         # database type: an integer type (storage size set based on schema)
         type_cast = None
     elif column_type is Float or column_type is Double:
         # original JSON type: `number`
         # deserialized Python type: `int` or `float` (depending on presence of fractional digits)
         # database type: a floating-point type (storage size set based on schema)
         # use conversion to ensure the proper type when passing to database
-        type_cast = float
+        type_cast = float  # type: ignore
     elif column_type is String:
         # original JSON type: `string`
         # deserialized Python type: `str`
         # database type: `varchar` or `text`
         type_cast = None
     elif column_type is SqlEnum:
         # original JSON type: `string`
@@ -131,46 +145,25 @@
         # converted back to `str` to pass to database as `jsonb`
         type_cast = _json_dump
     elif column_type is TIMESTAMP:
         # original JSON type: `str` (format: ISO-8601 string)
         # deserialized Python type: `str`
         # database type: `timestamp without time zone`
         # converted to naive `datetime` to pass to database
-        type_cast = valid_naive_datetime
+        type_cast = valid_naive_datetime  # type: ignore
     elif column_type is Boolean:
         # original JSON type: `boolean`
         # deserialized Python type: `bool`
         type_cast = None
     elif column_type is ARRAY:
         # original JSON type: `array` (nested)
         # deserialized Python type: `list` (nested)
         # convert elements recursively
         type_cast = None
     else:
         raise TypeError(f"cannot convert to {column_type}")
 
-    # make sure to return a single lambda that takes a record and returns the value directly
-    # perform as much pre-processing outside the lambda as possible, avoid expensive computations within the lambda
-    column_name = col.name
-    if col.primary_key:
-        return _get_primary_extractor(column_name, type_cast)
-    elif col.nullable:
-        return _get_optional_extractor(column_name, type_cast)
-    else:
-        return _get_required_extractor(column_name, type_cast)
-
-
-ConverterDict = Dict[str, Callable[[JsonRecord], Any]]
-
-
-def create_upsert_converters(table_def: Table) -> ConverterDict:
-    # create a tuple of converter objects for each column for UPSERT records
-    return {col.name: _get_column_converter(col) for col in table_def.columns}
-
-
-def create_delete_converters(table_def: Table) -> ConverterDict:
-    # create a tuple of converter objects for each column for DELETE records
-    return {col.name: _get_column_converter(col) for col in table_def.primary_key}
+    return type_cast
 
 
-def create_copy_converters(table_def: Table) -> Tuple:
-    return tuple(_get_column_converter(col) for col in table_def.columns)
+Converter = Callable[[JsonRecord], Any]
+ConverterDict = Dict[str, Converter]
```

### Comparing `instructure-dap-client-0.3.7/instructure_dap_client.egg-info/PKG-INFO` & `instructure-dap-client-0.3.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: instructure-dap-client
-Version: 0.3.7
-Summary: Data Access Platform client library
-Author: Levente Hunyadi
-Author-email: levente.hunyadi@instructure.com
-Maintainer: Edina Tipter
-Maintainer-email: edina.tipter@instructure.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Data Access Platform Client Library
 
 Data Access Platform (DAP) acts as a single source of data for analytics at Instructure. It provides efficient access to data collected across various educational products in bulk with high fidelity and low latency, adhering to a canonical data model.
 
 The outgoing interface for DAP is the [Query API](https://data-access-platform-api.s3.amazonaws.com/index.html), which is an HTTP REST service. Users initiate asynchronous queries to retrieve data associated with their account. The client library is a Python wrapper around the DAP API, allowing users to fetch an initial snapshot and incremental changes, or initialize a database and keep it synchronized with data in DAP.
 
 Each DAP user acts as a data administrator for the organization they represent. They have full read access to the top-level account and all descendant sub-accounts. For example, in Canvas, the top of the organization hierarchy is uniquely identified by a root account ID, and each data record is associated with a root account ID. A DAP user with Canvas access can query data that are assigned the user's root account ID.
@@ -86,14 +64,16 @@
 dap initdb --help
 dap syncdb --help
 dap dropdb --help
 ```
 
 ## Common use cases
 
+If you are a first-time user of DAP client library, it's best to start with two high-level commands of the CLI (command-line interface): `initdb` and `syncdb`. `initdb` fetches the data stored in DAP and replicates them in a (local) database table. It takes care of authenticating with DAP, fetching data schema, creating a database table, starting a snapshot query, monitoring job progress, downloading data, and inserting records into the table. Subsequently, `syncdb` helps keep the database table up-to-date with the data in DAP. As in the case of `initdb`, `syncdb` manages all the details of verifying the data schema, altering database table structure (if necessary), getting the right data and inserting, updating or deleting the corresponding database table records.
+
 ### Obtain a full snapshot of a table in a database or data warehouse
 
 The command-line utility is capable of automatically copying a full table snapshot to a (local) database with the `initdb` command. Along with the parameters `--table` and `--namespace`, you have to specify your target database with a connection string using the `--connection-string` parameter.
 
 Typically, the connection string looks as follows:
 
 ```sh
@@ -189,22 +169,23 @@
 ## Code examples
 
 While basic functionality of the DAP client library is exposed over its command-line interface (CLI), more advanced functionality requires interacting with classes and functions defined in the module `dap.api`. This enables seamless integration into workflow management platforms like Apache Airflow.
 
 First, we need to instantiate the `DAPClient` class:
 
 ```python
+import os
 from dap.api import DAPClient
 from dap.dap_types import Credentials
 
 base_url: str = os.environ["DAP_API_URL"]
 client_id: str = os.environ["DAP_CLIENT_ID"]
 client_secret: str = os.environ["DAP_CLIENT_SECRET"]
 
-credentials = Credentials.create(client_id, client_secret)
+credentials = Credentials.create(client_id=client_id, client_secret=client_secret)
 async with DAPClient(base_url, credentials) as session:
     ...
 ```
 
 However, `DAPClient` can automatically extract the value of these parameters from the above environment variables, allowing us to write:
 
 ```python
@@ -217,39 +198,43 @@
 Let's explore a few common use cases with `DAPClient`.
 
 ### Obtaining the latest schema
 
 Before we obtain data, we need to get the latest schema of a table. The following example retrieves the JSON schema of the table `accounts` in the namespace `canvas` as a JSON schema object. A JSON object is a recursive Python data structure whose outermost layer is a Python `dict` whose keys are strings (type `str`) and values are JSON objects. We can use the Python package [jsonschema](https://python-jsonschema.readthedocs.io/en/stable/) to validate data against this JSON schema.
 
 ```python
+from dap.api import DAPClient
+
 async with DAPClient() as session:
     schema = await session.get_table_schema("canvas", "accounts")
 ```
 
 We can also save the schema to a file. 
 
 ```python
-output_directory: str = os.getcwd()
+import os
+from dap.api import DAPClient
 
+output_directory: str = os.getcwd()
 async with DAPClient() as session:
     tables = await session.get_tables("canvas")
     for table in tables:
         await session.download_table_schema("canvas", table, output_directory)
 ```
 
 ### Fetching table data with a snapshot query
 
 In order to get an initial copy of the full table contents, we need to perform a snapshot query. The parameter `format` determines the output data format, including CSV, TSV, JSONL and Parquet. We recommend JSONL or Parquet. For JSONL, each line in the output can be parsed into a JSON object, conforming to the JSON schema returned above.
 
 ```python
+import os
 from dap.api import DAPClient
 from dap.dap_types import Format, SnapshotQuery
 
 output_directory = os.getcwd()
-
 async with DAPClient() as session:
     query = SnapshotQuery(format=Format.JSONL, filter=None)
     await session.download_table_data("canvas", "accounts", query, output_directory)
 ```
 
 ### Getting latest changes with an incremental query
 
@@ -297,30 +282,33 @@
 
 1. initialize a database, and
 2. synchronize a database with the data in DAP.
 
 In order to replicate data in DAP locally, we must first initialize a database:
 
 ```python
-connection_string: str = "postgresql://scott:password@localhost/testdb"
+from dap.api import DAPClient
+from dap.database.connection import DatabaseConnection
+from dap.replicator.sql import SQLReplicator
 
+connection_string: str = "postgresql://scott:password@localhost/testdb"
 async with DatabaseConnection(connection_string).open() as db_connection:
-    async with DAPClient(base_url, credentials) as session:
+    async with DAPClient() as session:
         await SQLReplicator(session, db_connection).initialize(namespace, table_name)
 ```
 
 Initialization creates a database schema for the DAP namespace, and  a corresponding database table for each DAP table. In addition, it creates a *meta-table*, which is a special database table that holds synchronization information, e.g. the last time the data was synchronized with DAP, and the schema version that the locally stored data conforms to. Finally, it issues a snapshot query to DAP API, and populates the database table with output returned by the snapshot query.
 
 ### Synchronizing data in a local database
 
 Once the table has been initialized, it can be kept up to date using the synchronize operation:
 
 ```python
 async with DatabaseConnection(connection_string).open() as db_connection:
-    async with DAPClient(base_url, credentials) as session:
+    async with DAPClient() as session:
         await SQLReplicator(session, db_connection).synchronize(namespace, table_name)
 ```
 
 This inspects the information in the meta-table, and issues an incremental query to DAP API with a `since` timestamp corresponding to the last synchronization time. Based on the results of the incremental query, it inserts new records, updates existing records, and deletes records that have been added to, updated in, or removed from the DAP service.
 
 If the local schema version in the meta-table is identical to the remote schema version in DAP, inserting, updating and deleting records proceeds normally. However, if there is a mismatch, the table structure of the local database has to evolve to match the current structure of the data in DAP. This includes the following schema changes in the back-end:
```

### Comparing `instructure-dap-client-0.3.7/instructure_dap_client.egg-info/SOURCES.txt` & `instructure-dap-client-0.3.8/instructure_dap_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 setup.cfg
 setup.py
 dap/__init__.py
 dap/__main__.py
 dap/api.py
 dap/arguments.py
 dap/concurrency.py
+dap/conversion_common.py
+dap/conversion_nonperf.py
+dap/conversion_perf.py
 dap/dap_error.py
 dap/dap_types.py
 dap/downloader.py
 dap/log.py
 dap/networking.py
 dap/payload.py
+dap/py.typed
 dap/timer.py
 dap/timestamp.py
-dap/type_conversion.py
 dap/actions/__init__.py
 dap/actions/drop_db.py
 dap/actions/init_db.py
 dap/actions/sync_db.py
 dap/commands/__init__.py
 dap/commands/abstract_db_command.py
 dap/commands/base.py
@@ -36,14 +39,15 @@
 dap/database/base_processor.py
 dap/database/connection.py
 dap/database/database_errors.py
 dap/database/database_operations.py
 dap/database/init_processor.py
 dap/database/sync_processor.py
 dap/model/__init__.py
+dap/model/ddl.py
 dap/model/meta_table.py
 dap/model/metadata.py
 dap/replicator/__init__.py
 dap/replicator/sql.py
 instructure_dap_client.egg-info/PKG-INFO
 instructure_dap_client.egg-info/SOURCES.txt
 instructure_dap_client.egg-info/dependency_links.txt
```

### Comparing `instructure-dap-client-0.3.7/setup.cfg` & `instructure-dap-client-0.3.8/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -16,34 +16,40 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Typing :: Typed
 
 [options]
 zip_safe = True
 include_package_data = True
 packages = find:
+python_requires = >=3.8
 install_requires = 
-	aiohttp >= 3.8.3
+	aiohttp >= 3.8.4
 	aiofiles >= 23.1.0
 	types-aiofiles >= 23.1.0
-	json_strong_typing >= 0.2.6
-	orjson >= 3.8.9
+	json_strong_typing >= 0.2.7
+	orjson >= 3.8.10
 	PyJWT >= 2.6.0
 	asyncpg >= 0.27.0
-	SQLAlchemy[asyncio] >= 2.0.1
+	SQLAlchemy[asyncio] >= 2.0.10
 
 [options.entry_points]
 console_scripts = 
 	dap = dap.__main__:console_entry
 
 [options.packages.find]
 exclude = 
 	dap.tests*
 
+[options.package_data]
+dap = 
+	py.typed
+
 [egg_info]
 tag_build = 
 tag_date = 0
```


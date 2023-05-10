# Comparing `tmp/dbt-oracle-1.4.2rc1.tar.gz` & `tmp/dbt-oracle-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-oracle-1.4.2rc1.tar", last modified: Fri Mar 24 17:05:04 2023, max compression
+gzip compressed data, was "dbt-oracle-1.5.0rc1.tar", last modified: Wed May 10 21:49:02 2023, max compression
```

## Comparing `dbt-oracle-1.4.2rc1.tar` & `dbt-oracle-1.5.0rc1.tar`

### file list

```diff
@@ -1,111 +1,119 @@
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.918228 dbt-oracle-1.4.2rc1/
--rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.4.2rc1/HISTORY.md
--rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.4.2rc1/LICENSE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.4.2rc1/MANIFEST.in
--rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.4.2rc1/NOTICE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-03-24 17:05:04.918424 dbt-oracle-1.4.2rc1/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.4.2rc1/README.md
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.713816 dbt-oracle-1.4.2rc1/bin/
--rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.4.2rc1/bin/create-pem-from-p12
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.717931 dbt-oracle-1.4.2rc1/dbt/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.4.2rc1/dbt/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.720424 dbt-oracle-1.4.2rc1/dbt/adapters/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.4.2rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.730040 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-03-24 16:45:44.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/__version__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/column.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/connection_helper.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     9587 2023-02-24 21:25:42.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/connections.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    11582 2023-02-10 17:55:45.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/impl.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/keyword_catalog.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.4.2rc1/dbt/adapters/oracle/relation.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.732276 dbt-oracle-1.4.2rc1/dbt/include/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.4.2rc1/dbt/include/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.736089 dbt-oracle-1.4.2rc1/dbt/include/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/dbt_project.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.743592 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)    13099 2023-03-24 16:45:44.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/adapters.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/apply_grants.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/catalog.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/columns.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.700920 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.745976 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/incremental/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4087 2023-02-10 17:55:45.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.746913 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.751517 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/
--rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.752467 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/table/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4403 2023-01-21 00:48:03.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/table/table.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.753407 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.754619 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-01-21 00:48:03.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/view/view.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/schema_tests.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.786061 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/data_types.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/dateadd.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/datediff.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/datetrunc.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/except.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/hash.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/last_day.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/position.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/right.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/timestamps.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.4.2rc1/dbt/include/oracle/profile_template.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.803132 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-03-24 17:05:04.000000 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     3808 2023-03-24 17:05:04.000000 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-03-24 17:05:04.000000 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/not-zip-safe
--rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-03-24 17:05:04.000000 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/requires.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-03-24 17:05:04.000000 dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/top_level.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.4.2rc1/pyproject.toml
--rw-r--r--   0 abhisoms   (501) staff       (20)     1449 2023-03-24 17:05:04.920113 dbt-oracle-1.4.2rc1/setup.cfg
--rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-03-24 16:54:42.000000 dbt-oracle-1.4.2rc1/setup.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.866992 dbt-oracle-1.4.2rc1/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/tests/README.md
--rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.4.2rc1/tests/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.4.2rc1/tests/conftest.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.701876 dbt-oracle-1.4.2rc1/tests/functional/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.880805 dbt-oracle-1.4.2rc1/tests/functional/adapter/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.890923 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.897645 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.901482 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/sync_schema/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.909531 dbt-oracle-1.4.2rc1/tests/functional/adapter/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/macros/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/macros/test_alter_column_type.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.914750 dbt-oracle-1.4.2rc1/tests/functional/adapter/snapshots/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/snapshots/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_basic.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_config.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_data_types.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_docs_genreferences.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_generictests_where.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_grants.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/test_quoted_relations.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-03-24 17:05:04.917725 dbt-oracle-1.4.2rc1/tests/functional/adapter/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/utils/test_common_utils.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.4.2rc1/tests/functional/adapter/utils/test_dateutils.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.404169 dbt-oracle-1.5.0rc1/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.0rc1/HISTORY.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.0rc1/LICENSE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.0rc1/NOTICE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-05-10 21:49:02.404362 dbt-oracle-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0rc1/README.md
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.150342 dbt-oracle-1.5.0rc1/bin/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.0rc1/bin/create-pem-from-p12
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.152805 dbt-oracle-1.5.0rc1/dbt/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.154669 dbt-oracle-1.5.0rc1/dbt/adapters/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.172775 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__version__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/column.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connection_helper.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    10683 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connections.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    12691 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/impl.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/keyword_catalog.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/relation.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.174615 dbt-oracle-1.5.0rc1/dbt/include/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.0rc1/dbt/include/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.180484 dbt-oracle-1.5.0rc1/dbt/include/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/dbt_project.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.198140 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)    14448 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/adapters.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/apply_grants.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/catalog.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/columns.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.135121 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.210903 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4087 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.214059 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.226700 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.229583 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4403 2023-01-21 00:48:03.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/table.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.232665 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.238576 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/view/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-01-21 00:48:03.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/view/view.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/schema_tests.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.310552 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/data_types.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/dateadd.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datediff.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datetrunc.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/except.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/hash.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/last_day.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/position.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/right.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/timestamps.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/profile_template.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.341211 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4110 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/requires.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/top_level.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.0rc1/pyproject.toml
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1446 2023-05-10 21:49:02.406084 dbt-oracle-1.5.0rc1/setup.cfg
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-05-10 21:24:58.000000 dbt-oracle-1.5.0rc1/setup.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.349241 dbt-oracle-1.5.0rc1/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/README.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.0rc1/tests/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.0rc1/tests/conftest.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.136285 dbt-oracle-1.5.0rc1/tests/functional/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.371791 dbt-oracle-1.5.0rc1/tests/functional/adapter/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.376784 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/fixtures.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.384419 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.389141 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.390833 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.392581 dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/test_alter_column_type.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.398334 dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/test_simple_seed.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.400175 dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_basic.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_caching.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_config.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_data_types.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_genreferences.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_generictests_where.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_grants.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_quoted_relations.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.403370 dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_common_utils.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_dateutils.py
```

### Comparing `dbt-oracle-1.4.2rc1/LICENSE.txt` & `dbt-oracle-1.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/PKG-INFO` & `dbt-oracle-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.4.2rc1
+Version: 1.5.0rc1
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.4.2rc1/README.md` & `dbt-oracle-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/bin/create-pem-from-p12` & `dbt-oracle-1.5.0rc1/bin/create-pem-from-p12`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/__version__.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 """
-version = "1.4.5"
+version = "1.5.0"
```

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/column.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/column.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/connection_helper.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connection_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/connections.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022, Oracle and/or its affiliates.
+Copyright (c) 2023, Oracle and/or its affiliates.
 Copyright (c) 2020, Vitor Avancini
 
   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at
 
      https://www.apache.org/licenses/LICENSE-2.0
@@ -29,14 +29,43 @@
 
 from dbt.version import __version__ as dbt_version
 from dbt.adapters.oracle.connection_helper import oracledb, SQLNET_ORA_CONFIG
 
 logger = AdapterLogger("oracle")
 
 
+DATATYPES = {
+    "DB_TYPE_BFILE": "BFILE",
+    "DB_TYPE_BINARY_DOUBLE": "BINARY_DOUBLE",
+    "DB_TYPE_BINARY_FLOAT": "BINARY_FLOAT",
+    "DB_TYPE_BINARY_INTEGER": "BINARY_INTEGER",
+    "DB_TYPE_BLOB": "BLOB",
+    "DB_TYPE_BOOLEAN": "BOOLEAN",
+    "DB_TYPE_CHAR": "CHAR",
+    "DB_TYPE_CLOB": "CLOB",
+    "DB_TYPE_DATE": "DATE",
+    "DB_TYPE_INTERVAL_DS": "INTERVAL DAY TO SECOND",
+    "DB_TYPE_INTERVAL_YM": "INTERVAL YEAR TO MONTH",
+    "DB_TYPE_JSON": "JSON",
+    "DB_TYPE_LONG": "LONG",
+    "DB_TYPE_LONG_NVARCHAR": "LONG NVARCHAR",
+    "DB_TYPE_LONG_RAW": "LONG RAW",
+    "DB_TYPE_NCHAR": "NCHAR",
+    "DB_TYPE_NCLOB": "NCLOB",
+    "DB_TYPE_NUMBER": "NUMBER",
+    "DB_TYPE_NVARCHAR": "NVARCHAR2",
+    "DB_TYPE_OBJECT": "OBJECT",
+    "DB_TYPE_RAW": "RAW",
+    "DB_TYPE_ROWID": "ROWID",
+    "DB_TYPE_TIMESTAMP": "TIMESTAMP",
+    "DB_TYPE_TIMESTAMP_LTZ": "TIMESTAMP WITH LOCAL TZ",
+    "DB_TYPE_TIMESTAMP_TZ": "TIMESTAMP WITH TZ",
+    "DB_TYPE_VARCHAR": "VARCHAR2"
+}
+
 class OracleConnectionMethod(enum.Enum):
     HOST = 1
     TNS = 2
     CONNECTION_STRING = 3
 
 
 @dataclass
@@ -84,15 +113,15 @@
 
     @property
     def type(self):
         return 'oracle'
 
     @property
     def unique_field(self):
-        return self.database
+        return self.database or self.user
 
     def _connection_keys(self) -> Tuple[str]:
         """
         List of keys to display in the `dbt debug` output. Omit password.
         """
         return (
             'user', 'database', 'schema',
@@ -280,7 +309,11 @@
             logger.debug(f"SQL status: {self.get_status(cursor)} in {(time.time() - pre)} seconds")
             return connection, cursor
 
     def add_begin_query(self):
         connection = self.get_thread_connection()
         cursor = connection.handle.cursor
         return connection, cursor
+
+    @classmethod
+    def data_type_code_to_name(cls, type_code) -> str:
+        return DATATYPES[type_code.name]
```

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/impl.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022, Oracle and/or its affiliates.
+Copyright (c) 2023, Oracle and/or its affiliates.
 Copyright (c) 2020, Vitor Avancini
 
   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at
 
      https://www.apache.org/licenses/LICENSE-2.0
@@ -14,29 +14,33 @@
   See the License for the specific language governing permissions and
   limitations under the License.
 """
 from typing import (
     Optional, List, Set
 )
 from itertools import chain
+from typing import (
+    Any,
+    Callable,
+    Dict)
 
 import agate
 
 import dbt.exceptions
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
-from dbt.adapters.base.impl import GET_CATALOG_MACRO_NAME
+from dbt.adapters.base.impl import GET_CATALOG_MACRO_NAME, ConstraintSupport
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.base.meta import available
 from dbt.adapters.oracle import OracleAdapterConnectionManager
 from dbt.adapters.oracle.column import OracleColumn
 from dbt.adapters.oracle.relation import OracleRelation
 from dbt.contracts.graph.manifest import Manifest
+from dbt.contracts.graph.nodes import ConstraintType
 from dbt.events import AdapterLogger
 
-from dbt.exceptions import raise_compiler_error
 from dbt.utils import filter_null_values
 
 from dbt.adapters.oracle.keyword_catalog import KEYWORDS
 
 logger = AdapterLogger("oracle")
 
 # Added 6 random hex letters (56c36b) to table_a and table_b to avoid ORA-32031.
@@ -75,14 +79,22 @@
 
 
 class OracleAdapter(SQLAdapter):
     ConnectionManager = OracleAdapterConnectionManager
     Relation = OracleRelation
     Column = OracleColumn
 
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.ENFORCED,
+        ConstraintType.not_null: ConstraintSupport.ENFORCED,
+        ConstraintType.unique: ConstraintSupport.ENFORCED,
+        ConstraintType.primary_key: ConstraintSupport.ENFORCED,
+        ConstraintType.foreign_key: ConstraintSupport.ENFORCED,
+    }
+
     def debug_query(self) -> None:
         self.execute("select 1 as id from dual")
 
     @classmethod
     def date_function(cls):
         return 'CURRENT_DATE'
 
@@ -313,7 +325,23 @@
         if quote_columns:
             return self.quote(column)
         else:
             return column
 
     def valid_incremental_strategies(self):
         return ["append", "merge"]
+
+    @available
+    @classmethod
+    def render_raw_columns_constraints(cls, raw_columns: Dict[str, Dict[str, Any]]) -> List:
+        rendered_column_constraints = []
+
+        for v in raw_columns.values():
+            rendered_column_constraint = [f"{v['name']}"]
+            for con in v.get("constraints", None):
+                constraint = cls._parse_column_constraint(con)
+                c = cls.process_parsed_constraint(constraint, cls.render_column_constraint)
+                if c is not None:
+                    rendered_column_constraint.append(c)
+            rendered_column_constraints.append(" ".join(rendered_column_constraint))
+
+        return rendered_column_constraints
```

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/keyword_catalog.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/keyword_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/adapters/oracle/relation.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/adapters.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/adapters.sql`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,47 @@
         ) dbt_sbq_tmp
         where 1 = 0 and rownum < 1
     {% endcall %}
 
     {{ return(load_result('get_columns_in_query').table.columns | map(attribute='name') | list) }}
 {% endmacro %}
 
+{% macro oracle__get_empty_subquery_sql(select_sql) %}
+    select * from (
+        {{ select_sql }}
+    ) dbt_sbq_tmp
+    where 1 = 0 and rownum < 1
+{% endmacro %}
+
+{% macro oracle__get_empty_schema_sql(columns) %}
+    {%- set col_err = [] -%}
+    select
+    {% for i in columns %}
+      {%- set col = columns[i] -%}
+      {%- if col['data_type'] is not defined -%}
+        {{ col_err.append(col['name']) }}
+      {%- endif -%}
+      cast(null as {{ col['data_type'] }}) as {{ col['name'] }}{{ ", " if not loop.last }}
+    {%- endfor -%}
+    {# Override for Oracle #}
+     from dual
+    {%- if (col_err | length) > 0 -%}
+      {{ exceptions.column_type_missing(column_names=col_err) }}
+    {%- endif -%}
+{% endmacro %}
+
+{% macro oracle__get_select_subquery(sql) %}
+    select
+    {% for column in model['columns'] %}
+      {{ column }}{{ ", " if not loop.last }}
+    {% endfor %}
+    from (
+        {{ sql }}
+    ) model_subq
+{%- endmacro %}
 
 {% macro oracle__create_schema(relation, schema_name) -%}
   {% if relation.database -%}
     {{ adapter.verify_database(relation.database) }}
   {%- endif -%}
   {%- call statement('create_schema') -%}
     -- Noop for not breaking tests, oracle
@@ -103,32 +136,41 @@
 {%- endmacro %}
 
 
 {% macro oracle__create_table_as(temporary, relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
   {%- set parallel = config.get('parallel', none) -%}
   {%- set compression_clause = config.get('table_compression_clause', none) -%}
+  {%- set contract_config = config.get('contract') -%}
 
   {{ sql_header if sql_header is not none }}
 
   create {% if temporary -%}
     global temporary
   {%- endif %} table {{ relation.include(schema=(not temporary)) }}
+  {%- if contract_config.enforced -%}
+      {{ get_assert_columns_equivalent(sql) }}
+      {{ get_table_columns_and_constraints() }}
+      {%- set sql = get_select_subquery(sql) %}
+  {% endif %}
   {% if temporary -%} on commit preserve rows {%- endif %}
   {% if not temporary -%}
     {% if parallel %} parallel {{ parallel }}{% endif %}
     {% if compression_clause %} {{ compression_clause }} {% endif %}
   {%- endif %}
   as
     {{ sql }}
 
 {%- endmacro %}
 {% macro oracle__create_view_as(relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
-
+   {%- set contract_config = config.get('contract') -%}
+   {%- if contract_config.enforced -%}
+      {{ get_assert_columns_equivalent(sql) }}
+   {%- endif %}
   {{ sql_header if sql_header is not none }}
   create or replace view {{ relation }} as
     {{ sql }}
 
 {% endmacro %}
 
 {% macro oracle__get_columns_in_relation(relation) -%}
```

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/apply_grants.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/catalog.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/columns.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/seed/seed.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/table/table.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/materializations/view/view.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/schema_tests.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/schema_tests.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/data_types.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/dateadd.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/datediff.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/datetrunc.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datetrunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/except.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/except.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/hash.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/last_day.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/position.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/right.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/macros/utils/timestamps.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt/include/oracle/profile_template.yml` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/PKG-INFO` & `dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.4.2rc1
+Version: 1.5.0rc1
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.4.2rc1/dbt_oracle.egg-info/SOURCES.txt` & `dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -52,33 +52,39 @@
 dbt_oracle.egg-info/not-zip-safe
 dbt_oracle.egg-info/requires.txt
 dbt_oracle.egg-info/top_level.txt
 tests/README.md
 tests/__init__.py
 tests/conftest.py
 tests/functional/adapter/test_basic.py
+tests/functional/adapter/test_caching.py
 tests/functional/adapter/test_concurrency.py
 tests/functional/adapter/test_config.py
 tests/functional/adapter/test_data_types.py
 tests/functional/adapter/test_docs_generate.py
 tests/functional/adapter/test_docs_genreferences.py
 tests/functional/adapter/test_ephemeral.py
 tests/functional/adapter/test_generictests_where.py
 tests/functional/adapter/test_grants.py
 tests/functional/adapter/test_quoted_relations.py
+tests/functional/adapter/constraints/__init__.py
+tests/functional/adapter/constraints/fixtures.py
+tests/functional/adapter/constraints/test_constraints.py
 tests/functional/adapter/incremental_materialization/__init__.py
 tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
 tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
 tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
 tests/functional/adapter/incremental_materialization/test_unique_id.py
 tests/functional/adapter/incremental_materialization/quotes/__init__.py
 tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
 tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
 tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
 tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
 tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
 tests/functional/adapter/macros/__init__.py
 tests/functional/adapter/macros/test_alter_column_type.py
+tests/functional/adapter/simple_seed/__init__.py
+tests/functional/adapter/simple_seed/test_simple_seed.py
 tests/functional/adapter/snapshots/__init__.py
 tests/functional/adapter/snapshots/test_invalidate_deletes.py
 tests/functional/adapter/utils/test_common_utils.py
 tests/functional/adapter/utils/test_dateutils.py
```

### Comparing `dbt-oracle-1.4.2rc1/setup.cfg` & `dbt-oracle-1.5.0rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dbt-oracle
-version = 1.4.2rc1
+version = 1.5.0
 description = dbt (data build tool) adapter for the Oracle database
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Oracle dbt
 author = Oracle
 license = Apache Software License 2.0
 classifiers = 
@@ -26,20 +26,20 @@
 
 [options]
 python_requires = >=3.7.2
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
-	dbt-core==1.4.5
+	dbt-core==1.5.0
 	cx_Oracle==8.3.0
-	oracledb==1.2.2
+	oracledb==1.3.1
 test_suite = tests
 test_requires = 
-	dbt-tests-adapter==1.4.5
+	dbt-tests-adapter==1.5.0
 	pytest
 scripts = 
 	bin/create-pem-from-p12
 
 [options.package_data]
 dbt = include/oracle/dbt_project.yml, include/oracle/macros/*.sql, include/oracle/macros/**/**/*.sql, include/oracle/profile_template.yml
```

### Comparing `dbt-oracle-1.4.2rc1/setup.py` & `dbt-oracle-1.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 
 requirements = [
-        "dbt-core==1.4.5",
+        "dbt-core==1.5.0",
         "cx_Oracle==8.3.0",
-        "oracledb==1.2.2"
+        "oracledb==1.3.1"
 ]
 
 test_requirements = [
-    "dbt-tests-adapter==1.4.5",
+    "dbt-tests-adapter==1.5.0",
     "pytest"
 ]
 
 project_urls = {
     'Documentation': 'https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile',
     'Source': 'https://github.com/oracle/dbt-oracle',
     'Bug Tracker': 'https://github.com/oracle/dbt-oracle/issues',
     'CI': 'https://github.com/oracle/dbt-oracle/actions',
     "Release Notes": "https://github.com/oracle/dbt-oracle/releases"
 }
 
 url = 'https://github.com/oracle/dbt-oracle'
 
-VERSION = '1.4.2rc1'
+VERSION = '1.5.0rc1'
 setup(
     author="Oracle",
     python_requires='>=3.7.2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dbt-oracle-1.4.2rc1/tests/README.md` & `dbt-oracle-1.5.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/__init__.py` & `dbt-oracle-1.5.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/conftest.py` & `dbt-oracle-1.5.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/macros/test_alter_column_type.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/test_alter_column_type.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_basic.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_concurrency.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_config.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_config.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_data_types.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_docs_generate.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_docs_genreferences.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_genreferences.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_ephemeral.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_generictests_where.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_generictests_where.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_grants.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/test_quoted_relations.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_quoted_relations.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/utils/test_common_utils.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_common_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.4.2rc1/tests/functional/adapter/utils/test_dateutils.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_dateutils.py`

 * *Files identical despite different names*


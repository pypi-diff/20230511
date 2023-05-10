# Comparing `tmp/dbt-oracle-1.5.0.tar.gz` & `tmp/dbt-oracle-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-oracle-1.5.0.tar", last modified: Wed May 10 22:18:22 2023, max compression
+gzip compressed data, was "dbt-oracle-1.5.0rc1.tar", last modified: Wed May 10 21:49:02 2023, max compression
```

## Comparing `dbt-oracle-1.5.0.tar` & `dbt-oracle-1.5.0rc1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.230324 dbt-oracle-1.5.0/
--rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.0/HISTORY.md
--rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.0/LICENSE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.0/MANIFEST.in
--rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.0/NOTICE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)     3233 2023-05-10 22:18:22.230538 dbt-oracle-1.5.0/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0/README.md
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.834270 dbt-oracle-1.5.0/bin/
--rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.0/bin/create-pem-from-p12
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.838037 dbt-oracle-1.5.0/dbt/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.0/dbt/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.839807 dbt-oracle-1.5.0/dbt/adapters/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.853886 dbt-oracle-1.5.0/dbt/adapters/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/__version__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/column.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/connection_helper.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    10683 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/connections.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    12691 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/impl.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/keyword_catalog.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0/dbt/adapters/oracle/relation.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.856975 dbt-oracle-1.5.0/dbt/include/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.0/dbt/include/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.878076 dbt-oracle-1.5.0/dbt/include/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.0/dbt/include/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.0/dbt/include/oracle/dbt_project.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.900909 dbt-oracle-1.5.0/dbt/include/oracle/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)    14448 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/adapters.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/apply_grants.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/catalog.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/columns.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.812020 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.906209 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/incremental/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4087 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.921625 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.932903 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/
--rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.939219 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/table/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4403 2023-01-21 00:48:03.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/table/table.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.942918 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.948306 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-01-21 00:48:03.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/view/view.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/schema_tests.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.088767 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/data_types.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/dateadd.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/datediff.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/datetrunc.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/except.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/hash.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/last_day.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/position.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/right.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/timestamps.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.0/dbt/include/oracle/profile_template.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.126289 dbt-oracle-1.5.0/dbt_oracle.egg-info/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3233 2023-05-10 22:18:21.000000 dbt-oracle-1.5.0/dbt_oracle.egg-info/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     4110 2023-05-10 22:18:21.000000 dbt-oracle-1.5.0/dbt_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-05-10 22:18:21.000000 dbt-oracle-1.5.0/dbt_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.0/dbt_oracle.egg-info/not-zip-safe
--rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-05-10 22:18:21.000000 dbt-oracle-1.5.0/dbt_oracle.egg-info/requires.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-05-10 22:18:21.000000 dbt-oracle-1.5.0/dbt_oracle.egg-info/top_level.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.0/pyproject.toml
--rw-r--r--   0 abhisoms   (501) staff       (20)     1446 2023-05-10 22:18:22.231925 dbt-oracle-1.5.0/setup.cfg
--rw-r--r--   0 abhisoms   (501) staff       (20)     2970 2023-05-10 22:15:43.000000 dbt-oracle-1.5.0/setup.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.133486 dbt-oracle-1.5.0/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/tests/README.md
--rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.0/tests/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.0/tests/conftest.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:21.812930 dbt-oracle-1.5.0/tests/functional/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.177130 dbt-oracle-1.5.0/tests/functional/adapter/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.182258 dbt-oracle-1.5.0/tests/functional/adapter/constraints/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/tests/functional/adapter/constraints/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/tests/functional/adapter/constraints/fixtures.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/tests/functional/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.192139 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.202324 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.204368 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/sync_schema/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_unique_id.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.206416 dbt-oracle-1.5.0/tests/functional/adapter/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.0/tests/functional/adapter/macros/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/macros/test_alter_column_type.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.222950 dbt-oracle-1.5.0/tests/functional/adapter/simple_seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/tests/functional/adapter/simple_seed/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/tests/functional/adapter/simple_seed/test_simple_seed.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.225200 dbt-oracle-1.5.0/tests/functional/adapter/snapshots/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.0/tests/functional/adapter/snapshots/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.0/tests/functional/adapter/snapshots/test_invalidate_deletes.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_basic.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_caching.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_config.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_data_types.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_docs_genreferences.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_generictests_where.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_grants.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0/tests/functional/adapter/test_quoted_relations.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 22:18:22.229127 dbt-oracle-1.5.0/tests/functional/adapter/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0/tests/functional/adapter/utils/test_common_utils.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0/tests/functional/adapter/utils/test_dateutils.py
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

### Comparing `dbt-oracle-1.5.0/LICENSE.txt` & `dbt-oracle-1.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/PKG-INFO` & `dbt-oracle-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.0
+Version: 1.5.0rc1
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.0/README.md` & `dbt-oracle-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/bin/create-pem-from-p12` & `dbt-oracle-1.5.0rc1/bin/create-pem-from-p12`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/__version__.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__version__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/column.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/column.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/connection_helper.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connection_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/connections.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/impl.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/keyword_catalog.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/keyword_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/adapters/oracle/relation.py` & `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/__init__.py` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/adapters.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/apply_grants.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/catalog.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/columns.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/incremental/incremental.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/incremental/strategies.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/seed/seed.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/snapshot/strategies.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/table/table.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/tests/helpers.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/materializations/view/view.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/schema_tests.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/schema_tests.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/cast_bool_to_text.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/data_types.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/dateadd.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/datediff.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/datetrunc.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datetrunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/except.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/except.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/hash.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/last_day.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/position.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/right.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/macros/utils/timestamps.sql` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt/include/oracle/profile_template.yml` & `dbt-oracle-1.5.0rc1/dbt/include/oracle/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/dbt_oracle.egg-info/PKG-INFO` & `dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.0
+Version: 1.5.0rc1
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.0/dbt_oracle.egg-info/SOURCES.txt` & `dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/setup.cfg` & `dbt-oracle-1.5.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/setup.py` & `dbt-oracle-1.5.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     'Bug Tracker': 'https://github.com/oracle/dbt-oracle/issues',
     'CI': 'https://github.com/oracle/dbt-oracle/actions',
     "Release Notes": "https://github.com/oracle/dbt-oracle/releases"
 }
 
 url = 'https://github.com/oracle/dbt-oracle'
 
-VERSION = '1.5.0'
+VERSION = '1.5.0rc1'
 setup(
     author="Oracle",
     python_requires='>=3.7.2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dbt-oracle-1.5.0/tests/README.md` & `dbt-oracle-1.5.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/__init__.py` & `dbt-oracle-1.5.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/conftest.py` & `dbt-oracle-1.5.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/constraints/__init__.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/constraints/fixtures.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/constraints/test_constraints.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/incremental_materialization/test_unique_id.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/macros/test_alter_column_type.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/test_alter_column_type.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/simple_seed/__init__.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/simple_seed/test_simple_seed.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/test_simple_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/snapshots/test_invalidate_deletes.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_basic.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_caching.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_concurrency.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_config.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_config.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_data_types.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_docs_generate.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_docs_genreferences.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_genreferences.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_ephemeral.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_generictests_where.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_generictests_where.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_grants.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/test_quoted_relations.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_quoted_relations.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/utils/test_common_utils.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_common_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0/tests/functional/adapter/utils/test_dateutils.py` & `dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_dateutils.py`

 * *Files identical despite different names*


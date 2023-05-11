# Comparing `tmp/data_diff-0.7.5.tar.gz` & `tmp/data_diff-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.5.tar", max compression
+gzip compressed data, was "data_diff-0.7.6.tar", max compression
```

## Comparing `data_diff-0.7.5.tar` & `data_diff-0.7.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.5/LICENSE
--rw-r--r--   0        0        0     2106 2023-05-05 21:08:17.221526 data_diff-0.7.5/README.md
--rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.5/data_diff/__init__.py
--rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.5/data_diff/__main__.py
--rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.5/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.5/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0     9253 2023-04-21 21:58:08.194472 data_diff-0.7.5/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.5/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.5/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.5/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.5/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.5/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.5/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.5/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.5/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.5/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.5/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.5/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.5/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.5/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.5/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.5/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.5/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    12878 2023-05-05 21:08:17.222295 data_diff-0.7.5/data_diff/dbt.py
--rw-r--r--   0        0        0    16856 2023-05-05 21:08:17.222470 data_diff-0.7.5/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.5/data_diff/diff_tables.py
--rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.5/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.5/data_diff/info_tree.py
--rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.5/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.5/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.5/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.5/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.5/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.5/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.5/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.5/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.5/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.5/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.5/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.5/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.5/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    20130 2023-05-05 21:08:17.223365 data_diff-0.7.5/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.5/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.5/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.5/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.5/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.5/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.5/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.5/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.5/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.5/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     6312 2023-05-05 21:08:17.223928 data_diff-0.7.5/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.5/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.5/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.5/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.5/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.5/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.5/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.5/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.5/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.5/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.5/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.5/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.5/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.5/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.5/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.5/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.5/data_diff/tracking.py
--rw-r--r--   0        0        0     5247 2023-05-05 21:08:17.224565 data_diff-0.7.5/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-05-05 21:08:17.224662 data_diff-0.7.5/data_diff/version.py
--rwxr-xr-x   0        0        0     2865 2023-05-05 21:08:17.225592 data_diff-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 data_diff-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.6/LICENSE
+-rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.6/README.md
+-rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.6/data_diff/__init__.py
+-rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.6/data_diff/__main__.py
+-rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.6/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.6/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0     9335 2023-05-11 19:39:43.704637 data_diff-0.7.6/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.6/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.6/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.6/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.6/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.6/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.6/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.6/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.6/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.6/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.6/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.6/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.6/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.6/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.6/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.6/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.6/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    13326 2023-05-11 19:39:43.704995 data_diff-0.7.6/data_diff/dbt.py
+-rw-r--r--   0        0        0    17697 2023-05-11 19:39:43.705201 data_diff-0.7.6/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.6/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.6/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.6/data_diff/info_tree.py
+-rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.6/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.6/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.6/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.6/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.6/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.6/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.6/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.6/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.6/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.6/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.6/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.6/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.6/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.6/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.6/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.6/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.6/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.6/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.6/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.6/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.6/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.6/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.6/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6312 2023-05-05 21:08:17.223928 data_diff-0.7.6/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.6/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.6/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.6/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.6/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.6/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.6/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.6/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.6/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.6/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.6/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.6/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.6/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.6/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.6/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.6/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.6/data_diff/tracking.py
+-rw-r--r--   0        0        0     5247 2023-05-05 21:08:17.224565 data_diff-0.7.6/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-05-11 19:39:43.705598 data_diff-0.7.6/data_diff/version.py
+-rwxr-xr-x   0        0        0     2816 2023-05-11 19:39:43.706580 data_diff-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 data_diff-0.7.6/PKG-INFO
```

### Comparing `data_diff-0.7.5/LICENSE` & `data_diff-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/__init__.py` & `data_diff-0.7.6/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/__main__.py` & `data_diff-0.7.6/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/cloud/data_source.py` & `data_diff-0.7.6/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/cloud/datafold_api.py` & `data_diff-0.7.6/data_diff/cloud/datafold_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     data_source1_id: int
     data_source2_id: int
     table1: List[str]
     table2: List[str]
     pk_columns: List[str]
     filter1: Optional[str] = None
     filter2: Optional[str] = None
+    include_columns: Optional[List[str]]
+    exclude_columns: Optional[List[str]]
 
 
 class TSummaryResultPrimaryKeyStats(pydantic.BaseModel):
     total_rows: Tuple[int, int]
     nulls: Tuple[int, int]
     dupes: Tuple[int, int]
     exclusives: Tuple[int, int]
```

### Comparing `data_diff-0.7.5/data_diff/config.py` & `data_diff-0.7.6/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/databases/_connect.py` & `data_diff-0.7.6/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/dbt.py` & `data_diff-0.7.6/data_diff/dbt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import time
 import webbrowser
+import pydantic
 import rich
 from rich.prompt import Confirm
 
-from dataclasses import dataclass
 from typing import List, Optional, Dict
 from .utils import dbt_diff_string_template, getLogger
 from pathlib import Path
 
 import keyring
 
 from .cloud import DatafoldAPI, TCloudApiDataDiff, get_or_create_data_source
@@ -28,22 +28,23 @@
     send_event_json,
     is_tracking_enabled,
 )
 from .utils import run_as_daemon, truncate_error
 from . import connect_to_table, diff_tables, Algorithm
 
 
-@dataclass
-class DiffVars:
+class TDiffVars(pydantic.BaseModel):
     dev_path: List[str]
     prod_path: List[str]
     primary_keys: List[str]
-    connection: Dict[str, str]
-    threads: Optional[int]
+    connection: Dict[str, Optional[str]]
+    threads: Optional[int] = None
     where_filter: Optional[str] = None
+    include_columns: List[str]
+    exclude_columns: List[str]
 
 
 def dbt_diff(
     profiles_dir_override: Optional[str] = None,
     project_dir_override: Optional[str] = None,
     is_cloud: bool = False,
     dbt_selection: Optional[str] = None,
@@ -89,19 +90,14 @@
                     "\nvars:\n data_diff:\n   datasource_id: 1234"
                 )
         rich.print("[green][bold]\nDiffs in progress...[/][/]\n")
 
     else:
         dbt_parser.set_connection()
 
-    if config_prod_database is None:
-        raise ValueError(
-            "Expected a value for prod_database: OR prod_database: AND prod_schema: under \nvars:\n  data_diff: "
-        )
-
     for model in models:
         diff_vars = _get_diff_vars(
             dbt_parser, config_prod_database, config_prod_schema, config_prod_custom_schema, model
         )
 
         if diff_vars.primary_keys:
             if is_cloud:
@@ -123,15 +119,15 @@
 
 def _get_diff_vars(
     dbt_parser: "DbtParser",
     config_prod_database: Optional[str],
     config_prod_schema: Optional[str],
     config_prod_custom_schema: Optional[str],
     model,
-) -> DiffVars:
+) -> TDiffVars:
     dev_database = model.database
     dev_schema = model.schema_
 
     primary_keys = dbt_parser.get_pk_from_model(model, dbt_parser.unique_columns, "primary-key")
 
     prod_database = config_prod_database if config_prod_database else dev_database
 
@@ -150,34 +146,36 @@
         # no custom schema, use the default
         else:
             prod_schema = config_prod_schema
     else:
         prod_schema = dev_schema
 
     if dbt_parser.requires_upper:
-        dev_qualified_list = [x.upper() for x in [dev_database, dev_schema, model.alias]]
-        prod_qualified_list = [x.upper() for x in [prod_database, prod_schema, model.alias]]
+        dev_qualified_list = [x.upper() for x in [dev_database, dev_schema, model.alias] if x]
+        prod_qualified_list = [x.upper() for x in [prod_database, prod_schema, model.alias] if x]
         primary_keys = [x.upper() for x in primary_keys]
     else:
-        dev_qualified_list = [dev_database, dev_schema, model.alias]
-        prod_qualified_list = [prod_database, prod_schema, model.alias]
+        dev_qualified_list = [x for x in [dev_database, dev_schema, model.alias] if x]
+        prod_qualified_list = [x for x in [prod_database, prod_schema, model.alias] if x]
 
-    where_filter = None
-    if model.meta:
-        try:
-            where_filter = model.meta["datafold"]["datadiff"]["filter"]
-        except KeyError:
-            pass
+    datadiff_model_config = dbt_parser.get_datadiff_model_config(model.meta)
 
-    return DiffVars(
-        dev_qualified_list, prod_qualified_list, primary_keys, dbt_parser.connection, dbt_parser.threads, where_filter
+    return TDiffVars(
+        dev_path=dev_qualified_list,
+        prod_path=prod_qualified_list,
+        primary_keys=primary_keys,
+        connection=dbt_parser.connection,
+        threads=dbt_parser.threads,
+        where_filter=datadiff_model_config.where_filter,
+        include_columns=datadiff_model_config.include_columns,
+        exclude_columns=datadiff_model_config.exclude_columns,
     )
 
 
-def _local_diff(diff_vars: DiffVars) -> None:
+def _local_diff(diff_vars: TDiffVars) -> None:
     column_diffs_str = ""
     dev_qualified_str = ".".join(diff_vars.dev_path)
     prod_qualified_str = ".".join(diff_vars.prod_path)
     diff_output_str = _diff_output_base(dev_qualified_str, prod_qualified_str)
 
     table1 = connect_to_table(diff_vars.connection, dev_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads)
     table2 = connect_to_table(
@@ -190,26 +188,33 @@
     # Not ideal, but we don't have more specific exceptions yet
     except Exception as ex:
         logger.debug(ex)
         diff_output_str += "[red]New model or no access to prod table.[/] \n"
         rich.print(diff_output_str)
         return
 
-    mutual_set = set(table1_columns) & set(table2_columns)
-    table1_set_diff = list(set(table1_columns) - set(table2_columns))
-    table2_set_diff = list(set(table2_columns) - set(table1_columns))
+    column_set = set(table1_columns).intersection(table2_columns)
+    table1_diff = set(table1_columns).difference(table2_columns)
+    table2_diff = set(table2_columns).difference(table1_columns)
+
+    if table1_diff:
+        column_diffs_str += f"Column(s) added: {table1_diff}\n"
+
+    if table2_diff:
+        column_diffs_str += f"Column(s) removed: {table2_diff}\n"
+
+    column_set = column_set - set(diff_vars.primary_keys)
 
-    if table1_set_diff:
-        column_diffs_str += "Column(s) added: " + str(table1_set_diff) + "\n"
+    if diff_vars.include_columns:
+        column_set = {x for x in column_set if x.upper() in [y.upper() for y in diff_vars.include_columns]}
 
-    if table2_set_diff:
-        column_diffs_str += "Column(s) removed: " + str(table2_set_diff) + "\n"
+    if diff_vars.exclude_columns:
+        column_set = {x for x in column_set if x.upper() not in [y.upper() for y in diff_vars.exclude_columns]}
 
-    mutual_set = mutual_set - set(diff_vars.primary_keys)
-    extra_columns = tuple(mutual_set)
+    extra_columns = tuple(column_set)
 
     diff = diff_tables(
         table1,
         table2,
         threaded=True,
         algorithm=Algorithm.JOINDIFF,
         extra_columns=extra_columns,
@@ -251,38 +256,40 @@
         keyring.set_password("data-diff", "DATAFOLD_API_KEY", api_key)
     except Exception as e:
         rich.print(f"[red]Failed when saving the API key to the system keyring service. Reason: {e}")
 
     return DatafoldAPI(api_key=api_key, host=datafold_host)
 
 
-def _cloud_diff(diff_vars: DiffVars, datasource_id: int, api: DatafoldAPI) -> None:
+def _cloud_diff(diff_vars: TDiffVars, datasource_id: int, api: DatafoldAPI) -> None:
     diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
     payload = TCloudApiDataDiff(
         data_source1_id=datasource_id,
         data_source2_id=datasource_id,
         table1=diff_vars.prod_path,
         table2=diff_vars.dev_path,
         pk_columns=diff_vars.primary_keys,
         filter1=diff_vars.where_filter,
         filter2=diff_vars.where_filter,
+        include_columns=diff_vars.include_columns,
+        exclude_columns=diff_vars.exclude_columns,
     )
 
     if is_tracking_enabled():
         event_json = create_start_event_json({"is_cloud": True, "datasource_id": datasource_id})
         run_as_daemon(send_event_json, event_json)
 
     start = time.monotonic()
     error = None
     diff_id = None
     diff_url = None
     try:
         diff_id = api.create_data_diff(payload=payload)
         diff_url = f"{api.host}/datadiffs/{diff_id}/overview"
-        rich.print(f"{diff_vars.dev_path[2]}: {diff_url}")
+        rich.print(f"{diff_vars.dev_path[-1]}: {diff_url}")
 
         if diff_id is None:
             raise Exception(f"Api response did not contain a diff_id")
 
         diff_results = api.poll_data_diff_results(diff_id)
 
         rows_added_count = diff_results.pks.exclusives[1]
```

### Comparing `data_diff-0.7.5/data_diff/dbt_parser.py` & `data_diff-0.7.6/data_diff/dbt_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 from argparse import Namespace
 from collections import defaultdict
 import json
 import os
 from pathlib import Path
 from typing import List, Dict, Tuple, Set, Optional
+import yaml
 
 from packaging.version import parse as parse_version
+import pydantic
+from dbt_artifacts_parser.parser import parse_run_results, parse_manifest
+from dbt.config.renderer import ProfileRenderer
 
 from .utils import getLogger, get_from_dict_with_raise
 from .version import __version__
 
 
 logger = getLogger(__name__)
 
 
-def import_dbt_dependencies():
-    try:
-        from dbt_artifacts_parser.parser import parse_run_results, parse_manifest
-        from dbt.config.renderer import ProfileRenderer
-        import yaml
-    except ImportError:
-        raise RuntimeError("Could not import 'dbt' package. You can install it using: pip install 'data-diff[dbt]'.")
-
-    # dbt 1.5+ specific stuff to power selection of models
-    try:
-        # ProfileRenderer.render_data() fails without instantiating global flag MACRO_DEBUGGING in dbt-core 1.5
-        from dbt.flags import set_flags
-
-        set_flags(Namespace(MACRO_DEBUGGING=False))
-    except:
-        pass
-
+# getting this dbt_runner will only succeed in dbt-core>=1.5
+# it's needed for `--select` functionality
+def try_get_dbt_runner():
     try:
         from dbt.cli.main import dbtRunner
     except ImportError:
         dbtRunner = None
 
     if dbtRunner is not None:
         dbt_runner = dbtRunner()
     else:
         dbt_runner = None
 
-    return parse_run_results, parse_manifest, ProfileRenderer, yaml, dbt_runner
+    return dbt_runner
+
+
+# ProfileRenderer.render_data() fails without instantiating global flag MACRO_DEBUGGING in dbt-core 1.5
+# hacky but seems to be a bug on dbt's end
+def try_set_dbt_flags():
+    try:
+        from dbt.flags import set_flags
+
+        set_flags(Namespace(MACRO_DEBUGGING=False))
+    except:
+        pass
 
 
 RUN_RESULTS_PATH = "target/run_results.json"
 MANIFEST_PATH = "target/manifest.json"
 PROJECT_FILE = "dbt_project.yml"
 PROFILES_FILE = "profiles.yml"
 LOWER_DBT_V = "1.0.0"
@@ -64,26 +65,27 @@
     return Path.cwd() if (Path.cwd() / PROFILES_FILE).exists() else Path.home() / ".dbt"
 
 
 def legacy_profiles_dir() -> Path:
     return Path.home() / ".dbt"
 
 
+class TDatadiffModelConfig(pydantic.BaseModel):
+    where_filter: Optional[str] = None
+    include_columns: List[str] = []
+    exclude_columns: List[str] = []
+
+
 class DbtParser:
     def __init__(self, profiles_dir_override: str, project_dir_override: str) -> None:
-        (
-            self.parse_run_results,
-            self.parse_manifest,
-            self.ProfileRenderer,
-            self.yaml,
-            self.dbt_runner,
-        ) = import_dbt_dependencies()
+        try_set_dbt_flags()
+        self.dbt_runner = try_get_dbt_runner()
         self.profiles_dir = Path(profiles_dir_override or default_profiles_dir())
         self.project_dir = Path(project_dir_override or default_project_dir())
-        self.connection = None
+        self.connection = {}
         self.project_dict = self.get_project_dict()
         self.manifest_obj = self.get_manifest_obj()
         self.dbt_user_id = self.manifest_obj.metadata.user_id
         self.dbt_version = self.manifest_obj.metadata.dbt_version
         self.dbt_project_id = self.manifest_obj.metadata.project_id
         self.requires_upper = False
         self.threads = None
@@ -91,28 +93,43 @@
 
     def get_datadiff_variables(self) -> dict:
         doc_url = "https://docs.datafold.com/development_testing/open_source#configure-your-dbt-project"
         error_message = f"vars: data_diff: section not found in dbt_project.yml.\n\nTo solve this, please configure your dbt project: \n{doc_url}\n"
         vars = get_from_dict_with_raise(self.project_dict, "vars", error_message)
         return get_from_dict_with_raise(vars, "data_diff", error_message)
 
+    def get_datadiff_model_config(self, model_meta: dict) -> TDatadiffModelConfig:
+        where_filter = None
+        include_columns = []
+        exclude_columns = []
+
+        if "datafold" in model_meta and "datadiff" in model_meta["datafold"]:
+            config = model_meta["datafold"]["datadiff"]
+            where_filter = config.get("filter")
+            include_columns = config.get("include_columns") or []
+            exclude_columns = config.get("exclude_columns") or []
+
+        return TDatadiffModelConfig(
+            where_filter=where_filter, include_columns=include_columns, exclude_columns=exclude_columns
+        )
+
     def get_models(self, dbt_selection: Optional[str] = None):
         dbt_version = parse_version(self.dbt_version)
         if dbt_selection:
             if (dbt_version.major, dbt_version.minor) >= (1, 5):
                 if self.dbt_runner:
                     return self.get_dbt_selection_models(dbt_selection)
                 # edge case if running data-diff from a separate env than dbt (likely local development)
                 else:
                     raise Exception(
                         "data-diff is using a dbt-core version < 1.5, update the environment's dbt-core version via pip install 'dbt-core>=1.5' in order to use `--select`"
                     )
             else:
                 raise Exception(
-                    f"Use of the `--select` feature requires dbt >= 1.5. Found dbt manifest: v{dbt_version}"
+                    f"The `--select` feature requires dbt >= 1.5, but your project's manifest.json is from dbt v{dbt_version}. Please follow these steps to use the `--select` feature: \n 1. Update your dbt-core version via pip install 'dbt-core>=1.5'. Details: https://docs.getdbt.com/docs/core/pip-install#change-dbt-core-versions \n 2. Execute any `dbt` command (`run`, `compile`, `build`) to create a new manifest.json."
                 )
         else:
             return self.get_run_results_models()
 
     def get_dbt_selection_models(self, dbt_selection: str) -> List[str]:
         # log level and format settings needed to prevent dbt from printing to stdout
         # ls command is used to get the list of model unique_ids
@@ -147,15 +164,15 @@
             logger.debug(str(results))
             raise Exception("Encountered an unexpected error while finding `--select` models")
 
     def get_run_results_models(self):
         with open(self.project_dir / RUN_RESULTS_PATH) as run_results:
             logger.info(f"Parsing file {RUN_RESULTS_PATH}")
             run_results_dict = json.load(run_results)
-            run_results_obj = self.parse_run_results(run_results=run_results_dict)
+            run_results_obj = parse_run_results(run_results=run_results_dict)
 
         dbt_version = parse_version(run_results_obj.metadata.dbt_version)
 
         if dbt_version < parse_version("1.3.0"):
             self.profiles_dir = legacy_profiles_dir()
 
         if dbt_version < parse_version(LOWER_DBT_V):
@@ -173,36 +190,36 @@
         print(f"Running with data-diff={__version__}\n")
         return models
 
     def get_manifest_obj(self):
         with open(self.project_dir / MANIFEST_PATH) as manifest:
             logger.info(f"Parsing file {MANIFEST_PATH}")
             manifest_dict = json.load(manifest)
-            manifest_obj = self.parse_manifest(manifest=manifest_dict)
+            manifest_obj = parse_manifest(manifest=manifest_dict)
         return manifest_obj
 
     def get_project_dict(self):
         with open(self.project_dir / PROJECT_FILE) as project:
             logger.info(f"Parsing file {PROJECT_FILE}")
-            project_dict = self.yaml.safe_load(project)
+            project_dict = yaml.safe_load(project)
         return project_dict
 
     def get_connection_creds(self) -> Tuple[Dict[str, str], str]:
         profiles_path = self.profiles_dir / PROFILES_FILE
         with open(profiles_path) as profiles:
             logger.info(f"Parsing file {profiles_path}")
-            profiles = self.yaml.safe_load(profiles)
+            profiles = yaml.safe_load(profiles)
 
         dbt_profile_var = self.project_dict.get("profile")
 
         profile = get_from_dict_with_raise(
             profiles, dbt_profile_var, f"No profile '{dbt_profile_var}' found in '{profiles_path}'."
         )
         # values can contain env_vars
-        rendered_profile = self.ProfileRenderer().render_data(profile)
+        rendered_profile = ProfileRenderer().render_data(profile)
         profile_target = get_from_dict_with_raise(
             rendered_profile, "target", f"No target found in profile '{dbt_profile_var}' in '{profiles_path}'."
         )
         outputs = get_from_dict_with_raise(
             rendered_profile, "outputs", f"No outputs found in profile '{dbt_profile_var}' in '{profiles_path}'."
         )
         credentials = get_from_dict_with_raise(
```

### Comparing `data_diff-0.7.5/data_diff/diff_tables.py` & `data_diff-0.7.6/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/hashdiff_tables.py` & `data_diff-0.7.6/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/info_tree.py` & `data_diff-0.7.6/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/joindiff_tables.py` & `data_diff-0.7.6/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/lexicographic_space.py` & `data_diff-0.7.6/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/parse_time.py` & `data_diff-0.7.6/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/query_utils.py` & `data_diff-0.7.6/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.7.6/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.7.6/data_diff/sqeleton/abcs/mixins.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.7.6/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/base.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     TemporalType,
     UnknownColType,
     TimestampTZ,
     Text,
     DbTime,
     DbPath,
     Boolean,
-    JSON
+    JSON,
 )
 from ..abcs.mixins import Compilable
 from ..abcs.mixins import (
     AbstractMixin_Schema,
     AbstractMixin_RandomSample,
     AbstractMixin_NormalizeValue,
     AbstractMixin_OptimizerHints,
@@ -59,15 +59,15 @@
         @wraps(f)
         def _inner():
             try:
                 return f()
             except ModuleNotFoundError as e:
                 s = text
                 if package:
-                    s += f"You can install it using 'pip install data_diff[{package}]'."
+                    s += f"Please complete setup by running: pip install 'data_diff[{package}]'."
                 raise ModuleNotFoundError(f"{e}\n\n{s}\n")
 
         return _inner
 
     return dec
```

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/bigquery.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/presto.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/redshift.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/trino.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.7.6/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/queries/api.py` & `data_diff-0.7.6/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.7.6/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.7.6/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/queries/extras.py` & `data_diff-0.7.6/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/query_utils.py` & `data_diff-0.7.6/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/repl.py` & `data_diff-0.7.6/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/schema.py` & `data_diff-0.7.6/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/sqeleton/utils.py` & `data_diff-0.7.6/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/table_segment.py` & `data_diff-0.7.6/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/thread_utils.py` & `data_diff-0.7.6/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/tracking.py` & `data_diff-0.7.6/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/data_diff/utils.py` & `data_diff-0.7.6/data_diff/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.5/pyproject.toml` & `data_diff-0.7.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.5"
+version = "0.7.6"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -36,16 +36,16 @@
 psycopg2 = {version="*", optional=true}
 snowflake-connector-python = {version="^2.7.2", optional=true}
 cryptography = {version="*", optional=true}
 trino = {version="^0.314.0", optional=true}
 presto-python-client = {version="*", optional=true}
 clickhouse-driver = {version="*", optional=true}
 duckdb = {version="^0.7.0", optional=true}
-dbt-artifacts-parser = {version="^0.3.0", optional=true}
-dbt-core = {version="^1.0.0", optional=true}
+dbt-artifacts-parser = {version="^0.3.0"}
+dbt-core = {version="^1.0.0"}
 keyring = "*"
 tabulate = "^0.9.0"
 preql = {version="^0.2.19", optional=true}
 cx_Oracle = {version="*", optional=true}
 vertica-python = {version="*", optional=true}
 
 [tool.poetry.dev-dependencies]
@@ -67,23 +67,23 @@
 # databricks-sql-connector = "*"
 
 [tool.poetry.extras]
 # When adding, update also: README + dev deps just above
 preql = ["preql"]
 mysql = ["mysql-connector-python"]
 postgresql = ["psycopg2"]
+redshift = ["psycopg2"]
 snowflake = ["snowflake-connector-python", "cryptography"]
 presto = ["presto-python-client"]
 oracle = ["cx_Oracle"]
 # databricks = ["databricks-sql-connector"]
 trino = ["trino"]
 clickhouse = ["clickhouse-driver"]
 vertica = ["vertica-python"]
 duckdb = ["duckdb"]
-dbt = ["dbt-core", "dbt-artifacts-parser"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 data-diff = 'data_diff.__main__:main'
```

### Comparing `data_diff-0.7.5/PKG-INFO` & `data_diff-0.7.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.5
+Version: 0.7.6
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,38 +22,38 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Typing :: Typed
 Provides-Extra: clickhouse
-Provides-Extra: dbt
 Provides-Extra: duckdb
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
 Provides-Extra: preql
 Provides-Extra: presto
+Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: trino
 Provides-Extra: vertica
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: clickhouse-driver ; extra == "clickhouse"
 Requires-Dist: cryptography ; extra == "snowflake"
 Requires-Dist: cx_Oracle ; extra == "oracle"
-Requires-Dist: dbt-artifacts-parser (>=0.3.0,<0.4.0) ; extra == "dbt"
-Requires-Dist: dbt-core (>=1.0.0,<2.0.0) ; extra == "dbt"
+Requires-Dist: dbt-artifacts-parser (>=0.3.0,<0.4.0)
+Requires-Dist: dbt-core (>=1.0.0,<2.0.0)
 Requires-Dist: dsnparse (<0.2.0) ; python_version < "3.8.0"
 Requires-Dist: dsnparse ; python_version >= "3.8.0"
 Requires-Dist: duckdb (>=0.7.0,<0.8.0) ; extra == "duckdb"
 Requires-Dist: keyring
 Requires-Dist: mysql-connector-python (==8.0.29) ; extra == "mysql"
 Requires-Dist: preql (>=0.2.19,<0.3.0) ; extra == "preql"
 Requires-Dist: presto-python-client ; extra == "presto"
-Requires-Dist: psycopg2 ; extra == "postgresql"
+Requires-Dist: psycopg2 ; extra == "postgresql" or extra == "redshift"
 Requires-Dist: rich
 Requires-Dist: runtype (>=0.2.6,<0.3.0)
 Requires-Dist: snowflake-connector-python (>=2.7.2,<3.0.0) ; extra == "snowflake"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: trino (>=0.314.0,<0.315.0) ; extra == "trino"
 Requires-Dist: vertica-python ; extra == "vertica"
@@ -84,22 +84,53 @@
 
 ![development_testing_gif](https://user-images.githubusercontent.com/1799931/236354286-d1d044cf-2168-4128-8a21-8c8ca7fd494c.gif)
 
 </div>
 
 <br>
 
+:eyes: **Watch 4-min demo video [here](https://www.loom.com/share/ad3df969ba6b4298939efb2fbcc14cde)**
+
 ## Getting Started
 
 **Install `data-diff`**
+
+Install `data-diff` with the command that is specific to the database you use with dbt.
+
+### Snowflake
+```
+pip install data-diff 'data-diff[snowflake,dbt]' -U
+```
+
+### BigQuery
+```
+pip install data-diff 'data-diff[dbt]' google-cloud-bigquery -U
+```
+
+### Redshift
+```
+pip install data-diff 'data-diff[redshift,dbt]' -U
+```
+
+### Postgres
+```
+pip install data-diff 'data-diff[postgres,dbt]' -U
+```
+
+### Databricks
+```
+pip install data-diff 'data-diff[databricks,dbt]' -U
+```
+
+### DuckDB
 ```
-pip install data-diff
+pip install data-diff 'data-diff[duckdb,dbt]' -U
 ```
 
-**Update a few lines in your `dbt_project.yml`**
+**Update a few lines in your `dbt_project.yml`**.
 ```
 #dbt_project.yml
 vars:
   data_diff:
     prod_database: my_database
     prod_schema: my_default_schema
 ```
@@ -114,15 +145,15 @@
 
 Please reach out on the dbt Slack in [#tools-datafold](https://getdbt.slack.com/archives/C03D25A92UU) if you have any trouble whatsoever getting started!
 
 <br><br>
 
 ### Diffing between databases
 
-Check out our [documentation](https://github.com/datafold/data-diff/blob/master/docs/supported-databases.md) if you're looking to compare data across databases (for example, between Postgres and Snowflake).
+Check out our [documentation](https://docs.datafold.com/reference/open_source/cli) if you're looking to compare data across databases (for example, between Postgres and Snowflake).
 
 <br>
 
 ## Contributors
 
 We thank everyone who contributed so far!
```


# Comparing `tmp/dbt-clickhouse-1.4.0.tar.gz` & `tmp/dbt-clickhouse-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickhouse-1.4.0.tar", last modified: Mon Feb  6 17:54:24 2023, max compression
+gzip compressed data, was "dbt-clickhouse-1.4.1.tar", last modified: Thu May 11 16:26:47 2023, max compression
```

## Comparing `dbt-clickhouse-1.4.0.tar` & `dbt-clickhouse-1.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/dbclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/nativeclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/include/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.571637 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/s3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/persist_docs.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/schema_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/utils/utils.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-02-06 17:54:24.000000 dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-06 17:54:24.000000 dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 17:54:24.000000 dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-06 17:54:24.000000 dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-06 17:54:24.000000 dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 17:54:24.575637 dbt-clickhouse-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-02-06 17:54:18.000000 dbt-clickhouse-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.678781 dbt-clickhouse-1.4.1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.678781 dbt-clickhouse-1.4.1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/dbclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/nativeclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.678781 dbt-clickhouse-1.4.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.682782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/persist_docs.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/schema_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/utils.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 16:26:47.000000 dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:26:47.686782 dbt-clickhouse-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-11 16:26:43.000000 dbt-clickhouse-1.4.1/setup.py
```

### Comparing `dbt-clickhouse-1.4.0/LICENSE` & `dbt-clickhouse-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/PKG-INFO` & `dbt-clickhouse-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.4.0
+Version: 1.4.1
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,15 @@
 </p>
 
 # dbt-clickhouse
 
 This plugin ports [dbt](https://getdbt.com) functionality to [Clickhouse](https://clickhouse.tech/).
 
 The plugin uses syntax that requires ClickHouse version 22.1 or newer. We do not test older versions of Clickhouse.  We also do not currently test
-Replicated tables/`ON CLUSTER` functionality.
+Replicated tables or the related `ON CLUSTER` functionality.
 
 ## Installation
 
 Use your favorite Python package manager to install the app from PyPI, e.g.
 
 ```bash
 pip install dbt-clickhouse
@@ -47,15 +47,15 @@
 - [x] Incremental materialization
 - [x] Seeds
 - [x] Sources
 - [x] Docs generate
 - [x] Tests
 - [x] Snapshots
 - [x] Most dbt-utils macros (now included in dbt-core)  
-- [x] Ephemeral materialization (but incompatible with table materializations)
+- [x] Ephemeral materialization
 
 # Usage Notes
 
 ## Database
 
 The dbt model relation identifier `database.schema.table` is not compatible with Clickhouse because Clickhouse does not support a `schema`.
 So we use a simplified approach `schema.table`, where `schema` is the Clickhouse database. Using the `default` database is not recommended.
@@ -107,16 +107,16 @@
 | unique_key             | A tuple of column names that uniquely identify rows.  Used with incremental models for updates.                                                                                                                                                        | Optional                          |
 | inserts_only           | If set to True for an incremental model, incremental updates will be inserted directly to the target table without creating intermediate table. It has been deprecated in favor of the `append` incremental `strategy`, which operates in the same way | Optional                          |
 | incremental_strategy   | Incremental model update strategy of `delete+insert` or `append`.  See the following Incremental Model Strategies                                                                                                                                      | Optional (default: `default`)     |
 | incremental_predicates | Additional conditions to be applied to the incremental materialization (only applied to `delete+insert` strategy                                                                                                                                       |
 ## Known Limitations
 
 * Replicated tables (combined with the `cluster` profile setting) are available using the `on_cluster_clause` macro but are not included in the test suite and not formally tested. 
-* Ephemeral models/CTEs don't work with INSERT statements in ClickHouse, so table materializations that incorporate an ephemeral model will fail.
-See https://github.com/ClickHouse/ClickHouse/issues/30323.  View models and other SQL statements using ephemeral models should work correctly.
+* Ephemeral models/CTEs don't work if placed before the "INSERT INTO" in a ClickHouse insert statement, see https://github.com/ClickHouse/ClickHouse/issues/30323.  This
+should not affect most models, but care should be taken where an ephemeral model is placed in model definitions and other SQL statements.
 
 ## Incremental Model Strategies
 
 As of version 1.3.2, dbt-clickhouse supports three incremental model strategies.
 
 ### The Default (Legacy) Strategy
```

### Comparing `dbt-clickhouse-1.4.0/README.md` & `dbt-clickhouse-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 # dbt-clickhouse
 
 This plugin ports [dbt](https://getdbt.com) functionality to [Clickhouse](https://clickhouse.tech/).
 
 The plugin uses syntax that requires ClickHouse version 22.1 or newer. We do not test older versions of Clickhouse.  We also do not currently test
-Replicated tables/`ON CLUSTER` functionality.
+Replicated tables or the related `ON CLUSTER` functionality.
 
 ## Installation
 
 Use your favorite Python package manager to install the app from PyPI, e.g.
 
 ```bash
 pip install dbt-clickhouse
@@ -24,15 +24,15 @@
 - [x] Incremental materialization
 - [x] Seeds
 - [x] Sources
 - [x] Docs generate
 - [x] Tests
 - [x] Snapshots
 - [x] Most dbt-utils macros (now included in dbt-core)  
-- [x] Ephemeral materialization (but incompatible with table materializations)
+- [x] Ephemeral materialization
 
 # Usage Notes
 
 ## Database
 
 The dbt model relation identifier `database.schema.table` is not compatible with Clickhouse because Clickhouse does not support a `schema`.
 So we use a simplified approach `schema.table`, where `schema` is the Clickhouse database. Using the `default` database is not recommended.
@@ -84,16 +84,16 @@
 | unique_key             | A tuple of column names that uniquely identify rows.  Used with incremental models for updates.                                                                                                                                                        | Optional                          |
 | inserts_only           | If set to True for an incremental model, incremental updates will be inserted directly to the target table without creating intermediate table. It has been deprecated in favor of the `append` incremental `strategy`, which operates in the same way | Optional                          |
 | incremental_strategy   | Incremental model update strategy of `delete+insert` or `append`.  See the following Incremental Model Strategies                                                                                                                                      | Optional (default: `default`)     |
 | incremental_predicates | Additional conditions to be applied to the incremental materialization (only applied to `delete+insert` strategy                                                                                                                                       |
 ## Known Limitations
 
 * Replicated tables (combined with the `cluster` profile setting) are available using the `on_cluster_clause` macro but are not included in the test suite and not formally tested. 
-* Ephemeral models/CTEs don't work with INSERT statements in ClickHouse, so table materializations that incorporate an ephemeral model will fail.
-See https://github.com/ClickHouse/ClickHouse/issues/30323.  View models and other SQL statements using ephemeral models should work correctly.
+* Ephemeral models/CTEs don't work if placed before the "INSERT INTO" in a ClickHouse insert statement, see https://github.com/ClickHouse/ClickHouse/issues/30323.  This
+should not affect most models, but care should be taken where an ephemeral model is placed in model definitions and other SQL statements.
 
 ## Incremental Model Strategies
 
 As of version 1.3.2, dbt-clickhouse supports three incremental model strategies.
 
 ### The Default (Legacy) Strategy
```

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/__init__.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/column.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/connections.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/credentials.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/dbclient.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/dbclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/httpclient.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/httpclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/impl.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         fmt = fmt or s3config.get('fmt')
         bucket = bucket or s3config.get('bucket', '')
         path = path or s3config.get('path', '')
         url = bucket
         if path:
             if bucket and path and not bucket.endswith('/') and not bucket.startswith('/'):
                 path = f'/{path}'
-            url = f'{url}{path}'
+            url = f'{url}{path}'.replace('//', '/')
         if not url.startswith('http'):
             url = f'https://{url}'
         access = ''
         if aws_access_key_id and not aws_secret_access_key:
             raise DbtRuntimeError('S3 aws_access_key_id specified without aws_secret_access_key')
         if aws_secret_access_key and not aws_access_key_id:
             raise DbtRuntimeError('S3 aws_secret_access_key specified without aws_access_key_id')
```

### Comparing `dbt-clickhouse-1.4.0/dbt/adapters/clickhouse/nativeclient.py` & `dbt-clickhouse-1.4.1/dbt/adapters/clickhouse/nativeclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters/apply_grants.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters/relation.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/adapters.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/adapters.sql`

 * *Files 4% similar despite different names*

```diff
@@ -101,11 +101,16 @@
 {% macro clickhouse__alter_column_type(relation, column_name, new_column_type) -%}
   {% call statement('alter_column_type') %}
     alter table {{ relation }} {{ on_cluster_clause()}} modify column {{ adapter.quote(column_name) }} {{ new_column_type }}
   {% endcall %}
 {% endmacro %}
 
 {% macro exchange_tables_atomic(old_relation, target_relation, obj_types='TABLES') %}
+
+  {%- if adapter.get_clickhouse_cluster_name() is not none and obj_types == 'TABLES' %}
+    {% do run_query("SYSTEM SYNC REPLICA "+ target_relation.identifier + on_cluster_clause()) %}
+  {%- endif %}
+  
   {%- call statement('exchange_tables_atomic') -%}
     EXCHANGE {{ obj_types }} {{ old_relation }} AND {{ target_relation }} {{ on_cluster_clause()}}
   {% endcall %}
 {% endmacro %}
```

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/incremental.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/incremental.sql`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,16 @@
 
     {% do adapter.drop_relation(new_data_relation) %}
 
 {% endmacro %}
 
 
 {% macro clickhouse__incremental_delete_insert(existing_relation, unique_key, incremental_predicates) %}
-    {% set new_data_relation = existing_relation.incorporate(path={"identifier": model['name'] + '__dbt_new_data'}) %}
+    {% set new_data_relation = existing_relation.incorporate(path={"identifier": model['name']
+       + '__dbt_new_data_' + invocation_id.replace('-', '_')}) %}
     {{ drop_relation_if_exists(new_data_relation) }}
     {% call statement('main') %}
         {{ get_create_table_as_sql(False, new_data_relation, sql) }}
     {% endcall %}
     {% call statement('delete_existing_data') %}
       delete from {{ existing_relation }} where ({{ unique_key }}) in (select {{ unique_key }}
                                           from {{ new_data_relation }})
```

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/s3.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/s3.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/seed.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/seed.sql`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {% endmacro %}
 
 {% macro clickhouse__create_csv_table(model, agate_table) %}
   {%- set column_override = model['config'].get('column_types', {}) -%}
   {%- set quote_seed_column = model['config'].get('quote_columns', None) -%}
 
   {% set sql %}
-    create table {{ this.render() }} (
+    create table {{ this.render() }} {{ on_cluster_clause() }} (
       {%- for col_name in agate_table.column_names -%}
         {%- set inferred_type = adapter.convert_type(agate_table, loop.index0) -%}
         {%- set type = column_override.get(col_name, inferred_type) -%}
         {%- set column_name = (col_name | string) -%}
           {{ adapter.quote_seed_column(column_name, quote_seed_column) }} {{ type }} {%- if not loop.last -%}, {%- endif -%}
       {%- endfor -%}
     )
```

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/snapshot.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/table.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/materializations/view.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/persist_docs.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/persist_docs.sql`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,54 @@
+{% macro one_alter_relation(relation, alter_comments) %}
+  alter table {{ relation }} {{ on_cluster_clause() }} {{ alter_comments }}
+{% endmacro %}
+
 {% macro one_alter_column_comment(relation, column_name, comment) %}
-  alter table {{ relation }} comment column {{ column_name }} '{{ comment }}'
+  alter table {{ relation }} {{ on_cluster_clause() }} comment column {{ column_name }} '{{ comment }}'
 {% endmacro %}
 
 {% macro clickhouse__alter_relation_comment(relation, comment) %}
-  alter table {{ relation }} modify comment '{{ comment }}'
+  alter table {{ relation }} {{ on_cluster_clause() }} modify comment '{{ comment }}'
 {% endmacro %}
 
 {% macro clickhouse__persist_docs(relation, model, for_relation, for_columns) %}
+  {%- set alter_comments = [] %}
+
   {%- if for_relation and config.persist_relation_docs() and model.description -%}
-    {% do run_query(alter_relation_comment(relation, model.description)) %}
+    {% set escaped_comment = clickhouse_escape_comment(model.description) %}
+    {% do alter_comments.append("modify comment {comment}".format(comment=escaped_comment)) %}
   {%- endif -%}
 
   {%- if for_columns and config.persist_column_docs() and model.columns -%}
-    {%- for column_name in model.columns -%}
+    {% set existing_columns = adapter.get_columns_in_relation(relation) | map(attribute="name") | list %}
+    {% for column_name in model.columns if (column_name in existing_columns) %}
       {%- set comment = model.columns[column_name]['description'] -%}
-      {% do run_query(one_alter_column_comment(relation, column_name, comment)) %}
+      {%- if comment %}
+        {% set escaped_comment = clickhouse_escape_comment(comment) %}
+        {% do alter_comments.append("comment column {column_name} {comment}".format(column_name=column_name, comment=escaped_comment)) %}
+      {%- endif %}
     {%- endfor -%}
   {%- endif -%}
-{% endmacro %}
+
+  {%- if alter_comments | length > 0 -%}
+    {% do run_query(one_alter_relation(relation, alter_comments|join(', '))) %}
+  {%- endif -%}
+{% endmacro %}
+
+{#
+  By using dollar-quoting like this, users can embed anything they want into their comments
+  (including nested dollar-quoting), as long as they do not use this exact dollar-quoting
+  label. It would be nice to just pick a new one but eventually you do have to give up.
+#}
+{% macro clickhouse_escape_comment(comment) -%}
+  {% if adapter.is_before_version('21.9.2.17') %}
+    {% do exceptions.raise_compiler_error('Unsupported ClickHouse version for using heredoc syntax') %}
+  {% endif %}
+  {% if comment is not string %}
+    {% do exceptions.raise_compiler_error('cannot escape a non-string: ' ~ comment) %}
+  {% endif %}
+  {%- set magic = '$dbt_comment_literal_block$' -%}
+  {%- if magic in comment -%}
+    {%- do exceptions.raise_compiler_error('The string ' ~ magic ~ ' is not allowed in comments.') -%}
+  {%- endif -%}
+  {{ magic }}{{ comment }}{{ magic }}
+{%- endmacro %}
```

### Comparing `dbt-clickhouse-1.4.0/dbt/include/clickhouse/macros/utils/utils.sql` & `dbt-clickhouse-1.4.1/dbt/include/clickhouse/macros/utils/utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/PKG-INFO` & `dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.4.0
+Version: 1.4.1
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,15 @@
 </p>
 
 # dbt-clickhouse
 
 This plugin ports [dbt](https://getdbt.com) functionality to [Clickhouse](https://clickhouse.tech/).
 
 The plugin uses syntax that requires ClickHouse version 22.1 or newer. We do not test older versions of Clickhouse.  We also do not currently test
-Replicated tables/`ON CLUSTER` functionality.
+Replicated tables or the related `ON CLUSTER` functionality.
 
 ## Installation
 
 Use your favorite Python package manager to install the app from PyPI, e.g.
 
 ```bash
 pip install dbt-clickhouse
@@ -47,15 +47,15 @@
 - [x] Incremental materialization
 - [x] Seeds
 - [x] Sources
 - [x] Docs generate
 - [x] Tests
 - [x] Snapshots
 - [x] Most dbt-utils macros (now included in dbt-core)  
-- [x] Ephemeral materialization (but incompatible with table materializations)
+- [x] Ephemeral materialization
 
 # Usage Notes
 
 ## Database
 
 The dbt model relation identifier `database.schema.table` is not compatible with Clickhouse because Clickhouse does not support a `schema`.
 So we use a simplified approach `schema.table`, where `schema` is the Clickhouse database. Using the `default` database is not recommended.
@@ -107,16 +107,16 @@
 | unique_key             | A tuple of column names that uniquely identify rows.  Used with incremental models for updates.                                                                                                                                                        | Optional                          |
 | inserts_only           | If set to True for an incremental model, incremental updates will be inserted directly to the target table without creating intermediate table. It has been deprecated in favor of the `append` incremental `strategy`, which operates in the same way | Optional                          |
 | incremental_strategy   | Incremental model update strategy of `delete+insert` or `append`.  See the following Incremental Model Strategies                                                                                                                                      | Optional (default: `default`)     |
 | incremental_predicates | Additional conditions to be applied to the incremental materialization (only applied to `delete+insert` strategy                                                                                                                                       |
 ## Known Limitations
 
 * Replicated tables (combined with the `cluster` profile setting) are available using the `on_cluster_clause` macro but are not included in the test suite and not formally tested. 
-* Ephemeral models/CTEs don't work with INSERT statements in ClickHouse, so table materializations that incorporate an ephemeral model will fail.
-See https://github.com/ClickHouse/ClickHouse/issues/30323.  View models and other SQL statements using ephemeral models should work correctly.
+* Ephemeral models/CTEs don't work if placed before the "INSERT INTO" in a ClickHouse insert statement, see https://github.com/ClickHouse/ClickHouse/issues/30323.  This
+should not affect most models, but care should be taken where an ephemeral model is placed in model definitions and other SQL statements.
 
 ## Incremental Model Strategies
 
 As of version 1.3.2, dbt-clickhouse supports three incremental model strategies.
 
 ### The Default (Legacy) Strategy
```

### Comparing `dbt-clickhouse-1.4.0/dbt_clickhouse.egg-info/SOURCES.txt` & `dbt-clickhouse-1.4.1/dbt_clickhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.0/setup.py` & `dbt-clickhouse-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             'include/clickhouse/dbt_project.yml',
             'include/clickhouse/macros/*.sql',
             'include/clickhouse/macros/**/*.sql',
         ]
     },
     install_requires=[
         f'dbt-core~={dbt_version}',
-        'clickhouse-connect>=0.5.5',
+        'clickhouse-connect>=0.5.24',
         'clickhouse-driver>=0.2.3',
     ],
     python_requires=">=3.7",
     platforms='any',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
```


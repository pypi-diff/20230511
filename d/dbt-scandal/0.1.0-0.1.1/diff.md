# Comparing `tmp/dbt_scandal-0.1.0.tar.gz` & `tmp/dbt_scandal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_scandal-0.1.0.tar", max compression
+gzip compressed data, was "dbt_scandal-0.1.1.tar", max compression
```

## Comparing `dbt_scandal-0.1.0.tar` & `dbt_scandal-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,16 @@
--rw-r--r--   0        0        0        0 2023-04-20 11:14:29.608650 dbt_scandal-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 11:15:17.117219 dbt_scandal-0.1.0/dbt/__init__.py
--rw-r--r--   0        0        0      302 2023-05-08 14:26:00.024817 dbt_scandal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 dbt_scandal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/README.md
+-rw-r--r--   0        0        0       76 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/adapters/scandal/__init__.py
+-rw-r--r--   0        0        0       18 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/adapters/scandal/__version__.py
+-rw-r--r--   0        0        0     7330 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/adapters/scandal/connections.py
+-rw-r--r--   0        0        0    11845 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/adapters/scandal/impl.py
+-rw-r--r--   0        0        0       92 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/scandal/__init__.py
+-rw-r--r--   0        0        0       76 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/scandal/dbt_project.yml
+-rw-r--r--   0        0        0      860 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/scandal/macros/materializations/seeds/create_csv_table.sql
+-rw-r--r--   0        0        0     1060 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/scandal/macros/materializations/seeds/load_csv_rows.sql
+-rw-r--r--   0        0        0      424 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/scandal/macros/materializations/seeds/reset_csv_table.sql
+-rw-r--r--   0        0        0      357 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/dbt/include/scandal/profile_template.yml
+-rw-r--r--   0        0        0     1414 2023-05-11 11:49:30.006322 dbt_scandal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 dbt_scandal-0.1.1/PKG-INFO
```


# Comparing `tmp/sqlalchemy_hawq-1.0.1.tar.gz` & `tmp/sqlalchemy_hawq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlalchemy_hawq-1.0.1.tar", last modified: Mon Oct  7 23:56:59 2019, max compression
+gzip compressed data, was "sqlalchemy_hawq-1.0.3.tar", last modified: Wed May 10 22:42:17 2023, max compression
```

## Comparing `sqlalchemy_hawq-1.0.1.tar` & `sqlalchemy_hawq-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 creisle   (1365) users      (100)        0 2019-10-07 23:56:59.000000 sqlalchemy_hawq-1.0.1/
--rw-rw-r--   0 creisle   (1365) users      (100)       55 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/MANIFEST.in
--rw-rw-r--   0 creisle   (1365) users      (100)    18796 2019-10-07 23:56:59.000000 sqlalchemy_hawq-1.0.1/PKG-INFO
--rw-rw-r--   0 creisle   (1365) users      (100)    15785 2019-10-07 23:56:39.000000 sqlalchemy_hawq-1.0.1/README.md
--rw-rw-r--   0 creisle   (1365) users      (100)      266 2019-10-07 23:56:59.000000 sqlalchemy_hawq-1.0.1/setup.cfg
--rw-rw-r--   0 creisle   (1365) users      (100)     1684 2019-10-07 23:55:31.000000 sqlalchemy_hawq-1.0.1/setup.py
-drwxrwxr-x   0 creisle   (1365) users      (100)        0 2019-10-07 23:56:59.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/
--rw-rw-r--   0 creisle   (1365) users      (100)      350 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/__init__.py
--rw-rw-r--   0 creisle   (1365) users      (100)     4820 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/ddl.py
--rw-rw-r--   0 creisle   (1365) users      (100)     1816 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/dialect.py
--rw-rw-r--   0 creisle   (1365) users      (100)     9306 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/partition.py
--rw-rw-r--   0 creisle   (1365) users      (100)     1939 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/point.py
-drwxrwxr-x   0 creisle   (1365) users      (100)        0 2019-10-07 23:56:59.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/
--rw-rw-r--   0 creisle   (1365) users      (100)    18796 2019-10-07 23:56:58.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/PKG-INFO
--rw-rw-r--   0 creisle   (1365) users      (100)      552 2019-10-07 23:56:58.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/SOURCES.txt
--rw-rw-r--   0 creisle   (1365) users      (100)        1 2019-10-07 23:56:58.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/dependency_links.txt
--rw-rw-r--   0 creisle   (1365) users      (100)      118 2019-10-07 23:56:58.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/entry_points.txt
--rw-rw-r--   0 creisle   (1365) users      (100)      211 2019-10-07 23:56:58.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/requires.txt
--rw-rw-r--   0 creisle   (1365) users      (100)       21 2019-10-07 23:56:58.000000 sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/top_level.txt
-drwxrwxr-x   0 creisle   (1365) users      (100)        0 2019-10-07 23:56:59.000000 sqlalchemy_hawq-1.0.1/test/
--rw-rw-r--   0 creisle   (1365) users      (100)        0 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/__init__.py
--rw-rw-r--   0 creisle   (1365) users      (100)     3743 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/conftest.py
--rw-rw-r--   0 creisle   (1365) users      (100)     2324 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/requirements.py
--rw-rw-r--   0 creisle   (1365) users      (100)    15651 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/test_create_all.py
--rw-rw-r--   0 creisle   (1365) users      (100)     3351 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/test_ddl.py
--rw-rw-r--   0 creisle   (1365) users      (100)     4983 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/test_live_connection.py
--rw-rw-r--   0 creisle   (1365) users      (100)     1952 2019-10-07 17:43:57.000000 sqlalchemy_hawq-1.0.1/test/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:42:17.378947 sqlalchemy_hawq-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-10 22:42:17.378947 sqlalchemy_hawq-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-10 22:42:17.378947 sqlalchemy_hawq-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:42:17.374947 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:42:17.374947 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-10 22:42:17.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-10 22:42:17.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-10 22:42:17.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 22:42:17.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 22:42:17.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 22:42:17.000000 sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:42:17.378947 sqlalchemy_hawq-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/test_create_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/test_ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/test_live_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-10 22:42:04.000000 sqlalchemy_hawq-1.0.3/test/test_suite.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sqlalchemy_hawq-1.0.1/PKG-INFO` & `sqlalchemy_hawq-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,436 +1,403 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_hawq
-Version: 1.0.1
+Version: 1.0.3
 Summary: UNKNOWN
-Home-page: https://github.com/bcgsc/sqlalchemy_hawq
-Author-email: creisle@bcgsc.ca
+Home-page: UNKNOWN
+Author-email: dat@bcgsc.ca
+Maintainer: vardb
+Maintainer-email: dat@bcgsc.ca
 License: UNKNOWN
-Description: 
-        Sqlalchemy Hawq
-        ===============
+Description: # Sqlalchemy Hawq
         
+        ![build](https://github.com/bcgsc/sqlalchemy_hawq/workflows/build/badge.svg) [![PyPi](https://img.shields.io/pypi/v/sqlalchemy_hawq.svg)](https://pypi.org/project/sqlalchemy-hawq) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apache-airflow.svg)](https://pypi.org/project/apache-airflow/)
         
-        .. image:: https://travis-ci.org/bcgsc/sqlalchemy_hawq.svg?branch=master
-           :target: https://travis-ci.org/bcgsc/sqlalchemy_hawq
-           :alt: Build Status
+        - [Getting Started](#getting-started)
+          - [Install (For developers)](#install-for-developers)
+          - [Run Tests](#run-tests)
+          - [Deploy (For developers)](#deploy-for-developers)
+        - [Using in a SQLAlchemy project](#using-in-a-sqlalchemy-project)
+          - [How to incorporate sqlalchemy-hawq](#how-to-incorporate-sqlalchemy-hawq)
+          - [Hawq-specific table arguments](#hawq-specific-table-arguments)
+          - [Example of hawq table arguments with declarative syntax](#example-of-hawq-table-arguments-with-declarative-syntax)
+        - [Using partitions](#using-partitions)
         
-        
-        
-        * `Getting Started <#getting-started>`_
-        
-          * `Install (For developers) <#install-for-developers>`_
-          * `Run Tests <#run-tests>`_
-          * `Deploy (For developers) <#deploy-for-developers>`_
-        
-        * `Using in a SQLAlchemy project <#using-in-a-sqlalchemy-project>`_
-        
-          * `How to incorporate sqlalchemy-hawq <#how-to-incorporate-sqlalchemy-hawq>`_
-          * `Hawq-specific table arguments <#hawq-specific-table-arguments>`_
-          * `Example of hawq table arguments with declarative syntax <#example-of-hawq-table-arguments-with-declarative-syntax>`_
-        
-        * `Using partitions <#using-partitions>`_
-        
-        This is a custom dialect for using SQLAlchemy with a `HAWQ <http://hawq.apache.org/docs/userguide/2.3.0.0-incubating/tutorial/overview.html>`_
+        This is a custom dialect for using SQLAlchemy with a [HAWQ](http://hawq.apache.org/docs/userguide/2.3.0.0-incubating/tutorial/overview.html)
         database.
         
         It extends the Postgresql dialect.
         
         Features include:
+        - Hawq options for 'CREATE TABLE' statements
+        - a point class
+        - a modified 'DELETE' statement for compatibility with SQLAlchemy's test suite
         
+        Unless specifically overridden, any functionality in SQLAlchemy's Postgresql dialect is also available. Note that in general, functionality that is available in Postgresql but not in Hawq has not yet been disabled.
         
-        * Hawq options for 'CREATE TABLE' statements
-        * a point class
-        * a modified 'DELETE' statement for compatibility with SQLAlchemy's test suite
         
-        Unless specifically overridden, any functionality in SQLAlchemy's Postgresql dialect is also available. Note that in general, functionality that is available in Postgresql but not in Hawq has not yet been disabled.
+        ## Getting Started
         
-        Getting Started
-        ---------------
+        ### Install (For developers)
         
-        Install (For developers)
-        ^^^^^^^^^^^^^^^^^^^^^^^^
         
         clone this repository
         
-        .. code::
-        
-           git clone https://creisle@svn.bcgsc.ca/bitbucket/scm/dat/sqlalchemy_hawq.git
-           cd sqlalchemy_hawq
+        ```bash
+        git clone https://creisle@svn.bcgsc.ca/bitbucket/scm/dat/sqlalchemy_hawq.git
+        cd sqlalchemy_hawq
+        ```
         
         create a virtual environment
         
-        .. code::
-        
-           python3 -m venv venv
-           source venv/bin/activate
+        ```bash
+        python3 -m venv venv
+        source venv/bin/activate
+        ```
         
         install the package and its development dependencies
         
-        .. code::
+        ```bash
+        pip install -e .[dev]
+        ```
         
-           pip install -e .[dev]
-        
-        Run Tests
-        ^^^^^^^^^
+        ### Run Tests
         
         sqlalchemy_hawq incorporates the standard SQLAlchemy test suite as well as some tests of its own. Run them all as follows:
         
-        .. code::
-        
-           pytest test --hawq://username:password@hostname:port/database
+        ```bash
+        export HAWQ_DB_HOST=<host>
+        export HAWQ_DB_PORT=<port>
+        export HAWQ_DB_NAME=<test db>
+        export HAWQ_DB_DRIVER=hawq
+        export HAWQ_DB_USER=<your username>
+        export HAWQ_DB_PASS=<your password>
+        pytest test
+        ```
         
         Run only the standard SQLAlchemy test suite:
         
-        .. code::
-        
-           pytest test --hawq://username:password@hostname:port/database --sqla-only
+        ```bash
+        pytest test --hawq://username:password@hostname:port/database --sqla-only
+        ```
         
         Run only the custom sqlalchemy_hawq tests:
         
-        .. code::
-        
-           pytest test --hawq://username:password@hostname:port/database --custom-only
-        
-        Run only the custom tests that don't require a live db connection - e.g., for ci:
-        
-        .. code::
-        
-           pytest test --offline-only
+        ```bash
+        pytest test --hawq://username:password@hostname:port/database --custom-only
+        ```
+        
+        Run only the custom tests that don't require a live db connection:
+        
+        ```bash
+        pytest test --offline-only --disable-asyncio
+        ```
         
         For tests that use a live db connection, user running the tests must be able to create and drop tables on the db provided. Also, many of the tests require that there are pre-existing schemas 'test_schema' and 'test_schema_2' on the db. The test suite can be run without them but the tests will fail.
         
         See https://github.com/zzzeek/sqlalchemy/blob/master/README.unittests.rst and https://github.com/zzzeek/sqlalchemy/blob/master/README.dialects.rst for more information on test configuration. Note that no default db url is stored in sqlalchemy_hawq's setup.cfg.
         
-        Deploy (For developers)
-        ^^^^^^^^^^^^^^^^^^^^^^^
+        ### Deploy (For developers)
         
         Create the venv and ensure the latest versions of setuptools and pip are installed:
         
-        .. code::
-        
-           python3 -m venv venv
-           source venv/bin/activate
-           pip install -U setuptools pip
+        ```bash
+        python3 -m venv venv
+        source venv/bin/activate
+        pip install -U setuptools pip
+        ```
         
         Install sqlalchemy_hawq for deployment and create the distribution packages:
         
-        .. code::
-        
-           pip install .[deploy]
-           python setup.py install sdist bdist_wheel
+        ```bash
+        pip install .[deploy]
+        python3 setup.py sdist
+        ```
         
         If you want, you can now check for any problems in the distribution files:
         
-        .. code::
-        
-           twine check dist/*
+        ```bash
+        twine check dist/*
+        ```
         
         Then:
         
-        .. code::
+        ```bash
+        twine upload dist/* --repository-url http://pyshop.bcgsc.ca/simple/
+        ```
         
-           twine upload dist/* --repository-url http://pyshop.bcgsc.ca/simple/
+        ---
         
-        ----
+        ## Using in a SQLAlchemy project
         
-        Using in a SQLAlchemy project
-        -----------------------------
-        
-        How to incorporate sqlalchemy-hawq
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        ### How to incorporate sqlalchemy-hawq
         
         Add sqlalchemy_hawq to your dependencies and install.
         
-        .. code::
-        
-           pip install sqlalchemy_hawq
+        ```bash
+        pip install sqlalchemy_hawq
+        ```
         
         Then the plugin can be used like any other engine
         
-        .. code::
+        ```python
+        from sqlalchemy import create_engine
         
-           from sqlalchemy import create_engine
+        engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
+        ```
         
-           engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
+        For instructions on how to use the SQLAlchemy engine, see https://docs.sqlalchemy.org/en/20/core/engines.html.
         
-        For sqlalchemy's instructions on how to use their engine, see https://docs.sqlalchemy.org/en/13/core/engines.html.
         
-        Hawq-specific table arguments
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        ### Hawq-specific table arguments
         
         Hawq specific table arguments are also supported (Not all features are supported yet)
         
-        .. list-table::
-           :header-rows: 1
+        | Argument            | Type                            | Example                                                                                                                                            | Notes                                                               |
+        | ------------------- | ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
+        | hawq_distributed_by | str                             | `'column_name'`                                                                                                                                    |                                                                     |
+        | hawq_partition_by   | RangePartition or ListPartition | `ListPartition('chrom', {'chr1': '1', 'chr2':'2', 'chr3':'3'}, [RangeSubpartition('year', 2002, 2012, 1), RangeSubpartition('month', 1, 13, 1),])` | Does not currently support range partitioning on dates              |
+        | hawq_apppendonly    | bool                            | `True`                                                                                                                                             |                                                                     |
+        | hawq_orientation    | str                             | `'ROW'`                                                                                                                                            | expects one of `{'ROW', 'PARQUET'}`                                 |
+        | hawq_compresstype   | str                             | `'ZLIB'`                                                                                                                                           | expects one of `{'ZLIB', 'SNAPPY', 'GZIP', 'NONE'}`                 |
+        | hawq_compresslevel  | int                             | `0`                                                                                                                                                | expects an integer between 0-9                                      |
+        | hawq_bucketnum      | int                             | `6`                                                                                                                                                | expects an integer between 0 and `default_hash_table_bucket_number` |
+        
+        
+        ### Example of hawq table arguments with declarative syntax
+        
+        ```python
+        from sqlalchemy.ext.declarative import declarative_base
+        from sqlalchemy import Column, Text
+        
+        Base = declarative_base()
+        
+        class ExampleTable(Base):
+            __tablename__ = 'example_table'
+        
+            __table_args__ = {
+                'hawq_distributed_by': 'attr1'
+                'hawq_appendonly': 'True'
+            }
+        
+            attr1 = Column(Integer())
+            attr2 = Column(Integer())
+        
         
-           * - Argument
-             - Type
-             - Example
-             - Notes
-           * - hawq_distributed_by
-             - str
-             - ``'column_name'``
-             - 
-           * - hawq_partition_by
-             - RangePartition or ListPartition
-             - ``ListPartition('chrom', {'chr1': '1', 'chr2':'2', 'chr3':'3'}, [RangeSubpartition('year', 2002, 2012, 1), RangeSubpartition('month', 1, 13, 1),])``
-             - Does not currently support range partitioning on dates
-           * - hawq_apppendonly
-             - bool
-             - ``True``
-             - 
-           * - hawq_orientation
-             - str
-             - ``'ROW'``
-             - expects one of ``{'ROW', 'PARQUET'}``
-           * - hawq_compresstype
-             - str
-             - ``'ZLIB'``
-             - expects one of ``{'ZLIB', 'SNAPPY', 'GZIP', 'NONE'}``
-           * - hawq_compresslevel
-             - int
-             - ``0``
-             - expects an integer between 0-9
-           * - hawq_bucketnum
-             - int
-             - ``6``
-             - expects an integer between 0 and ``default_hash_table_bucket_number``
-        
-        
-        Example of hawq table arguments with declarative syntax
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        .. code::
-        
-           from sqlalchemy.ext.declarative import declarative_base
-           from sqlalchemy import Column, Text
-        
-           Base = declarative_base()
-        
-           class ExampleTable(Base):
-               __tablename__ = 'example_table'
-        
-               __table_args__ = {
-                   'hawq_distributed_by': 'attr1'
-                   'hawq_appendonly': 'True'
-               }
-        
-               attr1 = Column(Integer())
-               attr2 = Column(Integer())
-        
-        
-           def main():
-               engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
-               engine.create_all()
+        def main():
+            engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
+            engine.create_all()
+        ```
         
-        ----
+        ---
         
-        Using partitions
-        ----------------
+        ## Using partitions
         
         See https://hawq.apache.org/docs/userguide/2.3.0.0-incubating/ddl/ddl-partition.html for an extended discussion of how partitions work in Hawq.
         
         Basically, partitioning divides a table into several smaller tables on the value of one or more columns, in order to reduce search time on those columns. The parent table can then be queried/added to without any further reference to the partitions, as Hawq handles all the parent-partition interactions.
         
         Partition arguments are:
         
-        .. code::
-        
-           RangePartition(
-               column_name=str,
-               start=int,
-               end=int,
-               every=int,
-               subpartitions=[])
-        
+        ```python
+        RangePartition(
+            column_name=str,
+            start=int,
+            end=int,
+            every=int,
+            subpartitions=[])
+        ```
         or
         
-        .. code::
-        
-           ListPartition(
-               column_name=str,
-               columns=dict{name_of_partition:value_to_partition_on},
-               subpartitions=[])
+        ```python
+        ListPartition(
+            column_name=str,
+            columns=dict{name_of_partition:value_to_partition_on},
+            subpartitions=[])
+        ```
         
         where 'subpartitions' is an array of RangeSubpartitions and/or ListSubpartitions.
         
         Subpartition arguments are
         
-        .. code::
-        
-           RangeSubpartition(
-               column_name=str,
-               start=int,
-               end=int,
-               every=int)
-        
+        ```python
+        RangeSubpartition(
+            column_name=str,
+            start=int,
+            end=int,
+            every=int)
+        ```
         or
         
-        .. code::
-        
-           ListSubpartition(
-               column_name=str,
-               columns=dict{name_of_partition:value_to_partition_on})
+        ```python
+        ListSubpartition(
+            column_name=str,
+            columns=dict{name_of_partition:value_to_partition_on})
+        ```
         
         Note that the params are the same for the Subpartitions are for the Partitions, except that Subpartitions do not have a nested subpartition array.
         
         Partition level is determined by the order of the subpartitions in the subpartition array.
         
-        Using sqlalchemy-hawq syntax to define a partition:
         
-        .. code::
+        Using sqlalchemy-hawq syntax to define a partition:
         
-           class MockTable(base):
-               __tablename__ = 'MockTable'
-               __table_args__ = {
-                   'hawq_partition_by': RangePartition(
-                       'year',
-                       2009,
-                       2012,
-                       1,
-                       [
-                           RangeSubpartition(
-                               'quarter',
-                               1,
-                               5,
-                               1),
-                           ListSubpartition(
-                               'chrom',
-                               {
-                                   'chr1': '1',
-                                   'chr2': '2',
-                                   'chr3': '3'}),
-                       ],
-                   )
-               }
-               id = Column('id', Integer(), primary_key=True, autoincrement=False)
-               year = Column('year', Integer())
-               quarter = Column('quarter', Integer())
-               chrom = Column('chrom', Text())
+        ```python
+        class MockTable(base):
+            __tablename__ = 'MockTable'
+            __table_args__ = {
+                'hawq_partition_by': RangePartition(
+                    'year',
+                    2009,
+                    2012,
+                    1,
+                    [
+                        RangeSubpartition(
+                            'quarter',
+                            1,
+                            5,
+                            1),
+                        ListSubpartition(
+                            'chrom',
+                            {
+                                'chr1': '1',
+                                'chr2': '2',
+                                'chr3': '3'}),
+                    ],
+                )
+            }
+            id = Column('id', Integer(), primary_key=True, autoincrement=False)
+            year = Column('year', Integer())
+            quarter = Column('quarter', Integer())
+            chrom = Column('chrom', Text())
+        ```
         
         The SQL output:
         
-        .. code::
+        ```sql
+        '''CREATE TABLE "MockTable" (
+        	id INTEGER NOT NULL,
+        	year INTEGER,
+        	quarter INTEGER,
+        	chrom TEXT
+        )
+        PARTITION BY RANGE (year)
+            SUBPARTITION BY RANGE (quarter)
+            SUBPARTITION TEMPLATE
+            (
+                START (1) END (5) EVERY (1),
+                DEFAULT SUBPARTITION extra
+            )
+            SUBPARTITION BY LIST (chrom)
+            SUBPARTITION TEMPLATE
+            (
+                SUBPARTITION chr1 VALUES ('1'),
+                SUBPARTITION chr2 VALUES ('2'),
+                SUBPARTITION chr3 VALUES ('3'),
+                DEFAULT SUBPARTITION other
+            )
+        (
+            START (2009) END (2012) EVERY (2),
+            DEFAULT PARTITION extra
+        )'''
+        ```
         
-           '''CREATE TABLE "MockTable" (
-               id INTEGER NOT NULL,
-               year INTEGER,
-               quarter INTEGER,
-               chrom TEXT
-           )
-           PARTITION BY RANGE (year)
-               SUBPARTITION BY RANGE (quarter)
-               SUBPARTITION TEMPLATE
-               (
-                   START (1) END (5) EVERY (1),
-                   DEFAULT SUBPARTITION extra
-               )
-               SUBPARTITION BY LIST (chrom)
-               SUBPARTITION TEMPLATE
-               (
-                   SUBPARTITION chr1 VALUES ('1'),
-                   SUBPARTITION chr2 VALUES ('2'),
-                   SUBPARTITION chr3 VALUES ('3'),
-                   DEFAULT SUBPARTITION other
-               )
-           (
-               START (2009) END (2012) EVERY (2),
-               DEFAULT PARTITION extra
-           )'''
         
         The resulting tables:
         
-        .. code::
         
-           test_refactor=> \dt
-                                       List of relations
-            Schema |                     Name                      | Type  |  Owner
-           --------+-----------------------------------------------+-------+---------
-            public | MockTable                                     | table | elewis
-            public | MockTable_1_prt_2                             | table | elewis
-            public | MockTable_1_prt_2_2_prt_2                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_3                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_4                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_5                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra                 | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_other     | table | elewis
-            public | MockTable_1_prt_3                             | table | elewis
-            public | MockTable_1_prt_3_2_prt_2                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_3                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_4                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_5                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra                 | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra                         | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra             | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr1  | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr2  | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr3  | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_other | table | elewis
+        ```sql
+        test_refactor=> \dt
+                                    List of relations
+         Schema |                     Name                      | Type  |  Owner
+        --------+-----------------------------------------------+-------+---------
+         public | MockTable                                     | table | elewis
+         public | MockTable_1_prt_2                             | table | elewis
+         public | MockTable_1_prt_2_2_prt_2                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_3                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_4                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_5                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra                 | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_other     | table | elewis
+         public | MockTable_1_prt_3                             | table | elewis
+         public | MockTable_1_prt_3_2_prt_2                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_3                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_4                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_5                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra                 | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra                         | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra             | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr1  | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr2  | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr3  | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_other | table | elewis
+         ```
         
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
+Requires-Python: >=3.7.1
+Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: deploy
-Provides-Extra: dev
```

### Comparing `sqlalchemy_hawq-1.0.1/README.md` & `sqlalchemy_hawq-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Sqlalchemy Hawq
 
-[![Build Status](https://travis-ci.org/bcgsc/sqlalchemy_hawq.svg?branch=master)](https://travis-ci.org/bcgsc/sqlalchemy_hawq)
+![build](https://github.com/bcgsc/sqlalchemy_hawq/workflows/build/badge.svg) [![PyPi](https://img.shields.io/pypi/v/sqlalchemy_hawq.svg)](https://pypi.org/project/sqlalchemy-hawq) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apache-airflow.svg)](https://pypi.org/project/apache-airflow/)
 
 - [Getting Started](#getting-started)
   - [Install (For developers)](#install-for-developers)
   - [Run Tests](#run-tests)
   - [Deploy (For developers)](#deploy-for-developers)
 - [Using in a SQLAlchemy project](#using-in-a-sqlalchemy-project)
   - [How to incorporate sqlalchemy-hawq](#how-to-incorporate-sqlalchemy-hawq)
@@ -51,33 +51,39 @@
 ```
 
 ### Run Tests
 
 sqlalchemy_hawq incorporates the standard SQLAlchemy test suite as well as some tests of its own. Run them all as follows:
 
 ```bash
-pytest test --hawq://username:password@hostname:port/database
+export HAWQ_DB_HOST=<host>
+export HAWQ_DB_PORT=<port>
+export HAWQ_DB_NAME=<test db>
+export HAWQ_DB_DRIVER=hawq
+export HAWQ_DB_USER=<your username>
+export HAWQ_DB_PASS=<your password>
+pytest test
 ```
 
 Run only the standard SQLAlchemy test suite:
 
 ```bash
 pytest test --hawq://username:password@hostname:port/database --sqla-only
 ```
 
 Run only the custom sqlalchemy_hawq tests:
 
 ```bash
 pytest test --hawq://username:password@hostname:port/database --custom-only
 ```
 
-Run only the custom tests that don't require a live db connection - e.g., for ci:
+Run only the custom tests that don't require a live db connection:
 
 ```bash
-pytest test --offline-only
+pytest test --offline-only --disable-asyncio
 ```
 
 For tests that use a live db connection, user running the tests must be able to create and drop tables on the db provided. Also, many of the tests require that there are pre-existing schemas 'test_schema' and 'test_schema_2' on the db. The test suite can be run without them but the tests will fail.
 
 See https://github.com/zzzeek/sqlalchemy/blob/master/README.unittests.rst and https://github.com/zzzeek/sqlalchemy/blob/master/README.dialects.rst for more information on test configuration. Note that no default db url is stored in sqlalchemy_hawq's setup.cfg.
 
 ### Deploy (For developers)
@@ -90,15 +96,15 @@
 pip install -U setuptools pip
 ```
 
 Install sqlalchemy_hawq for deployment and create the distribution packages:
 
 ```bash
 pip install .[deploy]
-python setup.py install sdist bdist_wheel
+python3 setup.py sdist
 ```
 
 If you want, you can now check for any problems in the distribution files:
 
 ```bash
 twine check dist/*
 ```
@@ -125,15 +131,15 @@
 
 ```python
 from sqlalchemy import create_engine
 
 engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
 ```
 
-For sqlalchemy's instructions on how to use their engine, see https://docs.sqlalchemy.org/en/13/core/engines.html.
+For instructions on how to use the SQLAlchemy engine, see https://docs.sqlalchemy.org/en/20/core/engines.html.
 
 
 ### Hawq-specific table arguments
 
 Hawq specific table arguments are also supported (Not all features are supported yet)
 
 | Argument            | Type                            | Example                                                                                                                                            | Notes                                                               |
@@ -199,15 +205,14 @@
     subpartitions=[])
 ```
 
 where 'subpartitions' is an array of RangeSubpartitions and/or ListSubpartitions.
 
 Subpartition arguments are
 
-
 ```python
 RangeSubpartition(
     column_name=str,
     start=int,
     end=int,
     every=int)
 ```
```

### Comparing `sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/ddl.py` & `sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/partition.py` & `sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 import re
 import decimal
 
 
 class Partition:
-    """ Base class.
+    """Base class.
 
     Implements methods for checking partition name
     and assembling subpartition clauses.
 
     Args:
         column_name (str): The name of the column to partition on.
         subpartitions (array of subpartitions, optional): Any subpartitions to include
@@ -37,15 +37,17 @@
 
         Raises:
             ValueError if column to partition on is not found in the table.
 
         """
         column = table.columns.get(self.column_name)
         if column is None:
-            raise ValueError('Column ({}) to use for partitioning not found'.format(self.column_name))
+            raise ValueError(
+                'Column ({}) to use for partitioning not found'.format(self.column_name)
+            )
         return column
 
     def get_subpartition_statements(self, table):
         """Assembles the clauses generated by each subpartition into a list.
 
         Args:
             table(:obj:) the table to partition.
@@ -62,15 +64,15 @@
 
     def clause(self, table):
         """Base version of func that returns the assembled clause."""
         raise NotImplementedError('abstract method must be overridden')
 
 
 class ListPartition(Partition):
-    """ A class representing a list-style top-level partition.
+    """A class representing a list-style top-level partition.
 
     Initializes with values specific to list-style partitions and implements
     methods to return a list-style partition clause.
 
     Inherits from Partition.
 
     Attributes:
@@ -82,37 +84,39 @@
     #  mapping is a dict of str to value
     def __init__(self, column_name, mapping, subpartitions=[]):
         self.column_name = column_name
         self.mapping = mapping
         self.subpartitions = subpartitions
 
     def get_partition_statements(self, column, partition_level=''):
-        """ Assembles a partition clause.
+        """Assembles a partition clause.
 
         Args:
             column(Column): the column to partition on.
             partition_level(str, optional): either '' or 'SUB'. Prepended to
             'PARTITION' in strs.
 
         Returns:
             partition_statements(`list` of str): a list of str defining the partitions
             for this column.
 
         """
         partition_statements = []
         for name, value in self.mapping.items():
-            partition_statements.append("""    {}PARTITION {} VALUES ({}),""".format(
-                partition_level,
-                valid_partition_name(name),
-                format_partition_value(column.type, value)
-            ))
+            partition_statements.append(
+                """    {}PARTITION {} VALUES ({}),""".format(
+                    partition_level,
+                    valid_partition_name(name),
+                    format_partition_value(column.type, value),
+                )
+            )
         return partition_statements
 
     def clause(self, table):
-        """ Assembles the partition clause.
+        """Assembles the partition clause.
 
         Args:
             table: the table to partition.
 
         Returns:
             statement(str): the partition clause for this table.
 
@@ -121,51 +125,53 @@
         partition_statements = self.get_partition_statements(column)
         subpartition_statements = self.get_subpartition_statements(table)
 
         statement = """PARTITION BY LIST ({}){}
 (
 {}
     DEFAULT PARTITION other
-)""".format(self.column_name,
-            "\n".join(subpartition_statements),
-            "\n".join(partition_statements))
+)""".format(
+            self.column_name, "\n".join(subpartition_statements), "\n".join(partition_statements)
+        )
         return statement
 
 
 class ListSubpartition(ListPartition):
-    """ Overrides a parent method in order to provide a modified partition clause.
+    """Overrides a parent method in order to provide a modified partition clause.
 
-        Inherits from ListPartition.
+    Inherits from ListPartition.
 
     """
 
     def clause(self, table):
-        """ Returns a clause defining a list-type subpartition.
+        """Returns a clause defining a list-type subpartition.
 
         Args:
             table: the table being partitioned
 
         Returns:
             statement(str): the clause for this subpartition.
-         """
+        """
 
         column = self.partition_column(table)
         partition_statements = self.get_partition_statements(column, 'SUB')
 
         statement = """    SUBPARTITION BY LIST ({})
     SUBPARTITION TEMPLATE
     (
     {}
         DEFAULT SUBPARTITION other
-    )""".format(self.column_name, "\n    ".join(partition_statements))
+    )""".format(
+            self.column_name, "\n    ".join(partition_statements)
+        )
         return statement
 
 
 class RangePartition(Partition):
-    """ A class representing a range-style top-level partition.
+    """A class representing a range-style top-level partition.
 
     Initializes with values specific to range-style partitions and implements
     methods to return a range-style partition clause.
 
     Inherits from Partition.
 
     Attributes:
@@ -179,64 +185,64 @@
         self.column_name = column_name
         self.start = start
         self.end = end
         self.every = every
         self.subpartitions = subpartitions
 
     def clause(self, table):
-        """ Assembles the partition clause.
+        """Assembles the partition clause.
 
         Args:
             table: the table to partition.
 
         Returns:
             statement(str): the partition clause for this table.
 
-         """
+        """
 
         self.partition_column(table)  # raises an error if column_name is invalid
         subpartition_statements = self.get_subpartition_statements(table)
 
         statement = """PARTITION BY RANGE ({}){}
 (
     START ({}) END ({}) EVERY ({}),
     DEFAULT PARTITION extra
-)""".format(self.column_name,
-            "".join(subpartition_statements),
-            self.start,
-            self.end,
-            self.every)
+)""".format(
+            self.column_name, "".join(subpartition_statements), self.start, self.end, self.every
+        )
         return statement
 
 
 class RangeSubpartition(RangePartition):
-    """ Overrides a parent method in order to provide a modified partition clause.
+    """Overrides a parent method in order to provide a modified partition clause.
 
     Inherits from RangePartition.
 
     """
 
     def clause(self, table):
-        """ Returns a clause defining a range-type subpartition.
+        """Returns a clause defining a range-type subpartition.
 
         Args:
             table: the table being partitioned
 
         Returns:
             statement(str): the clause for this subpartition.
-         """
+        """
 
         self.partition_column(table)  # raises an error if column_name is invalid
 
         statement = """    SUBPARTITION BY RANGE ({})
     SUBPARTITION TEMPLATE
     (
         START ({}) END ({}) EVERY ({}),
         DEFAULT SUBPARTITION extra
-    )""".format(self.column_name, self.start, self.end, self.every)
+    )""".format(
+            self.column_name, self.start, self.end, self.every
+        )
         return statement
 
 
 def format_partition_value(type_, value):
     '''
     Cast an input value based on the SQL type. This is done so
     that we can use the repr function to insert the value into
@@ -261,17 +267,19 @@
         return '\'{}\''.format(value)
     if type_.python_type == bool:
         if str(value).lower() in ['t', 'true', '1']:
             return 'TRUE'
         if str(value).lower() in ['f', 'false', '0']:
             return 'FALSE'
         return 'FALSE'
-    raise NotImplementedError('unsupported type ({}) for the given value ({}) in hawq has not been implemented'.format(
-        type_.python_type, value
-    ))
+    raise NotImplementedError(
+        'unsupported type ({}) for the given value ({}) in hawq has not been implemented'.format(
+            type_.python_type, value
+        )
+    )
 
 
 def valid_partition_name(name):
     '''
     Checks that a partition name is word characters only (to avoid injection)
 
     Args:
```

### Comparing `sqlalchemy_hawq-1.0.1/sqlalchemy_hawq/point.py` & `sqlalchemy_hawq-1.0.3/sqlalchemy_hawq/point.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,45 +14,54 @@
 
 
 class Point(UserDefinedType):
     """
     Wrapper for a 2-element tuple.
     The Point type is available in HAWQ db and postgres DBAPI, but not in SQLAlchemy.
     """
+
     def get_col_spec(value):  # pylint: disable=no-self-argument
         """
         Returns type name.
         get_col_spec must be overridden when implementing a custom class.
         """
         return "POINT"
 
     def bind_processor(self, dialect):
         """
         Returns a method to convert the tuple input to a its SQL string.
         """
+
         def process(value):
             if value is None:
                 return None
             try:
                 val1, val2 = value
                 if val1 is None or val2 is None:
                     if val1 is not None or val2 is not None:
-                        raise SQLAlchemyHawqException('Both values must be non-null or no data will be saved for Point({})'.format(value))
+                        raise SQLAlchemyHawqException(
+                            'Both values must be non-null or no data will be saved for Point({})'.format(
+                                value
+                            )
+                        )
                     return None
                 return str(value)
             except (ValueError, TypeError):
                 raise SQLAlchemyHawqException('Unexpected input type for Point ({})'.format(value))
+
         return process
 
     def result_processor(self, dialect, coltype):
         """
         Transforms the SQL string into a Python tuple.
         Point((float x),(float y)) -> (float x, float y)
         """
+
         def process(value):
             if value is None:
                 return None
             match = re.match(r'^\((?P<x>\d+(\.\d+)?),(?P<y>\d+(\.\d+)?)\)$', value)
             if match:
                 return (float(match.group('x')), float(match.group('y')))
             raise SQLAlchemyHawqException('Failed to get Point value from SQL ({})'.format(value))
+
         return process
```

### Comparing `sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/PKG-INFO` & `sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,436 +1,403 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-hawq
-Version: 1.0.1
+Version: 1.0.3
 Summary: UNKNOWN
-Home-page: https://github.com/bcgsc/sqlalchemy_hawq
-Author-email: creisle@bcgsc.ca
+Home-page: UNKNOWN
+Author-email: dat@bcgsc.ca
+Maintainer: vardb
+Maintainer-email: dat@bcgsc.ca
 License: UNKNOWN
-Description: 
-        Sqlalchemy Hawq
-        ===============
+Description: # Sqlalchemy Hawq
         
+        ![build](https://github.com/bcgsc/sqlalchemy_hawq/workflows/build/badge.svg) [![PyPi](https://img.shields.io/pypi/v/sqlalchemy_hawq.svg)](https://pypi.org/project/sqlalchemy-hawq) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apache-airflow.svg)](https://pypi.org/project/apache-airflow/)
         
-        .. image:: https://travis-ci.org/bcgsc/sqlalchemy_hawq.svg?branch=master
-           :target: https://travis-ci.org/bcgsc/sqlalchemy_hawq
-           :alt: Build Status
+        - [Getting Started](#getting-started)
+          - [Install (For developers)](#install-for-developers)
+          - [Run Tests](#run-tests)
+          - [Deploy (For developers)](#deploy-for-developers)
+        - [Using in a SQLAlchemy project](#using-in-a-sqlalchemy-project)
+          - [How to incorporate sqlalchemy-hawq](#how-to-incorporate-sqlalchemy-hawq)
+          - [Hawq-specific table arguments](#hawq-specific-table-arguments)
+          - [Example of hawq table arguments with declarative syntax](#example-of-hawq-table-arguments-with-declarative-syntax)
+        - [Using partitions](#using-partitions)
         
-        
-        
-        * `Getting Started <#getting-started>`_
-        
-          * `Install (For developers) <#install-for-developers>`_
-          * `Run Tests <#run-tests>`_
-          * `Deploy (For developers) <#deploy-for-developers>`_
-        
-        * `Using in a SQLAlchemy project <#using-in-a-sqlalchemy-project>`_
-        
-          * `How to incorporate sqlalchemy-hawq <#how-to-incorporate-sqlalchemy-hawq>`_
-          * `Hawq-specific table arguments <#hawq-specific-table-arguments>`_
-          * `Example of hawq table arguments with declarative syntax <#example-of-hawq-table-arguments-with-declarative-syntax>`_
-        
-        * `Using partitions <#using-partitions>`_
-        
-        This is a custom dialect for using SQLAlchemy with a `HAWQ <http://hawq.apache.org/docs/userguide/2.3.0.0-incubating/tutorial/overview.html>`_
+        This is a custom dialect for using SQLAlchemy with a [HAWQ](http://hawq.apache.org/docs/userguide/2.3.0.0-incubating/tutorial/overview.html)
         database.
         
         It extends the Postgresql dialect.
         
         Features include:
+        - Hawq options for 'CREATE TABLE' statements
+        - a point class
+        - a modified 'DELETE' statement for compatibility with SQLAlchemy's test suite
         
+        Unless specifically overridden, any functionality in SQLAlchemy's Postgresql dialect is also available. Note that in general, functionality that is available in Postgresql but not in Hawq has not yet been disabled.
         
-        * Hawq options for 'CREATE TABLE' statements
-        * a point class
-        * a modified 'DELETE' statement for compatibility with SQLAlchemy's test suite
         
-        Unless specifically overridden, any functionality in SQLAlchemy's Postgresql dialect is also available. Note that in general, functionality that is available in Postgresql but not in Hawq has not yet been disabled.
+        ## Getting Started
         
-        Getting Started
-        ---------------
+        ### Install (For developers)
         
-        Install (For developers)
-        ^^^^^^^^^^^^^^^^^^^^^^^^
         
         clone this repository
         
-        .. code::
-        
-           git clone https://creisle@svn.bcgsc.ca/bitbucket/scm/dat/sqlalchemy_hawq.git
-           cd sqlalchemy_hawq
+        ```bash
+        git clone https://creisle@svn.bcgsc.ca/bitbucket/scm/dat/sqlalchemy_hawq.git
+        cd sqlalchemy_hawq
+        ```
         
         create a virtual environment
         
-        .. code::
-        
-           python3 -m venv venv
-           source venv/bin/activate
+        ```bash
+        python3 -m venv venv
+        source venv/bin/activate
+        ```
         
         install the package and its development dependencies
         
-        .. code::
+        ```bash
+        pip install -e .[dev]
+        ```
         
-           pip install -e .[dev]
-        
-        Run Tests
-        ^^^^^^^^^
+        ### Run Tests
         
         sqlalchemy_hawq incorporates the standard SQLAlchemy test suite as well as some tests of its own. Run them all as follows:
         
-        .. code::
-        
-           pytest test --hawq://username:password@hostname:port/database
+        ```bash
+        export HAWQ_DB_HOST=<host>
+        export HAWQ_DB_PORT=<port>
+        export HAWQ_DB_NAME=<test db>
+        export HAWQ_DB_DRIVER=hawq
+        export HAWQ_DB_USER=<your username>
+        export HAWQ_DB_PASS=<your password>
+        pytest test
+        ```
         
         Run only the standard SQLAlchemy test suite:
         
-        .. code::
-        
-           pytest test --hawq://username:password@hostname:port/database --sqla-only
+        ```bash
+        pytest test --hawq://username:password@hostname:port/database --sqla-only
+        ```
         
         Run only the custom sqlalchemy_hawq tests:
         
-        .. code::
-        
-           pytest test --hawq://username:password@hostname:port/database --custom-only
-        
-        Run only the custom tests that don't require a live db connection - e.g., for ci:
-        
-        .. code::
-        
-           pytest test --offline-only
+        ```bash
+        pytest test --hawq://username:password@hostname:port/database --custom-only
+        ```
+        
+        Run only the custom tests that don't require a live db connection:
+        
+        ```bash
+        pytest test --offline-only --disable-asyncio
+        ```
         
         For tests that use a live db connection, user running the tests must be able to create and drop tables on the db provided. Also, many of the tests require that there are pre-existing schemas 'test_schema' and 'test_schema_2' on the db. The test suite can be run without them but the tests will fail.
         
         See https://github.com/zzzeek/sqlalchemy/blob/master/README.unittests.rst and https://github.com/zzzeek/sqlalchemy/blob/master/README.dialects.rst for more information on test configuration. Note that no default db url is stored in sqlalchemy_hawq's setup.cfg.
         
-        Deploy (For developers)
-        ^^^^^^^^^^^^^^^^^^^^^^^
+        ### Deploy (For developers)
         
         Create the venv and ensure the latest versions of setuptools and pip are installed:
         
-        .. code::
-        
-           python3 -m venv venv
-           source venv/bin/activate
-           pip install -U setuptools pip
+        ```bash
+        python3 -m venv venv
+        source venv/bin/activate
+        pip install -U setuptools pip
+        ```
         
         Install sqlalchemy_hawq for deployment and create the distribution packages:
         
-        .. code::
-        
-           pip install .[deploy]
-           python setup.py install sdist bdist_wheel
+        ```bash
+        pip install .[deploy]
+        python3 setup.py sdist
+        ```
         
         If you want, you can now check for any problems in the distribution files:
         
-        .. code::
-        
-           twine check dist/*
+        ```bash
+        twine check dist/*
+        ```
         
         Then:
         
-        .. code::
+        ```bash
+        twine upload dist/* --repository-url http://pyshop.bcgsc.ca/simple/
+        ```
         
-           twine upload dist/* --repository-url http://pyshop.bcgsc.ca/simple/
+        ---
         
-        ----
+        ## Using in a SQLAlchemy project
         
-        Using in a SQLAlchemy project
-        -----------------------------
-        
-        How to incorporate sqlalchemy-hawq
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        ### How to incorporate sqlalchemy-hawq
         
         Add sqlalchemy_hawq to your dependencies and install.
         
-        .. code::
-        
-           pip install sqlalchemy_hawq
+        ```bash
+        pip install sqlalchemy_hawq
+        ```
         
         Then the plugin can be used like any other engine
         
-        .. code::
+        ```python
+        from sqlalchemy import create_engine
         
-           from sqlalchemy import create_engine
+        engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
+        ```
         
-           engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
+        For instructions on how to use the SQLAlchemy engine, see https://docs.sqlalchemy.org/en/20/core/engines.html.
         
-        For sqlalchemy's instructions on how to use their engine, see https://docs.sqlalchemy.org/en/13/core/engines.html.
         
-        Hawq-specific table arguments
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        ### Hawq-specific table arguments
         
         Hawq specific table arguments are also supported (Not all features are supported yet)
         
-        .. list-table::
-           :header-rows: 1
+        | Argument            | Type                            | Example                                                                                                                                            | Notes                                                               |
+        | ------------------- | ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
+        | hawq_distributed_by | str                             | `'column_name'`                                                                                                                                    |                                                                     |
+        | hawq_partition_by   | RangePartition or ListPartition | `ListPartition('chrom', {'chr1': '1', 'chr2':'2', 'chr3':'3'}, [RangeSubpartition('year', 2002, 2012, 1), RangeSubpartition('month', 1, 13, 1),])` | Does not currently support range partitioning on dates              |
+        | hawq_apppendonly    | bool                            | `True`                                                                                                                                             |                                                                     |
+        | hawq_orientation    | str                             | `'ROW'`                                                                                                                                            | expects one of `{'ROW', 'PARQUET'}`                                 |
+        | hawq_compresstype   | str                             | `'ZLIB'`                                                                                                                                           | expects one of `{'ZLIB', 'SNAPPY', 'GZIP', 'NONE'}`                 |
+        | hawq_compresslevel  | int                             | `0`                                                                                                                                                | expects an integer between 0-9                                      |
+        | hawq_bucketnum      | int                             | `6`                                                                                                                                                | expects an integer between 0 and `default_hash_table_bucket_number` |
+        
+        
+        ### Example of hawq table arguments with declarative syntax
+        
+        ```python
+        from sqlalchemy.ext.declarative import declarative_base
+        from sqlalchemy import Column, Text
+        
+        Base = declarative_base()
+        
+        class ExampleTable(Base):
+            __tablename__ = 'example_table'
+        
+            __table_args__ = {
+                'hawq_distributed_by': 'attr1'
+                'hawq_appendonly': 'True'
+            }
+        
+            attr1 = Column(Integer())
+            attr2 = Column(Integer())
+        
         
-           * - Argument
-             - Type
-             - Example
-             - Notes
-           * - hawq_distributed_by
-             - str
-             - ``'column_name'``
-             - 
-           * - hawq_partition_by
-             - RangePartition or ListPartition
-             - ``ListPartition('chrom', {'chr1': '1', 'chr2':'2', 'chr3':'3'}, [RangeSubpartition('year', 2002, 2012, 1), RangeSubpartition('month', 1, 13, 1),])``
-             - Does not currently support range partitioning on dates
-           * - hawq_apppendonly
-             - bool
-             - ``True``
-             - 
-           * - hawq_orientation
-             - str
-             - ``'ROW'``
-             - expects one of ``{'ROW', 'PARQUET'}``
-           * - hawq_compresstype
-             - str
-             - ``'ZLIB'``
-             - expects one of ``{'ZLIB', 'SNAPPY', 'GZIP', 'NONE'}``
-           * - hawq_compresslevel
-             - int
-             - ``0``
-             - expects an integer between 0-9
-           * - hawq_bucketnum
-             - int
-             - ``6``
-             - expects an integer between 0 and ``default_hash_table_bucket_number``
-        
-        
-        Example of hawq table arguments with declarative syntax
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        .. code::
-        
-           from sqlalchemy.ext.declarative import declarative_base
-           from sqlalchemy import Column, Text
-        
-           Base = declarative_base()
-        
-           class ExampleTable(Base):
-               __tablename__ = 'example_table'
-        
-               __table_args__ = {
-                   'hawq_distributed_by': 'attr1'
-                   'hawq_appendonly': 'True'
-               }
-        
-               attr1 = Column(Integer())
-               attr2 = Column(Integer())
-        
-        
-           def main():
-               engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
-               engine.create_all()
+        def main():
+            engine = create_engine('hawq://USERNAME:PASSWORD@hdp-master02.hadoop.bcgsc.ca:5432/test_refactor/')
+            engine.create_all()
+        ```
         
-        ----
+        ---
         
-        Using partitions
-        ----------------
+        ## Using partitions
         
         See https://hawq.apache.org/docs/userguide/2.3.0.0-incubating/ddl/ddl-partition.html for an extended discussion of how partitions work in Hawq.
         
         Basically, partitioning divides a table into several smaller tables on the value of one or more columns, in order to reduce search time on those columns. The parent table can then be queried/added to without any further reference to the partitions, as Hawq handles all the parent-partition interactions.
         
         Partition arguments are:
         
-        .. code::
-        
-           RangePartition(
-               column_name=str,
-               start=int,
-               end=int,
-               every=int,
-               subpartitions=[])
-        
+        ```python
+        RangePartition(
+            column_name=str,
+            start=int,
+            end=int,
+            every=int,
+            subpartitions=[])
+        ```
         or
         
-        .. code::
-        
-           ListPartition(
-               column_name=str,
-               columns=dict{name_of_partition:value_to_partition_on},
-               subpartitions=[])
+        ```python
+        ListPartition(
+            column_name=str,
+            columns=dict{name_of_partition:value_to_partition_on},
+            subpartitions=[])
+        ```
         
         where 'subpartitions' is an array of RangeSubpartitions and/or ListSubpartitions.
         
         Subpartition arguments are
         
-        .. code::
-        
-           RangeSubpartition(
-               column_name=str,
-               start=int,
-               end=int,
-               every=int)
-        
+        ```python
+        RangeSubpartition(
+            column_name=str,
+            start=int,
+            end=int,
+            every=int)
+        ```
         or
         
-        .. code::
-        
-           ListSubpartition(
-               column_name=str,
-               columns=dict{name_of_partition:value_to_partition_on})
+        ```python
+        ListSubpartition(
+            column_name=str,
+            columns=dict{name_of_partition:value_to_partition_on})
+        ```
         
         Note that the params are the same for the Subpartitions are for the Partitions, except that Subpartitions do not have a nested subpartition array.
         
         Partition level is determined by the order of the subpartitions in the subpartition array.
         
-        Using sqlalchemy-hawq syntax to define a partition:
         
-        .. code::
+        Using sqlalchemy-hawq syntax to define a partition:
         
-           class MockTable(base):
-               __tablename__ = 'MockTable'
-               __table_args__ = {
-                   'hawq_partition_by': RangePartition(
-                       'year',
-                       2009,
-                       2012,
-                       1,
-                       [
-                           RangeSubpartition(
-                               'quarter',
-                               1,
-                               5,
-                               1),
-                           ListSubpartition(
-                               'chrom',
-                               {
-                                   'chr1': '1',
-                                   'chr2': '2',
-                                   'chr3': '3'}),
-                       ],
-                   )
-               }
-               id = Column('id', Integer(), primary_key=True, autoincrement=False)
-               year = Column('year', Integer())
-               quarter = Column('quarter', Integer())
-               chrom = Column('chrom', Text())
+        ```python
+        class MockTable(base):
+            __tablename__ = 'MockTable'
+            __table_args__ = {
+                'hawq_partition_by': RangePartition(
+                    'year',
+                    2009,
+                    2012,
+                    1,
+                    [
+                        RangeSubpartition(
+                            'quarter',
+                            1,
+                            5,
+                            1),
+                        ListSubpartition(
+                            'chrom',
+                            {
+                                'chr1': '1',
+                                'chr2': '2',
+                                'chr3': '3'}),
+                    ],
+                )
+            }
+            id = Column('id', Integer(), primary_key=True, autoincrement=False)
+            year = Column('year', Integer())
+            quarter = Column('quarter', Integer())
+            chrom = Column('chrom', Text())
+        ```
         
         The SQL output:
         
-        .. code::
+        ```sql
+        '''CREATE TABLE "MockTable" (
+        	id INTEGER NOT NULL,
+        	year INTEGER,
+        	quarter INTEGER,
+        	chrom TEXT
+        )
+        PARTITION BY RANGE (year)
+            SUBPARTITION BY RANGE (quarter)
+            SUBPARTITION TEMPLATE
+            (
+                START (1) END (5) EVERY (1),
+                DEFAULT SUBPARTITION extra
+            )
+            SUBPARTITION BY LIST (chrom)
+            SUBPARTITION TEMPLATE
+            (
+                SUBPARTITION chr1 VALUES ('1'),
+                SUBPARTITION chr2 VALUES ('2'),
+                SUBPARTITION chr3 VALUES ('3'),
+                DEFAULT SUBPARTITION other
+            )
+        (
+            START (2009) END (2012) EVERY (2),
+            DEFAULT PARTITION extra
+        )'''
+        ```
         
-           '''CREATE TABLE "MockTable" (
-               id INTEGER NOT NULL,
-               year INTEGER,
-               quarter INTEGER,
-               chrom TEXT
-           )
-           PARTITION BY RANGE (year)
-               SUBPARTITION BY RANGE (quarter)
-               SUBPARTITION TEMPLATE
-               (
-                   START (1) END (5) EVERY (1),
-                   DEFAULT SUBPARTITION extra
-               )
-               SUBPARTITION BY LIST (chrom)
-               SUBPARTITION TEMPLATE
-               (
-                   SUBPARTITION chr1 VALUES ('1'),
-                   SUBPARTITION chr2 VALUES ('2'),
-                   SUBPARTITION chr3 VALUES ('3'),
-                   DEFAULT SUBPARTITION other
-               )
-           (
-               START (2009) END (2012) EVERY (2),
-               DEFAULT PARTITION extra
-           )'''
         
         The resulting tables:
         
-        .. code::
         
-           test_refactor=> \dt
-                                       List of relations
-            Schema |                     Name                      | Type  |  Owner
-           --------+-----------------------------------------------+-------+---------
-            public | MockTable                                     | table | elewis
-            public | MockTable_1_prt_2                             | table | elewis
-            public | MockTable_1_prt_2_2_prt_2                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_2_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_3                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_3_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_4                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_4_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_5                     | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_2_2_prt_5_3_prt_other         | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra                 | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_2_2_prt_extra_3_prt_other     | table | elewis
-            public | MockTable_1_prt_3                             | table | elewis
-            public | MockTable_1_prt_3_2_prt_2                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_2_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_3                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_3_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_4                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_4_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_5                     | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_chr1          | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_chr2          | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_chr3          | table | elewis
-            public | MockTable_1_prt_3_2_prt_5_3_prt_other         | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra                 | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_3_2_prt_extra_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra                         | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_2_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_3_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_4_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5                 | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_chr1      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_chr2      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_chr3      | table | elewis
-            public | MockTable_1_prt_extra_2_prt_5_3_prt_other     | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra             | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr1  | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr2  | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr3  | table | elewis
-            public | MockTable_1_prt_extra_2_prt_extra_3_prt_other | table | elewis
+        ```sql
+        test_refactor=> \dt
+                                    List of relations
+         Schema |                     Name                      | Type  |  Owner
+        --------+-----------------------------------------------+-------+---------
+         public | MockTable                                     | table | elewis
+         public | MockTable_1_prt_2                             | table | elewis
+         public | MockTable_1_prt_2_2_prt_2                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_2_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_3                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_3_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_4                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_4_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_5                     | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_2_2_prt_5_3_prt_other         | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra                 | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_2_2_prt_extra_3_prt_other     | table | elewis
+         public | MockTable_1_prt_3                             | table | elewis
+         public | MockTable_1_prt_3_2_prt_2                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_2_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_3                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_3_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_4                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_4_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_5                     | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_chr1          | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_chr2          | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_chr3          | table | elewis
+         public | MockTable_1_prt_3_2_prt_5_3_prt_other         | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra                 | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_3_2_prt_extra_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra                         | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_2_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_3_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_4_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5                 | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_chr1      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_chr2      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_chr3      | table | elewis
+         public | MockTable_1_prt_extra_2_prt_5_3_prt_other     | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra             | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr1  | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr2  | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_chr3  | table | elewis
+         public | MockTable_1_prt_extra_2_prt_extra_3_prt_other | table | elewis
+         ```
         
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
+Requires-Python: >=3.7.1
+Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: deploy
-Provides-Extra: dev
```

### Comparing `sqlalchemy_hawq-1.0.1/sqlalchemy_hawq.egg-info/SOURCES.txt` & `sqlalchemy_hawq-1.0.3/sqlalchemy_hawq.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 sqlalchemy_hawq/__init__.py
 sqlalchemy_hawq/ddl.py
 sqlalchemy_hawq/dialect.py
 sqlalchemy_hawq/partition.py
 sqlalchemy_hawq/point.py
```

### Comparing `sqlalchemy_hawq-1.0.1/test/conftest.py` & `sqlalchemy_hawq-1.0.3/test/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 The entry point for the sqlalchemy test suite.
 
 Command line args are added and the test collector
 is modified to check them.
  """
 
-
+from sqlalchemy.engine.url import URL
 from sqlalchemy.dialects import registry
 from sqlalchemy.testing import config
 from sqlalchemy.testing.plugin import pytestplugin
 from sqlalchemy.testing.plugin import plugin_base
 from sqlalchemy.testing.plugin.pytestplugin import *
-from sqlalchemy.testing.plugin.pytestplugin import pytest, inspect
+from sqlalchemy.testing.plugin.pytestplugin import (
+    pytest,
+    inspect,
+)
+from sqlalchemy.testing import asyncio
 
+import os
 
+registry.register('hawq.psycopg2', 'sqlalchemy_hawq.dialect', 'HawqDialect')
 registry.register('hawq', 'sqlalchemy_hawq.dialect', 'HawqDialect')
-registry.register('hawq+psycopq2', 'sqlalchemy_hawq.dialect', 'HawqDialect')
 
 
 def pytest_addoption(parser):
     """
     Adds custom args, then calls the sqlalchemy pytest_addoption method to handle the rest
     """
     parser.addoption(
@@ -39,32 +44,76 @@
     )
     parser.addoption(
         "--offline-only",
         action="store_true",
         default=False,
         help="run only the tests that don't require a live connection",
     )
+    parser.addoption('--db-uri', default=os.environ.get('HAWQ_DB_URI'))
+    parser.addoption(
+        '--hawq-db-user',
+        help='The username for connecting to the hawq db',
+        default=os.environ.get('HAWQ_DB_USER'),
+    )
+    parser.addoption(
+        '--hawq-db-pass',
+        help='The password for connecting to the hawq db',
+        default=os.environ.get('HAWQ_DB_PASS'),
+    )
+    parser.addoption(
+        '--hawq-db-driver',
+        help='The password for connecting to the hawq db',
+        default=os.environ.get('HAWQ_DB_DRIVER'),
+    )
+    parser.addoption(
+        '--hawq-db-port',
+        help='The password for connecting to the hawq db',
+        default=os.environ.get('HAWQ_DB_PORT'),
+    )
+    parser.addoption(
+        '--hawq-db-host',
+        help='The password for connecting to the hawq db',
+        default=os.environ.get('HAWQ_DB_HOST'),
+    )
+    parser.addoption(
+        '--hawq-db-name',
+        help='The password for connecting to the hawq db',
+        default=os.environ.get('HAWQ_DB_NAME'),
+    )
+
     pytestplugin.pytest_addoption(parser)
 
 
 def pytest_sessionstart(session):
-
-    # skip setting up engine, but do everything else
     if plugin_base.options.offline_only:
+        plugin_base.post_configure = [
+            item for item in plugin_base.post_configure if item.__qualname__ != '_engine_uri'
+        ]
+        asyncio._assume_async(plugin_base.post_begin)
 
-        # Lazy setup of other options (post coverage)
-        for fn in plugin_base.post_configure:
+    else:
+        if not plugin_base.options.dburi:
+            urlArgs = dict(
+                host=plugin_base.options.hawq_db_host,
+                port=plugin_base.options.hawq_db_port,
+                drivername=plugin_base.options.hawq_db_driver,
+                database=plugin_base.options.hawq_db_name,
+                username=plugin_base.options.hawq_db_user,
+                password=plugin_base.options.hawq_db_pass,
+            )
+            dburl = URL.create(**urlArgs)
+            plugin_base.options.dburi = [dburl]
 
-            if fn.__qualname__ == '_engine_uri':
-                continue
+        asyncio._assume_async(plugin_base.post_begin)
 
-            fn(plugin_base.options, plugin_base.file_config)
 
-    else:
-        pytestplugin.pytest_sessionstart(session)
+def pytest_collection_modifyitems(session, config, items):
+    if plugin_base.options.offline_only:
+        return
+    pytestplugin.pytest_collection_modifyitems(session, config, items)
 
 
 def pytest_pycollect_makeitem(collector, name, obj):
     """
     Decides which tests not to run, then passes the rest of the work to
     the sqla method with the same name
     """
@@ -73,22 +122,21 @@
     # only run custom unit tests:
     if plugin_base.options.offline_only:
         if collector.name == 'test_suite.py':
             return []
         elif collector.name == 'test_live_connection.py':
             return []
         elif inspect.isclass(obj) and name.startswith('Test'):
-            return pytest.Class(name, parent=collector)
+            return pytest.Class.from_parent(collector, name=name)
         elif inspect.isfunction(obj) and name.startswith('test_'):
-            return pytest.Function(name, parent=collector)
+            return pytest.Function.from_parent(collector, name=name)
         else:
             return []
 
-    if inspect.isclass(obj) and plugin_base.want_class(obj):
-
+    if inspect.isclass(obj) and plugin_base.want_class(name, obj):
         # only run custom tests, not sqla_tests
         if config.options.custom_only:
             if collector.name == 'test_suite.py':
                 return []
 
         # only run custom unit tests
         if config.options.unit_only:
@@ -98,27 +146,26 @@
                 return []
 
         # only run the sqla test suite
         if config.options.sqla_only:
             if collector.name != 'test_suite.py':
                 return []
 
-        return pytestplugin.pytest_pycollect_makeitem(collector, name, obj)
     return pytestplugin.pytest_pycollect_makeitem(collector, name, obj)
 
 
 def pytest_runtest_setup(item):
     if plugin_base.options.offline_only:
         return
     pytestplugin.pytest_runtest_setup(item)
 
 
-def pytest_runtest_teardown(item):
+def pytest_runtest_teardown(item, nextitem):
     if plugin_base.options.offline_only:
         return
-    pytestplugin.pytest_runtest_teardown(item)
+    pytestplugin.pytest_runtest_teardown(item, nextitem)
 
 
 def pytest_sessionfinish(session):
     if plugin_base.options.offline_only:
         return
     plugin_base.final_process_cleanup()
```

### Comparing `sqlalchemy_hawq-1.0.1/test/test_create_all.py` & `sqlalchemy_hawq-1.0.3/test/test_create_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,14 @@
             __table_args__ = (UniqueConstraint('chrom'), {'hawq_orientation': 'bad value'})
             chrom = Column('chrom', Text(), primary_key=True)
 
         metadata = MockTable.__table__.metadata
         assert_raises(ValueError, metadata.create_all, engine_spy.engine)
 
     def test_compresstype(self, engine_spy=get_engine_spy()):
-
         for compresstype in {'ZLIB', 'SNAPPY', 'GZIP', 'NONE'}:
             Base = declarative_base()
 
             class MockTable(Base):
                 __tablename__ = 'MockTable'
                 __table_args__ = (UniqueConstraint('chrom'), {'hawq_compresstype': compresstype})
                 chrom = Column('chrom', Text(), primary_key=True)
@@ -353,15 +352,14 @@
             __table_args__ = (UniqueConstraint('chrom'), {'hawq_compresstype': 'tar'})
             chrom = Column('chrom', Text(), primary_key=True)
 
         metadata = MockTable.__table__.metadata
         assert_raises(ValueError, metadata.create_all, engine_spy.engine)
 
     def test_compresslevel(self, engine_spy=get_engine_spy()):
-
         for compresslevel in range(10):
             Base = declarative_base()
 
             class MockTable(Base):
                 __tablename__ = 'MockTable'
                 __table_args__ = (UniqueConstraint('chrom'), {'hawq_compresslevel': compresslevel})
                 chrom = Column('chrom', Text(), primary_key=True)
```

### Comparing `sqlalchemy_hawq-1.0.1/test/test_ddl.py` & `sqlalchemy_hawq-1.0.3/test/test_ddl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from sqlalchemy.dialects import postgresql
-from sqlalchemy.testing.suite import fixtures
+from sqlalchemy.testing import fixtures
 from sqlalchemy.testing import assert_raises
 
+import pytest
 
 from sqlalchemy_hawq.partition import format_partition_value
 from sqlalchemy_hawq.point import Point
 from sqlalchemy_hawq.point import SQLAlchemyHawqException
 
 
 class TestFormatPartitionValue(fixtures.TestBase):
@@ -29,15 +30,15 @@
         assert result == '1.1'
 
     def test_float(self):
         result = format_partition_value(postgresql.FLOAT(), '1.1')
         assert result == '1.1'
 
     def test_enum(self):
-        result = format_partition_value(postgresql.ENUM(), '1.1')
+        result = format_partition_value(postgresql.ENUM(name='test'), '1.1')
         assert result == '\'1.1\''
 
     def test_varchar(self):
         result = format_partition_value(postgresql.VARCHAR(), 'something')
         assert result == '\'something\''
 
     def test_text(self):
```

### Comparing `sqlalchemy_hawq-1.0.1/test/test_live_connection.py` & `sqlalchemy_hawq-1.0.3/test/test_live_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Defines tests that require a live db connection.
 """
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy import Column, Integer
 from sqlalchemy.exc import StatementError
 from sqlalchemy.testing.suite import fixtures
 from sqlalchemy.testing import assert_raises
 from sqlalchemy.orm import Session
 
 
 from sqlalchemy_hawq.point import Point
 
 
 class TestWithLiveConnection(fixtures.DeclarativeMappedTest):
-
     # ensures this test class is run when option --backend-only is specified
     __backend__ = True
+    run_create_tables = True
 
     @classmethod
     def setup_classes(cls):
         Base = cls.DeclarativeBasic
 
         class MockTable(fixtures.ComparableEntity, Base):
             __tablename__ = 'mocktable'
@@ -39,15 +39,15 @@
         that a table can be made and data entered and queried.
 
         This is also a test of disable-implicit-returning clause:
         if the 'returning' clause is attached, an exception will be
         thrown; if no sql is sent, the test will fail.
         """
         mocktable = self.classes.MockTable
-        session = Session()
+        session = Session(bind=self.bind)
         session.add(mocktable(test=5))
         session.commit()
         session.close()
 
         res = session.query(mocktable).all()
         session.close()
         expected = (res[0].test, len(res))
@@ -59,22 +59,22 @@
         Checks that the dialect is passing 'implicit_returning'=False
         to the engine, and no 'returning' clause is added to the sql.
         """
 
         MockTable = self.classes.MockTable
         ins = MockTable.__table__.insert().values(test=5).compile()
         expected = str(ins)
-        assert expected == 'INSERT INTO test_schema.mocktable (id, test) VALUES (%(id)s, %(test)s)'
+        assert expected == 'INSERT INTO test_schema.mocktable (test) VALUES (:test)'
 
     def test_point_type_insert_select(self):
         """
         Checks that point type data can be inserted and selected.
         """
         point_table = self.classes.PointTable
-        session = Session()
+        session = Session(bind=self.bind)
         session.add(point_table(id=1, ptest=(14, 201)))
         session.commit()
         session.close()
 
         res = session.query(point_table).filter_by(id=1)
         session.close()
 
@@ -82,15 +82,15 @@
         assert expected == res[0].ptest
 
     def test_point_type_insert_select_nonetype(self):
         """
         Checks that none-type point type data is inserted and retrieved correctly.
         """
         point_table = self.classes.PointTable
-        session = Session()
+        session = Session(bind=self.bind)
         session.add(point_table(id=2, ptest=None))
         session.commit()
         session.close()
 
         res = session.query(point_table).filter_by(id=2)
         session.close()
 
@@ -98,15 +98,15 @@
         assert expected == res[0].ptest
 
     def test_point_type_insert_select_none_in_tuple_type(self):
         """
         Checks that none-type point type data is inserted and retrieved correctly.
         """
         point_table = self.classes.PointTable
-        session = Session()
+        session = Session(bind=self.bind)
         session.add(point_table(id=3, ptest=(None, None)))
         session.commit()
         session.close()
 
         res = session.query(point_table).filter_by(id=3)
         session.close()
 
@@ -114,41 +114,43 @@
         assert expected == res[0].ptest
 
     def test_point_type_insert_select_mixed_type(self):
         """
         Checks that exception is raised when mixed none and non-none-type data is passed
         """
         point_table = self.classes.PointTable
-        session = Session()
+        session = Session(bind=self.bind)
 
         def func():
             """
             Ensure session is closed before exception is raised
             """
             try:
                 session.add(point_table(id=4, ptest=(1, None)))
                 session.commit()
                 session.close()
             except Exception as e:
                 session.close()
                 raise e
+
         assert_raises(StatementError, func)
 
     def test_point_type_insert_select_mixed_type_2(self):
         """
         Checks that exception is raised when mixed none and non-none-type data is passed
         """
         point_table = self.classes.PointTable
-        session = Session()
+        session = Session(bind=self.bind)
 
         def func():
             """
             Ensure session is closed before exception is raised
             """
             try:
                 session.add(point_table(id=5, ptest=(None, 1)))
                 session.commit()
                 session.close()
             except Exception as e:
                 session.close()
                 raise e
+
         assert_raises(StatementError, func)
```


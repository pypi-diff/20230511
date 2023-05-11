# Comparing `tmp/pynamodb-dax-0.0.5.tar.gz` & `tmp/pynamodb-dax-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb-dax-0.0.5.tar", last modified: Wed Feb  8 04:10:44 2023, max compression
+gzip compressed data, was "pynamodb-dax-0.0.6.tar", last modified: Thu May 11 19:23:53 2023, max compression
```

## Comparing `pynamodb-dax-0.0.5.tar` & `pynamodb-dax-0.0.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.158653 pynamodb-dax-0.0.5/
--rw-r--r--   0 nic        (501) staff       (20)     1080 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/LICENSE
--rw-r--r--   0 nic        (501) staff       (20)       60 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/MANIFEST.in
--rw-r--r--   0 nic        (501) staff       (20)     7110 2023-02-08 04:10:44.158743 pynamodb-dax-0.0.5/PKG-INFO
--rw-r--r--   0 nic        (501) staff       (20)     6318 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/README.rst
--rw-r--r--   0 nic        (501) staff       (20)      402 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/mypy.ini
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.148166 pynamodb-dax-0.0.5/pynamodb/
--rw-r--r--   0 nic        (501) staff       (20)      148 2023-02-08 04:10:37.000000 pynamodb-dax-0.0.5/pynamodb/__init__.py
--rw-r--r--   0 nic        (501) staff       (20)     1162 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/_schema.py
--rw-r--r--   0 nic        (501) staff       (20)     3350 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/_util.py
--rw-r--r--   0 nic        (501) staff       (20)    58474 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/attributes.py
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.150010 pynamodb-dax-0.0.5/pynamodb/connection/
--rw-r--r--   0 nic        (501) staff       (20)      201 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/connection/__init__.py
--rw-r--r--   0 nic        (501) staff       (20)     1377 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/connection/_botocore_private.py
--rw-r--r--   0 nic        (501) staff       (20)    61541 2023-02-08 03:13:21.000000 pynamodb-dax-0.0.5/pynamodb/connection/base.py
--rw-r--r--   0 nic        (501) staff       (20)     1009 2023-02-08 03:14:43.000000 pynamodb-dax-0.0.5/pynamodb/connection/dax.py
--rw-r--r--   0 nic        (501) staff       (20)    13242 2023-02-07 17:21:14.000000 pynamodb-dax-0.0.5/pynamodb/connection/table.py
--rw-r--r--   0 nic        (501) staff       (20)     6794 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/constants.py
--rw-r--r--   0 nic        (501) staff       (20)     7604 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/exceptions.py
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.151418 pynamodb-dax-0.0.5/pynamodb/expressions/
--rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/pynamodb/expressions/__init__.py
--rw-r--r--   0 nic        (501) staff       (20)     4393 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/expressions/condition.py
--rw-r--r--   0 nic        (501) staff       (20)    14015 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/expressions/operand.py
--rw-r--r--   0 nic        (501) staff       (20)      811 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/expressions/projection.py
--rw-r--r--   0 nic        (501) staff       (20)     4661 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/expressions/update.py
--rw-r--r--   0 nic        (501) staff       (20)     2476 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/expressions/util.py
--rw-r--r--   0 nic        (501) staff       (20)     8217 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/indexes.py
--rw-r--r--   0 nic        (501) staff       (20)    49662 2023-02-08 03:27:20.000000 pynamodb-dax-0.0.5/pynamodb/models.py
--rw-r--r--   0 nic        (501) staff       (20)     7603 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/pagination.py
--rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/pynamodb/py.typed
--rw-r--r--   0 nic        (501) staff       (20)     2569 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/settings.py
--rw-r--r--   0 nic        (501) staff       (20)     1517 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/pynamodb/signals.py
--rw-r--r--   0 nic        (501) staff       (20)     5334 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/pynamodb/transactions.py
--rw-r--r--   0 nic        (501) staff       (20)      101 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/pynamodb/types.py
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.152355 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/
--rw-r--r--   0 nic        (501) staff       (20)     7110 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/PKG-INFO
--rw-r--r--   0 nic        (501) staff       (20)     1751 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/SOURCES.txt
--rw-r--r--   0 nic        (501) staff       (20)        1 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/dependency_links.txt
--rw-r--r--   0 nic        (501) staff       (20)        1 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/not-zip-safe
--rw-r--r--   0 nic        (501) staff       (20)      148 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/requires.txt
--rw-r--r--   0 nic        (501) staff       (20)       28 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.5/pynamodb_dax.egg-info/top_level.txt
--rw-r--r--   0 nic        (501) staff       (20)      189 2023-02-08 03:29:27.000000 pynamodb-dax-0.0.5/requirements-dev.txt
--rw-r--r--   0 nic        (501) staff       (20)      100 2023-02-08 04:10:44.159074 pynamodb-dax-0.0.5/setup.cfg
--rw-r--r--   0 nic        (501) staff       (20)     1295 2023-02-08 04:09:34.000000 pynamodb-dax-0.0.5/setup.py
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.156361 pynamodb-dax-0.0.5/tests/
--rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/__init__.py
--rw-r--r--   0 nic        (501) staff       (20)    42087 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/data.py
--rw-r--r--   0 nic        (501) staff       (20)     5472 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/deep_eq.py
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.157796 pynamodb-dax-0.0.5/tests/integration/
--rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/integration/__init__.py
--rw-r--r--   0 nic        (501) staff       (20)     4826 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/integration/base_integration_test.py
--rw-r--r--   0 nic        (501) staff       (20)     1676 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/integration/binary_update_test.py
--rw-r--r--   0 nic        (501) staff       (20)      602 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/integration/conftest.py
--rw-r--r--   0 nic        (501) staff       (20)     4176 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/integration/model_integration_test.py
--rw-r--r--   0 nic        (501) staff       (20)     4608 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/integration/table_integration_test.py
--rw-r--r--   0 nic        (501) staff       (20)     4426 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/integration/test_discriminator_index.py
--rw-r--r--   0 nic        (501) staff       (20)    13872 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/integration/test_transaction_integration.py
--rw-r--r--   0 nic        (501) staff       (20)      552 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/response.py
--rw-r--r--   0 nic        (501) staff       (20)    50294 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_attributes.py
--rw-r--r--   0 nic        (501) staff       (20)    63577 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_base_connection.py
--rw-r--r--   0 nic        (501) staff       (20)      466 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_binary_legacy_encoding.py
--rw-r--r--   0 nic        (501) staff       (20)     6828 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_discriminator.py
--rw-r--r--   0 nic        (501) staff       (20)     1155 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_exceptions.py
--rw-r--r--   0 nic        (501) staff       (20)    30181 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_expressions.py
--rw-r--r--   0 nic        (501) staff       (20)   125584 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_model.py
--rw-r--r--   0 nic        (501) staff       (20)     2078 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/test_pagination.py
--rw-r--r--   0 nic        (501) staff       (20)      643 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/test_settings.py
--rw-r--r--   0 nic        (501) staff       (20)     3788 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.5/tests/test_signals.py
--rw-r--r--   0 nic        (501) staff       (20)    19859 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_table_connection.py
--rw-r--r--   0 nic        (501) staff       (20)     4551 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/tests/test_transaction.py
-drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-02-08 04:10:44.158477 pynamodb-dax-0.0.5/typing_tests/
--rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/typing_tests/__init__.py
--rw-r--r--   0 nic        (501) staff       (20)     2018 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/typing_tests/attributes.py
--rw-r--r--   0 nic        (501) staff       (20)     4903 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/typing_tests/models.py
--rw-r--r--   0 nic        (501) staff       (20)      874 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.5/typing_tests/transactions.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.693802 pynamodb-dax-0.0.6/
+-rw-r--r--   0 nic        (501) staff       (20)     1080 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/LICENSE
+-rw-r--r--   0 nic        (501) staff       (20)       60 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/MANIFEST.in
+-rw-r--r--   0 nic        (501) staff       (20)     7110 2023-05-11 19:23:53.693883 pynamodb-dax-0.0.6/PKG-INFO
+-rw-r--r--   0 nic        (501) staff       (20)     6318 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/README.rst
+-rw-r--r--   0 nic        (501) staff       (20)      402 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/mypy.ini
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.686759 pynamodb-dax-0.0.6/pynamodb/
+-rw-r--r--   0 nic        (501) staff       (20)      148 2023-05-11 19:22:19.000000 pynamodb-dax-0.0.6/pynamodb/__init__.py
+-rw-r--r--   0 nic        (501) staff       (20)     1162 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/_schema.py
+-rw-r--r--   0 nic        (501) staff       (20)     3350 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/_util.py
+-rw-r--r--   0 nic        (501) staff       (20)    58474 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/attributes.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.687469 pynamodb-dax-0.0.6/pynamodb/connection/
+-rw-r--r--   0 nic        (501) staff       (20)      201 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/connection/__init__.py
+-rw-r--r--   0 nic        (501) staff       (20)      877 2023-05-11 18:12:20.000000 pynamodb-dax-0.0.6/pynamodb/connection/_botocore_private.py
+-rw-r--r--   0 nic        (501) staff       (20)    60902 2023-05-11 19:02:43.000000 pynamodb-dax-0.0.6/pynamodb/connection/base.py
+-rw-r--r--   0 nic        (501) staff       (20)     1009 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/connection/dax.py
+-rw-r--r--   0 nic        (501) staff       (20)    13242 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/connection/table.py
+-rw-r--r--   0 nic        (501) staff       (20)     6794 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/constants.py
+-rw-r--r--   0 nic        (501) staff       (20)     7604 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/exceptions.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.688302 pynamodb-dax-0.0.6/pynamodb/expressions/
+-rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/pynamodb/expressions/__init__.py
+-rw-r--r--   0 nic        (501) staff       (20)     4393 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/expressions/condition.py
+-rw-r--r--   0 nic        (501) staff       (20)    14015 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/expressions/operand.py
+-rw-r--r--   0 nic        (501) staff       (20)      811 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/expressions/projection.py
+-rw-r--r--   0 nic        (501) staff       (20)     4661 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/expressions/update.py
+-rw-r--r--   0 nic        (501) staff       (20)     2476 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/expressions/util.py
+-rw-r--r--   0 nic        (501) staff       (20)     8217 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/indexes.py
+-rw-r--r--   0 nic        (501) staff       (20)    49662 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/models.py
+-rw-r--r--   0 nic        (501) staff       (20)     7603 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/pynamodb/pagination.py
+-rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/pynamodb/py.typed
+-rw-r--r--   0 nic        (501) staff       (20)     2569 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/settings.py
+-rw-r--r--   0 nic        (501) staff       (20)     1517 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/signals.py
+-rw-r--r--   0 nic        (501) staff       (20)     5334 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/pynamodb/transactions.py
+-rw-r--r--   0 nic        (501) staff       (20)      101 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/pynamodb/types.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.689166 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/
+-rw-r--r--   0 nic        (501) staff       (20)     7110 2023-05-11 19:23:53.000000 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/PKG-INFO
+-rw-r--r--   0 nic        (501) staff       (20)     1751 2023-05-11 19:23:53.000000 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 nic        (501) staff       (20)        1 2023-05-11 19:23:53.000000 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 nic        (501) staff       (20)        1 2023-02-08 04:10:44.000000 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/not-zip-safe
+-rw-r--r--   0 nic        (501) staff       (20)      149 2023-05-11 19:23:53.000000 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/requires.txt
+-rw-r--r--   0 nic        (501) staff       (20)       28 2023-05-11 19:23:53.000000 pynamodb-dax-0.0.6/pynamodb_dax.egg-info/top_level.txt
+-rw-r--r--   0 nic        (501) staff       (20)      189 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/requirements-dev.txt
+-rw-r--r--   0 nic        (501) staff       (20)      100 2023-05-11 19:23:53.694191 pynamodb-dax-0.0.6/setup.cfg
+-rw-r--r--   0 nic        (501) staff       (20)     1296 2023-05-11 19:19:22.000000 pynamodb-dax-0.0.6/setup.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.691888 pynamodb-dax-0.0.6/tests/
+-rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/__init__.py
+-rw-r--r--   0 nic        (501) staff       (20)    42087 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/data.py
+-rw-r--r--   0 nic        (501) staff       (20)     5472 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/deep_eq.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.693018 pynamodb-dax-0.0.6/tests/integration/
+-rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/integration/__init__.py
+-rw-r--r--   0 nic        (501) staff       (20)     4826 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/integration/base_integration_test.py
+-rw-r--r--   0 nic        (501) staff       (20)     1676 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/integration/binary_update_test.py
+-rw-r--r--   0 nic        (501) staff       (20)      602 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/integration/conftest.py
+-rw-r--r--   0 nic        (501) staff       (20)     4176 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/integration/model_integration_test.py
+-rw-r--r--   0 nic        (501) staff       (20)     4608 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/integration/table_integration_test.py
+-rw-r--r--   0 nic        (501) staff       (20)     4426 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/integration/test_discriminator_index.py
+-rw-r--r--   0 nic        (501) staff       (20)    13872 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/tests/integration/test_transaction_integration.py
+-rw-r--r--   0 nic        (501) staff       (20)      552 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/response.py
+-rw-r--r--   0 nic        (501) staff       (20)    50294 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/tests/test_attributes.py
+-rw-r--r--   0 nic        (501) staff       (20)    63577 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/test_base_connection.py
+-rw-r--r--   0 nic        (501) staff       (20)      466 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/test_binary_legacy_encoding.py
+-rw-r--r--   0 nic        (501) staff       (20)     6828 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/test_discriminator.py
+-rw-r--r--   0 nic        (501) staff       (20)     1155 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/test_exceptions.py
+-rw-r--r--   0 nic        (501) staff       (20)    30181 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/test_expressions.py
+-rw-r--r--   0 nic        (501) staff       (20)   125584 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/tests/test_model.py
+-rw-r--r--   0 nic        (501) staff       (20)     2078 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/test_pagination.py
+-rw-r--r--   0 nic        (501) staff       (20)      643 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/test_settings.py
+-rw-r--r--   0 nic        (501) staff       (20)     3788 2023-02-07 17:07:32.000000 pynamodb-dax-0.0.6/tests/test_signals.py
+-rw-r--r--   0 nic        (501) staff       (20)    19859 2023-05-11 18:08:42.000000 pynamodb-dax-0.0.6/tests/test_table_connection.py
+-rw-r--r--   0 nic        (501) staff       (20)     4551 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/tests/test_transaction.py
+drwxr-xr-x   0 nic        (501) staff       (20)        0 2023-05-11 19:23:53.693664 pynamodb-dax-0.0.6/typing_tests/
+-rw-r--r--   0 nic        (501) staff       (20)        0 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/typing_tests/__init__.py
+-rw-r--r--   0 nic        (501) staff       (20)     2018 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/typing_tests/attributes.py
+-rw-r--r--   0 nic        (501) staff       (20)     4903 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/typing_tests/models.py
+-rw-r--r--   0 nic        (501) staff       (20)      874 2023-02-07 17:13:25.000000 pynamodb-dax-0.0.6/typing_tests/transactions.py
```

### Comparing `pynamodb-dax-0.0.5/LICENSE` & `pynamodb-dax-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/PKG-INFO` & `pynamodb-dax-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb-dax
-Version: 0.0.5
+Version: 0.0.6
 Summary: fork to pynamodb for supporting dax
 Home-page: https://github.com/thanakijwanavit/PynamoDB
 Author: Nic Wanavit (fork)
 Author-email: nwanavit@gmail.com
 License: MIT
 Keywords: python dynamodb amazon dax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynamodb-dax-0.0.5/README.rst` & `pynamodb-dax-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/_schema.py` & `pynamodb-dax-0.0.6/pynamodb/_schema.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/_util.py` & `pynamodb-dax-0.0.6/pynamodb/_util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/attributes.py` & `pynamodb-dax-0.0.6/pynamodb/attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/connection/base.py` & `pynamodb-dax-0.0.6/pynamodb/connection/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,15 @@
                  dax_write_endpoints: Optional[List[str]] = None,
                  dax_read_endpoints: Optional[List[str]] = None):
         self._tables: Dict[str, MetaTable] = {}
         self.host = host
         self._local = local()
         self._client: Optional[BotocoreBaseClientPrivate] = None
         self._convert_to_request_dict__endpoint_url = False
+        self._convert_to_request_dict_kwargs: Dict[str, Any] = {}
         if region:
             self.region = region
         else:
             self.region = get_settings_value('region')
 
         if connect_timeout_seconds is not None:
             self._connect_timeout_seconds = connect_timeout_seconds
@@ -383,36 +384,19 @@
             if operation_name in OP_WRITE and self.dax_write_endpoints:
                 return self.dax_write_client.dispatch(operation_name, operation_kwargs)
             elif operation_name in OP_READ and self.dax_read_endpoints:
                 return self.dax_read_client.dispatch(operation_name, operation_kwargs)
         except DaxClientError:
             raise
         operation_model = self.client._service_model.operation_model(operation_name)
-        if self._convert_to_request_dict__endpoint_url:
-            request_context = {
-                'client_region': self.region,
-                'client_config': self.client.meta.config,
-                'has_streaming_input': operation_model.has_streaming_input,
-                'auth_type': operation_model.auth_type,
-            }
-            endpoint_url, additional_headers = self.client._resolve_endpoint_ruleset(
-                operation_model, operation_kwargs, request_context
-            )
-            request_dict = self.client._convert_to_request_dict(
-                api_params=operation_kwargs,
-                operation_model=operation_model,
-                endpoint_url=endpoint_url,
-                context=request_context,
-                headers=additional_headers,
-            )
-        else:
-            request_dict = self.client._convert_to_request_dict(
-                operation_kwargs,
-                operation_model,
-            )
+        request_dict = self.client._convert_to_request_dict(
+            operation_kwargs,
+            operation_model,
+            **self._convert_to_request_dict_kwargs,
+        )
 
         for i in range(0, self._max_retry_attempts_exception + 1):
             attempt_number = i + 1
             is_last_attempt_for_exceptions = i == self._max_retry_attempts_exception
 
             http_response = None
             prepared_request = None
@@ -591,18 +575,19 @@
         # if the client does not have credentials, we create a new client
         # otherwise the client is permanently poisoned in the case of metadata service flakiness when using IAM roles
         if not self._client or (self._client._request_signer and not self._client._request_signer._credentials):
             config = botocore.client.Config(
                 parameter_validation=False,  # Disable unnecessary validation for performance
                 connect_timeout=self._connect_timeout_seconds,
                 read_timeout=self._read_timeout_seconds,
-                max_pool_connections=self._max_pool_connections,
-            )
+                max_pool_connections=self._max_pool_connections)
             self._client = cast(BotocoreBaseClientPrivate, self.session.create_client(SERVICE_NAME, self.region, endpoint_url=self.host, config=config))
-            self._convert_to_request_dict__endpoint_url = 'endpoint_url' in inspect.signature(self._client._convert_to_request_dict).parameters
+            self._convert_to_request_dict_kwargs = {}
+            if 'endpoint_url' in inspect.signature(self._client._convert_to_request_dict).parameters:
+                self._convert_to_request_dict_kwargs['endpoint_url'] = self.host
         return self._client
 
     @property
     def dax_write_client(self):
         if self._dax_write_client is None:
             self._dax_write_client = DaxClient(
                 endpoints=self.dax_write_endpoints,
```

### Comparing `pynamodb-dax-0.0.5/pynamodb/connection/dax.py` & `pynamodb-dax-0.0.6/pynamodb/connection/dax.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/connection/table.py` & `pynamodb-dax-0.0.6/pynamodb/connection/table.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/constants.py` & `pynamodb-dax-0.0.6/pynamodb/constants.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/exceptions.py` & `pynamodb-dax-0.0.6/pynamodb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/expressions/condition.py` & `pynamodb-dax-0.0.6/pynamodb/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/expressions/operand.py` & `pynamodb-dax-0.0.6/pynamodb/expressions/operand.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/expressions/projection.py` & `pynamodb-dax-0.0.6/pynamodb/expressions/projection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/expressions/update.py` & `pynamodb-dax-0.0.6/pynamodb/expressions/update.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/expressions/util.py` & `pynamodb-dax-0.0.6/pynamodb/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/indexes.py` & `pynamodb-dax-0.0.6/pynamodb/indexes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/models.py` & `pynamodb-dax-0.0.6/pynamodb/models.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/pagination.py` & `pynamodb-dax-0.0.6/pynamodb/pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/settings.py` & `pynamodb-dax-0.0.6/pynamodb/settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/signals.py` & `pynamodb-dax-0.0.6/pynamodb/signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb/transactions.py` & `pynamodb-dax-0.0.6/pynamodb/transactions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/pynamodb_dax.egg-info/PKG-INFO` & `pynamodb-dax-0.0.6/pynamodb_dax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb-dax
-Version: 0.0.5
+Version: 0.0.6
 Summary: fork to pynamodb for supporting dax
 Home-page: https://github.com/thanakijwanavit/PynamoDB
 Author: Nic Wanavit (fork)
 Author-email: nwanavit@gmail.com
 License: MIT
 Keywords: python dynamodb amazon dax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynamodb-dax-0.0.5/pynamodb_dax.egg-info/SOURCES.txt` & `pynamodb-dax-0.0.6/pynamodb_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/setup.py` & `pynamodb-dax-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 install_requires = [
     'botocore>=1.12.54',
     'python-dateutil>=2.1,<3.0.0',
-    'amazon-dax-client>=1.1.7'
+    'amazon-dax-client>=1.1.7',
     'typing-extensions>=4; python_version<"3.11"',
 ]
 
 setup(
     name='pynamodb-dax',
     version=__import__('pynamodb').__version__,
     packages=find_packages(),
```

### Comparing `pynamodb-dax-0.0.5/tests/data.py` & `pynamodb-dax-0.0.6/tests/data.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/deep_eq.py` & `pynamodb-dax-0.0.6/tests/deep_eq.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/base_integration_test.py` & `pynamodb-dax-0.0.6/tests/integration/base_integration_test.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/binary_update_test.py` & `pynamodb-dax-0.0.6/tests/integration/binary_update_test.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/conftest.py` & `pynamodb-dax-0.0.6/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/model_integration_test.py` & `pynamodb-dax-0.0.6/tests/integration/model_integration_test.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/table_integration_test.py` & `pynamodb-dax-0.0.6/tests/integration/table_integration_test.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/test_discriminator_index.py` & `pynamodb-dax-0.0.6/tests/integration/test_discriminator_index.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/integration/test_transaction_integration.py` & `pynamodb-dax-0.0.6/tests/integration/test_transaction_integration.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/response.py` & `pynamodb-dax-0.0.6/tests/response.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_attributes.py` & `pynamodb-dax-0.0.6/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_base_connection.py` & `pynamodb-dax-0.0.6/tests/test_base_connection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_discriminator.py` & `pynamodb-dax-0.0.6/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_exceptions.py` & `pynamodb-dax-0.0.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_expressions.py` & `pynamodb-dax-0.0.6/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_model.py` & `pynamodb-dax-0.0.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_pagination.py` & `pynamodb-dax-0.0.6/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_settings.py` & `pynamodb-dax-0.0.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_signals.py` & `pynamodb-dax-0.0.6/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_table_connection.py` & `pynamodb-dax-0.0.6/tests/test_table_connection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/tests/test_transaction.py` & `pynamodb-dax-0.0.6/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/typing_tests/attributes.py` & `pynamodb-dax-0.0.6/typing_tests/attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/typing_tests/models.py` & `pynamodb-dax-0.0.6/typing_tests/models.py`

 * *Files identical despite different names*

### Comparing `pynamodb-dax-0.0.5/typing_tests/transactions.py` & `pynamodb-dax-0.0.6/typing_tests/transactions.py`

 * *Files identical despite different names*


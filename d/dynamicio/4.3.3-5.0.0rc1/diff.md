# Comparing `tmp/dynamicio-4.3.3.tar.gz` & `tmp/dynamicio-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicio-4.3.3.tar", last modified: Tue Mar 28 13:08:19 2023, max compression
+gzip compressed data, was "dynamicio-5.0.0rc1.tar", last modified: Thu May 11 14:07:00 2023, max compression
```

## Comparing `dynamicio-4.3.3.tar` & `dynamicio-5.0.0rc1.tar`

### file list

```diff
@@ -1,75 +1,52 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.509345 dynamicio-4.3.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2023-03-28 13:08:10.000000 dynamicio-4.3.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39880 2023-03-28 13:08:19.509345 dynamicio-4.3.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2023-03-28 13:08:10.000000 dynamicio-4.3.3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.501345 dynamicio-4.3.3/demo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.501345 dynamicio-4.3.3/demo/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/environment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      972 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1904 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/runner_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.501345 dynamicio-4.3.3/demo/src/runners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/runners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1203 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/runners/staging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/src/runners/transform.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/demo/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/demo/tests/runners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/runners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/runners/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/runners/test_staging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/runners/test_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/test_pipeline.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2023-03-28 13:08:10.000000 dynamicio-4.3.3/demo/tests/test_runner_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/dynamicio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1714 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3710 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/dynamicio/config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      134 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/config/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9530 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/config/io_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/dynamicio/config/pydantic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      394 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/config/pydantic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/config/pydantic/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6823 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/config/pydantic/io_resources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3653 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/config/pydantic/table_schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12966 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3172 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5700 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/metrics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/dynamicio/mixins/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/mixins/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/mixins/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7816 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/mixins/with_kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9903 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/mixins/with_local.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8017 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/mixins/with_postgres.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16065 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/mixins/with_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/py.typed
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13236 2023-03-28 13:08:10.000000 dynamicio-4.3.3/dynamicio/validations.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.505345 dynamicio-4.3.3/dynamicio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39880 2023-03-28 13:08:19.000000 dynamicio-4.3.3/dynamicio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1536 2023-03-28 13:08:19.000000 dynamicio-4.3.3/dynamicio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-28 13:08:19.000000 dynamicio-4.3.3/dynamicio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-03-28 13:08:19.000000 dynamicio-4.3.3/dynamicio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2023-03-28 13:08:19.000000 dynamicio-4.3.3/dynamicio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-03-28 13:08:19.000000 dynamicio-4.3.3/dynamicio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2023-03-28 13:08:10.000000 dynamicio-4.3.3/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-28 13:08:19.509345 dynamicio-4.3.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-03-28 13:08:10.000000 dynamicio-4.3.3/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.509345 dynamicio-4.3.3/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33324 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:19.509345 dynamicio-4.3.3/tests/mocking/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/mocking/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4755 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/mocking/io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/mocking/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14102 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/test_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6491 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/test_config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    42740 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/test_core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6108 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/test_metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16805 2023-03-28 13:08:10.000000 dynamicio-4.3.3/tests/test_validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.476336 dynamicio-5.0.0rc1/dynamicio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/inject.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/dynamicio/io/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/dynamicio/io/file/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1650 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/csv.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1915 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/hdf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1648 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1733 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/parquet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3745 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2305 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/keyed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7553 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/postgres.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/dynamicio/io/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/contexts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2363 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/csv.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5203 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/hdf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2362 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2417 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/parquet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      522 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/validators.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.476336 dynamicio-5.0.0rc1/dynamicio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1007 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      525 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      125 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/tests/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3141 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/test_hdf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2939 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/test_s3_implementations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1810 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_file_implementations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2315 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_inject.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3329 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_keyed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7516 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_postgres.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_validations.py
```

### Comparing `dynamicio-4.3.3/LICENSE` & `dynamicio-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicio-4.3.3/PKG-INFO` & `dynamicio-5.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 4.3.3
+Version: 5.0.0rc1
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-4.3.3/README.md` & `dynamicio-5.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dynamicio-4.3.3/dynamicio.egg-info/PKG-INFO` & `dynamicio-5.0.0rc1/dynamicio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 4.3.3
+Version: 5.0.0rc1
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-4.3.3/pyproject.toml` & `dynamicio-5.0.0rc1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 py38 = true
-line-length = 185
+line-length = 120
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.git
     | \.mypy_cache
     | \.github
```

### Comparing `dynamicio-4.3.3/setup.py` & `dynamicio-5.0.0rc1/setup.py`

 * *Files identical despite different names*


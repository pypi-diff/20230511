# Comparing `tmp/cleanlab-studio-1.0.3.tar.gz` & `tmp/cleanlab-studio-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.3.tar", last modified: Wed May 10 22:29:08 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.4.tar", last modified: Thu May 11 00:02:06 2023, max compression
```

## Comparing `cleanlab-studio-1.0.3.tar` & `cleanlab-studio-1.0.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.585124 cleanlab-studio-1.0.3/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.585124 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.838179 cleanlab-studio-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-11 00:02:06.838179 cleanlab-studio-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.822179 cleanlab-studio-1.0.4/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:02:06.838179 cleanlab-studio-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.3/LICENSE` & `cleanlab-studio-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/PKG-INFO` & `cleanlab-studio-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.3
+Version: 1.0.4
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Keywords: cleanlab
```

### Comparing `cleanlab-studio-1.0.3/README.md` & `cleanlab-studio-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.4/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.4/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/api/api.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.4/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.0.4/cleanlab_studio/studio/studio.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,18 +182,21 @@
                     f"Invalid label column: {label_column}. Label column must have categorical feature type"
                 )
         else:
             label_column = str(dataset_details["label_column_guess"])
             print(f"Label column not supplied. Using best guess {label_column}")
 
         if feature_columns is not None and modality != "tabular":
+            if label_column in feature_columns:
+                raise ValueError("Label column cannot be included in feature columns")
             raise ValueError("Feature columns supplied, but project modality is not tabular")
         if feature_columns is None:
             if modality == "tabular":
                 feature_columns = dataset_details["distinct_columns"]
+                feature_columns.remove(label_column)
                 print(f"Feature columns not supplied. Using all valid feature columns")
 
         if text_column is not None:
             if modality != "text":
                 raise ValueError("Text column supplied, but project modality is not text")
             elif text_column not in dataset_details["text_columns"]:
                 raise ValueError(
```

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.4/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.4/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.3
+Version: 1.0.4
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Keywords: cleanlab
```

### Comparing `cleanlab-studio-1.0.3/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.4/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/setup.py` & `cleanlab-studio-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/tests/bench.py` & `cleanlab-studio-1.0.4/tests/bench.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.4/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.4/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.4/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.3/tests/datasets/utils.py` & `cleanlab-studio-1.0.4/tests/datasets/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/cleanlab-studio-1.0.2.tar.gz` & `tmp/cleanlab-studio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.2.tar", last modified: Tue May  9 19:52:21 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.3.tar", last modified: Wed May 10 22:29:08 2023, max compression
```

## Comparing `cleanlab-studio-1.0.2.tar` & `cleanlab-studio-1.0.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.824782 cleanlab-studio-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-09 19:52:21.824782 cleanlab-studio-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.812781 cleanlab-studio-1.0.2/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.816781 cleanlab-studio-1.0.2/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.816781 cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.816781 cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.816781 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-09 19:52:21.000000 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-09 19:52:21.000000 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:52:21.000000 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 19:52:21.000000 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-09 19:52:21.000000 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 19:52:21.000000 cleanlab-studio-1.0.2/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:52:21.824782 cleanlab-studio-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.820782 cleanlab-studio-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:21.824782 cleanlab-studio-1.0.2/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-09 19:52:02.000000 cleanlab-studio-1.0.2/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.585124 cleanlab-studio-1.0.3/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.589124 cleanlab-studio-1.0.3/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.585124 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 22:29:08.000000 cleanlab-studio-1.0.3/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:29:08.593124 cleanlab-studio-1.0.3/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-10 22:28:54.000000 cleanlab-studio-1.0.3/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.2/LICENSE` & `cleanlab-studio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/PKG-INFO` & `cleanlab-studio-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Keywords: cleanlab
```

### Comparing `cleanlab-studio-1.0.2/README.md` & `cleanlab-studio-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/api_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 from cleanlab_studio.version import __version__
 from cleanlab_studio.cli.click_helpers import abort, warn, info
 from cleanlab_studio.cli.dataset.image_utils import get_image_filepath
 from cleanlab_studio.cli.dataset.schema_types import Schema
 from cleanlab_studio.cli.types import JSONDict, IDType, MEDIA_MODALITIES
 
-base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api/cli/v0")
+base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api")
+cli_base_url = f"{base_url}/cli/v0"
 
 
 MAX_PARALLEL_UPLOADS = 32  # XXX choose this dynamically?
 INITIAL_BACKOFF = 0.25  # seconds
 MAX_RETRIES = 4
 
 
@@ -51,34 +52,34 @@
     if res_json.get("error", None) is not None:
         abort(res_json["error"])
 
 
 def initialize_dataset(api_key: str, schema: Schema) -> str:
     request_json = dict(schema=schema.to_dict())
     res = requests.post(
-        base_url + "/datasets", json=request_json, headers=_construct_headers(api_key)
+        cli_base_url + "/datasets", json=request_json, headers=_construct_headers(api_key)
     )
     handle_api_error(res)
     dataset_id: str = res.json()["dataset_id"]
     return dataset_id
 
 
 def get_existing_ids(api_key: str, dataset_id: str) -> List[IDType]:
     res = requests.get(
-        base_url + f"/datasets/{dataset_id}/ids",
+        cli_base_url + f"/datasets/{dataset_id}/ids",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     existing_ids: List[IDType] = res.json()["existing_ids"]
     return existing_ids
 
 
 def get_dataset_schema(api_key: str, dataset_id: str) -> Schema:
     res = requests.get(
-        base_url + f"/datasets/{dataset_id}/schema",
+        cli_base_url + f"/datasets/{dataset_id}/schema",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     schema = Schema.from_dict(res.json()["schema"])
     return schema
 
 
@@ -128,15 +129,15 @@
                     filepath_column=col,
                     media_type=modality.value,
                 )
                 for col in filepath_columns
             ]
             await asyncio.gather(*upload_tasks)
 
-        url = base_url + f"/datasets/{dataset_id}"
+        url = cli_base_url + f"/datasets/{dataset_id}"
         data = gzip.compress(
             json.dumps(dict(rows=json.dumps(rows), columns=json.dumps(columns))).encode("utf-8")
         )
         headers = _construct_headers(api_key)
         headers["Content-Encoding"] = "gzip"
 
         async with session.post(url=url, data=data, headers=headers) as res:
@@ -260,83 +261,83 @@
 
     :param api_key:
     :param cleanset_id:
     :param all: whether to download all Cleanlab columns or just the clean_label column
     :return: return (rows, id_column)
     """
     res = requests.get(
-        base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
+        cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     rows: List[List[Any]] = res.json()["rows"]
     return rows
 
 
 def get_completion_status(api_key: str, dataset_id: str) -> bool:
     res = requests.get(
-        base_url + f"/datasets/{dataset_id}/complete",
+        cli_base_url + f"/datasets/{dataset_id}/complete",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     completed: bool = res.json()["complete"]
     return completed
 
 
 def complete_upload(api_key: str, dataset_id: str) -> None:
     res = requests.patch(
-        base_url + f"/datasets/{dataset_id}/complete",
+        cli_base_url + f"/datasets/{dataset_id}/complete",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
 
 
 def get_id_column(api_key: str, cleanset_id: str) -> str:
     res = requests.get(
-        base_url + f"/cleansets/{cleanset_id}/id_column",
+        cli_base_url + f"/cleansets/{cleanset_id}/id_column",
         headers={"Authorization": f"bearer {api_key}"},
     )
     handle_api_error(res)
     id_column: str = res.json()["id_column"]
     return id_column
 
 
 def validate_api_key(api_key: str) -> bool:
     res = requests.get(
-        base_url + "/validate", json=dict(api_key=api_key), headers=_construct_headers(api_key)
+        cli_base_url + "/validate", json=dict(api_key=api_key), headers=_construct_headers(api_key)
     )
     handle_api_error(res)
     valid: bool = res.json()["valid"]
     return valid
 
 
 def check_client_version() -> bool:
-    res = requests.post(base_url + "/check_client_version", json=dict(version=__version__))
+    res = requests.post(cli_base_url + "/check_client_version", json=dict(version=__version__))
     handle_api_error(res)
     valid: bool = res.json()["valid"]
     return valid
 
 
 def check_dataset_limit(
     api_key: str, file_size: int, modality: str, show_warning: bool = False
 ) -> JSONDict:
     res = requests.post(
-        base_url + "/check_dataset_limit",
+        cli_base_url + "/check_dataset_limit",
         json=dict(file_size=file_size, modality=modality),
         headers=_construct_headers(api_key),
     )
     handle_api_error(res, show_warning=show_warning)
     res_json: JSONDict = res.json()
     return res_json
 
 
 def get_presigned_posts(
     api_key: str, dataset_id: str, filepaths: List[str], row_ids: List[str], media_type: str
 ) -> JSONDict:
     res = requests.get(
-        base_url + "/media_upload/presigned_posts",
+        cli_base_url + "/media_upload/presigned_posts",
         json=dict(dataset_id=dataset_id, filepaths=filepaths, row_ids=row_ids, type=media_type),
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     res_json: JSONDict = res.json()
     return res_json
```

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import click
 import os
 import subprocess
 
-from cleanlab_studio.cli import api_service
+from cleanlab_studio.internal.api import api
 from cleanlab_studio.cli.click_helpers import abort
 from cleanlab_studio.cli.dataset.commands import dataset
 from cleanlab_studio.cli.cleanset.commands import cleanset
 from cleanlab_studio.cli.login.login import login
 from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.version import __version__
 
 
 @click.group()
 @click.pass_context
 def cli(ctx: click.Context) -> None:
     if ctx.invoked_subcommand == "version":
         return  # avoid RTT / dependence on API to get client version
     CleanlabSettings.init_cleanlab_settings()
-    valid_version = api_service.check_client_version()
+    valid_version = api.is_valid_client_version()
     if not valid_version:
         abort(
             "CLI is out of date and must be updated. Run 'pip install --upgrade cleanlab-studio'."
         )
     pass
```

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.3/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.3/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/api/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 import requests
 from tqdm import tqdm
 
 from cleanlab_studio.internal.types import JSONDict
 from cleanlab_studio.version import __version__
 
-base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api/cli/v0")
-upload_base_url = os.environ.get(
-    "CLEANLAB_API_UPLOAD_BASE_URL", "https://api.cleanlab.ai/api/upload/v0"
-)
+base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api")
+cli_base_url = f"{base_url}/cli/v0"
+upload_base_url = f"{base_url}/upload/v0"
+dataset_base_url = f"{base_url}/datasets"
+project_base_url = f"{base_url}/projects"
 
 
 def _construct_headers(
     api_key: Optional[str], content_type: Optional[str] = "application/json"
 ) -> JSONDict:
     retval = dict()
     if api_key:
@@ -38,23 +39,23 @@
             raise APIError(res_json["description"])
     if res_json.get("error", None) is not None:
         raise APIError(res_json["error"])
 
 
 def validate_api_key(api_key: str) -> bool:
     res = requests.get(
-        base_url + "/validate", json=dict(api_key=api_key), headers=_construct_headers(api_key)
+        cli_base_url + "/validate", json=dict(api_key=api_key), headers=_construct_headers(api_key)
     )
     handle_api_error(res)
     valid: bool = res.json()["valid"]
     return valid
 
 
-def check_client_version() -> bool:
-    res = requests.post(base_url + "/check_client_version", json=dict(version=__version__))
+def is_valid_client_version() -> bool:
+    res = requests.post(cli_base_url + "/check_client_version", json=dict(version=__version__))
     handle_api_error(res)
     valid: bool = res.json()["valid"]
     return valid
 
 
 def initialize_upload(
     api_key: str, filename: str, file_type: str, file_size: int
@@ -122,25 +123,25 @@
     handle_api_error(res)
     res_json: JSONDict = res.json()
     return res_json
 
 
 def get_project_of_cleanset(api_key: str, cleanset_id: str) -> str:
     res = requests.get(
-        base_url + f"/cleansets/{cleanset_id}/project",
+        cli_base_url + f"/cleansets/{cleanset_id}/project",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     project_id: str = res.json()["project_id"]
     return project_id
 
 
 def get_label_column_of_project(api_key: str, project_id: str) -> str:
     res = requests.get(
-        base_url + f"/projects/{project_id}/label_column",
+        cli_base_url + f"/projects/{project_id}/label_column",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     label_column: str = res.json()["label_column"]
     return label_column
 
 
@@ -150,52 +151,91 @@
 
     :param api_key:
     :param cleanset_id:
     :param all: whether to download all Cleanlab columns or just the clean_label column
     :return: return (rows, id_column)
     """
     res = requests.get(
-        base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
+        cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     rows: List[List[Any]] = res.json()["rows"]
     return rows
 
 
 def get_id_column(api_key: str, cleanset_id: str) -> str:
     res = requests.get(
-        base_url + f"/cleansets/{cleanset_id}/id_column",
+        cli_base_url + f"/cleansets/{cleanset_id}/id_column",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     id_column: str = res.json()["id_column"]
     return id_column
 
 
 def get_dataset_of_project(api_key: str, project_id: str) -> str:
     res = requests.get(
-        base_url + f"/projects/{project_id}/dataset",
+        cli_base_url + f"/projects/{project_id}/dataset",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     dataset_id: str = res.json()["dataset_id"]
     return dataset_id
 
 
 def get_dataset_schema(api_key: str, dataset_id: str) -> JSONDict:
     res = requests.get(
-        base_url + f"/datasets/{dataset_id}/schema",
+        cli_base_url + f"/datasets/{dataset_id}/schema",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     schema: JSONDict = res.json()["schema"]
     return schema
 
 
+def get_dataset_details(api_key: str, dataset_id: str) -> JSONDict:
+    res = requests.get(
+        dataset_base_url + f"/details/{dataset_id}",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+    dataset_details: JSONDict = res.json()
+    return dataset_details
+
+
+def clean_dataset(
+    api_key: str,
+    dataset_id: str,
+    project_name: str,
+    tasktype: str,
+    modality: str,
+    modeltype: str,
+    label_column: str,
+    feature_columns: List[str],
+    text_column: Optional[str],
+) -> str:
+    request_json = dict(
+        name=project_name,
+        dataset_id=dataset_id,
+        tasktype=tasktype,
+        modality=modality,
+        model_type=modeltype,
+        label_column=label_column,
+        feature_columns=feature_columns,
+        text_column=text_column,
+    )
+    res = requests.post(
+        project_base_url + f"/clean", headers=_construct_headers(api_key), json=request_json
+    )
+    handle_api_error(res)
+    project_id = res.json()["project_id"]
+    return str(project_id)
+
+
 def poll_progress(
     progress_id: str, request_function: Callable[[str], JSONDict], description: str
 ) -> JSONDict:
     with tqdm(total=1, desc=description, bar_format="{desc}: {percentage:3.0f}%|{bar}|") as pbar:
         res = request_function(progress_id)
         while res["status"] != "complete":
             if res["status"] == "error":
```

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.3/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.3/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.3/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Keywords: cleanlab
```

### Comparing `cleanlab-studio-1.0.2/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.3/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/setup.py` & `cleanlab-studio-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/tests/bench.py` & `cleanlab-studio-1.0.3/tests/bench.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.3/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.3/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.3/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.2/tests/datasets/utils.py` & `cleanlab-studio-1.0.3/tests/datasets/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/autogluon.common-0.7.1b20230509.tar.gz` & `tmp/autogluon.common-0.7.1b20230510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230509.tar", last modified: Tue May  9 09:03:52 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230510.tar", last modified: Wed May 10 09:03:55 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230509.tar` & `autogluon.common-0.7.1b20230510.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.690410 autogluon.common-0.7.1b20230509/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-09 09:03:52.690410 autogluon.common-0.7.1b20230509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:03:52.690410 autogluon.common-0.7.1b20230509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.682410 autogluon.common-0.7.1b20230509/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.682410 autogluon.common-0.7.1b20230509/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.682410 autogluon.common-0.7.1b20230509/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.686411 autogluon.common-0.7.1b20230509/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.686411 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.686411 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.690410 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-09 09:03:39.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:03:52.682410 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:03:52.000000 autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.299237 autogluon.common-0.7.1b20230510/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-10 09:03:55.299237 autogluon.common-0.7.1b20230510/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:03:55.299237 autogluon.common-0.7.1b20230510/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.295237 autogluon.common-0.7.1b20230510/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.295237 autogluon.common-0.7.1b20230510/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.295237 autogluon.common-0.7.1b20230510/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.295237 autogluon.common-0.7.1b20230510/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.299237 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.299237 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.299237 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-10 09:03:42.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:03:55.295237 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-10 09:03:55.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:03:54.000000 autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230509/LICENSE` & `autogluon.common-0.7.1b20230510/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/PKG-INFO` & `autogluon.common-0.7.1b20230510/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230509
+Version: 0.7.1b20230510
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230509/setup.py` & `autogluon.common-0.7.1b20230510/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/deprecated.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/try_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,17 @@
             "A quick tip is to install via `pip install mxboard`. ")
 
 
 def try_import_mxnet():
     mx_version = '1.6.0'
     try:
         import mxnet as mx
-        from distutils.version import LooseVersion
+        from packaging import version
 
-        if LooseVersion(mx.__version__) < LooseVersion(mx_version):
+        if version.parse(mx.__version__) < version.parse(mx_version):
             msg = (
                 "Legacy mxnet=={} detected, some new modules will not work properly. "
                 "mxnet>={} is required. You can use pip to upgrade mxnet "
                 "`pip install mxnet --upgrade` "
                 "or `pip install mxnet_cu101 --upgrade`").format(mx.__version__, mx_version)
             raise ValueError(msg)
     except ImportError:
@@ -61,17 +61,17 @@
         Linux=RAY_MAX_VERSION,
     )
     ray_min_version = '2.2.0'
     current_os = platform.system()
     ray_max_version = ray_max_version_os_map.get(current_os, RAY_MAX_VERSION)
     try:
         import ray
-        from distutils.version import LooseVersion
+        from packaging import version
 
-        if LooseVersion(ray.__version__) < LooseVersion(ray_min_version) or LooseVersion(ray.__version__) >= LooseVersion(ray_max_version):
+        if version.parse(ray.__version__) < version.parse(ray_min_version) or version.parse(ray.__version__) >= version.parse(ray_max_version):
             msg = (
                 f"ray=={ray.__version__} detected. "
                 f"{ray_min_version} <= ray < {ray_max_version} is required. You can use pip to install certain version of ray "
                 f"`pip install ray=={ray_min_version}` "
             )
             raise ValueError(msg)
         return ray
@@ -94,40 +94,40 @@
     ray_lightining_torch_lightning_compatibility_range_map = {
         ('0.2.0', '0.3.0'): ('1.5.0', '1.6.0'),
     }
     try:
         import pkg_resources
         import pytorch_lightning
         import ray_lightning
-        from distutils.version import LooseVersion
+        from packaging import version
         
         ray_lightning_version = pkg_resources.get_distribution('ray_lightning').version # ray_lightning doesn't have __version__...
         
-        if not (LooseVersion(supported_ray_lightning_min_version)
-                <= LooseVersion(ray_lightning_version)
-                < LooseVersion(supported_ray_lightning_max_version)):
+        if not (version.parse(supported_ray_lightning_min_version)
+                <= version.parse(ray_lightning_version)
+                < version.parse(supported_ray_lightning_max_version)):
             logger.log(
                 f"ray_lightning=={ray_lightning_version} detected. "
                 f"{supported_ray_lightning_min_version} <= ray_lighting < {supported_ray_lightning_max_version} is required."
                 "You can use pip to install certain version of ray_lightning."
                 f"Supported ray_lightning versions and the compatible torch lightning versions are {ray_lightning_torch_lightning_compatibility_map}."
             )
             return False
         
         for ray_lightning_versions, torch_lightning_versions in ray_lightining_torch_lightning_compatibility_range_map.items():
             ray_lightning_min_version, ray_lightning_max_version = ray_lightning_versions
             torch_lightning_min_version, torch_lightning_max_version = torch_lightning_versions
             if (
-                LooseVersion(ray_lightning_min_version)
-                <= LooseVersion(ray_lightning_version)
-                < LooseVersion(ray_lightning_max_version)
+                version.parse(ray_lightning_min_version)
+                <= version.parse(ray_lightning_version)
+                < version.parse(ray_lightning_max_version)
             ):
-                if not (LooseVersion(torch_lightning_min_version)
-                        <= LooseVersion(pytorch_lightning.__version__)
-                        < LooseVersion(torch_lightning_max_version)):
+                if not (version.parse(torch_lightning_min_version)
+                        <= version.parse(pytorch_lightning.__version__)
+                        < version.parse(torch_lightning_max_version)):
                     logger.log(
                         f"Found ray_lightning {ray_lightning_version} that's not compatible with pytorch_lightning."
                         f"The compatible version of pytorch_lightning is >= {torch_lightning_min_version} and < {torch_lightning_max_version}."
                     )
                     return False
         return True
```

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230510/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230509
+Version: 0.7.1b20230510
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230509/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230510/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*


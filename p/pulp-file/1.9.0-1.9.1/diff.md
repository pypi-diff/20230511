# Comparing `tmp/pulp-file-1.9.0.tar.gz` & `tmp/pulp-file-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-file-1.9.0.tar", last modified: Thu Aug 26 16:43:35 2021, max compression
+gzip compressed data, was "pulp-file-1.9.1.tar", last modified: Mon Aug 30 14:40:05 2021, max compression
```

## Comparing `pulp-file-1.9.0.tar` & `pulp-file-1.9.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.083766 pulp-file-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11576 2021-08-26 16:43:33.000000 pulp-file-1.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-08-26 16:43:12.000000 pulp-file-1.9.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-08-26 16:43:12.000000 pulp-file-1.9.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    17988 2021-08-26 16:43:12.000000 pulp-file-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-08-26 16:43:12.000000 pulp-file-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-26 16:43:35.083766 pulp-file-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-08-26 16:43:12.000000 pulp-file-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-26 16:43:12.000000 pulp-file-1.9.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.071766 pulp-file-1.9.0/pulp_file/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.075766 pulp-file-1.9.0/pulp_file/app/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-08-26 16:43:34.000000 pulp-file-1.9.0/pulp_file/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.075766 pulp-file-1.9.0/pulp_file/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0002_file_related_names.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0003_auto_20191014_1721.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0004_filefilesystemexporter.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0005_filerepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0006_delete_filefilesystemexporter.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0007_filefilesystemexporter.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0008_add_manifest_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0009_move_data_to_new_master_distribution_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0010_auto_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0011_fix_auto_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0012_delete_filefilesystemexporter.py
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/0013_file_acs.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/modelresource.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.075766 pulp-file-1.9.0/pulp_file/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/tasks/publishing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4060 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/tasks/synchronizing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6469 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/app/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.075766 pulp-file-1.9.0/pulp_file/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4332 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_auto_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)    12668 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     8987 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4776 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     9498 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_download_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_pulp_manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8942 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/performance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/interact.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7743 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/performance/test_performance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/unit/test_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/unit/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/unit/test_core/test_repo_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/unit/test_core/test_viewsets.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/unit/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.079766 pulp-file-1.9.0/pulp_file/tests/upgrade/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.083766 pulp-file-1.9.0/pulp_file/tests/upgrade/post/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/upgrade/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5523 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/upgrade/post/test_publish.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.083766 pulp-file-1.9.0/pulp_file/tests/upgrade/pre/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/upgrade/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pulp_file/tests/upgrade/pre/test_publish.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:43:35.071766 pulp-file-1.9.0/pulp_file.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-26 16:43:35.000000 pulp-file-1.9.0/pulp_file.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2021-08-26 16:43:35.000000 pulp-file-1.9.0/pulp_file.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-26 16:43:35.000000 pulp-file-1.9.0/pulp_file.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-08-26 16:43:35.000000 pulp-file-1.9.0/pulp_file.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-26 16:43:35.000000 pulp-file-1.9.0/pulp_file.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-08-26 16:43:35.000000 pulp-file-1.9.0/pulp_file.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-08-26 16:43:12.000000 pulp-file-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-26 16:43:12.000000 pulp-file-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-26 16:43:35.083766 pulp-file-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2021-08-26 16:43:34.000000 pulp-file-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-08-26 16:43:12.000000 pulp-file-1.9.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-26 16:43:12.000000 pulp-file-1.9.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11781 2021-08-30 14:40:04.000000 pulp-file-1.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-08-30 14:39:52.000000 pulp-file-1.9.1/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2021-08-30 14:39:52.000000 pulp-file-1.9.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (121)    17988 2021-08-30 14:39:52.000000 pulp-file-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-08-30 14:39:52.000000 pulp-file-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-30 14:40:05.920914 pulp-file-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-08-30 14:39:52.000000 pulp-file-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-30 14:39:52.000000 pulp-file-1.9.1/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.912913 pulp-file-1.9.1/pulp_file/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.916913 pulp-file-1.9.1/pulp_file/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.916913 pulp-file-1.9.1/pulp_file/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     2253 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0002_file_related_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0003_auto_20191014_1721.py
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0004_filefilesystemexporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0005_filerepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0006_delete_filefilesystemexporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0007_filefilesystemexporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0008_add_manifest_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3215 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0009_move_data_to_new_master_distribution_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0010_auto_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0011_fix_auto_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0012_delete_filefilesystemexporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/0013_file_acs.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/modelresource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.916913 pulp-file-1.9.1/pulp_file/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/tasks/publishing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4137 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6469 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/app/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3248 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.916913 pulp-file-1.9.1/pulp_file/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.916913 pulp-file-1.9.1/pulp_file/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.916913 pulp-file-1.9.1/pulp_file/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4332 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_auto_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12668 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8987 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4776 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9498 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_download_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_pulp_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8942 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4876 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2163 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/interact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7743 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/performance/test_performance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/unit/test_core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/unit/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/unit/test_core/test_repo_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/unit/test_core/test_viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/unit/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/upgrade/post/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/upgrade/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5523 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/upgrade/post/test_publish.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.920914 pulp-file-1.9.1/pulp_file/tests/upgrade/pre/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/upgrade/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pulp_file/tests/upgrade/pre/test_publish.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:40:05.912913 pulp-file-1.9.1/pulp_file.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2740 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-08-30 14:40:05.000000 pulp-file-1.9.1/pulp_file.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2021-08-30 14:39:52.000000 pulp-file-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-30 14:39:52.000000 pulp-file-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-30 14:40:05.920914 pulp-file-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2021-08-30 14:40:05.000000 pulp-file-1.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-08-30 14:39:52.000000 pulp-file-1.9.1/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-30 14:39:52.000000 pulp-file-1.9.1/unittest_requirements.txt
```

### Comparing `pulp-file-1.9.0/CHANGES.rst` & `pulp-file-1.9.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,29 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+1.9.1 (2021-08-30)
+==================
+
+
+Bugfixes
+--------
+
+- Fixed bug where sync tasks would open a lot of DB connections.
+  (backported from #9252)
+  `#9311 <https://pulp.plan.io/issues/9311>`_
+
+
+----
+
+
 1.9.0 (2021-08-26)
 ==================
 
 
 Features
 --------
```

### Comparing `pulp-file-1.9.0/COMMITMENT` & `pulp-file-1.9.1/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/COPYRIGHT` & `pulp-file-1.9.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/LICENSE` & `pulp-file-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/PKG-INFO` & `pulp-file-1.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-file
-Version: 1.9.0
+Version: 1.9.1
 Summary: File plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Description: pulp_file
         =========
```

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0001_initial.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0002_file_related_names.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0002_file_related_names.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0004_filefilesystemexporter.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0004_filefilesystemexporter.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0005_filerepository.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0005_filerepository.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0007_filefilesystemexporter.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0007_filefilesystemexporter.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0009_move_data_to_new_master_distribution_model.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0009_move_data_to_new_master_distribution_model.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0010_auto_publish.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0010_auto_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0011_fix_auto_publish.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0011_fix_auto_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0012_delete_filefilesystemexporter.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0012_delete_filefilesystemexporter.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/migrations/0013_file_acs.py` & `pulp-file-1.9.1/pulp_file/app/migrations/0013_file_acs.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/modelresource.py` & `pulp-file-1.9.1/pulp_file/app/modelresource.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/models.py` & `pulp-file-1.9.1/pulp_file/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/serializers.py` & `pulp-file-1.9.1/pulp_file/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/tasks/publishing.py` & `pulp-file-1.9.1/pulp_file/app/tasks/publishing.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/app/tasks/synchronizing.py` & `pulp-file-1.9.1/pulp_file/app/tasks/synchronizing.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,37 +86,41 @@
     async def run(self):
         """
         Build and emit `DeclarativeContent` from the Manifest data.
         """
         global metadata_files
 
         deferred_download = self.remote.policy != Remote.IMMEDIATE  # Interpret download policy
-        with ProgressReport(message="Downloading Metadata", code="sync.downloading.metadata") as pb:
+        async with ProgressReport(
+            message="Downloading Metadata", code="sync.downloading.metadata"
+        ) as pb:
             parsed_url = urlparse(self.remote.url)
             root_dir = os.path.dirname(parsed_url.path)
             downloader = self.remote.get_downloader(url=self.remote.url)
             result = await downloader.run()
-            pb.increment()
+            await pb.aincrement()
             metadata_files.append((result.path, self.remote.url.split("/")[-1]))
 
-        with ProgressReport(message="Parsing Metadata Lines", code="sync.parsing.metadata") as pb:
+        async with ProgressReport(
+            message="Parsing Metadata Lines", code="sync.parsing.metadata"
+        ) as pb:
             manifest = Manifest(result.path)
             entries = list(manifest.read())
 
             pb.total = len(entries)
-            pb.save()
+            await pb.asave()
 
             for entry in entries:
                 path = os.path.join(root_dir, entry.relative_path)
                 url = urlunparse(parsed_url._replace(path=path))
                 file = FileContent(relative_path=entry.relative_path, digest=entry.digest)
                 artifact = Artifact(size=entry.size, sha256=entry.digest)
                 da = DeclarativeArtifact(
                     artifact=artifact,
                     url=url,
                     relative_path=entry.relative_path,
                     remote=self.remote,
                     deferred_download=deferred_download,
                 )
                 dc = DeclarativeContent(content=file, d_artifacts=[da])
-                pb.increment()
+                await pb.aincrement()
                 await self.put(dc)
```

### Comparing `pulp-file-1.9.0/pulp_file/app/viewsets.py` & `pulp-file-1.9.1/pulp_file/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/manifest.py` & `pulp-file-1.9.1/pulp_file/manifest.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_auto_publish.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_auto_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_crud_content_unit.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_crud_content_unit.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_crud_remotes.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_download_content.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_download_content.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_download_policies.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_download_policies.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_publish.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_pulp_manifest.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_pulp_manifest.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/api/test_sync.py` & `pulp-file-1.9.1/pulp_file/tests/functional/api/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/constants.py` & `pulp-file-1.9.1/pulp_file/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/functional/utils.py` & `pulp-file-1.9.1/pulp_file/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/interact.py` & `pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/interact.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/reporting.py` & `pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/reporting.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/performance/pulpperf/utils.py` & `pulp-file-1.9.1/pulp_file/tests/performance/pulpperf/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/performance/test_performance.py` & `pulp-file-1.9.1/pulp_file/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/unit/test_core/test_repo_version.py` & `pulp-file-1.9.1/pulp_file/tests/unit/test_core/test_repo_version.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/unit/test_core/test_viewsets.py` & `pulp-file-1.9.1/pulp_file/tests/unit/test_core/test_viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/unit/test_serializers.py` & `pulp-file-1.9.1/pulp_file/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/upgrade/post/test_publish.py` & `pulp-file-1.9.1/pulp_file/tests/upgrade/post/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file/tests/upgrade/pre/test_publish.py` & `pulp-file-1.9.1/pulp_file/tests/upgrade/pre/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pulp_file.egg-info/PKG-INFO` & `pulp-file-1.9.1/pulp_file.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-file
-Version: 1.9.0
+Version: 1.9.1
 Summary: File plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Description: pulp_file
         =========
```

### Comparing `pulp-file-1.9.0/pulp_file.egg-info/SOURCES.txt` & `pulp-file-1.9.1/pulp_file.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/pyproject.toml` & `pulp-file-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-file-1.9.0/setup.py` & `pulp-file-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as requirements:
     requirements = requirements.readlines()
 
 setup(
     name="pulp-file",
-    version="1.9.0",
+    version="1.9.1",
     description="File plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-dev@redhat.com",
     url="https://pulpproject.org/",
     python_requires=">=3.8",
```


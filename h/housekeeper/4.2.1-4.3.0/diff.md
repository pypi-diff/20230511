# Comparing `tmp/housekeeper-4.2.1.tar.gz` & `tmp/housekeeper-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/housekeeper-4.2.1.tar", last modified: Wed May 10 09:56:55 2023, max compression
+gzip compressed data, was "dist/housekeeper-4.3.0.tar", last modified: Thu May 11 10:16:42 2023, max compression
```

## Comparing `housekeeper-4.2.1.tar` & `housekeeper-4.3.0.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-10 09:56:44.000000 housekeeper-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-10 09:56:44.000000 housekeeper-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-10 09:56:55.000000 housekeeper-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-10 09:56:44.000000 housekeeper-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/store/api/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/handlers/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/handlers/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/file_tags_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-10 09:56:44.000000 housekeeper-4.2.1/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 09:56:55.000000 housekeeper-4.2.1/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 09:56:44.000000 housekeeper-4.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 09:56:44.000000 housekeeper-4.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 09:56:55.000000 housekeeper-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-10 09:56:44.000000 housekeeper-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/filters/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/filters/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/filters/test_file_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/filters/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/filters/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/filters/test_version_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:56:55.000000 housekeeper-4.2.1/tests/store/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/handlers/test_createhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/handlers/test_readhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/store/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-10 09:56:44.000000 housekeeper-4.2.1/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-11 10:16:30.000000 housekeeper-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-11 10:16:30.000000 housekeeper-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-11 10:16:42.000000 housekeeper-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-11 10:16:30.000000 housekeeper-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 10:16:30.000000 housekeeper-4.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 10:16:30.000000 housekeeper-4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 10:16:42.000000 housekeeper-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-11 10:16:30.000000 housekeeper-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/fixtures/sequencing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/sequencing_files/lane1.spring
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/sequencing_files/lane2.spring
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_file_join_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_version_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/store/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/handlers/test_createhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/handlers/test_readhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/test_include.py
```

### Comparing `housekeeper-4.2.1/LICENSE` & `housekeeper-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/PKG-INFO` & `housekeeper-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.2.1
+Version: 4.3.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.2.1/README.md` & `housekeeper-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/add.py` & `housekeeper-4.3.0/housekeeper/cli/add.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/core.py` & `housekeeper-4.3.0/housekeeper/cli/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/delete.py` & `housekeeper-4.3.0/housekeeper/cli/delete.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/get.py` & `housekeeper-4.3.0/housekeeper/cli/get.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/include.py` & `housekeeper-4.3.0/housekeeper/cli/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/init.py` & `housekeeper-4.3.0/housekeeper/cli/init.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/cli/tables.py` & `housekeeper-4.3.0/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/date.py` & `housekeeper-4.3.0/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/files.py` & `housekeeper-4.3.0/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/include.py` & `housekeeper-4.3.0/housekeeper/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/store/api/core.py` & `housekeeper-4.3.0/housekeeper/store/api/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/store/api/handlers/create.py` & `housekeeper-4.3.0/housekeeper/store/api/handlers/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import logging
 from pathlib import Path
 from typing import Dict, List, Tuple
 from sqlalchemy.orm import Session
 
-from housekeeper.store import models
+from housekeeper.store.models import Archive, Bundle, File, Tag, Version
 from housekeeper.store.api.handlers.base import BaseHandler
 from housekeeper.store.api.handlers.read import ReadHandler
 
 LOG = logging.getLogger(__name__)
 
 
 class CreateHandler(BaseHandler):
@@ -20,21 +20,21 @@
         super().__init__(session=session)
         CreateHandler.get_bundle_by_name = ReadHandler.get_bundle_by_name
         CreateHandler.get_tag = ReadHandler.get_tag
         CreateHandler.get_version_by_date_and_bundle_name = (
             ReadHandler.get_version_by_date_and_bundle_name
         )
 
-    def new_bundle(self, name: str, created_at: dt.datetime = None) -> models.Bundle:
+    def new_bundle(self, name: str, created_at: dt.datetime = None) -> Bundle:
         """Create a new file bundle."""
         new_bundle = self.Bundle(name=name, created_at=created_at)
         LOG.info("Created new bundle: %s", new_bundle.name)
         return new_bundle
 
-    def add_bundle(self, data: dict) -> Tuple[models.Bundle, models.Version]:
+    def add_bundle(self, data: dict) -> Tuple[Bundle, Version]:
         """Build a new bundle version of files.
 
         The format of the input dict is defined in the `schema` module.
         """
         bundle_obj = self.get_bundle_by_name(bundle_name=data["name"])
         # These lines can be removed when decoupled from CG
         created_at = data.get("created_at", data.get("created"))
@@ -50,17 +50,15 @@
 
         version_obj = self.new_version(created_at=created_at, expires_at=expires_at)
         self._add_files_to_version(data["files"], version_obj)
 
         version_obj.bundle = bundle_obj
         return bundle_obj, version_obj
 
-    def _add_files_to_version(
-        self, files: List[dict], version_obj: models.Version
-    ) -> None:
+    def _add_files_to_version(self, files: List[dict], version_obj: Version) -> None:
         """Create file objects and the tags and add them to a version object"""
 
         tag_names = set(
             tag_name for file_data in files for tag_name in file_data["tags"]
         )
         tag_map = self._build_tags(tag_names)
 
@@ -78,25 +76,25 @@
                 new_file = self.new_file(
                     path, to_archive=file_data["archive"], tags=tags
                 )
                 version_obj.files.append(new_file)
 
     def new_version(
         self, created_at: dt.datetime, expires_at: dt.datetime = None
-    ) -> models.Version:
+    ) -> Version:
         """Create a new bundle version."""
         LOG.info("Created new version")
         new_version = self.Version(created_at=created_at, expires_at=expires_at)
         return new_version
 
     def add_version(
         self,
         data: dict,
-        bundle: models.Bundle,
-    ) -> models.Version:
+        bundle: Bundle,
+    ) -> Version:
         """Build a new version object and add it to an existing bundle"""
         created_at = data.get("created_at", data.get("created"))
         if self.get_version_by_date_and_bundle_name(
             version_date=created_at, bundle_name=bundle.name
         ):
             LOG.info("version of bundle already added")
             return None
@@ -110,31 +108,31 @@
 
         version_obj.bundle = bundle
         return version_obj
 
     def add_file(
         self,
         file_path: Path,
-        bundle: models.Bundle,
+        bundle: Bundle,
         to_archive: bool = False,
         tags: List[str] = None,
-    ) -> models.File:
+    ) -> File:
         """Build a new file object and add it to the latest version of an existing bundle"""
         version_obj = bundle.versions[0]
         tags = tags or []
         tag_objs = [tag_obj for tag_name, tag_obj in self._build_tags(tags).items()]
         new_file = self.new_file(
             path=str(file_path.absolute()),
             to_archive=to_archive,
             tags=tag_objs,
         )
         new_file.version = version_obj
         return new_file
 
-    def _build_tags(self, tag_names: List[str]) -> Dict[str, models.Tag]:
+    def _build_tags(self, tag_names: List[str]) -> Dict[str, Tag]:
         """Build a list of tag objects.
 
         Take a list of tags, if a tag does not exist create a new tag object.
         Map the tag name to a tag object and return a list of those
         """
         tags = {}
         for tag_name in tag_names:
@@ -146,19 +144,21 @@
         return tags
 
     def new_file(
         self,
         path: str,
         checksum: str = None,
         to_archive: bool = False,
-        tags: List[models.Tag] = None,
-    ) -> models.File:
+        tags: List[Tag] = None,
+    ) -> File:
         """Create a new file object based on the information given."""
-        new_file = self.File(
-            path=path, checksum=checksum, to_archive=to_archive, tags=tags
-        )
-        return new_file
+        return self.File(path=path, checksum=checksum, to_archive=to_archive, tags=tags)
 
-    def new_tag(self, name: str, category: str = None) -> models.Tag:
+    def new_tag(self, name: str, category: str = None) -> Tag:
         """Create a new tag object based on the information given."""
         new_tag = self.Tag(name=name, category=category)
         return new_tag
+
+    def create_archive(self, file_id: int, archiving_task_id: int) -> Archive:
+        """Creates an archive object to the given file, with the given archive task id."""
+        return Archive(file_id=file_id, archiving_task_id=archiving_task_id)
+
```

### Comparing `housekeeper-4.2.1/housekeeper/store/api/handlers/read.py` & `housekeeper-4.3.0/housekeeper/store/api/handlers/read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 This module handles finding things in the store/database
 """
 import datetime as dt
 import logging
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 from sqlalchemy.orm import Query, Session
 
 from housekeeper.store.filters.bundle_filters import BundleFilters, apply_bundle_filter
 from housekeeper.store.filters.file_filters import FileFilter, apply_file_filter
-from housekeeper.store.filters.file_tags_filters import (
-    FileTagFilter,
-    apply_file_tag_filter,
+from housekeeper.store.filters.file_filters import (
+    FileFilter,
+    apply_file_filter,
 )
 from housekeeper.store.filters.version_bundle_filters import (
     VersionBundleFilters,
     apply_version_bundle_filter,
 )
 from housekeeper.store.filters.version_filters import (
     VersionFilter,
     apply_version_filter,
 )
 from housekeeper.store.models import Bundle, File, Tag, Version
 from housekeeper.store.filters.tag_filters import TagFilter, apply_tag_filter
 
 from .base import BaseHandler
 
+
 LOG = logging.getLogger(__name__)
 
 
 class ReadHandler(BaseHandler):
     """Handler for searching the database"""
 
     def __init__(self, session: Session):
@@ -125,17 +126,17 @@
                 bundle_name=bundle_name,
             )
 
         if tag_names:
             formatted_tags = ",".join(tag_names)
             LOG.info(f"Fetching files with tags in [{formatted_tags}]")
 
-            query = apply_file_tag_filter(
-                files_tags=query.join(File.tags),
-                filter_functions=[FileTagFilter.FILTER_FILES_BY_TAGS],
+            query = apply_file_filter(
+                files=query.join(File.tags),
+                filter_functions=[FileFilter.FILTER_FILES_BY_TAGS],
                 tag_names=tag_names,
             )
 
         if version_id:
             LOG.info(f"Fetching files from version {version_id}")
             query = apply_version_filter(
                 versions=query.join(self.File.version),
@@ -173,7 +174,41 @@
     def get_files_not_on_disk(files: List[File]) -> List[File]:
         """Return list of files that are not on disk."""
         if not files:
             return []
 
         files_not_on_disk = [f for f in files if not Path(f.full_path).is_file()]
         return files_not_on_disk
+
+    def get_archived_files(self, bundle_name: str, tags: Optional[List]) -> List[File]:
+        """Returns all files in the given bundle, with the given tags, and are archived."""
+        files_filtered_on_bundle: Query = apply_bundle_filter(
+            bundles=self._get_join_file_tags_archive_query(),
+            bundle_name=bundle_name,
+            filter_functions=[BundleFilters.FILTER_BY_NAME],
+        )
+        return apply_file_filter(
+            files=files_filtered_on_bundle,
+            filter_functions=[
+                FileFilter.FILTER_FILES_BY_TAGS,
+                FileFilter.FILTER_FILES_BY_IS_ARCHIVED,
+            ],
+            is_archived=True,
+            tag_names=tags,
+        ).all()
+
+    def get_non_archived_files(self, bundle_name: str, tags: Optional[List]) -> List[File]:
+        """Returns all files in the given bundle, with the given tags, and are not archived."""
+        files_filtered_om_bundle: Query = apply_bundle_filter(
+            bundles=self._get_join_file_tags_archive_query(),
+            bundle_name=bundle_name,
+            filter_functions=[BundleFilters.FILTER_BY_NAME],
+        )
+        return apply_file_filter(
+            files=files_filtered_om_bundle,
+            filter_functions=[
+                FileFilter.FILTER_FILES_BY_TAGS,
+                FileFilter.FILTER_FILES_BY_IS_ARCHIVED,
+            ],
+            is_archived=False,
+            tag_names=tags,
+        ).all()
```

### Comparing `housekeeper-4.2.1/housekeeper/store/api/schema.py` & `housekeeper-4.3.0/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.3.0/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/store/filters/file_tags_filters.py` & `housekeeper-4.3.0/housekeeper/store/filters/tag_filters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 from enum import Enum
 from typing import Callable, List, Optional
 from sqlalchemy.orm import Query
-from sqlalchemy import func as sqlalchemy_func
+from housekeeper.store.models import Tag
 
-from housekeeper.store.models import File, Tag
 
+def filter_tag_by_name(tags: Query, tag_name: str) -> Query:
+    """Return tag by bundle name."""
+    return tags.filter(Tag.name == tag_name)
 
-def filter_files_by_tags(files_tags: Query, tag_names: List[str], **kwargs) -> Query:
-    """Filter files by tag_names."""
-    return (
-        files_tags.filter(Tag.name.in_(tag_names))
-        .group_by(File.id)
-        .having(sqlalchemy_func.count(Tag.name) == len(tag_names))
-    )
 
+class TagFilter(Enum):
+    """Define Tag filter functions."""
+    FILTER_BY_NAME: Callable = filter_tag_by_name
 
-class FileTagFilter(Enum):
-    """Define File Tag filter functions."""
 
-    FILTER_FILES_BY_TAGS: Callable = filter_files_by_tags
-
-
-def apply_file_tag_filter(
-    files_tags: Query,
-    filter_functions: List[Callable],
-    tag_names: Optional[List[str]] = None,
-) -> Query:
-    """Apply filtering functions and return filtered query."""
+def apply_tag_filter(tags: Query, filter_functions: List[Callable],
+                     tag_name: Optional[str] = None, ) -> Query:
+    """Apply filtering functions to tag and return filtered Query."""
     for filter_function in filter_functions:
-        files_tags: Query = filter_function(files_tags=files_tags, tag_names=tag_names)
-    return files_tags
+        tags: Query = filter_function(
+            tags=tags,
+            tag_name=tag_name,
+        )
+    return tags
```

### Comparing `housekeeper-4.2.1/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.3.0/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/store/filters/version_filters.py` & `housekeeper-4.3.0/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper/store/models.py` & `housekeeper-4.3.0/housekeeper/store/models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/housekeeper.egg-info/PKG-INFO` & `housekeeper-4.3.0/housekeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.2.1
+Version: 4.3.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.2.1/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.3.0/housekeeper.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 housekeeper/store/api/handlers/__init__.py
 housekeeper/store/api/handlers/base.py
 housekeeper/store/api/handlers/create.py
 housekeeper/store/api/handlers/read.py
 housekeeper/store/filters/__init__.py
 housekeeper/store/filters/bundle_filters.py
 housekeeper/store/filters/file_filters.py
-housekeeper/store/filters/file_tags_filters.py
 housekeeper/store/filters/tag_filters.py
 housekeeper/store/filters/version_bundle_filters.py
 housekeeper/store/filters/version_filters.py
 tests/__init__.py
 tests/conftest.py
 tests/helper_functions.py
 tests/test_date.py
@@ -62,22 +61,24 @@
 tests/cli/delete/test_cli_delete_files.py
 tests/cli/delete/test_cli_delete_version.py
 tests/cli/get/test_get_bundle.py
 tests/cli/get/test_get_files.py
 tests/cli/get/test_get_tag.py
 tests/cli/get/test_get_version.py
 tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+tests/fixtures/sequencing_files/lane1.spring
+tests/fixtures/sequencing_files/lane2.spring
 tests/fixtures/vcfs/example.2.vcf
 tests/fixtures/vcfs/example.vcf
 tests/fixtures/vcfs/family.2.vcf
 tests/fixtures/vcfs/family.3.vcf
 tests/fixtures/vcfs/family.vcf
 tests/store/conftest.py
 tests/store/test_models.py
 tests/store/filters/test_bundle_filters.py
 tests/store/filters/test_file_filters.py
-tests/store/filters/test_file_tag_filters.py
+tests/store/filters/test_file_join_filters.py
 tests/store/filters/test_tag_filters.py
 tests/store/filters/test_version_bundle_filters.py
 tests/store/filters/test_version_filters.py
 tests/store/handlers/test_createhandler.py
 tests/store/handlers/test_readhandler.py
```

### Comparing `housekeeper-4.2.1/setup.py` & `housekeeper-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.2.1",
+    version="4.3.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.2.1/tests/cli/add/conftest.py` & `housekeeper-4.3.0/tests/cli/add/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.3.0/tests/cli/add/test_cli_add_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.3.0/tests/cli/add/test_cli_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.3.0/tests/cli/add/test_cli_add_tags.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.3.0/tests/cli/add/test_cli_add_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/conftest.py` & `housekeeper-4.3.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/get/test_get_bundle.py` & `housekeeper-4.3.0/tests/cli/get/test_get_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/get/test_get_files.py` & `housekeeper-4.3.0/tests/cli/get/test_get_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/get/test_get_tag.py` & `housekeeper-4.3.0/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/get/test_get_version.py` & `housekeeper-4.3.0/tests/cli/get/test_get_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/test_cli_core.py` & `housekeeper-4.3.0/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/cli/test_cli_include.py` & `housekeeper-4.3.0/tests/cli/test_cli_include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/conftest.py` & `housekeeper-4.3.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 import yaml
 
 from housekeeper.date import get_date
-from housekeeper.store import Store, models
+from housekeeper.store import Store
+from housekeeper.store.models import Archive, Bundle, Tag, Version
 
 from .helper_functions import Helpers
 
 
 # basic fixtures
 
+
 @pytest.fixture(scope="function", name="helpers")
 def fixture_helpers() -> Helpers:
     """Return a test helper object."""
     return Helpers()
 
 
 @pytest.fixture(scope="function", name="vcf_tag_name")
@@ -56,14 +58,37 @@
 
 @pytest.fixture(scope="function", name="sample_tag_names")
 def fixture_sample_tag_names(vcf_tag_name: str, sample_tag_name: str) -> List[str]:
     """Return a list of the sample tag names."""
     return [vcf_tag_name, sample_tag_name]
 
 
+@pytest.fixture(scope="function", name="spring_tag")
+def fixture_spring_tag() -> str:
+    """Return the tag marking SPRING files."""
+    return "spring"
+
+
+@pytest.fixture(scope="function", name="sample_id")
+def fixture_sample_id() -> str:
+    """Return name of a sample."""
+    return "ACC123456A1"
+
+
+@pytest.fixture(scope="function", name="archiving_task_id")
+def fixture_archiving_task_id() -> int:
+    """Return an id of an archiving task."""
+    return 1234
+
+@pytest.fixture(scope="function", name="retrieval_task_id")
+def fixture_retrieval_task_id() -> int:
+    """Return an id of a retrieval task."""
+    return 4321
+
+
 @pytest.fixture(scope="function", name="case_id")
 def fixture_case_id() -> str:
     """Return name of a case."""
     return "handsomepig"
 
 
 @pytest.fixture(scope="function", name="other_case_id")
@@ -80,14 +105,30 @@
 
 @pytest.fixture(scope="function", name="sample2_data")
 def fixture_sample2_data(sample_tag_names: List[str], second_sample_vcf: Path) -> dict:
     """Return file and tags for sample."""
     return {"tags": sample_tag_names, "file": second_sample_vcf}
 
 
+@pytest.fixture(scope="function", name="spring_file_1_with_tags")
+def fixture_spring_file_1_with_tags(
+    sample_id: str, spring_tag: str, spring_file_1: Path
+) -> dict:
+    """Return spring file and tags for a sample."""
+    return {"tags": [sample_id, spring_tag], "file": spring_file_1}
+
+
+@pytest.fixture(scope="function", name="spring_file_2_with_tags")
+def fixture_spring_file_2_with_tags(
+    sample_id: str, spring_tag: str, spring_file_2: Path
+) -> dict:
+    """Return a second spring file and tags for a sample."""
+    return {"tags": [sample_id, spring_tag], "file": spring_file_2}
+
+
 @pytest.fixture(scope="function", name="family_data")
 def fixture_family_data(family_tag_names: List[str], family_vcf: Path) -> dict:
     """Return file and tags for sample."""
     return {"tags": family_tag_names, "file": family_vcf}
 
 
 @pytest.fixture(scope="function", name="family2_data")
@@ -118,30 +159,57 @@
 def fixture_later_timestamp() -> datetime.datetime:
     """Return a time stamp in date time format to a later date."""
     return datetime.datetime(2020, 5, 25)
 
 
 @pytest.fixture(scope="function", name="bundle_data")
 def fixture_bundle_data(
-    case_id: str, sample_data: dict, family_data: dict, timestamp: datetime.datetime, helpers: Helpers
+    case_id: str,
+    sample_data: dict,
+    family_data: dict,
+    timestamp: datetime.datetime,
+    helpers: Helpers,
 ) -> dict:
     """Return a bundle."""
-    data = helpers.create_bundle_data(case_id=case_id, files=[family_data, sample_data], created_at=timestamp)
+    data = helpers.create_bundle_data(
+        case_id=case_id, files=[family_data, sample_data], created_at=timestamp
+    )
     return data
 
 
+@pytest.fixture(scope="function", name="sample_bundle_data")
+def fixture_sample_bundle_data(
+    sample_id: str,
+    sample_data: dict,
+    spring_file_1_with_tags: dict,
+    spring_file_2_with_tags: dict,
+    timestamp: datetime.datetime,
+    helpers: Helpers,
+) -> dict:
+    """Return a bundle containing mock sequencing files."""
+    return helpers.create_bundle_data(
+        case_id=sample_id,
+        files=[spring_file_1_with_tags, spring_file_2_with_tags],
+        created_at=timestamp,
+    )
+
+
 @pytest.fixture(scope="function", name="empty_version_data")
-def fixture_empty_version_data(later_timestamp: datetime.datetime, case_id: str) -> dict:
+def fixture_empty_version_data(
+    later_timestamp: datetime.datetime, case_id: str
+) -> dict:
     """Return a dummy bundle."""
     data = {"bundle_name": case_id, "created_at": later_timestamp, "files": []}
     return data
 
 
 @pytest.fixture(scope="function", name="version_data")
-def fixture_version_data(empty_version_data: dict, family2_data: dict, sample2_data: dict) -> dict:
+def fixture_version_data(
+    empty_version_data: dict, family2_data: dict, sample2_data: dict
+) -> dict:
     """Return a dummy bundle."""
     data = copy.deepcopy(empty_version_data)
     data["files"] = [
         {
             "path": str(sample2_data["file"]),
             "archive": False,
             "tags": sample2_data["tags"],
@@ -177,19 +245,19 @@
     json_data = copy.deepcopy(version_data)
     json_data["created_at"] = str(json_data.pop("created_at"))
     return json.dumps(json_data)
 
 
 @pytest.fixture(scope="function", name="other_bundle")
 def fixture_other_bundle(
-        bundle_data: dict,
-        other_case_id: str,
-        later_timestamp: datetime.datetime,
-        second_sample_vcf: Path,
-        second_family_vcf: Path,
+    bundle_data: dict,
+    other_case_id: str,
+    later_timestamp: datetime.datetime,
+    second_sample_vcf: Path,
+    second_family_vcf: Path,
 ) -> dict:
     """Return a dummy bundle."""
     data = deepcopy(bundle_data)
     data["name"] = other_case_id
     data["created_at"] = later_timestamp
     data["files"][0]["path"] = str(second_sample_vcf)
     data["files"][1]["path"] = str(second_family_vcf)
@@ -229,28 +297,39 @@
 
 # object fixtures
 
 
 @pytest.fixture(scope="function", name="vcf_tag_obj")
 def fixture_vcf_tag_obj(vcf_tag_name: str, timestamp: datetime.datetime) -> str:
     """Return a tag object."""
-    return models.Tag(name=vcf_tag_name, created_at=timestamp)
+    return Tag(name=vcf_tag_name, created_at=timestamp)
 
 
 @pytest.fixture(scope="function", name="bundle_obj")
-def fixture_bundle_obj(bundle_data: dict, store: Store) -> models.Bundle:
+def fixture_bundle_obj(bundle_data: dict, store: Store) -> Bundle:
     """Return a bundle object."""
     return store.add_bundle(bundle_data)[0]
 
 
+@pytest.fixture(scope="function", name="sample_bundle")
+def fixture_sample_bundle(sample_bundle_data: dict, store: Store) -> Bundle:
+    """Return a bundle object."""
+    return store.add_bundle(sample_bundle_data)[0]
+
+
 @pytest.fixture(scope="function", name="version_obj")
-def fixture_version_obj(bundle_data: dict, store: Store) -> models.Version:
+def fixture_version_obj(bundle_data: dict, store: Store) -> Version:
     """Return a version object."""
     return store.add_bundle(bundle_data)[1]
 
+@pytest.fixture(scope="function", name="archive")
+def fixture_archive(populated_store: Store) -> Archive:
+    """Return an archive object."""
+    return populated_store._get_query(table=Archive).first()
+
 
 # dir fixtures
 
 
 @pytest.fixture(scope="function", name="fixtures_dir")
 def fixture_fixtures_dir() -> Path:
     """Return the path to the fixtures directory."""
@@ -259,14 +338,20 @@
 
 @pytest.fixture(scope="function", name="vcf_dir")
 def fixture_vcf_dir(fixtures_dir: Path) -> Path:
     """Return the path to the vcf fixtures directory."""
     return fixtures_dir / "vcfs"
 
 
+@pytest.fixture(scope="function", name="sequencing_files_dir")
+def fixture_sequencing_files_dir(fixtures_dir: Path) -> Path:
+    """Return the path to the sequencing_files fixtures directory."""
+    return Path(fixtures_dir, "sequencing_files")
+
+
 @pytest.fixture(scope="function", name="project_dir")
 def fixture_project_dir(tmpdir_factory) -> Path:
     """Path to a temporary working directory."""
     my_tmpdir = Path(tmpdir_factory.mktemp("workdir"))
     yield my_tmpdir
     shutil.rmtree(str(my_tmpdir))
 
@@ -298,68 +383,110 @@
         yaml.dump(configs, out_file)
     return conf_path
 
 
 @pytest.fixture(scope="function", name="sample_vcf")
 def fixture_sample_vcf(vcf_dir: Path) -> Path:
     """Return the path to a vcf file."""
-    return vcf_dir / "example.vcf"
+    return Path(vcf_dir, "example.vcf")
+
+
+@pytest.fixture(scope="function", name="spring_file_1")
+def fixture_spring_file_1(sequencing_files_dir: Path) -> Path:
+    """Return the path to a SPRING file."""
+    return Path(sequencing_files_dir, "lane1.spring")
+
+
+@pytest.fixture(scope="function", name="spring_file_2")
+def fixture_spring_file_2(sequencing_files_dir: Path) -> Path:
+    """Return the path to a SPRING file."""
+    return Path(sequencing_files_dir, "lane2.spring")
+
+@pytest.fixture(scope="function", name="archived_file")
+def fixture_archived_file(spring_file_1: Path) -> Path:
+    """Return the path to an archived file."""
+    return spring_file_1
+
+@pytest.fixture(scope="function", name="non_archived_file")
+def fixture_non_archived_file(spring_file_2: Path) -> Path:
+    """Return the path to a non-archived file."""
+    return spring_file_2
+
+@pytest.fixture(scope="function", name="spring_file_2")
+def fixture_spring_file_2(sequencing_files_dir: Path) -> Path:
+    """Return the path to a SPRING file."""
+    return Path(sequencing_files_dir, "lane2.spring")
 
 
 @pytest.fixture(scope="function", name="family_vcf")
 def fixture_family_vcf(vcf_dir: Path) -> Path:
     """Return the path to a vcf file."""
-    return vcf_dir / "family.vcf"
+    return Path(vcf_dir, "family.vcf")
 
 
 @pytest.fixture(scope="function", name="second_sample_vcf")
 def fixture_second_sample_vcf(vcf_dir: Path) -> Path:
     """Return the path to a vcf file."""
-    return vcf_dir / "example.2.vcf"
+    return Path(vcf_dir, "example.2.vcf")
 
 
 @pytest.fixture(scope="function", name="second_family_vcf")
 def fixture_second_family_vcf(vcf_dir: Path) -> Path:
     """Return the path to a vcf file."""
-    return vcf_dir / "family.2.vcf"
+    return Path(vcf_dir, "family.2.vcf")
 
 
 @pytest.fixture(scope="function", name="third_family_vcf")
 def fixture_third_family_vcf(vcf_dir: Path) -> Path:
     """Return the path to a vcf file."""
-    return vcf_dir / "family.3.vcf"
+    return Path(vcf_dir, "family.3.vcf")
 
 
 @pytest.fixture(scope="function", name="checksum_file")
 def fixture_checksum_file(fixtures_dir: Path) -> Path:
     """Return the path to file to test checksum."""
-    return fixtures_dir / "26a90105b99c05381328317f913e9509e373b64f.txt"
+    return Path(fixtures_dir, "26a90105b99c05381328317f913e9509e373b64f.txt")
 
 
 @pytest.fixture(scope="function", name="checksum")
 def fixture_checksum(checksum_file: Path) -> Path:
     """Return the checksum for checksum test file."""
     return checksum_file.name.rstrip(".txt")
 
 
 @pytest.fixture(scope="function", name="helpers")
 def fixture_helpers() -> Helpers:
     """Return a test helper object."""
     return Helpers()
 
+
 # Store fixtures
 
 
 @pytest.fixture(scope="function", name="store")
 def fixture_store(project_dir: Path) -> Store:
     """Return a store setup with all tables."""
     _store = Store(uri="sqlite:///", root=str(project_dir))
     _store.create_all()
     yield _store
     _store.drop_all()
 
 
 @pytest.fixture(scope="function", name="populated_store")
-def fixture_populated_store(store: Store, bundle_data: dict, helpers: Helpers) -> Store:
+def fixture_populated_store(
+    archiving_task_id: int,
+    bundle_data: dict,
+    helpers: Helpers,
+    sample_bundle_data: dict,
+    spring_file_1: Path,
+    store: Store,
+) -> Store:
     """Returns a populated store."""
-    helpers.add_bundle(store, bundle_data)
+    helpers.add_bundle(store=store, bundle=bundle_data)
+    helpers.add_bundle(store=store, bundle=sample_bundle_data)
+    helpers.add_archive(
+        store=store,
+        file_id=store.get_files(file_path=spring_file_1.as_posix()).first().id,
+        archiving_task_id=archiving_task_id,
+    )
+
     return store
```

### Comparing `housekeeper-4.2.1/tests/helper_functions.py` & `housekeeper-4.3.0/tests/helper_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import datetime as dt
 import json
 from pathlib import Path
 from typing import Iterable, List
 
 from housekeeper.constants import LOGLEVELS
 from housekeeper.store import Store
+from housekeeper.store.models import Archive
 
 
 class Helpers:
     """Hold small methods that might be helpful for the tests"""
 
     @staticmethod
     def count_iterable(iter_obj: Iterable) -> int:
@@ -38,14 +39,23 @@
     def add_bundle(store: Store, bundle: dict) -> None:
         """Add and commit bundle to housekeeper store"""
         bundle_obj, _ = store.add_bundle(bundle)
         store.session.add(bundle_obj)
         store.session.commit()
 
     @staticmethod
+    def add_archive(store: Store, file_id: int, archiving_task_id:int=1234) -> None:
+        """Adds an archive object to the database."""
+        new_archive: Archive = store.create_archive(
+            file_id=file_id, archiving_task_id=archiving_task_id
+        )
+        store.session.add(new_archive)
+        store.session.commit()
+
+    @staticmethod
     def create_bundle_data(
         case_id: str, files: List[dict], created_at: dt.datetime = None
     ) -> dict:
         """
         Create a new bundle_data dictionary with the given parameters.
 
         :param case_id: The name of the bundle.
```

### Comparing `housekeeper-4.2.1/tests/store/conftest.py` & `housekeeper-4.3.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/store/filters/test_bundle_filters.py` & `housekeeper-4.3.0/tests/store/filters/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/store/filters/test_file_filters.py` & `housekeeper-4.3.0/tests/store/filters/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/store/filters/test_file_tag_filters.py` & `housekeeper-4.3.0/tests/store/filters/test_file_join_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from typing import List
+
+from sqlalchemy.orm import Query
+
 from housekeeper.store.api.core import Store
-from housekeeper.store.filters.file_tags_filters import filter_files_by_tags
+from housekeeper.store.filters.file_filters import (
+    filter_files_by_tags,
+    filter_files_by_is_archived,
+)
 from housekeeper.store.models import File
 
 
 def test_filter_files_by_tags_returns_correct_files(populated_store: Store):
     """Test filtering files by tags."""
 
     # GIVEN a store with files
     file: File = populated_store._get_query(table=File).first()
     tag_names: List[str] = [tag.name for tag in file.tags]
 
     # WHEN filtering files by tags
     filtered_files_query = filter_files_by_tags(
-        files_tags=populated_store._get_join_file_tag_query(),
+        files=populated_store._get_join_file_tag_query(),
         tag_names=tag_names,
     )
 
     filtered_files: List[File] = filtered_files_query.all()
 
     # THEN each file should have all the requested tags
     for filtered_file in filtered_files:
@@ -26,18 +32,50 @@
 
 def test_filter_files_by_tags_returns_empty_list_when_no_files_match_tags(
     populated_store: Store,
 ):
     """Test filtering files by tags when no files match the given tags."""
 
     # GIVEN a store with files
-    # create a tag that does not exist in any files in the store
+    # GIVEN a tag that does not exist in any files in the store
     tag_name = "nonexistent_tag"
 
     # WHEN filtering files by the nonexistent tag
     filtered_files_query = filter_files_by_tags(
-        files_tags=populated_store._get_join_file_tag_query(),
+        files=populated_store._get_join_file_tag_query(),
         tag_names=[tag_name],
     )
 
     # THEN the filtered files list should be empty
     assert len(filtered_files_query.all()) == 0
+
+
+def test_filter_files_by_archive_true(populated_store: Store):
+    """Tests the filtering for archived files."""
+
+    # GIVEN as store with files
+
+    # WHEN filtering on archived files
+    archived_files_query: Query = filter_files_by_is_archived(
+        files=populated_store._get_join_file_tags_archive_query(),
+        is_archived=True,
+    )
+
+    # THEN all files returned should have an archive object linked to it
+    for file in archived_files_query:
+        assert file.archive
+
+
+def test_filter_files_by_archive_false(populated_store: Store):
+    """Tests the filtering for non-archived files."""
+
+    # GIVEN as store with files
+
+    # WHEN filtering on non-archived files
+    archived_files_query: Query = filter_files_by_is_archived(
+        files=populated_store._get_join_file_tags_archive_query(),
+        is_archived=False,
+    )
+
+    # THEN none of the files returned should have an archive object linked to it
+    for file in archived_files_query:
+        assert file.archive is None
```

### Comparing `housekeeper-4.2.1/tests/store/filters/test_tag_filters.py` & `housekeeper-4.3.0/tests/store/filters/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/store/filters/test_version_bundle_filters.py` & `housekeeper-4.3.0/tests/store/filters/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/store/filters/test_version_filters.py` & `housekeeper-4.3.0/tests/store/filters/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/store/handlers/test_createhandler.py` & `housekeeper-4.3.0/tests/store/handlers/test_createhandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Tests for store core functions."""
 from pathlib import Path
 from typing import List
 
+import pytest
+from sqlalchemy.exc import IntegrityError
+
 from housekeeper.store.api import schema
-from housekeeper.store.models import Bundle, File, Tag, Version
 from housekeeper.store.api.core import Store
+from housekeeper.store.models import Bundle, File, Tag, Version, Archive
 
 
 def test_schema_with_invalid_input(bundle_data_json):
     """Tests that errors are thrown when validating incorrect input data."""
     # GIVEN input data with missing name of the bundle
     del bundle_data_json["name"]
     # WHEN validating it against the schema
@@ -103,31 +106,69 @@
     assert store._get_query(table=Bundle).count() > 0
     # WHEN adding the same bundle again
     new_bundle = store.add_bundle(bundle_data)
     # THEN it should return None
     assert new_bundle is None
 
 
-def test_add_two_versions_of_bundle(populated_store: Store, second_bundle_data):
+def test_add_two_versions_of_bundle(populated_store: Store, second_bundle_data: dict):
     """Test to add two versions of the same bundle."""
     store: Store = populated_store
     # GIVEN a populated store and some modified bundle data
-    assert store._get_query(table=Bundle).count() > 0
+    starting_bundle_count: int = store._get_query(table=Bundle).count()
+    starting_version_count: int = store._get_query(table=Version).count()
+    starting_file_count: int = store._get_query(table=File).count()
 
     # WHEN adding the modified bundle to the database
     new_bundle_obj = store.add_bundle(second_bundle_data)[0]
     store.session.add(new_bundle_obj)
     store.session.commit()
 
-    # THEN there should still be one bundle
-    assert store._get_query(table=Bundle).count() == 1
-    # THEN there should be two versions
-    assert store._get_query(table=Version).count() == 2
-    # THEN tere should be all four files
-    assert store._get_query(table=File).count() == 4
+    # THEN there should still be the same number of bundles
+    assert store._get_query(table=Bundle).count() == starting_bundle_count
+    # THEN there should be one more version
+    assert store._get_query(table=Version).count() == starting_version_count + 1
+    # THEN there should be two more files
+    assert store._get_query(table=File).count() == starting_file_count + 2
+
+
+def test_add_archive(archiving_task_id: int, populated_store: Store, spring_file_2: Path):
+    """Test that adding an archive works as expected."""
+    # GIVEN a file that is not archived
+    non_archived_file: File = populated_store.get_files(
+        file_path=spring_file_2.as_posix()
+    ).first()
+    # WHEN adding an archive
+    new_archive: Archive = populated_store.create_archive(
+        file_id=non_archived_file.id, archiving_task_id=archiving_task_id
+    )
+    populated_store.session.add(new_archive)
+    populated_store.session.commit()
+    # THEN an archive should be created
+    assert isinstance(new_archive, Archive)
+    # THEN the archive should be reachable via the file
+    assert non_archived_file.archive == new_archive
+
+
+def test_add_archive_to_archived_file(archiving_task_id: int, populated_store: Store,
+                                      spring_file_1: Path):
+    """Test that adding an archive to an already archived file raises an error."""
+    # GIVEN a file that is archived
+    non_archived_file: File = populated_store.get_files(
+        file_path=spring_file_1.as_posix()
+    ).first()
+    # WHEN adding an archive
+    new_archive: Archive = populated_store.create_archive(
+        file_id=non_archived_file.id, archiving_task_id=archiving_task_id
+    )
+    populated_store.session.add(new_archive)
+
+    # THEN an SQLAlchemy error should be thrown
+    with pytest.raises(IntegrityError):
+        populated_store.session.commit()
 
 
 def test_add_file(
     populated_store: Store, second_family_vcf: Path, family_tag_names: List[str]
 ):
     """Test to create a file with the add file method."""
     # GIVEN the path and the tags for a file
```

### Comparing `housekeeper-4.2.1/tests/store/test_models.py` & `housekeeper-4.3.0/tests/store/test_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/test_date.py` & `housekeeper-4.3.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.2.1/tests/test_include.py` & `housekeeper-4.3.0/tests/test_include.py`

 * *Files identical despite different names*


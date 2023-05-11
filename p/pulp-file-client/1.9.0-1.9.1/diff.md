# Comparing `tmp/pulp_file-client-1.9.0.tar.gz` & `tmp/pulp_file-client-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_file-client-1.9.0.tar", last modified: Thu Aug 26 16:47:35 2021, max compression
+gzip compressed data, was "pulp_file-client-1.9.1.tar", last modified: Mon Aug 30 14:44:14 2021, max compression
```

## Comparing `pulp_file-client-1.9.0.tar` & `pulp_file-client-1.9.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.032414 pulp_file-client-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-08-26 16:47:35.032414 pulp_file-client-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10889 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.020414 pulp_file-client-1.9.0/pulp_file_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulp_file_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4575 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulp_file_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulp_file_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulp_file_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulp_file_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.020414 pulp_file-client-1.9.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.020414 pulp_file-client-1.9.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.020414 pulp_file-client-1.9.0/pulpcore/client/pulp_file/
--rw-r--r--   0 runner    (1001) docker     (121)     4612 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.024414 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/
--rw-r--r--   0 runner    (1001) docker     (121)      658 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    47765 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/acs_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    21803 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/content_files_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    41836 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/distributions_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28430 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/publications_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    42275 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/remotes_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    52078 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/repositories_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    31997 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/repositories_file_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26279 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13957 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.028414 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5172 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     8389 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6292 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_content.py
--rw-r--r--   0 runner    (1001) docker     (121)    10854 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_content_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     8117 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    10895 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_publication.py
--rw-r--r--   0 runner    (1001) docker     (121)     8114 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    23229 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    22286 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    12956 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5630 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5745 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6332 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     8000 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    23538 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     9393 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6397 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7916 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (121)    12312 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/pulpcore/client/pulp_file/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-08-26 16:47:35.032414 pulp_file-client-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 16:47:35.032414 pulp_file-client-1.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_acs_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_content_files_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_content_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_distributions_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_alternate_content_source_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_content_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_publication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_file_file_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginatedfile_file_alternate_content_source_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2483 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginatedfile_file_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginatedfile_file_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginatedfile_file_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginatedfile_file_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_paginatedfile_file_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_patchedfile_file_alternate_content_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_patchedfile_file_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_patchedfile_file_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_patchedfile_file_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_publications_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_remotes_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_repositories_file_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_repositories_file_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_repository_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-08-26 16:47:34.000000 pulp_file-client-1.9.0/test/test_repository_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.218270 pulp_file-client-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-08-30 14:44:14.218270 pulp_file-client-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10889 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.202270 pulp_file-client-1.9.1/pulp_file_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-08-30 14:44:14.000000 pulp_file-client-1.9.1/pulp_file_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4575 2021-08-30 14:44:14.000000 pulp_file-client-1.9.1/pulp_file_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-30 14:44:14.000000 pulp_file-client-1.9.1/pulp_file_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-08-30 14:44:14.000000 pulp_file-client-1.9.1/pulp_file_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-30 14:44:14.000000 pulp_file-client-1.9.1/pulp_file_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.202270 pulp_file-client-1.9.1/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.202270 pulp_file-client-1.9.1/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.206270 pulp_file-client-1.9.1/pulpcore/client/pulp_file/
+-rw-r--r--   0 runner    (1001) docker     (121)     4612 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.210270 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47765 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/acs_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21803 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/content_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41836 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/distributions_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28430 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/publications_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42275 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/remotes_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52078 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/repositories_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31997 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/repositories_file_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26279 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13957 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.214270 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     3528 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5172 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5300 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6502 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8389 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6292 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10854 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8117 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10895 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5324 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8114 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23229 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22286 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9323 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12956 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5676 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5630 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5745 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5722 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5699 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6332 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8000 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23538 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9393 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2860 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6397 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4482 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7916 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12312 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/pulpcore/client/pulp_file/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-08-30 14:44:14.218270 pulp_file-client-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 14:44:14.218270 pulp_file-client-1.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1727 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_acs_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_content_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_distributions_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_alternate_content_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1742 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2262 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_file_file_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginatedfile_file_alternate_content_source_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2483 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginatedfile_file_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginatedfile_file_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginatedfile_file_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginatedfile_file_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2672 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_paginatedfile_file_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_patchedfile_file_alternate_content_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_patchedfile_file_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_patchedfile_file_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_patchedfile_file_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_publications_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_remotes_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_repositories_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_repositories_file_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-08-30 14:44:13.000000 pulp_file-client-1.9.1/test/test_repository_version_response.py
```

### Comparing `pulp_file-client-1.9.0/README.md` & `pulp_file-client-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_file-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_file-client-1.9.0/pulp_file_client.egg-info/SOURCES.txt` & `pulp_file-client-1.9.1/pulp_file_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/__init__.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 # import apis into sdk package
 from pulpcore.client.pulp_file.api.acs_file_api import AcsFileApi
 from pulpcore.client.pulp_file.api.content_files_api import ContentFilesApi
 from pulpcore.client.pulp_file.api.distributions_file_api import DistributionsFileApi
 from pulpcore.client.pulp_file.api.publications_file_api import PublicationsFileApi
 from pulpcore.client.pulp_file.api.remotes_file_api import RemotesFileApi
```

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/__init__.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/acs_file_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/acs_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/content_files_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/content_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/distributions_file_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/distributions_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/publications_file_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/publications_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/remotes_file_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/remotes_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/repositories_file_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/repositories_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api/repositories_file_versions_api.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api/repositories_file_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/api_client.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.9.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.9.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/configuration.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 1.9.0".\
+               "SDK Package Version: 1.9.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/exceptions.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/__init__.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/async_operation_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/content_summary.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/content_summary_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_alternate_content_source_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_content.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_content_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_distribution.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_distribution_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_publication.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_publication_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_remote.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_remote_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_repository.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/file_file_repository_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/file_file_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_alternate_content_source_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/paginatedfile_file_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_remote.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/patchedfile_file_repository.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/patchedfile_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/policy_enum.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_add_remove_content.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_sync_url.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_version.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/models/repository_version_response.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/pulpcore/client/pulp_file/rest.py` & `pulp_file-client-1.9.1/pulpcore/client/pulp_file/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/setup.py` & `pulp_file-client-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_file-client"
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_file-client-1.9.0/test/test_acs_file_api.py` & `pulp_file-client-1.9.1/test/test_acs_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_async_operation_response.py` & `pulp_file-client-1.9.1/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_content_files_api.py` & `pulp_file-client-1.9.1/test/test_content_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_content_summary.py` & `pulp_file-client-1.9.1/test/test_content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_content_summary_response.py` & `pulp_file-client-1.9.1/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_distributions_file_api.py` & `pulp_file-client-1.9.1/test/test_distributions_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_alternate_content_source.py` & `pulp_file-client-1.9.1/test/test_file_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_alternate_content_source_response.py` & `pulp_file-client-1.9.1/test/test_file_file_alternate_content_source_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_content.py` & `pulp_file-client-1.9.1/test/test_file_file_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_content_response.py` & `pulp_file-client-1.9.1/test/test_file_file_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_distribution.py` & `pulp_file-client-1.9.1/test/test_file_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_distribution_response.py` & `pulp_file-client-1.9.1/test/test_file_file_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_publication.py` & `pulp_file-client-1.9.1/test/test_file_file_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_publication_response.py` & `pulp_file-client-1.9.1/test/test_file_file_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_remote.py` & `pulp_file-client-1.9.1/test/test_file_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_remote_response.py` & `pulp_file-client-1.9.1/test/test_file_file_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_repository.py` & `pulp_file-client-1.9.1/test/test_file_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_file_file_repository_response.py` & `pulp_file-client-1.9.1/test/test_file_file_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginated_repository_version_response_list.py` & `pulp_file-client-1.9.1/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginatedfile_file_alternate_content_source_response_list.py` & `pulp_file-client-1.9.1/test/test_paginatedfile_file_alternate_content_source_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginatedfile_file_content_response_list.py` & `pulp_file-client-1.9.1/test/test_paginatedfile_file_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginatedfile_file_distribution_response_list.py` & `pulp_file-client-1.9.1/test/test_paginatedfile_file_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginatedfile_file_publication_response_list.py` & `pulp_file-client-1.9.1/test/test_paginatedfile_file_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginatedfile_file_remote_response_list.py` & `pulp_file-client-1.9.1/test/test_paginatedfile_file_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_paginatedfile_file_repository_response_list.py` & `pulp_file-client-1.9.1/test/test_paginatedfile_file_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_patchedfile_file_alternate_content_source.py` & `pulp_file-client-1.9.1/test/test_patchedfile_file_alternate_content_source.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_patchedfile_file_distribution.py` & `pulp_file-client-1.9.1/test/test_patchedfile_file_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_patchedfile_file_remote.py` & `pulp_file-client-1.9.1/test/test_patchedfile_file_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_patchedfile_file_repository.py` & `pulp_file-client-1.9.1/test/test_patchedfile_file_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_policy_enum.py` & `pulp_file-client-1.9.1/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_publications_file_api.py` & `pulp_file-client-1.9.1/test/test_publications_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_remotes_file_api.py` & `pulp_file-client-1.9.1/test/test_remotes_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_repositories_file_api.py` & `pulp_file-client-1.9.1/test/test_repositories_file_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_repositories_file_versions_api.py` & `pulp_file-client-1.9.1/test/test_repositories_file_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_repository_add_remove_content.py` & `pulp_file-client-1.9.1/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_repository_sync_url.py` & `pulp_file-client-1.9.1/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_repository_version.py` & `pulp_file-client-1.9.1/test/test_repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_file-client-1.9.0/test/test_repository_version_response.py` & `pulp_file-client-1.9.1/test/test_repository_version_response.py`

 * *Files identical despite different names*


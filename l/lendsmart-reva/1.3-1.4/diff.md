# Comparing `tmp/lendsmart_reva-1.3.tar.gz` & `tmp/lendsmart_reva-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_reva-1.3.tar", last modified: Thu Dec 15 11:36:45 2022, max compression
+gzip compressed data, was "lendsmart_reva-1.4.tar", last modified: Thu May 11 12:31:41 2023, max compression
```

## Comparing `lendsmart_reva-1.3.tar` & `lendsmart_reva-1.4.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.879140 lendsmart_reva-1.3/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)       36 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/LICENSE
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     2823 2022-12-15 11:36:45.879140 lendsmart_reva-1.3/PKG-INFO
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     2442 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/README.md
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/lendsmart_reva.egg-info/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     2823 2022-12-15 11:36:45.000000 lendsmart_reva-1.3/lendsmart_reva.egg-info/PKG-INFO
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1678 2022-12-15 11:36:45.000000 lendsmart_reva-1.3/lendsmart_reva.egg-info/SOURCES.txt
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        1 2022-12-15 11:36:45.000000 lendsmart_reva-1.3/lendsmart_reva.egg-info/dependency_links.txt
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      414 2022-12-15 11:36:45.000000 lendsmart_reva-1.3/lendsmart_reva.egg-info/entry_points.txt
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      139 2022-12-15 11:36:45.000000 lendsmart_reva-1.3/lendsmart_reva.egg-info/requires.txt
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        5 2022-12-15 11:36:45.000000 lendsmart_reva-1.3/lendsmart_reva.egg-info/top_level.txt
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)       22 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     3528 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/cli.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/conf/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/conf/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      740 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/conf/reva.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      953 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/document_access_control.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      943 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/exception.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      954 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/info.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/__init__.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/base/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/base/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1101 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/base/base.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      948 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/base/run_query.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/client/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/client/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      399 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/client/builder.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     2926 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/client/graphql_client.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/document_access_control/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/document_access_control/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      728 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/document_access_control/main.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1599 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/document_access_control/update.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/graphql_queries/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/graphql_queries/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      806 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/graphql_queries/document_access_control.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      551 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/graphql_queries/loan_products.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      944 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/graphql_queries/roles_and_permissions.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      590 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/graphql_queries/site_settings.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      802 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/graphql_queries/workflow.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/loan_productus/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/loan_productus/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      642 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/loan_productus/main.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1482 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/loan_productus/update.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.875140 lendsmart_reva-1.3/reva/lib/roles_and_permissions/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/roles_and_permissions/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      687 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/roles_and_permissions/main.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1880 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/roles_and_permissions/update.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.879140 lendsmart_reva-1.3/reva/lib/site_settings/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/site_settings/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      639 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/site_settings/main.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1416 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/site_settings/update.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.879140 lendsmart_reva-1.3/reva/lib/utils/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/utils/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      433 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/utils/filter_data_with_id.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1607 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/utils/get_json_files.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     2968 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/utils/get_namespaces.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     3463 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/utils/get_paths.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      236 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/utils/list_files.py
-drwxrwxr-x   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:36:45.879140 lendsmart_reva-1.3/reva/lib/workflow/
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)        0 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/workflow/__init__.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      608 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/workflow/main.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1386 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/lib/workflow/update.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      878 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/loan_products.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     1125 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/namespaces.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      933 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/roles_and_permissions.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      853 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/site_settings.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)      820 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/reva/workflow.py
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)       86 2022-12-15 11:36:45.879140 lendsmart_reva-1.3/setup.cfg
--rw-rw-r--   0 lendsmart  (1000) lendsmart  (1000)     2035 2022-12-15 11:35:45.000000 lendsmart_reva-1.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.872145 lendsmart_reva-1.4/lendsmart_reva.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1743 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      448 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      158 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/autotest.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/cli.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/conf/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/conf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/conf/reva.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)      954 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/info.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/lib/auto/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/auto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/auto/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/lib/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1101 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/base/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      948 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/base/run_query.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/client/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/client/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      399 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/client/builder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/client/graphql_client.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/document_access_control/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/document_access_control/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      728 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/document_access_control/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/document_access_control/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/graphql_queries/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      806 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)      551 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)      944 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      590 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      802 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/workflow.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/loan_productus/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/loan_productus/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/loan_productus/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/loan_productus/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/roles_and_permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/roles_and_permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      687 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/roles_and_permissions/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/roles_and_permissions/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/site_settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/site_settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/site_settings/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/site_settings/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/reva/lib/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/filter_data_with_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/get_json_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/get_namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/get_paths.py
+-rw-rw-r--   0 user      (1000) user      (1000)      236 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/list_files.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/reva/lib/workflow/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/workflow/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      608 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/workflow/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/workflow/update.py
+-rw-rw-r--   0 user      (1000) user      (1000)      878 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)      933 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      853 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      820 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/workflow.py
+-rw-rw-r--   0 user      (1000) user      (1000)       86 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2144 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/setup.py
```

### Comparing `lendsmart_reva-1.3/PKG-INFO` & `lendsmart_reva-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart_reva
-Version: 1.3
+Version: 1.4
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.3/README.md` & `lendsmart_reva-1.4/README.md`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/lendsmart_reva.egg-info/PKG-INFO` & `lendsmart_reva-1.4/lendsmart_reva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart-reva
-Version: 1.3
+Version: 1.4
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.3/lendsmart_reva.egg-info/SOURCES.txt` & `lendsmart_reva-1.4/lendsmart_reva.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 lendsmart_reva.egg-info/PKG-INFO
 lendsmart_reva.egg-info/SOURCES.txt
 lendsmart_reva.egg-info/dependency_links.txt
 lendsmart_reva.egg-info/entry_points.txt
 lendsmart_reva.egg-info/requires.txt
 lendsmart_reva.egg-info/top_level.txt
 reva/__init__.py
+reva/autotest.py
 reva/cli.py
 reva/document_access_control.py
 reva/exception.py
 reva/info.py
 reva/loan_products.py
 reva/namespaces.py
 reva/roles_and_permissions.py
 reva/site_settings.py
 reva/workflow.py
 reva/conf/__init__.py
 reva/conf/reva.py
 reva/lib/__init__.py
+reva/lib/auto/__init__.py
+reva/lib/auto/main.py
 reva/lib/base/__init__.py
 reva/lib/base/base.py
 reva/lib/base/run_query.py
 reva/lib/client/__init__.py
 reva/lib/client/builder.py
 reva/lib/client/graphql_client.py
 reva/lib/document_access_control/__init__.py
```

### Comparing `lendsmart_reva-1.3/reva/cli.py` & `lendsmart_reva-1.4/reva/cli.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/conf/reva.py` & `lendsmart_reva-1.4/reva/conf/reva.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/document_access_control.py` & `lendsmart_reva-1.4/reva/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/exception.py` & `lendsmart_reva-1.4/reva/exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,7 +37,12 @@
     """
         This exception will be raised when config not found
     """
 class EnvPathNotConfigured(RevaError):
     """
         This exception will be raised when the environment path is not configured
     """
+
+class UnsupportedPlatformError(RevaError):
+    """
+        This exception will be raised when the platform is not supported
+    """
```

### Comparing `lendsmart_reva-1.3/reva/info.py` & `lendsmart_reva-1.4/reva/info.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/base/base.py` & `lendsmart_reva-1.4/reva/lib/base/base.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/base/run_query.py` & `lendsmart_reva-1.4/reva/lib/base/run_query.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/client/graphql_client.py` & `lendsmart_reva-1.4/reva/lib/client/graphql_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/document_access_control/main.py` & `lendsmart_reva-1.4/reva/lib/document_access_control/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/document_access_control/update.py` & `lendsmart_reva-1.4/reva/lib/document_access_control/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/graphql_queries/document_access_control.py` & `lendsmart_reva-1.4/reva/lib/graphql_queries/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/graphql_queries/loan_products.py` & `lendsmart_reva-1.4/reva/lib/graphql_queries/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/graphql_queries/roles_and_permissions.py` & `lendsmart_reva-1.4/reva/lib/graphql_queries/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/graphql_queries/site_settings.py` & `lendsmart_reva-1.4/reva/lib/graphql_queries/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/graphql_queries/workflow.py` & `lendsmart_reva-1.4/reva/lib/graphql_queries/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/loan_productus/main.py` & `lendsmart_reva-1.4/reva/lib/loan_productus/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/loan_productus/update.py` & `lendsmart_reva-1.4/reva/lib/loan_productus/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/roles_and_permissions/main.py` & `lendsmart_reva-1.4/reva/lib/roles_and_permissions/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/roles_and_permissions/update.py` & `lendsmart_reva-1.4/reva/lib/roles_and_permissions/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/site_settings/main.py` & `lendsmart_reva-1.4/reva/lib/site_settings/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/site_settings/update.py` & `lendsmart_reva-1.4/reva/lib/site_settings/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/utils/get_json_files.py` & `lendsmart_reva-1.4/reva/lib/utils/get_json_files.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/utils/get_namespaces.py` & `lendsmart_reva-1.4/reva/lib/utils/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/utils/get_paths.py` & `lendsmart_reva-1.4/reva/lib/utils/get_paths.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/workflow/main.py` & `lendsmart_reva-1.4/reva/lib/workflow/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/lib/workflow/update.py` & `lendsmart_reva-1.4/reva/lib/workflow/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/loan_products.py` & `lendsmart_reva-1.4/reva/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/namespaces.py` & `lendsmart_reva-1.4/reva/namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/roles_and_permissions.py` & `lendsmart_reva-1.4/reva/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/site_settings.py` & `lendsmart_reva-1.4/reva/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/reva/workflow.py` & `lendsmart_reva-1.4/reva/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.3/setup.py` & `lendsmart_reva-1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,21 +14,23 @@
     pkg_resources.parse_version('36.2.0')):
     install_requires = [
         "remoto >= 1.1.4",
         "configparser;python_version<'3.0'",
         "setuptools < 45.0.0;python_version<'3.0'",
         "python-graphql-client",
         "ramda",
+        "lendsmart-autotest",
         "setuptools;python_version>='3.0'"]
 else:
     install_requires = [
         "remoto >= 1.1.4",
         "configparser",
         "python-graphql-client",
         "ramda",
+        "lendsmart-autotest",
         "setuptools < 45.0.0"]
 
 setup(
     name='lendsmart_reva',
     version=reva.__version__,
     packages=find_packages(),
 
@@ -59,14 +61,15 @@
 
         'reva.cli': [
             'info = reva.info:show',
             'ready = reva.info:ready',
             'workflow = reva.workflow:workflow',
             'sitesettings = reva.site_settings:site_settings',
             'namespace = reva.namespaces:namespaces',
+            'autotest = reva.autotest:autotest',
             'loanproducts = reva.loan_products:loan_products',
             'documentaccesscontrol = reva.document_access_control:document_access_control',
             'rolesandpermissions = reva.roles_and_permissions:roles_and_permissions'
             ],
 
         },
     )
```


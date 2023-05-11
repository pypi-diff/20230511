# Comparing `tmp/dciclient-2.5.0.tar.gz` & `tmp/dciclient-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dciclient-2.5.0.tar", last modified: Fri Nov  4 13:20:22 2022, max compression
+gzip compressed data, was "dciclient-3.1.0.tar", last modified: Thu May 11 09:51:05 2023, max compression
```

## Comparing `dciclient-2.5.0.tar` & `dciclient-3.1.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 13:20:22.191537 dciclient-2.5.0/
--rw-r--r--   0 root         (0) root         (0)    10142 2022-11-04 13:19:58.000000 dciclient-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       79 2022-11-04 13:19:58.000000 dciclient-2.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10130 2022-11-04 13:20:22.191537 dciclient-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7614 2022-11-04 13:19:58.000000 dciclient-2.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 13:20:22.185537 dciclient-2.5.0/dciclient/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4478 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/create_component.py
--rw-r--r--   0 root         (0) root         (0)     5465 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/find_latest_component.py
--rw-r--r--   0 root         (0) root         (0)     3297 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/printer.py
--rw-r--r--   0 root         (0) root         (0)     3158 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/rhel_kernel.py
--rwxr-xr-x   0 root         (0) root         (0)     1236 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 13:20:22.186537 dciclient-2.5.0/dciclient/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 13:20:22.189537 dciclient-2.5.0/dciclient/v1/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5193 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/base.py
--rw-r--r--   0 root         (0) root         (0)     2833 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/component.py
--rw-r--r--   0 root         (0) root         (0)     7447 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/context.py
--rw-r--r--   0 root         (0) root         (0)     1314 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/feeder.py
--rw-r--r--   0 root         (0) root         (0)     3473 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/file.py
--rw-r--r--   0 root         (0) root         (0)     1109 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     3533 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/job.py
--rw-r--r--   0 root         (0) root         (0)     1896 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/jobs_events.py
--rw-r--r--   0 root         (0) root         (0)      973 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/jobstate.py
--rw-r--r--   0 root         (0) root         (0)     1362 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1800 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/product.py
--rw-r--r--   0 root         (0) root         (0)     2141 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/remoteci.py
--rw-r--r--   0 root         (0) root         (0)     1403 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/tag.py
--rw-r--r--   0 root         (0) root         (0)     1171 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/team.py
--rw-r--r--   0 root         (0) root         (0)     2874 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/topic.py
--rw-r--r--   0 root         (0) root         (0)     1670 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/api/user.py
--rw-r--r--   0 root         (0) root         (0)      862 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 13:20:22.191537 dciclient-2.5.0/dciclient/v1/shell_commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26996 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/cli.py
--rw-r--r--   0 root         (0) root         (0)     1173 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/columns.py
--rw-r--r--   0 root         (0) root         (0)     2918 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/component.py
--rw-r--r--   0 root         (0) root         (0)     4052 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/context.py
--rw-r--r--   0 root         (0) root         (0)     1531 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/feeder.py
--rw-r--r--   0 root         (0) root         (0)      991 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/file.py
--rw-r--r--   0 root         (0) root         (0)     3063 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/job.py
--rw-r--r--   0 root         (0) root         (0)      822 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/jobstate.py
--rw-r--r--   0 root         (0) root         (0)     1553 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1917 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/product.py
--rw-r--r--   0 root         (0) root         (0)     2426 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/purge.py
--rw-r--r--   0 root         (0) root         (0)     2446 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/remoteci.py
--rw-r--r--   0 root         (0) root         (0)     4188 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/runner.py
--rw-r--r--   0 root         (0) root         (0)     1430 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/team.py
--rw-r--r--   0 root         (0) root         (0)     2425 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/topic.py
--rw-r--r--   0 root         (0) root         (0)     1852 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/shell_commands/user.py
--rw-r--r--   0 root         (0) root         (0)     1614 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/v1/utils.py
--rw-r--r--   0 root         (0) root         (0)     1544 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/vault.py
--rw-r--r--   0 root         (0) root         (0)     1838 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/vault_client.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-04 13:19:58.000000 dciclient-2.5.0/dciclient/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 13:20:22.186537 dciclient-2.5.0/dciclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10130 2022-11-04 13:20:22.000000 dciclient-2.5.0/dciclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1669 2022-11-04 13:20:22.000000 dciclient-2.5.0/dciclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-04 13:20:22.000000 dciclient-2.5.0/dciclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      309 2022-11-04 13:20:22.000000 dciclient-2.5.0/dciclient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2022-11-04 13:20:22.000000 dciclient-2.5.0/dciclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-04 13:20:22.000000 dciclient-2.5.0/dciclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       63 2022-11-04 13:19:58.000000 dciclient-2.5.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-04 13:20:22.191537 dciclient-2.5.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2938 2022-11-04 13:19:58.000000 dciclient-2.5.0/setup.py
--rwxr-xr-x   0 root         (0) root         (0)     1222 2022-11-04 13:19:58.000000 dciclient-2.5.0/start_db.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:51:05.048343 dciclient-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)    10142 2023-05-11 09:48:17.000000 dciclient-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-11 09:48:17.000000 dciclient-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10533 2023-05-11 09:51:05.048343 dciclient-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9826 2023-05-11 09:48:17.000000 dciclient-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:51:05.041342 dciclient-3.1.0/dciclient/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/create_component.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/diff_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/find_latest_component.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/printer.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/rhel_kernel.py
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:51:05.043342 dciclient-3.1.0/dciclient/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:51:05.045343 dciclient-3.1.0/dciclient/v1/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/component.py
+-rw-r--r--   0 root         (0) root         (0)     7447 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/context.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/feeder.py
+-rw-r--r--   0 root         (0) root         (0)     3473 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/file.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/job.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/jobs_events.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/jobstate.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/product.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/remoteci.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/team.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/api/user.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:51:05.048343 dciclient-3.1.0/dciclient/v1/shell_commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27981 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/columns.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/component.py
+-rw-r--r--   0 root         (0) root         (0)     3905 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/context.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/feeder.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/file.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/job.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/jobstate.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/product.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/purge.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/remoteci.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/runner.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/team.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/shell_commands/user.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/v1/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 09:48:17.000000 dciclient-3.1.0/dciclient/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:51:05.043342 dciclient-3.1.0/dciclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10533 2023-05-11 09:51:04.000000 dciclient-3.1.0/dciclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-11 09:51:04.000000 dciclient-3.1.0/dciclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 09:51:04.000000 dciclient-3.1.0/dciclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-11 09:51:04.000000 dciclient-3.1.0/dciclient.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-11 09:51:04.000000 dciclient-3.1.0/dciclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-11 09:51:04.000000 dciclient-3.1.0/dciclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-11 09:48:17.000000 dciclient-3.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 09:51:05.048343 dciclient-3.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2738 2023-05-11 09:48:17.000000 dciclient-3.1.0/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)     1222 2023-05-11 09:48:17.000000 dciclient-3.1.0/start_db.sh
```

### Comparing `dciclient-2.5.0/LICENSE` & `dciclient-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/PKG-INFO` & `dciclient-3.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,244 +1,263 @@
-Metadata-Version: 2.1
-Name: dciclient
-Version: 2.5.0
-Summary: Python client for DCI Control Server
-Home-page: https://github.com/redhat-cip/python-dciclient
-Author: Distributed CI team
-Author-email: distributed-ci@redhat.com
-License: Apache v2.0
-Description: # python-dciclient
-        
-        The `python-dciclient` project provides both the python bindings and a CLI to the [DCI Control Server](https://github.com/redhat-cip/dci-control-server)
-        
-        ## Installation
-        
-        The team behind the project offers repositories for Red Hat/CentOS:
-        
-        - `yum -y install https://packages.distributed-ci.io/dci-release.el7.noarch.rpm`
-        
-        Then simply run `yum install python2-dciclient` for Python 2 or `yum install python3-dciclient` for Python 3.
-        
-        As mentioned above, the package provides two things:
-        
-        - The CLI: a `dcictl` command is provided. For more details `dcictl --help`.
-        - The API: a python module one can use to interact with a control server (`dciclient.v1.api.*`)
-        
-        ## Credentials
-        
-        Admitting one has valid credentials to use the DCI Control Server platform, there are two way to specify those informations while using dcictl:
-        
-        - A dcirc file:
-        
-        A file where the necessary credentials are stored. This file needs then to be sourced before using `dcictl`. Example:
-        
-        ```
-        export DCI_LOGIN=foo
-        export DCI_PASSWORD=bar
-        export DCI_CS_URL=https://api.distributed-ci.io
-        ```
-        
-        or using the API secret method:
-        
-        ```
-        export DCI_CLIENT_ID=<client_type>/<client_id>
-        export DCI_API_SECRET=<api_secret>
-        export DCI_CS_URL=https://api.distributed-ci.io
-        ```
-        
-        Where `client_type` can currently be `remoteci` or `feeder`
-        
-        Which will allow the user to run the command: `dcictl team-list`
-        
-        - At the command line level:
-        
-        One can pass those informations on the CLI level. Example: `dcictl --dci-login jdoe --dci-password jdoe --dci-cs-url 'https://api.distributed-ci.io' team-list`
-        or `dcictl --dci-client-id <client_type>/<client_id> --dci-api-secret <api_secret> --dci-cs-url 'https://api.distributed-ci.io' team-list`
-        
-        Where `client_type` can currently be `remoteci` or `feeder`
-        
-        For RemoteCIs or Feeders please use the API Secret to authenticate.
-        
-        ## List of available commands
-        
-        Run `dcictl --help` command to see the list of the available commands
-        
-        ```
-        Commands:
-          component-create             Create a component.
-          component-delete             Delete a component.
-          component-file-delete        Delete a component file.
-          component-file-download      Retrieve a component file.
-          component-file-list          List files attached to a component.
-          component-file-show          Show a component file.
-          component-file-upload        Attach a file to a component.
-          component-list               List all components.
-          component-show               Show a component.
-          component-status             Show an overview of the last jobs associated...
-          component-update             Update a component.
-          file-delete                  Delete a file.
-          file-list                    List all files.
-          file-show                    Show a file.
-          job-delete                   Delete a job.
-          job-list                     List all jobs.
-          job-output                   Show the job output.
-          job-recheck                  Recheck a job.
-          job-results                  List all job results.
-          job-show                     Show a job.
-          jobdefinition-annotate       Annotate a jobdefinition.
-          jobdefinition-attach-test    Attach a test to a jobdefinition.
-          jobdefinition-create         Create a jobdefinition.
-          jobdefinition-delete         Delete a jobdefinition.
-          jobdefinition-list           List all jobdefinitions.
-          jobdefinition-list-test      List tests attached to a jobdefinition.
-          jobdefinition-set-active     Annotate a jobdefinition.
-          jobdefinition-show           Show a jobdefinition.
-          jobdefinition-unattach-test  Unattach a test to a jobdefinition.
-          jobdefinition-update         Update a jobdefinition.
-          jobstate-list                List all jobstates.
-          jobstate-show                Show a jobstate.
-          purge                        Purge soft-deleted resources.
-          remoteci-create              Create a remoteci.
-          remoteci-delete              Delete a remoteci.
-          remoteci-get-data            Retrieve data field from a remoteci.
-          remoteci-list                List all remotecis.
-          remoteci-refresh-keys        Refresh a remoteci key pair.
-          remoteci-reset-api-secret    Reset a remoteci api secret.
-          remoteci-show                Show a remoteci.
-          remoteci-update              Update a remoteci.
-          team-create                  Create a team.
-          team-delete                  Delete a team.
-          team-list                    List all teams.
-          team-show                    Show a team.
-          team-update                  Update a team.
-          topic-attach-team            Attach a team to a topic.
-          topic-create                 Create a topic.
-          topic-delete                 Delete a topic.
-          topic-list                   List all topics.
-          topic-list-team              List teams attached to a topic.
-          topic-show                   Show a topic.
-          topic-unattach-team          Unattach a team from a topic.
-          user-create                  Create a user.
-          user-delete                  Delete a user.
-          user-list                    List all users.
-          user-show                    Show a user.
-          user-update                  Update a user.
-        ```
-        
-        ## dci-vault
-        
-        If you want to store secrets in your YAML configuration files
-        (settings or inventories), you can use the `dci-vault` command to do
-        so. The various agents will then decrypt the secrets
-        transparently. For example:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ echo -n 42 | dci-vault encrypt_string --stdin-name answer
-        Reading plaintext input from stdin. (ctrl-d to end input)
-        answer: !vault |
-                  $ANSIBLE_VAULT;1.1;AES256
-                  36373332616633313866333234303166616237613332316534393834663934663463353433363464
-                  6363626133323036383939633566383139373636633533390a316363393437653663363538343730
-                  65333862633131353030353137636236663036656264393638353464343138623664323731613331
-                  6466636637393865380a336365633465633037623935633866366562373732356635343361353334
-                  3732
-        Encryption successful
-        ```
-        
-        `dci-vault` is a thin layer on top of `ansible-vault` so all the
-        sub-commands of `ansible-vault` are available.
-        
-        ## dci-rhel-latest-kernel-version
-        
-        The dci-rhel-latest-kernel-version is a utility command to easily get the
-        latest kernel available for the RHEL product.
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-rhel-latest-kernel-version --topic RHEL-not-existing
-        topic RHEL-not-existing not found
-        
-        - available topics:
-        RHEL-9.2
-        RHEL-9.1
-        RHEL-8.7
-        RHEL-8.6
-        RHEL-8.5
-        RHEL-9.0
-        RHEL-8.4
-        RHEL-8.0
-        RHEL-8.1
-        RHEL-7.6
-        RHEL-7.7
-        RHEL-8.3
-        RHEL-8.2
-        RHEL-7.8
-        RHEL-7.9
-        RHEL-7-nightly
-        RHEL-7-milestone
-        $ dci-rhel-latest-kernel-version --topic-list
-        available topics:
-        RHEL-9.2
-        RHEL-9.1
-        RHEL-9.0
-        RHEL-8.7
-        RHEL-8.6
-        RHEL-8.5
-        RHEL-8.4
-        RHEL-8.3
-        RHEL-8.2
-        RHEL-8.1
-        RHEL-8.0
-        RHEL-7.9
-        $ dci-rhel-latest-kernel-version --topic RHEL-9.2
-        5.14.0-160.el9
-        ```
-        
-        ## dci-create-component
-        
-        to create a component, you can use the `dci-create-component`
-        utility. For example, to create the `my-product` version `1.0`
-        component on the `OCP-4.11` topic, use it like that:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-create-component OCP-4.11 "My Company Product" 1.0 ga
-        ```
-        
-        ## dci-find-latest-component
-        
-        `dci-find-latest-component` allows to find the latest component for a
-        product. For example to find the latest GA OCP component on the most
-        recent topic, you can do it like this:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-find-latest-component --tags build:ga OpenShift ocp
-        ```
-        
-        To lookup the latest GA OCP component for a specific topic for example
-        OCP-4.11, you can do it like this:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-find-latest-component --topic OCP-4.11 --tags build:ga OpenShift ocp
-        ```
-        
-        ## License
-        
-        Apache 2.0
-        
-        ## Author Information
-        
-        Distributed-CI Team <distributed-ci@redhat.com>
-        
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: System :: Distributed Computing
-Description-Content-Type: text/markdown
+# python-dciclient
+
+The `python-dciclient` project provides both the python bindings and a CLI to the [DCI Control Server](https://github.com/redhat-cip/dci-control-server)
+
+## Installation
+
+The team behind the project offers repositories for Red Hat/CentOS:
+
+- `yum -y install https://packages.distributed-ci.io/dci-release.el7.noarch.rpm`
+
+Then simply run `yum install python2-dciclient` for Python 2 or `yum install python3-dciclient` for Python 3.
+
+As mentioned above, the package provides two things:
+
+- The CLI: a `dcictl` command is provided. For more details `dcictl --help`.
+- The API: a python module one can use to interact with a control server (`dciclient.v1.api.*`)
+
+## Credentials
+
+Admitting one has valid credentials to use the DCI Control Server platform, there are two way to specify those informations while using dcictl:
+
+- A dcirc file:
+
+A file where the necessary credentials are stored. This file needs then to be sourced before using `dcictl`. Example:
+
+```
+export DCI_LOGIN=foo
+export DCI_PASSWORD=bar
+export DCI_CS_URL=https://api.distributed-ci.io
+```
+
+or using the API secret method:
+
+```
+export DCI_CLIENT_ID=<client_type>/<client_id>
+export DCI_API_SECRET=<api_secret>
+export DCI_CS_URL=https://api.distributed-ci.io
+```
+
+Where `client_type` can currently be `remoteci` or `feeder`
+
+Which will allow the user to run the command: `dcictl team-list`
+
+- At the command line level:
+
+One can pass those informations on the CLI level. Example: `dcictl --dci-login jdoe --dci-password jdoe --dci-cs-url 'https://api.distributed-ci.io' team-list`
+or `dcictl --dci-client-id <client_type>/<client_id> --dci-api-secret <api_secret> --dci-cs-url 'https://api.distributed-ci.io' team-list`
+
+Where `client_type` can currently be `remoteci` or `feeder`
+
+For RemoteCIs or Feeders please use the API Secret to authenticate.
+
+## List of available commands
+
+Run `dcictl --help` command to see the list of the available commands
+
+```
+Commands:
+  component-create             Create a component.
+  component-delete             Delete a component.
+  component-file-delete        Delete a component file.
+  component-file-download      Retrieve a component file.
+  component-file-list          List files attached to a component.
+  component-file-show          Show a component file.
+  component-file-upload        Attach a file to a component.
+  component-list               List all components.
+  component-show               Show a component.
+  component-status             Show an overview of the last jobs associated...
+  component-update             Update a component.
+  file-delete                  Delete a file.
+  file-list                    List all files.
+  file-show                    Show a file.
+  job-delete                   Delete a job.
+  job-list                     List all jobs.
+  job-output                   Show the job output.
+  job-recheck                  Recheck a job.
+  job-results                  List all job results.
+  job-show                     Show a job.
+  jobdefinition-annotate       Annotate a jobdefinition.
+  jobdefinition-attach-test    Attach a test to a jobdefinition.
+  jobdefinition-create         Create a jobdefinition.
+  jobdefinition-delete         Delete a jobdefinition.
+  jobdefinition-list           List all jobdefinitions.
+  jobdefinition-list-test      List tests attached to a jobdefinition.
+  jobdefinition-set-active     Annotate a jobdefinition.
+  jobdefinition-show           Show a jobdefinition.
+  jobdefinition-unattach-test  Unattach a test to a jobdefinition.
+  jobdefinition-update         Update a jobdefinition.
+  jobstate-list                List all jobstates.
+  jobstate-show                Show a jobstate.
+  purge                        Purge soft-deleted resources.
+  remoteci-create              Create a remoteci.
+  remoteci-delete              Delete a remoteci.
+  remoteci-get-data            Retrieve data field from a remoteci.
+  remoteci-list                List all remotecis.
+  remoteci-refresh-keys        Refresh a remoteci key pair.
+  remoteci-reset-api-secret    Reset a remoteci api secret.
+  remoteci-show                Show a remoteci.
+  remoteci-update              Update a remoteci.
+  team-create                  Create a team.
+  team-delete                  Delete a team.
+  team-list                    List all teams.
+  team-show                    Show a team.
+  team-update                  Update a team.
+  topic-attach-team            Attach a team to a topic.
+  topic-create                 Create a topic.
+  topic-delete                 Delete a topic.
+  topic-list                   List all topics.
+  topic-list-team              List teams attached to a topic.
+  topic-show                   Show a topic.
+  topic-unattach-team          Unattach a team from a topic.
+  user-create                  Create a user.
+  user-delete                  Delete a user.
+  user-list                    List all users.
+  user-show                    Show a user.
+  user-update                  Update a user.
+```
+
+## dci-vault
+
+If you want to store secrets in your YAML configuration files
+(settings or inventories), you can use the `dci-vault` command to do
+so. The various agents will then decrypt the secrets
+transparently. For example:
+
+```ShellSession
+$ source dcirc.sh
+$ echo -n 42 | dci-vault encrypt_string --stdin-name answer
+Reading plaintext input from stdin. (ctrl-d to end input)
+answer: !vault |
+          $ANSIBLE_VAULT;1.1;AES256
+          36373332616633313866333234303166616237613332316534393834663934663463353433363464
+          6363626133323036383939633566383139373636633533390a316363393437653663363538343730
+          65333862633131353030353137636236663036656264393638353464343138623664323731613331
+          6466636637393865380a336365633465633037623935633866366562373732356635343361353334
+          3732
+Encryption successful
+```
+
+`dci-vault` is a thin layer on top of `ansible-vault` so all the
+sub-commands of `ansible-vault` are available.
+
+## dci-rhel-latest-kernel-version
+
+The dci-rhel-latest-kernel-version is a utility command to easily get the
+latest kernel available for the RHEL product.
+
+```ShellSession
+$ source dcirc.sh
+$ dci-rhel-latest-kernel-version --topic RHEL-not-existing
+topic RHEL-not-existing not found
+
+- available topics:
+RHEL-9.2
+RHEL-9.1
+RHEL-8.7
+RHEL-8.6
+RHEL-8.5
+RHEL-9.0
+RHEL-8.4
+RHEL-8.0
+RHEL-8.1
+RHEL-7.6
+RHEL-7.7
+RHEL-8.3
+RHEL-8.2
+RHEL-7.8
+RHEL-7.9
+RHEL-7-nightly
+RHEL-7-milestone
+$ dci-rhel-latest-kernel-version --topic-list
+available topics:
+RHEL-9.2
+RHEL-9.1
+RHEL-9.0
+RHEL-8.7
+RHEL-8.6
+RHEL-8.5
+RHEL-8.4
+RHEL-8.3
+RHEL-8.2
+RHEL-8.1
+RHEL-8.0
+RHEL-7.9
+$ dci-rhel-latest-kernel-version --topic RHEL-9.2
+5.14.0-160.el9
+```
+
+## dci-create-component
+
+To create a component, you can use the `dci-create-component`
+utility. For example, to create the `ga` component called `My product` with version `1.0` on the `OCP-4.11` topic, use it like that:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-create-component OCP-4.11 "My Product" 1.0 ga
+```
+
+## dci-find-latest-component
+
+`dci-find-latest-component` allows to find the latest component for a
+product. For example to find the latest GA OCP component on the most
+recent topic, you can do it like this:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-find-latest-component --tags build:ga OpenShift ocp
+```
+
+To lookup the latest GA OCP component for a specific topic for example
+OCP-4.11, you can do it like this:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-find-latest-component --topic OCP-4.11 --tags build:ga OpenShift ocp
+```
+
+## dci-diff-jobs
+
+`dci-diff-jobs` allows to compare the components of 2 jobs:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-diff-jobs --job_id_1 9e3f3a4f-74c5-4bce-9c45-450b27006bed --job_id_2 b55fb5d6-3f01-44ce-9034-26a53e086137
++-----------------------+--------------------------------------+--------------------------------------+
+|       component       | 9e3f3a4f-74c5-4bce-9c45-450b27006bed | b55fb5d6-3f01-44ce-9034-26a53e086137 |
++-----------------------+--------------------------------------+--------------------------------------+
+|          ocp          |                4.9.50                |                4.8.52                |
+| redhat-operator-index |                 v4.9                 |                 v4.8                 |
++-----------------------+--------------------------------------+--------------------------------------+
+```
+
+or their tags:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-diff-jobs --tags --job_id_1 9e3f3a4f-74c5-4bce-9c45-450b27006bed --job_id_2 b55fb5d6-3f01-44ce-9034-26a53e086137
++--------------------------------------+--------------------------------------+
+| 9e3f3a4f-74c5-4bce-9c45-450b27006bed | b55fb5d6-3f01-44ce-9034-26a53e086137 |
++--------------------------------------+--------------------------------------+
+|       pipeline-id:8nodes.8225        |              Not found               |
+|          inventory:cluster6          |              Not found               |
+|         pipeline:install-4.9         |              Not found               |
+|           cluster:cluster6           |              Not found               |
+|              Not found               |       pipeline-id:8nodes.8239        |
+|              Not found               |          inventory:cluster4          |
+|              Not found               |         pipeline:install-4.8         |
+|              Not found               |           cluster:cluster4           |
++--------------------------------------+--------------------------------------+
+```
+
+If the `--job_id_1` is not specified, the last job in success status is searched.
+
+If the `--job_id_2` is not specified, a job is searched with the same
+name, remoteci, topic, configuration and url than the job 1.
+
+## License
+
+Apache 2.0
+
+## Author Information
+
+Distributed-CI Team <distributed-ci@redhat.com>
```

### Comparing `dciclient-2.5.0/dciclient/create_component.py` & `dciclient-3.1.0/dciclient/create_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     p = ArgumentParser(
         prog="dci-create-component",
         description=(
             "Tool to create a component for DCI "
             "(https://docs.distributed-ci.io/)"
         ),
     )
-    dci_context.parse_arguments(p, args, environment)
+    dci_context.parse_auth_arguments(p, environment)
     _create_array_argument(p, "--tags", help="Comma separated list of tags")
     p.add_argument(
         "--released-at",
         help="The release date",
         default=None,
         type=_date_isoformat,
     )
@@ -60,20 +60,20 @@
         help="Team to use when there are multiple",
     )
     p.add_argument(
         "topic",
         help="Topic type and version, examples: OCP-4.12 or RHEL-9.1",
     )
     p.add_argument(
-        "type",
+        "name",
         help='Name of the component, example: "my awesome component"',
         metavar="component_name",
     )
     p.add_argument(
-        "name",
+        "version",
         help="Version of the component, example: v2.3.4",
         metavar="component_version",
     )
     p.add_argument(
         "release_tag",
         help="Release type of the component",
         type=str,
@@ -129,22 +129,20 @@
 
 
 def run(context, args):
     args.team_id = get_team_id(context, args)
     args.topic_id = get_topic_id(context, args)
 
     # Required arguments for component creation
-    args.title = None
-    args.message = None
     args.state = True
-    args.type = "-".join([p.lower() for p in args.type.split(" ")])
-    args.canonical_project_name = "%s %s" % (" ".join([p.capitalize()
-                                                       for p in args.type.split("-")]),
-                                             args.name)
+    names = args.name.split(" ")
+    args.type = "-".join([name.lower() for name in names])
     args.tags += ["build:" + args.release_tag]
+    capitalized_name = " ".join([name.capitalize() for name in names])
+    args.display_name = "%s %s" % (capitalized_name, args.version)
     args.command = "component-create"
 
     return component.create(context, args)
 
 
 def main():
     args = parse_arguments(sys.argv[1:], os.environ)
```

### Comparing `dciclient-2.5.0/dciclient/find_latest_component.py` & `dciclient-3.1.0/dciclient/find_latest_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,42 +23,41 @@
 from dciclient.v1.shell_commands import context as dci_context
 from dciclient.v1.shell_commands import component
 from dciclient.v1.shell_commands import topic
 from dciclient.v1.shell_commands import product
 from dciclient.printer import print_result
 
 
-COLUMNS = ["canonical_project_name",
-           "created_at",
-           "data",
-           "etag",
-           "id",
-           "message",
-           "name",
-           "released_at",
-           "state",
-           "tags",
-           "team_id",
-           "title",
-           "topic_id",
-           "type",
-           "updated_at",
-           "url",
-           ]
+COLUMNS = [
+    "display_name",
+    "created_at",
+    "data",
+    "etag",
+    "id",
+    "released_at",
+    "state",
+    "tags",
+    "team_id",
+    "topic_id",
+    "type",
+    "updated_at",
+    "url",
+    "version"
+]
 
 
 def parse_arguments(args, environment={}):
     p = ArgumentParser(
         prog="dci-find-latest-component",
         description=(
             "Tool to find the latest component in DCI "
             "(https://docs.distributed-ci.io/)"
         ),
     )
-    dci_context.parse_arguments(p, args, environment)
+    dci_context.parse_auth_arguments(p, environment)
     _create_array_argument(p, "--tags", help="Comma separated list of tags")
     p.add_argument(
         "--topic",
         help="Topic type and version, examples: OCP-4.12 or RHEL-9.1",
     )
     p.add_argument(
         "product",
```

### Comparing `dciclient-2.5.0/dciclient/printer.py` & `dciclient-3.1.0/dciclient/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         first_row = data
     return list(first_row.keys())
 
 
 def _sort_headers(headers):
     """Ensure the column order is always the same."""
     headers = set(headers)
-    default_order = ["id", "name", "etag", "created_at", "updated_at", "state", "data"]
+    default_order = ["id", "name", "component", "tag", "etag", "created_at",
+                     "updated_at", "state", "data"]
     sorted_headers = []
     for i in default_order:
         if i not in headers:
             continue
         headers.remove(i)
         sorted_headers.append(i)
     sorted_headers += sorted(headers)
```

### Comparing `dciclient-2.5.0/dciclient/rhel_kernel.py` & `dciclient-3.1.0/dciclient/rhel_kernel.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,36 +16,38 @@
 import os
 import sys
 from argparse import ArgumentParser
 
 from dciclient.v1.api import topic
 from dciclient.v1.api import product
 from dciclient.v1.shell_commands import context as dci_context
+from dciclient.v1.shell_commands.cli import _create_array_argument
 
 
 _DEFAULT_DCI_CS_URL = "http:://127.0.0.1:5000"
 
 
 def parse_arguments(args, environment={}):
-    parser = ArgumentParser()
-    dci_context.parse_arguments(parser, args, environment)
-    parser.add_argument(
+    p = ArgumentParser()
+    dci_context.parse_auth_arguments(p, environment)
+    p.add_argument(
         "--topic",
         dest="topic_name",
         help="topic name",
     )
+    _create_array_argument(p, "--tags", help="Comma separated list of tags")
 
-    parser.add_argument(
+    p.add_argument(
         "--topic-list",
         default=False,
         action="store_true",
         help="list the available topics",
     )
 
-    return parser.parse_args(args)
+    return p.parse_args(args)
 
 
 def get_available_topics(context):
     product_list = product.list(context=context, where="name:RHEL").json()
     rhel_id = product_list["products"][0]["id"]
     topic_list = topic.list(
         context=context, where="product_id:%s,state:active" % rhel_id, sort="-name"
@@ -78,21 +80,25 @@
         sys.exit(1)
 
     if args.topic_list:
         print_available_topics(context)
         sys.exit(0)
 
     topic_id = get_topic_id_from_name(context, args.topic_name)
+    tags = ""
+    if args.tags and len(args.tags) > 0:
+        tags = ",tags:" + ",tags:".join(args.tags)
+
     latest_component = topic.list_components(
         context,
         topic_id,
         sort="-created_at",
         limit=1,
         offset=0,
-        where="type:compose,state:active",
+        where="type:compose,state:active" + tags
     ).json()
 
     if not latest_component["components"]:
         print("no components found")
         sys.exit(1)
     latest_component = latest_component["components"][0]
     kernel_found = False
```

### Comparing `dciclient-2.5.0/dciclient/shell.py` & `dciclient-3.1.0/dciclient/shell.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/base.py` & `dciclient-3.1.0/dciclient/v1/api/base.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/component.py` & `dciclient-3.1.0/dciclient/v1/api/component.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,39 +24,39 @@
     context,
     name,
     type,
     topic_id,
     team_id=None,
     canonical_project_name=None,
     data={},
-    title=None,
-    message=None,
     url=None,
     state="active",
     tags=[],
     released_at=None,
 ):
     return base.create(
         context,
         RESOURCE,
         name=name,
         type=type,
         canonical_project_name=canonical_project_name,
         data=data,
-        title=title,
-        message=message,
         url=url,
         topic_id=topic_id,
         team_id=team_id,
         state=state,
         tags=tags,
         released_at=released_at,
     )
 
 
+def create_v2(context, **kwargs):
+    return base.create(context, RESOURCE, **kwargs)
+
+
 def get_or_create(context, **kwargs):
     return base.get_or_create(
         context, "topics", id=kwargs["topic_id"], subresource="components", **kwargs
     )
 
 
 def get(context, id, **kwargs):
```

### Comparing `dciclient-2.5.0/dciclient/v1/api/context.py` & `dciclient-3.1.0/dciclient/v1/api/context.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/feeder.py` & `dciclient-3.1.0/dciclient/v1/api/feeder.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/file.py` & `dciclient-3.1.0/dciclient/v1/api/file.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/identity.py` & `dciclient-3.1.0/dciclient/v1/api/identity.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/job.py` & `dciclient-3.1.0/dciclient/v1/api/job.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/jobs_events.py` & `dciclient-3.1.0/dciclient/v1/api/jobs_events.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/jobstate.py` & `dciclient-3.1.0/dciclient/v1/api/jobstate.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/pipeline.py` & `dciclient-3.1.0/dciclient/v1/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/product.py` & `dciclient-3.1.0/dciclient/v1/api/product.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/remoteci.py` & `dciclient-3.1.0/dciclient/v1/api/remoteci.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/tag.py` & `dciclient-3.1.0/dciclient/v1/api/tag.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/team.py` & `dciclient-3.1.0/dciclient/v1/api/team.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/topic.py` & `dciclient-3.1.0/dciclient/v1/api/topic.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/api/user.py` & `dciclient-3.1.0/dciclient/v1/api/user.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/exceptions.py` & `dciclient-3.1.0/dciclient/v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/cli.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- encoding: utf-8 -*-
 #
-# Copyright 2020-2022 Red Hat, Inc.
+# Copyright 2020-2023 Red Hat, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,14 +14,15 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import argparse
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
+from dciclient.version import __version__
 from dciclient.v1.shell_commands import context as dci_context
 
 
 def _create_boolean_flags(parser, flags, default, dest=None):
     flags = flags.split("/")
     dest = dest if dest else flags[0].strip("--")
     group = parser.add_mutually_exclusive_group()
@@ -42,30 +43,39 @@
     try:
         datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.%f")
     except ValueError:
         raise argparse.ArgumentTypeError("'%s' is not an iso format date" % v)
     return v
 
 
+def print_version_compatible_py27(args):
+    if args == ['--version']:
+        print("dcictl %s" % __version__)
+        sys.exit()
+
+
 def parse_arguments(args, environment={}):
     base_parser = ArgumentParser(add_help=False)
 
     parser = ArgumentParser(prog="dcictl")
 
-    dci_context.parse_arguments(parser, args, environment)
+    print_version_compatible_py27(args)
+
+    dci_context.parse_auth_arguments(parser, environment)
 
     subparsers = parser.add_subparsers()
     # user commands
     p = subparsers.add_parser(
         "user-list", help="List all users.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="user-list")
 
     p = subparsers.add_parser(
         "user-create", help="Create a user.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
     p.add_argument("--password", required=True)
@@ -103,14 +113,15 @@
     p = subparsers.add_parser(
         "team-list", help="List all teams.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="team-list")
 
     p = subparsers.add_parser(
         "team-create", help="Create a team.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
     p.add_argument("--country")
@@ -143,14 +154,15 @@
     p = subparsers.add_parser(
         "product-list", help="List all products.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="product-list")
 
     p = subparsers.add_parser(
         "product-create", help="Create a product.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
     p.add_argument("--label")
@@ -203,24 +215,26 @@
         parents=[base_parser],
     )
     p.add_argument("id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="product-list-teams")
 
     # feeder commands
     p = subparsers.add_parser(
         "feeder-list", help="List all feeders.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="feeder-list")
 
     p = subparsers.add_parser(
         "feeder-create", help="Create a feeder.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
     p.add_argument("--data")
@@ -265,14 +279,15 @@
     p = subparsers.add_parser(
         "topic-list", help="List all topics.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="topic-list")
 
     p = subparsers.add_parser(
         "topic-create", help="Create a topic.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
     p.add_argument("--product-id")
@@ -333,14 +348,15 @@
         "topic-list-team", help="List teams attached to a topic.", parents=[base_parser]
     )
     p.add_argument("id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="topic-list-team")
 
     # jobstate commands
     p = subparsers.add_parser(
         "jobstate-show", help="Show a jobstate.", parents=[base_parser]
     )
     p.add_argument("id")
@@ -359,52 +375,47 @@
         "component-list", help="List all components.", parents=[base_parser]
     )
     p.add_argument("--topic-id", required=True, dest="id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="component-list")
 
     p = subparsers.add_parser(
         "component-create", help="Create a component.", parents=[base_parser]
     )
-    p.add_argument("--name", required=True, help="Name of component")
+    p.add_argument("display_name", metavar="name")
     p.add_argument("--type", required=True, help="Type of component")
     p.add_argument("--topic-id", required=True, help="Topic ID")
     p.add_argument("--team-id")
     _create_array_argument(p, "--tags", help="Comma separated list of tags")
-    p.add_argument(
-        "--canonical_project_name", default=None, help="Canonical project name."
-    )
-    p.add_argument("--title", help="Title of component")
-    p.add_argument("--message", help="Component message")
     p.add_argument("--url", help="URL to look for the component")
     _create_boolean_flags(p, "--active/--no-active", default=True, dest="state")
     p.add_argument("--data", default="{}", help="Data to pass (JSON)")
     p.add_argument(
         "--released-at", default=None, type=_date_isoformat, help="The release date"
     )
+    p.add_argument("--version", required=False, help="Version of the component")
     p.set_defaults(command="component-create")
 
     p = subparsers.add_parser(
         "component-update", help="Update a component.", parents=[base_parser]
     )
     p.add_argument("id")
     _create_boolean_flags(p, "--active/--no-active", default=None, dest="state")
-    p.add_argument("--name", required=False, help="Name of component")
-    p.add_argument("--type", required=False, help="Type of component")
-    _create_array_argument(p, "--tags", help="Comma separated list of tags")
     p.add_argument(
-        "--canonical_project_name", default=None, help="Canonical project name."
+        "--display-name", required=False, help="Display name of the component"
     )
-    p.add_argument("--title", help="Title of component")
-    p.add_argument("--message", help="Component message")
+    p.add_argument("--type", required=False, help="Type of component")
+    _create_array_argument(p, "--tags", help="Comma separated list of tags")
     p.add_argument("--url", help="URL to look for the component")
     p.add_argument("--data", default="{}", help="Data to pass (JSON)")
+    p.add_argument("--version", required=False, help="Version of the component")
     p.set_defaults(command="component-update")
 
     p = subparsers.add_parser(
         "component-delete", help="Delete a component.", parents=[base_parser]
     )
     p.add_argument("id")
     p.add_argument("--etag", required=True)
@@ -448,14 +459,15 @@
         parents=[base_parser],
     )
     p.add_argument("id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="component-file-list")
 
     p = subparsers.add_parser(
         "component-file-delete", help="Delete a component file.", parents=[base_parser]
     )
     p.add_argument("id")
     p.add_argument("--file-id", required=True)
@@ -467,14 +479,15 @@
         "file-list", help="List all files.", parents=[base_parser]
     )
     p.add_argument("job_id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="file-list")
 
     p = subparsers.add_parser("file-show", help="Show a file.", parents=[base_parser])
     p.add_argument("id")
     p.set_defaults(command="file-show")
 
     p = subparsers.add_parser(
@@ -485,14 +498,15 @@
 
     # job commands
     p = subparsers.add_parser("job-list", help="List all jobs.", parents=[base_parser])
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=10)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="job-list")
 
     p = subparsers.add_parser("job-show", help="Show a job.", parents=[base_parser])
     p.add_argument("id")
     p.set_defaults(command="job-show")
 
     p = subparsers.add_parser("job-delete", help="Delete a job.", parents=[base_parser])
@@ -507,15 +521,14 @@
     _create_boolean_flags(p, "--active/--no-active", default=None, dest="state")
     p.add_argument("--name", required=False, help="Name of the job")
     p.add_argument("--comment", required=False, help="Comment of the job")
     _create_array_argument(p, "--tags", help="Comma separated list of tags")
     p.add_argument("--status", default=None, help="Status of the job.")
     p.add_argument("--status_reason", default=None, help="Status reason of the job.")
     p.add_argument("--configuration", help="Configuration of the job.")
-    p.add_argument("--message", help="Component message")
     p.add_argument("--url", help="URL to look for the component")
     p.set_defaults(command="job-update")
 
     p = subparsers.add_parser(
         "job-results", help="List all job results.", parents=[base_parser]
     )
     p.add_argument("id")
@@ -559,14 +572,15 @@
         "job-list-file", help="List files attached to a job.", parents=[base_parser]
     )
     p.add_argument("id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="job-list-file")
 
     p = subparsers.add_parser(
         "job-delete-file", help="Delete a job file.", parents=[base_parser]
     )
     p.add_argument("id")
     p.add_argument("--file-id", required=True)
@@ -576,14 +590,15 @@
     p = subparsers.add_parser(
         "remoteci-list", help="List all remotecis.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="remoteci-list")
 
     p = subparsers.add_parser(
         "remoteci-create", help="Create a remoteci.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
     p.add_argument("--team-id", required=False)
@@ -666,14 +681,15 @@
         parents=[base_parser],
     )
     p.add_argument("id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="remoteci-list-user")
 
     # purge commands
     p = subparsers.add_parser(
         "purge", help="Purge soft-deleted resources.", parents=[base_parser]
     )
     p.add_argument(
@@ -705,14 +721,15 @@
     p = subparsers.add_parser(
         "pipeline-list", help="List all pipelines.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
     p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="pipeline-list")
 
     p = subparsers.add_parser(
         "pipeline-update", help="Update a pipeline.", parents=[base_parser]
     )
     p.add_argument("id")
     p.add_argument("--etag", required=True)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/columns.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/columns.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/component.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/component.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,47 +10,45 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from dciclient.v1.utils import active_string
-from dciclient.v1.utils import validate_json
+from dciclient.v1.utils import active_string, validate_json, get_search_params
 
 from dciclient.v1.api import component
 from dciclient.v1.api import topic
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["id", "sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
+    params["id"] = args.id
     return topic.list_components(context, **params)
 
 
 def create(context, args):
     params = {
         k: getattr(args, k)
         for k in [
-            "name",
+            "display_name",
+            "version",
             "type",
-            "canonical_project_name",
-            "title",
-            "message",
             "url",
             "team_id",
             "topic_id",
             "state",
             "data",
             "tags",
-            "released_at"
+            "released_at",
         ]
     }
     params["data"] = validate_json(context, "data", params["data"])
     params["state"] = active_string(params["state"])
-    return component.create(context, **params)
+    return component.create_v2(context, **params)
 
 
 def delete(context, args):
     return component.delete(context, args.id, args.etag)
 
 
 def show(context, args):
@@ -79,23 +77,21 @@
     component.file_delete(context, id=args.id, file_id=args.file_id, etag=args.etag)
 
 
 def update(context, args):
     params = {
         k: getattr(args, k)
         for k in [
-            "name",
+            "display_name",
             "type",
-            "canonical_project_name",
-            "title",
-            "message",
             "url",
             "state",
             "data",
             "tags",
+            "version"
         ]
     }
 
     component_info = component.get(context, args.id)
     params["etag"] = component_info.json()["component"]["etag"]
     params["data"] = validate_json(context, "data", params["data"])
     params["state"] = active_string(params["state"])
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/context.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from dciclient.version import __version__
 from dciclient.v1.api.context import (build_dci_context,
                                       build_signature_context,
                                       build_sso_context)
 
 
 _default_dci_cs_url = "http://127.0.0.1:5000"
 _default_sso_url = "http://127.0.0.1:8180"
 
 
-def parse_arguments(parser, args, environment={}):
-    parser.add_argument(
-        "--version", action="version", version="%(prog)s " + __version__
-    )
+def parse_auth_arguments(parser, environment={}):
     parser.add_argument(
         "--dci-login",
         default=environment.get("DCI_LOGIN", None),
         help="DCI login or 'DCI_LOGIN' environment variable.",
     )
     parser.add_argument(
         "--dci-password",
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/feeder.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/feeder.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dciclient.v1.api import feeder
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return feeder.list(context, **params)
 
 
 def create(context, args):
     params = {k: getattr(args, k) for k in ["name", "team_id", "data", "state"]}
     params["state"] = active_string(params["state"])
     return feeder.create(context, **params)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/file.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dciclient.v1.api import job
 from dciclient.v1.api import file
+from dciclient.v1.utils import get_search_params
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return job.list_files(context, id=args.job_id, **params)
 
 
 def show(context, args):
     return file.content(context, id=args.id)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/job.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/job.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dciclient.v1.api import file as dci_file
 from dciclient.v1.api import job
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     params["embed"] = "topic,remoteci,team"
     return job.list(context, **params)
 
 
 def show(context, args):
     return job.get(context, id=args.id)
 
@@ -70,15 +70,16 @@
         )
         for f in f_l.json()["files"]:
             res.append(dci_file.content(context, id=f["id"]).text)
     return res
 
 
 def list_tests(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "id", "where"]}
+    params = get_search_params(args)
+    params["id"] = args.id
     return job.list_tests(context, **params)
 
 
 def file_upload(context, args):
     params = {
         k: getattr(args, k)
         for k in ["job_id", "name", "file_path", "jobstate_id", "mime"]
@@ -92,14 +93,15 @@
 
 
 def file_show(context, args):
     return dci_file.get(context, id=args.file_id)
 
 
 def file_list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "id", "where"]}
+    params = get_search_params(args)
+    params["id"] = args.id
     return job.list_files(context, **params)
 
 
 def file_delete(context, args):
     dci_file.delete(context, id=args.file_id)
     return dci_file.delete(context, id=args.file_id)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/jobstate.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/jobstate.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/pipeline.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/pipeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dciclient.v1.api import pipeline
+from dciclient.v1.utils import get_search_params
 
 
 RESOURCE = "pipelines"
 
 HTTP_TIMEOUT = 600
 
 
@@ -27,15 +28,15 @@
 
 
 def show(context, args):
     return pipeline.get(context, args.id)
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return pipeline.list(context, **params)
 
 
 def update(context, args):
     params = {
         k: getattr(args, k)
         for k in [
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/product.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 from dciclient.v1.api import product
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return product.list(context, **params)
 
 
 def create(context, args):
     params = {k: getattr(args, k) for k in ["name", "label", "description", "state"]}
     params["state"] = active_string(params["state"])
     return product.create(context, **params)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/purge.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/purge.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/remoteci.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/remoteci.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 from dciclient.v1.utils import validate_json
 
 
 from dciclient.v1.api import identity
 from dciclient.v1.api import remoteci
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return remoteci.list(context, **params)
 
 
 def create(context, args):
     data = validate_json(context, "data", args.data)
     state = active_string(args.state)
     team_id = args.team_id or identity.my_team_id(context)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/runner.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/runner.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/team.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/team.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 from dciclient.v1.api import team
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return team.list(context, **params)
 
 
 def create(context, args):
     params = {k: getattr(args, k) for k in ["name", "country", "state"]}
     params["state"] = active_string(params["state"])
     return team.create(context, **params)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/topic.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/topic.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dciclient.v1.api import topic
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 
 COLUMNS = ["id", "name", "state", "export_control", "product_id", "component_types"]
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return topic.list(context, **params)
 
 
 def create(context, args):
     params = {
         k: getattr(args, k)
         for k in [
@@ -80,9 +80,9 @@
 
 
 def unattach_team(context, args):
     return topic.unattach_team(context, args.id, args.team_id)
 
 
 def list_team(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return topic.list_teams(context, args.id, **params)
```

### Comparing `dciclient-2.5.0/dciclient/v1/shell_commands/user.py` & `dciclient-3.1.0/dciclient/v1/shell_commands/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dciclient.v1.api import user
-from dciclient.v1.utils import active_string
+from dciclient.v1.utils import active_string, get_search_params
 
 COLUMNS = ["id", "created_at", "updated_at", "etag", "name",
            "sso_username", "fullname", "email", "password",
            "timezone", "state"]
 
 
 def list(context, args):
-    params = {k: getattr(args, k) for k in ["sort", "limit", "offset", "where"]}
+    params = get_search_params(args)
     return user.list(context, **params)
 
 
 def create(context, args):
     params = {
         k: getattr(args, k)
         for k in ["name", "password", "email", "fullname", "state"]
```

### Comparing `dciclient-2.5.0/dciclient/v1/utils.py` & `dciclient-3.1.0/dciclient/v1/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -53,7 +53,15 @@
         return json.loads(value)
     except ValueError:
         raise BadParameter("this option expects a valid JSON")
 
 
 def active_string(value):
     return {None: None, True: "active", False: "inactive"}[value]
+
+
+def get_search_params(args):
+    filtered_params = {}
+    for k in ["sort", "limit", "offset", "where", "query"]:
+        if k in args and getattr(args, k) not in [None, ""]:
+            filtered_params[k] = getattr(args, k)
+    return filtered_params
```

### Comparing `dciclient-2.5.0/dciclient/vault.py` & `dciclient-3.1.0/dciclient/vault.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient/vault_client.py` & `dciclient-3.1.0/dciclient/vault_client.py`

 * *Files identical despite different names*

### Comparing `dciclient-2.5.0/dciclient.egg-info/PKG-INFO` & `dciclient-3.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,244 +1,282 @@
 Metadata-Version: 2.1
 Name: dciclient
-Version: 2.5.0
+Version: 3.1.0
 Summary: Python client for DCI Control Server
 Home-page: https://github.com/redhat-cip/python-dciclient
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
-Description: # python-dciclient
-        
-        The `python-dciclient` project provides both the python bindings and a CLI to the [DCI Control Server](https://github.com/redhat-cip/dci-control-server)
-        
-        ## Installation
-        
-        The team behind the project offers repositories for Red Hat/CentOS:
-        
-        - `yum -y install https://packages.distributed-ci.io/dci-release.el7.noarch.rpm`
-        
-        Then simply run `yum install python2-dciclient` for Python 2 or `yum install python3-dciclient` for Python 3.
-        
-        As mentioned above, the package provides two things:
-        
-        - The CLI: a `dcictl` command is provided. For more details `dcictl --help`.
-        - The API: a python module one can use to interact with a control server (`dciclient.v1.api.*`)
-        
-        ## Credentials
-        
-        Admitting one has valid credentials to use the DCI Control Server platform, there are two way to specify those informations while using dcictl:
-        
-        - A dcirc file:
-        
-        A file where the necessary credentials are stored. This file needs then to be sourced before using `dcictl`. Example:
-        
-        ```
-        export DCI_LOGIN=foo
-        export DCI_PASSWORD=bar
-        export DCI_CS_URL=https://api.distributed-ci.io
-        ```
-        
-        or using the API secret method:
-        
-        ```
-        export DCI_CLIENT_ID=<client_type>/<client_id>
-        export DCI_API_SECRET=<api_secret>
-        export DCI_CS_URL=https://api.distributed-ci.io
-        ```
-        
-        Where `client_type` can currently be `remoteci` or `feeder`
-        
-        Which will allow the user to run the command: `dcictl team-list`
-        
-        - At the command line level:
-        
-        One can pass those informations on the CLI level. Example: `dcictl --dci-login jdoe --dci-password jdoe --dci-cs-url 'https://api.distributed-ci.io' team-list`
-        or `dcictl --dci-client-id <client_type>/<client_id> --dci-api-secret <api_secret> --dci-cs-url 'https://api.distributed-ci.io' team-list`
-        
-        Where `client_type` can currently be `remoteci` or `feeder`
-        
-        For RemoteCIs or Feeders please use the API Secret to authenticate.
-        
-        ## List of available commands
-        
-        Run `dcictl --help` command to see the list of the available commands
-        
-        ```
-        Commands:
-          component-create             Create a component.
-          component-delete             Delete a component.
-          component-file-delete        Delete a component file.
-          component-file-download      Retrieve a component file.
-          component-file-list          List files attached to a component.
-          component-file-show          Show a component file.
-          component-file-upload        Attach a file to a component.
-          component-list               List all components.
-          component-show               Show a component.
-          component-status             Show an overview of the last jobs associated...
-          component-update             Update a component.
-          file-delete                  Delete a file.
-          file-list                    List all files.
-          file-show                    Show a file.
-          job-delete                   Delete a job.
-          job-list                     List all jobs.
-          job-output                   Show the job output.
-          job-recheck                  Recheck a job.
-          job-results                  List all job results.
-          job-show                     Show a job.
-          jobdefinition-annotate       Annotate a jobdefinition.
-          jobdefinition-attach-test    Attach a test to a jobdefinition.
-          jobdefinition-create         Create a jobdefinition.
-          jobdefinition-delete         Delete a jobdefinition.
-          jobdefinition-list           List all jobdefinitions.
-          jobdefinition-list-test      List tests attached to a jobdefinition.
-          jobdefinition-set-active     Annotate a jobdefinition.
-          jobdefinition-show           Show a jobdefinition.
-          jobdefinition-unattach-test  Unattach a test to a jobdefinition.
-          jobdefinition-update         Update a jobdefinition.
-          jobstate-list                List all jobstates.
-          jobstate-show                Show a jobstate.
-          purge                        Purge soft-deleted resources.
-          remoteci-create              Create a remoteci.
-          remoteci-delete              Delete a remoteci.
-          remoteci-get-data            Retrieve data field from a remoteci.
-          remoteci-list                List all remotecis.
-          remoteci-refresh-keys        Refresh a remoteci key pair.
-          remoteci-reset-api-secret    Reset a remoteci api secret.
-          remoteci-show                Show a remoteci.
-          remoteci-update              Update a remoteci.
-          team-create                  Create a team.
-          team-delete                  Delete a team.
-          team-list                    List all teams.
-          team-show                    Show a team.
-          team-update                  Update a team.
-          topic-attach-team            Attach a team to a topic.
-          topic-create                 Create a topic.
-          topic-delete                 Delete a topic.
-          topic-list                   List all topics.
-          topic-list-team              List teams attached to a topic.
-          topic-show                   Show a topic.
-          topic-unattach-team          Unattach a team from a topic.
-          user-create                  Create a user.
-          user-delete                  Delete a user.
-          user-list                    List all users.
-          user-show                    Show a user.
-          user-update                  Update a user.
-        ```
-        
-        ## dci-vault
-        
-        If you want to store secrets in your YAML configuration files
-        (settings or inventories), you can use the `dci-vault` command to do
-        so. The various agents will then decrypt the secrets
-        transparently. For example:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ echo -n 42 | dci-vault encrypt_string --stdin-name answer
-        Reading plaintext input from stdin. (ctrl-d to end input)
-        answer: !vault |
-                  $ANSIBLE_VAULT;1.1;AES256
-                  36373332616633313866333234303166616237613332316534393834663934663463353433363464
-                  6363626133323036383939633566383139373636633533390a316363393437653663363538343730
-                  65333862633131353030353137636236663036656264393638353464343138623664323731613331
-                  6466636637393865380a336365633465633037623935633866366562373732356635343361353334
-                  3732
-        Encryption successful
-        ```
-        
-        `dci-vault` is a thin layer on top of `ansible-vault` so all the
-        sub-commands of `ansible-vault` are available.
-        
-        ## dci-rhel-latest-kernel-version
-        
-        The dci-rhel-latest-kernel-version is a utility command to easily get the
-        latest kernel available for the RHEL product.
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-rhel-latest-kernel-version --topic RHEL-not-existing
-        topic RHEL-not-existing not found
-        
-        - available topics:
-        RHEL-9.2
-        RHEL-9.1
-        RHEL-8.7
-        RHEL-8.6
-        RHEL-8.5
-        RHEL-9.0
-        RHEL-8.4
-        RHEL-8.0
-        RHEL-8.1
-        RHEL-7.6
-        RHEL-7.7
-        RHEL-8.3
-        RHEL-8.2
-        RHEL-7.8
-        RHEL-7.9
-        RHEL-7-nightly
-        RHEL-7-milestone
-        $ dci-rhel-latest-kernel-version --topic-list
-        available topics:
-        RHEL-9.2
-        RHEL-9.1
-        RHEL-9.0
-        RHEL-8.7
-        RHEL-8.6
-        RHEL-8.5
-        RHEL-8.4
-        RHEL-8.3
-        RHEL-8.2
-        RHEL-8.1
-        RHEL-8.0
-        RHEL-7.9
-        $ dci-rhel-latest-kernel-version --topic RHEL-9.2
-        5.14.0-160.el9
-        ```
-        
-        ## dci-create-component
-        
-        to create a component, you can use the `dci-create-component`
-        utility. For example, to create the `my-product` version `1.0`
-        component on the `OCP-4.11` topic, use it like that:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-create-component OCP-4.11 "My Company Product" 1.0 ga
-        ```
-        
-        ## dci-find-latest-component
-        
-        `dci-find-latest-component` allows to find the latest component for a
-        product. For example to find the latest GA OCP component on the most
-        recent topic, you can do it like this:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-find-latest-component --tags build:ga OpenShift ocp
-        ```
-        
-        To lookup the latest GA OCP component for a specific topic for example
-        OCP-4.11, you can do it like this:
-        
-        ```ShellSession
-        $ source dcirc.sh
-        $ dci-find-latest-component --topic OCP-4.11 --tags build:ga OpenShift ocp
-        ```
-        
-        ## License
-        
-        Apache 2.0
-        
-        ## Author Information
-        
-        Distributed-CI Team <distributed-ci@redhat.com>
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: System :: Distributed Computing
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# python-dciclient
+
+The `python-dciclient` project provides both the python bindings and a CLI to the [DCI Control Server](https://github.com/redhat-cip/dci-control-server)
+
+## Installation
+
+The team behind the project offers repositories for Red Hat/CentOS:
+
+- `yum -y install https://packages.distributed-ci.io/dci-release.el7.noarch.rpm`
+
+Then simply run `yum install python2-dciclient` for Python 2 or `yum install python3-dciclient` for Python 3.
+
+As mentioned above, the package provides two things:
+
+- The CLI: a `dcictl` command is provided. For more details `dcictl --help`.
+- The API: a python module one can use to interact with a control server (`dciclient.v1.api.*`)
+
+## Credentials
+
+Admitting one has valid credentials to use the DCI Control Server platform, there are two way to specify those informations while using dcictl:
+
+- A dcirc file:
+
+A file where the necessary credentials are stored. This file needs then to be sourced before using `dcictl`. Example:
+
+```
+export DCI_LOGIN=foo
+export DCI_PASSWORD=bar
+export DCI_CS_URL=https://api.distributed-ci.io
+```
+
+or using the API secret method:
+
+```
+export DCI_CLIENT_ID=<client_type>/<client_id>
+export DCI_API_SECRET=<api_secret>
+export DCI_CS_URL=https://api.distributed-ci.io
+```
+
+Where `client_type` can currently be `remoteci` or `feeder`
+
+Which will allow the user to run the command: `dcictl team-list`
+
+- At the command line level:
+
+One can pass those informations on the CLI level. Example: `dcictl --dci-login jdoe --dci-password jdoe --dci-cs-url 'https://api.distributed-ci.io' team-list`
+or `dcictl --dci-client-id <client_type>/<client_id> --dci-api-secret <api_secret> --dci-cs-url 'https://api.distributed-ci.io' team-list`
+
+Where `client_type` can currently be `remoteci` or `feeder`
+
+For RemoteCIs or Feeders please use the API Secret to authenticate.
+
+## List of available commands
+
+Run `dcictl --help` command to see the list of the available commands
+
+```
+Commands:
+  component-create             Create a component.
+  component-delete             Delete a component.
+  component-file-delete        Delete a component file.
+  component-file-download      Retrieve a component file.
+  component-file-list          List files attached to a component.
+  component-file-show          Show a component file.
+  component-file-upload        Attach a file to a component.
+  component-list               List all components.
+  component-show               Show a component.
+  component-status             Show an overview of the last jobs associated...
+  component-update             Update a component.
+  file-delete                  Delete a file.
+  file-list                    List all files.
+  file-show                    Show a file.
+  job-delete                   Delete a job.
+  job-list                     List all jobs.
+  job-output                   Show the job output.
+  job-recheck                  Recheck a job.
+  job-results                  List all job results.
+  job-show                     Show a job.
+  jobdefinition-annotate       Annotate a jobdefinition.
+  jobdefinition-attach-test    Attach a test to a jobdefinition.
+  jobdefinition-create         Create a jobdefinition.
+  jobdefinition-delete         Delete a jobdefinition.
+  jobdefinition-list           List all jobdefinitions.
+  jobdefinition-list-test      List tests attached to a jobdefinition.
+  jobdefinition-set-active     Annotate a jobdefinition.
+  jobdefinition-show           Show a jobdefinition.
+  jobdefinition-unattach-test  Unattach a test to a jobdefinition.
+  jobdefinition-update         Update a jobdefinition.
+  jobstate-list                List all jobstates.
+  jobstate-show                Show a jobstate.
+  purge                        Purge soft-deleted resources.
+  remoteci-create              Create a remoteci.
+  remoteci-delete              Delete a remoteci.
+  remoteci-get-data            Retrieve data field from a remoteci.
+  remoteci-list                List all remotecis.
+  remoteci-refresh-keys        Refresh a remoteci key pair.
+  remoteci-reset-api-secret    Reset a remoteci api secret.
+  remoteci-show                Show a remoteci.
+  remoteci-update              Update a remoteci.
+  team-create                  Create a team.
+  team-delete                  Delete a team.
+  team-list                    List all teams.
+  team-show                    Show a team.
+  team-update                  Update a team.
+  topic-attach-team            Attach a team to a topic.
+  topic-create                 Create a topic.
+  topic-delete                 Delete a topic.
+  topic-list                   List all topics.
+  topic-list-team              List teams attached to a topic.
+  topic-show                   Show a topic.
+  topic-unattach-team          Unattach a team from a topic.
+  user-create                  Create a user.
+  user-delete                  Delete a user.
+  user-list                    List all users.
+  user-show                    Show a user.
+  user-update                  Update a user.
+```
+
+## dci-vault
+
+If you want to store secrets in your YAML configuration files
+(settings or inventories), you can use the `dci-vault` command to do
+so. The various agents will then decrypt the secrets
+transparently. For example:
+
+```ShellSession
+$ source dcirc.sh
+$ echo -n 42 | dci-vault encrypt_string --stdin-name answer
+Reading plaintext input from stdin. (ctrl-d to end input)
+answer: !vault |
+          $ANSIBLE_VAULT;1.1;AES256
+          36373332616633313866333234303166616237613332316534393834663934663463353433363464
+          6363626133323036383939633566383139373636633533390a316363393437653663363538343730
+          65333862633131353030353137636236663036656264393638353464343138623664323731613331
+          6466636637393865380a336365633465633037623935633866366562373732356635343361353334
+          3732
+Encryption successful
+```
+
+`dci-vault` is a thin layer on top of `ansible-vault` so all the
+sub-commands of `ansible-vault` are available.
+
+## dci-rhel-latest-kernel-version
+
+The dci-rhel-latest-kernel-version is a utility command to easily get the
+latest kernel available for the RHEL product.
+
+```ShellSession
+$ source dcirc.sh
+$ dci-rhel-latest-kernel-version --topic RHEL-not-existing
+topic RHEL-not-existing not found
+
+- available topics:
+RHEL-9.2
+RHEL-9.1
+RHEL-8.7
+RHEL-8.6
+RHEL-8.5
+RHEL-9.0
+RHEL-8.4
+RHEL-8.0
+RHEL-8.1
+RHEL-7.6
+RHEL-7.7
+RHEL-8.3
+RHEL-8.2
+RHEL-7.8
+RHEL-7.9
+RHEL-7-nightly
+RHEL-7-milestone
+$ dci-rhel-latest-kernel-version --topic-list
+available topics:
+RHEL-9.2
+RHEL-9.1
+RHEL-9.0
+RHEL-8.7
+RHEL-8.6
+RHEL-8.5
+RHEL-8.4
+RHEL-8.3
+RHEL-8.2
+RHEL-8.1
+RHEL-8.0
+RHEL-7.9
+$ dci-rhel-latest-kernel-version --topic RHEL-9.2
+5.14.0-160.el9
+```
+
+## dci-create-component
+
+To create a component, you can use the `dci-create-component`
+utility. For example, to create the `ga` component called `My product` with version `1.0` on the `OCP-4.11` topic, use it like that:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-create-component OCP-4.11 "My Product" 1.0 ga
+```
+
+## dci-find-latest-component
+
+`dci-find-latest-component` allows to find the latest component for a
+product. For example to find the latest GA OCP component on the most
+recent topic, you can do it like this:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-find-latest-component --tags build:ga OpenShift ocp
+```
+
+To lookup the latest GA OCP component for a specific topic for example
+OCP-4.11, you can do it like this:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-find-latest-component --topic OCP-4.11 --tags build:ga OpenShift ocp
+```
+
+## dci-diff-jobs
+
+`dci-diff-jobs` allows to compare the components of 2 jobs:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-diff-jobs --job_id_1 9e3f3a4f-74c5-4bce-9c45-450b27006bed --job_id_2 b55fb5d6-3f01-44ce-9034-26a53e086137
++-----------------------+--------------------------------------+--------------------------------------+
+|       component       | 9e3f3a4f-74c5-4bce-9c45-450b27006bed | b55fb5d6-3f01-44ce-9034-26a53e086137 |
++-----------------------+--------------------------------------+--------------------------------------+
+|          ocp          |                4.9.50                |                4.8.52                |
+| redhat-operator-index |                 v4.9                 |                 v4.8                 |
++-----------------------+--------------------------------------+--------------------------------------+
+```
+
+or their tags:
+
+```ShellSession
+$ source dcirc.sh
+$ dci-diff-jobs --tags --job_id_1 9e3f3a4f-74c5-4bce-9c45-450b27006bed --job_id_2 b55fb5d6-3f01-44ce-9034-26a53e086137
++--------------------------------------+--------------------------------------+
+| 9e3f3a4f-74c5-4bce-9c45-450b27006bed | b55fb5d6-3f01-44ce-9034-26a53e086137 |
++--------------------------------------+--------------------------------------+
+|       pipeline-id:8nodes.8225        |              Not found               |
+|          inventory:cluster6          |              Not found               |
+|         pipeline:install-4.9         |              Not found               |
+|           cluster:cluster6           |              Not found               |
+|              Not found               |       pipeline-id:8nodes.8239        |
+|              Not found               |          inventory:cluster4          |
+|              Not found               |         pipeline:install-4.8         |
+|              Not found               |           cluster:cluster4           |
++--------------------------------------+--------------------------------------+
+```
+
+If the `--job_id_1` is not specified, the last job in success status is searched.
+
+If the `--job_id_2` is not specified, a job is searched with the same
+name, remoteci, topic, configuration and url than the job 1.
+
+## License
+
+Apache 2.0
+
+## Author Information
+
+Distributed-CI Team <distributed-ci@redhat.com>
```

### Comparing `dciclient-2.5.0/dciclient.egg-info/SOURCES.txt` & `dciclient-3.1.0/dciclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 start_db.sh
 dciclient/__init__.py
 dciclient/create_component.py
+dciclient/diff_jobs.py
 dciclient/find_latest_component.py
 dciclient/printer.py
 dciclient/rhel_kernel.py
 dciclient/shell.py
 dciclient/vault.py
 dciclient/vault_client.py
 dciclient/version.py
```

### Comparing `dciclient-2.5.0/setup.py` & `dciclient-3.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,18 +59,19 @@
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Topic :: System :: Distributed Computing",
     ],
-    entry_points={"console_scripts": ["dcictl = dciclient.shell:main",
-                                      "dci-vault = dciclient.vault:main",
-                                      "dci-vault-client = dciclient.vault_client:main",
-                                      "dci-create-component = "
-                                      "dciclient.create_component:main",
-                                      "dci-find-latest-component = "
-                                      "dciclient.find_latest_component:main",
-                                      "dci-rhel-latest-kernel-version = "
-                                      "dciclient.rhel_kernel:main",
-                                      ]},
+    entry_points={
+        "console_scripts": [
+            "dcictl = dciclient.shell:main",
+            "dci-vault = dciclient.vault:main",
+            "dci-vault-client = dciclient.vault_client:main",
+            "dci-create-component = dciclient.create_component:main",
+            "dci-find-latest-component = dciclient.find_latest_component:main",
+            "dci-rhel-latest-kernel-version = dciclient.rhel_kernel:main",
+            "dci-diff-jobs = dciclient.diff_jobs:main",
+        ]
+    },
 )
```

### Comparing `dciclient-2.5.0/start_db.sh` & `dciclient-3.1.0/start_db.sh`

 * *Files identical despite different names*


# Comparing `tmp/vdk-control-cli-1.3.854774602.tar.gz` & `tmp/vdk-control-cli-1.3.864600569.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.854774602.tar", last modified: Tue May  2 14:05:18 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.864600569.tar", last modified: Thu May 11 15:33:38 2023, max compression
```

## Comparing `vdk-control-cli-1.3.854774602.tar` & `vdk-control-cli-1.3.864600569.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    11236 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14012 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5115 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12088 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4768 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3458 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     2915 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-05-02 14:05:01.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-02 14:05:05.000000 vdk-control-cli-1.3.854774602/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2312 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-02 14:05:18.000000 vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-02 14:05:05.000000 vdk-control-cli-1.3.854774602/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    11236 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14329 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5115 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12198 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9834 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-11 15:33:25.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-11 15:33:25.000000 vdk-control-cli-1.3.864600569/version.txt
```

### Comparing `vdk-control-cli-1.3.854774602/PKG-INFO` & `vdk-control-cli-1.3.864600569/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.854774602
+Version: 1.3.864600569
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.854774602/README.md` & `vdk-control-cli-1.3.864600569/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/setup.cfg` & `vdk-control-cli-1.3.864600569/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,47 +150,47 @@
     def update(
         self,
         name: str,
         team: str,
         enabled: Optional[bool],  # true, false or None
         job_version: Optional[str],
         vdk_version: Optional[str],
+        python_version: Optional[str] = None,
     ) -> None:
         deployment = DataJobDeployment(enabled=None)
         if job_version:
             deployment.job_version = job_version
         if vdk_version:
             deployment.vdk_version = vdk_version
+        if python_version:
+            deployment.python_version = python_version
         deployment.enabled = enabled
 
-        if job_version:
-            self.__update_job_version(name, team, deployment)
-        elif vdk_version or enabled is not None:
+        if job_version or python_version or vdk_version:
             self.__update_deployment(name, team, deployment)
+        elif enabled is not None:
+            self.__patch_deployment(name, team, deployment)
             msg = f"Deployment of Data Job {name} updated; "
-            if vdk_version:
-                msg = msg + f"vdk version: {vdk_version}; "
-            if enabled is not None:
-                msg = msg + "status: " + ("enabled" if enabled else "disabled") + "; "
+            msg = msg + "status: " + ("enabled" if enabled else "disabled") + "; "
             log.info(msg)
         else:
             log.warning(f"Nothing to update for deployment of job {name}.")
 
-    def __update_deployment(
+    def __patch_deployment(
         self, name: str, team: str, deployment: DataJobDeployment
     ) -> None:
         log.debug(f"Update Deployment of a job {name} of team {team} : {deployment}")
         self.deploy_api.deployment_patch(
             team_name=team,
             job_name=name,
             deployment_id=self.__deployment_id,
             data_job_deployment=deployment,
         )
 
-    def __update_job_version(self, name: str, team: str, deployment: DataJobDeployment):
+    def __update_deployment(self, name: str, team: str, deployment: DataJobDeployment):
         log.debug(
             f"Update Deployment version of a job {name} of team {team} : {deployment}"
         )
         self.deploy_api.deployment_update(
             team_name=team, job_name=name, data_job_deployment=deployment
         )
         if self.__output_format == OutputFormat.TEXT.value:
@@ -203,14 +203,15 @@
                 f"to the one of the newly deployed job - {deployment.job_version} - to verify that the deployment "
                 f"was successful."
             )
         else:
             result = {
                 "job_name": name,
                 "job_version": deployment.job_version,
+                "python_version": deployment.python_version,
             }
             self.__printer.print_dict(result)
 
     @ApiClientErrorDecorator()
     def remove(self, name: str, team: str) -> None:
         log.debug(f"Remove Deployment of a job {name} of team {team}")
         self.deploy_api.deployment_delete(
@@ -229,14 +230,15 @@
             # d.to_dict() brings unnecessary parts of data
             deployments = map(
                 lambda d: dict(
                     job_name=name,
                     job_version=d.job_version,
                     last_deployed_by=d.last_deployed_by,
                     last_deployed_date=d.last_deployed_date,
+                    python_version=d.python_version,
                     enabled=d.enabled,
                 ),
                 deployments,
             )
             if self.__output_format == OutputFormat.TEXT.value:
                 click.echo(
                     "You can compare the version seen here to the one seen when "
@@ -300,11 +302,20 @@
                 data_job_version = self.job_sources_api.sources_upload(
                     team_name=team,
                     job_name=name,
                     body=job_archive_binary,
                     reason=reason,
                 )
 
+            python_version = job_config.get_python_version()
+
             self.__update_data_job_deploy_configuration(job_path, name, team)
-            self.update(name, team, enabled, data_job_version.version_sha, vdk_version)
+            self.update(
+                name,
+                team,
+                enabled,
+                data_job_version.version_sha,
+                vdk_version,
+                python_version,
+            )
         finally:
             self.__cleanup_archive(archive_path=archive_path)
```

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         self.__execution_api = ApiClientFactory(rest_api_url).get_execution_api()
 
     @staticmethod
     def __model_executions(executions, output_format: OutputFormat) -> str:
         def transform_execution(e: DataJobExecution):
             d = e.to_dict()
             d["job_version"] = e.deployment.job_version
+            if e.deployment.python_version:
+                d["python_version"] = e.deployment.python_version
             del d["deployment"]
             return d
 
         executions = list(map(lambda e: transform_execution(e), executions))
         output_printer.create_printer(output_format).print_table(executions)
 
     @staticmethod
```

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         Returns True if team is found and successfully set to 'value' in config.ini, False - otherwise
         """
         return self._set_value("owner", "team", value)
 
     def get_schedule_cron(self) -> str:
         return self._get_value("job", "schedule_cron")
 
+    def get_python_version(self) -> str:
+        return str(self._get_value("job", "python_version"))
+
     def get_enable_execution_notifications(self) -> bool:
         return self._get_boolean(
             "contacts", "enable_execution_notifications", fallback=True
         )
 
     def get_notification_delay_period_minutes(self) -> int:
         return self._get_positive_int(
```

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import click
 import click_log
 from vdk.internal.control.command_groups.common_group.default import (
     reset_default_command,
 )
 from vdk.internal.control.command_groups.common_group.default import set_default_command
+from vdk.internal.control.command_groups.info_group.info import info
 from vdk.internal.control.command_groups.job.create import create
 from vdk.internal.control.command_groups.job.delete import delete
 from vdk.internal.control.command_groups.job.deploy_cli import deploy
 from vdk.internal.control.command_groups.job.download_job import download_job
 from vdk.internal.control.command_groups.job.download_key import download_key
 from vdk.internal.control.command_groups.job.execute import execute
 from vdk.internal.control.command_groups.job.list import list_command
@@ -87,13 +88,14 @@
     cli.add_command(version)
     cli.add_command(execute)
     cli.add_command(set_default_command)
     cli.add_command(reset_default_command)
     cli.add_command(download_job)
     cli.add_command(show_command)
     cli.add_command(properties_command)
+    cli.add_command(info)
 
     cli()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from taurus_datajob_api import ApiClient
 from taurus_datajob_api import Configuration
 from taurus_datajob_api import DataJobsApi
 from taurus_datajob_api import DataJobsDeploymentApi
 from taurus_datajob_api import DataJobsExecutionApi
 from taurus_datajob_api import DataJobsPropertiesApi
+from taurus_datajob_api import DataJobsServiceApi
 from taurus_datajob_api import DataJobsSourcesApi
 from urllib3 import Retry
 from vdk.internal.control.configuration.vdk_config import VDKConfig
 from vdk.plugin.control_api_auth.authentication import Authentication
 
 log = logging.getLogger(__name__)
 
@@ -62,7 +63,10 @@
         return DataJobsDeploymentApi(self._new_api_client())
 
     def get_execution_api(self) -> DataJobsExecutionApi:
         return DataJobsExecutionApi(self._new_api_client())
 
     def get_properties_api(self) -> DataJobsPropertiesApi:
         return DataJobsPropertiesApi(self._new_api_client())
+
+    def get_service_api(self) -> DataJobsServiceApi:
+        return DataJobsServiceApi(self._new_api_client())
```

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.854774602
+Version: 1.3.864600569
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.854774602/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 version.txt
 src/vdk/api/control/plugin/markers.py
 src/vdk/api/control/plugin/specs.py
 src/vdk/internal/control/main.py
 src/vdk/internal/control/vdk_control_build_info.py
 src/vdk/internal/control/command_groups/common_group/default.py
+src/vdk/internal/control/command_groups/info_group/info.py
 src/vdk/internal/control/command_groups/job/create.py
 src/vdk/internal/control/command_groups/job/delete.py
 src/vdk/internal/control/command_groups/job/deploy_cli.py
 src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
 src/vdk/internal/control/command_groups/job/download_job.py
 src/vdk/internal/control/command_groups/job/download_key.py
 src/vdk/internal/control/command_groups/job/execute.py
```


# Comparing `tmp/dagster_cloud_cli-1.3.3.tar.gz` & `tmp/dagster_cloud_cli-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_cli-1.3.3.tar", last modified: Thu May  4 17:55:45 2023, max compression
+gzip compressed data, was "dagster_cloud_cli-1.3.4.tar", last modified: Thu May 11 17:10:52 2023, max compression
```

## Comparing `dagster_cloud_cli-1.3.3.tar` & `dagster_cloud_cli-1.3.4.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    17040 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.797916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.801916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.805916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11997 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17972 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.809916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.809916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.809916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9467 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13847 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)     5976 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5384 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6700 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.793916 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2765 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-04 17:55:45.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8588 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)     9821 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_state.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 17:55:45.817916 dagster_cloud_cli-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-04 17:42:29.000000 dagster_cloud_cli-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.447464 dagster_cloud_cli-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-11 17:10:52.447464 dagster_cloud_cli-1.3.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.651465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.655465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.655465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.767465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    20512 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.815465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.883465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.931465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.947465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.947465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.951465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.991464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.051464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    11997 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18291 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.163464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.199464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.219464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.279464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13847 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)     5976 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6700 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.655465 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.383464 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    15025 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 17:10:52.447464 dagster_cloud_cli-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/setup.py
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,35 @@
 from collections import Counter
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 import typer
 from typer import Typer
 
-from dagster_cloud_cli import docker_utils, gql, ui
+from dagster_cloud_cli import docker_utils, gql, pex_utils, ui
 from dagster_cloud_cli.commands.ci import utils
 from dagster_cloud_cli.commands.workspace import wait_for_load
 from dagster_cloud_cli.config_utils import (
     AGENT_HEARTBEAT_TIMEOUT_OPTION,
+    DAGSTER_ENV_OPTION,
     LOCATION_LOAD_TIMEOUT_OPTION,
+    ORGANIZATION_OPTION,
+    TOKEN_ENV_VAR_NAME,
+    URL_ENV_VAR_NAME,
+    dagster_cloud_options,
     get_location_document,
+    get_org_url,
 )
 from dagster_cloud_cli.core import pex_builder, pydantic_yaml
 
 from .. import metrics
 from . import checks, state
 
 app = Typer(hidden=True, help="CI/CD agnostic commands")
-from dagster_cloud_cli.core.pex_builder import code_location, github_context
+from dagster_cloud_cli.core.pex_builder import code_location, deps, github_context, parse_workspace
 from dagster_cloud_cli.types import CliEventTags
 
 
 @app.command(help="Print json information about current CI/CD environment")
 def inspect(project_dir: str):
     project_dir = os.path.abspath(project_dir)
     source = metrics.get_source()
@@ -48,44 +54,58 @@
         "commit-hash": event.github_sha,
     }
 
 
 @app.command(
     help=(
         "Print the branch deployment name (or nothing) for the current context. Creates a new"
-        " branch deployment if necessary. Requires DAGSTER_CLOUD_URL and DAGSTER_CLOUD_API_TOKEN"
-        " environment variables."
+        " branch deployment if necessary. Requires DAGSTER_CLOUD_ORGANIZATION and"
+        " DAGSTER_CLOUD_API_TOKEN environment variables."
     )
 )
-def branch_deployment(project_dir: str):
+def branch_deployment(
+    project_dir: str,
+    organization: Optional[str] = ORGANIZATION_OPTION,
+    dagster_env: Optional[str] = DAGSTER_ENV_OPTION,
+):
     try:
-        print(get_deployment_from_context(project_dir))
+        if organization:
+            url = get_org_url(organization, dagster_env)
+        else:
+            url = os.environ[URL_ENV_VAR_NAME]
+        print(get_deployment_from_context(url, project_dir))
     except ValueError as err:
         logging.error(
             f"cannot determine branch deployment: {err}",
         )
         sys.exit(1)
 
 
-def get_deployment_from_context(project_dir: str) -> Optional[str]:
+def get_deployment_from_context(url, project_dir: str) -> str:
     source = metrics.get_source()
     if source == CliEventTags.source.github:
         event = github_context.get_github_event(project_dir)
-        url = os.environ["DAGSTER_CLOUD_URL"]
-        api_token = os.environ["DAGSTER_CLOUD_API_TOKEN"]
+        api_token = os.environ[TOKEN_ENV_VAR_NAME]
         deployment_name = code_location.create_or_update_branch_deployment_from_github_context(
             url, api_token, event
         )
+        if not deployment_name:
+            raise ValueError(
+                f"could not determine branch deployment for PR {event.pull_request_id}"
+            )
+
         return deployment_name
     else:
         raise ValueError(f"unsupported for {source}")
 
 
 @app.command(help="Validate configuration")
 def check(
+    organization: Optional[str] = ORGANIZATION_OPTION,
+    dagster_env: Optional[str] = DAGSTER_ENV_OPTION,
     project_dir: str = typer.Option("."),
     dagster_cloud_yaml_path: str = "dagster_cloud.yaml",
     dagster_cloud_yaml_check: checks.Check = typer.Option("error"),
     dagster_cloud_connect_check: checks.Check = typer.Option("error"),
 ):
     project_path = pathlib.Path(project_dir)
 
@@ -97,21 +117,26 @@
             checks.handle_result(
                 result,
                 dagster_cloud_yaml_check,
                 prefix_message="[dagster_cloud.yaml] ",
                 success_message="Checked OK",
                 failure_message=(
                     "Invalid dagster_cloud.yaml, please see"
-                    " https://docs.dagster.io/dagster-cloud/developing-testing/code-locations#syncing-the-workspace"
+                    " https://docs.dagster.io/dagster-cloud/managing-deployments/dagster-cloud-yaml"
                 ),
             )
         )
 
     if dagster_cloud_connect_check != checks.Check.skip:
-        result = checks.check_connect_dagster_cloud()
+        if not organization:
+            raise ui.error(
+                "DAGSTER_CLOUD_ORGANIZATION or --organization required for connection check."
+            )
+        url = get_org_url(organization, dagster_env)
+        result = checks.check_connect_dagster_cloud(url)
         verdicts.append(
             checks.handle_result(
                 result,
                 dagster_cloud_connect_check,
                 prefix_message="[dagster.cloud connection] ",
                 success_message="Able to connect to dagster.cloud",
                 failure_message="Unable to connect to dagster.cloud",
@@ -127,58 +152,72 @@
         sys.exit(1)
 
 
 STATEDIR_OPTION = typer.Option(..., envvar="DAGSTER_BUILD_STATEDIR")
 
 
 @app.command(help="Initialize a build session")
+@dagster_cloud_options(allow_empty=False, allow_empty_deployment=True, requires_url=False)
 def init(
+    organization: str,
+    deployment: Optional[str],
+    dagster_env: Optional[str] = DAGSTER_ENV_OPTION,
     project_dir: str = typer.Option("."),
     dagster_cloud_yaml_path: str = "dagster_cloud.yaml",
-    deployment: Optional[str] = None,
     statedir: str = STATEDIR_OPTION,
     clean_statedir: bool = typer.Option(True, help="Delete any existing files in statedir"),
     location_name: List[str] = typer.Option([]),
+    git_url: Optional[str] = None,
+    commit_hash: Optional[str] = None,
 ):
     yaml_path = pathlib.Path(project_dir) / dagster_cloud_yaml_path
     locations_def = pydantic_yaml.load_dagster_cloud_yaml(yaml_path.read_text())
     locations = locations_def.locations
     if location_name:
         selected_locations = set(location_name)
         unknown = selected_locations - set(location.location_name for location in locations)
         if unknown:
             raise ui.error(f"Locations not found in {dagster_cloud_yaml_path}: {unknown}")
         locations = [
             location for location in locations if location.location_name in selected_locations
         ]
-
-    url = os.environ["DAGSTER_CLOUD_URL"]
-    if deployment is None:
-        try:
-            deployment = get_deployment_from_context(project_dir)
-        except ValueError as err:
+    url = get_org_url(organization, dagster_env)
+    # Deploy to the branch deployment for the current context. If there is no branch deployment
+    # available (eg. if not in a PR) then we fallback to the --deployment flag.
+    try:
+        branch_deployment = get_deployment_from_context(url, project_dir)
+        if deployment:
+            ui.print(
+                f"Deploying to branch deployment {branch_deployment}, ignoring"
+                f" --deployment={deployment}"
+            )
+        deployment = branch_deployment
+    except ValueError as err:
+        if deployment:
+            ui.print(f"Deploying to {deployment}. No branch deployment ({err}).")
+        else:
             raise ui.error(
                 f"Cannot determine deployment name in current context ({err}). Please specify"
                 " --deployment."
             )
-        if deployment is None:
-            deployment = "prod"
 
     if clean_statedir and os.path.exists(statedir):
         shutil.rmtree(statedir, ignore_errors=True)
     state_store = state.FileStore(statedir=statedir)
 
     ui.print(f"Initializing {statedir}")
     for location in locations:
         location_state = state.LocationState(
             url=url,
             deployment_name=deployment,
             location_file=str(yaml_path.absolute()),
             location_name=location.location_name,
-            build=location.build,
+            build=state.BuildMetadata(
+                git_url=git_url, commit_hash=commit_hash, build_config=location.build
+            ),
             build_output=None,
         )
         state_store.save(location_state)
 
     ui.print(
         f"Initialized {statedir} to build and deploying following locations for directory"
         f" {project_dir}:"
@@ -255,57 +294,64 @@
     build_directory: Optional[str] = typer.Option(
         None,
         help=(
             "Directory root for building this code location. Read from dagster_cloud.yaml by"
             " default."
         ),
     ),
-    image_tag: Optional[str] = typer.Option(
+    build_strategy: BuildStrategy = typer.Option(
+        "docker",
+        help=(
+            "Build strategy used to build code locations. 'docker' builds a docker image."
+            " 'python-executable' builds a set of pex files."
+        ),
+    ),
+    docker_image_tag: Optional[str] = typer.Option(
         None, help="Tag for built docker image. Auto-generated by default."
     ),
-    base_image: Optional[str] = typer.Option(
+    docker_base_image: Optional[str] = typer.Option(
         None,
         help="Base image used to build the docker image for --build-strategy=docker.",
     ),
-    env: List[str] = typer.Option([], help="Env vars for docker builds."),
-    commit_hash: Optional[str] = typer.Option(
-        None, help="Commit hash of project used to generate the default docker tag."
-    ),
-    python_version: Optional[str] = typer.Option(
+    docker_env: List[str] = typer.Option([], help="Env vars for docker builds."),
+    python_version: str = typer.Option(
         "3.8",
         help=(
             "Python version used to build the python-executable; or to determine the default base"
             " image for docker."
         ),
     ),
-    build_strategy: BuildStrategy = typer.Option(
-        "docker",
-        help=(
-            "Build strategy used to build code locations. 'docker' builds a docker image."
-            " 'python-executable' builds a set of pex files."
-        ),
+    pex_build_method: deps.BuildMethod = typer.Option("local"),
+    pex_deps_cache_from: Optional[str] = None,
+    pex_deps_cache_to: Optional[str] = None,
+    pex_base_image_tag: Optional[str] = typer.Option(
+        None,
+        help="Base image used to run python executable for --build-strategy=python-executable.",
     ),
-):
+) -> None:
     if python_version:
         # ensure version is parseable
         pex_builder.util.parse_python_version(python_version)
 
     if build_strategy == BuildStrategy.pex:
-        raise ui.error("--build-strategy=python-executable not implemented yet.")
+        if docker_base_image or docker_image_tag:
+            raise ui.error(
+                "--base-image or --image-tag not supported for --build-strategy=python-executable."
+            )
 
     state_store = state.FileStore(statedir=statedir)
     locations = _get_selected_locations(state_store, location_name)
     ui.print("Going to build the following locations:")
     for name in locations:
         ui.print(f"- {name}")
 
     for name, location_state in locations.items():
         configured_build_directory = (
-            location_state.build.directory
-            if (location_state.build and location_state.build.directory)
+            location_state.build.build_config.directory
+            if (location_state.build.build_config and location_state.build.build_config.directory)
             else None
         )
         if build_directory and configured_build_directory:
             ui.warn(
                 f"Overriding configured build:directory:{configured_build_directory!r} with"
                 f" cmdline provided --build-directory={build_directory!r}"
             )
@@ -314,59 +360,89 @@
             location_build_dir = configured_build_directory
         elif build_directory and (not configured_build_directory):
             location_build_dir = build_directory
         else:
             location_build_dir = "."
 
         if build_strategy == BuildStrategy.docker:
-            if not base_image:
-                base_image = f"python:{python_version}-slim"
+            if not docker_base_image:
+                docker_base_image = f"python:{python_version}-slim"
 
-            ui.print(f"Building docker image for location {name} using base image {base_image}")
+            ui.print(
+                f"Building docker image for location {name} using base image {docker_base_image}"
+            )
             docker_utils.verify_docker()
-            registry_info = utils.get_registry_info()
+            registry_info = utils.get_registry_info(location_state.url)
 
-            image_tag = docker_utils.default_image_tag(
-                location_state.deployment_name, name, commit_hash
+            docker_image_tag = docker_utils.default_image_tag(
+                location_state.deployment_name, name, location_state.build.commit_hash
             )
 
             retval = docker_utils.build_image(
-                location_build_dir, image_tag, registry_info, env_vars=env, base_image=base_image
+                location_build_dir,
+                docker_image_tag,
+                registry_info,
+                env_vars=docker_env,
+                base_image=docker_base_image,
             )
             if retval != 0:
                 raise ui.error(f"Failed to build docker image for location {name}")
 
-            retval = docker_utils.upload_image(image_tag, registry_info)
+            retval = docker_utils.upload_image(docker_image_tag, registry_info)
             if retval != 0:
                 raise ui.error(f"Failed to upload docker image for location {name}")
 
-            image = f'{registry_info["registry_url"]}:{image_tag}'
+            image = f'{registry_info["registry_url"]}:{docker_image_tag}'
 
             # Update and save build state
-            location_state.build_output = state.DockerBuildOutput(
-                image=image, commit_hash=commit_hash
-            )
+            location_state.build_output = state.DockerBuildOutput(image=image)
             state_store.save(location_state)
             ui.print(f"Built and uploaded image {image} for location {name}")
+        elif build_strategy == BuildStrategy.pex:
+            pex_location = parse_workspace.Location(
+                name,
+                directory=location_build_dir,
+                build_folder=location_build_dir,
+                location_file=location_state.location_file,
+            )
+            location_kwargs = pex_utils.build_upload_pex(
+                url=location_state.url,
+                api_token=os.environ[TOKEN_ENV_VAR_NAME],
+                location=pex_location,
+                build_method=pex_build_method,
+                kwargs={
+                    "python_version": python_version,
+                    "base_image_tag": pex_base_image_tag,
+                    "deps_cache_from": pex_deps_cache_from,
+                    "deps_cache_to": pex_deps_cache_to,
+                },
+            )
+            location_state.build_output = state.PexBuildOutput(
+                python_version=python_version,
+                image=location_kwargs["image"],
+                pex_tag=location_kwargs["pex_tag"],
+            )
+            state_store.save(location_state)
+            ui.print(
+                f"Build and uploaded python executable {location_state.build_output.pex_tag} for"
+                f" location {name}"
+            )
 
 
 @app.command(help="Update the current build session for an externally built docker image.")
 def set_build_output(
     statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
     location_name: List[str] = typer.Option([]),
     image_tag: str = typer.Option(
         ...,
         help=(
             "Tag for the built docker image. Note the registry must be specified in"
             " dagster_cloud.yaml."
         ),
     ),
-    commit_hash: Optional[str] = typer.Option(
-        None, help="Commit hash of project used to generate the docker image."
-    ),
 ) -> None:
     state_store = state.FileStore(statedir=statedir)
     locations = _get_selected_locations(state_store, location_name)
     ui.print("Going to update the following locations:")
     for name in locations:
         ui.print(f"- {name}")
 
@@ -387,17 +463,15 @@
             )
 
         images[name] = f"{registry}:{image_tag}"
 
     # save pass - save full image name computed in the previous pass for all locations
     for name, location_state in locations.items():
         # Update and save build state
-        location_state.build_output = state.DockerBuildOutput(
-            image=images[name], commit_hash=commit_hash
-        )
+        location_state.build_output = state.DockerBuildOutput(image=images[name])
         state_store.save(location_state)
         ui.print(f"Recorded image {images[name]} for location {name}")
     ui.print("Use 'ci deploy' to update dagster-cloud.")
 
 
 @app.command(help="Deploy built code locations to dagster cloud.")
 def deploy(
@@ -429,23 +503,28 @@
         ui.print("No locations to deploy")
         return
 
     for location_state in built_locations:
         location_args = {
             "image": location_state.build_output.image,
             "location_file": location_state.location_file,
-            "commit_hash": location_state.build_output.commit_hash,
+            "git_url": location_state.build.git_url,
+            "commit_hash": location_state.build.commit_hash,
         }
-        with utils.client_from_env(location_state.deployment_name) as client:
+        if location_state.build_output.strategy == "python-executable":
+            location_args["pex_tag"] = location_state.build_output.pex_tag
+        with utils.client_from_env(location_state.url, location_state.deployment_name) as client:
             location_document = get_location_document(location_state.location_name, location_args)
             gql.add_or_update_code_location(client, location_document)
             ui.print(f"Updated code location {location_state.location_name} in dagster-cloud")
 
     url = built_locations[0].url + "/" + built_locations[0].deployment_name
-    with utils.client_from_env(deployment=built_locations[0].deployment_name) as client:
+    with utils.client_from_env(
+        built_locations[0].url, deployment=built_locations[0].deployment_name
+    ) as client:
         wait_for_load(
             client,
             [location.location_name for location in built_locations],
             location_load_timeout=location_load_timeout,
             agent_heartbeat_timeout=agent_heartbeat_timeout,
             url=url,
         )
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/checks.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/checks.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import List
 
 import pydantic
 
 from dagster_cloud_cli import gql
+from dagster_cloud_cli.config_utils import TOKEN_ENV_VAR_NAME
 
 from ... import ui
 from ...core import pydantic_yaml
 
 
 def get_validation_errors(validation_error: pydantic.ValidationError) -> List[str]:
     errors = []
@@ -118,26 +119,20 @@
     else:
         passed(success_message)
         print_indented(result.messages)
         ui.print("\n")
         return Verdict.passed
 
 
-def check_connect_dagster_cloud() -> CheckResult:
-    if "DAGSTER_CLOUD_URL" not in os.environ:
-        return CheckResult(["DAGSTER_CLOUD_URL not set"])
-    if "DAGSTER_CLOUD_API_TOKEN" not in os.environ:
-        return CheckResult(["DAGSTER_CLOUD_API_TOKEN not set"])
+def check_connect_dagster_cloud(url) -> CheckResult:
+    if TOKEN_ENV_VAR_NAME not in os.environ:
+        return CheckResult([f"{TOKEN_ENV_VAR_NAME} not set"])
     result = CheckResult()
-    result.messages.append(
-        f"Connecting to {os.environ['DAGSTER_CLOUD_URL']} using DAGSTER_CLOUD_API_TOKEN"
-    )
-    with gql.graphql_client_from_url(
-        os.environ["DAGSTER_CLOUD_URL"], os.environ["DAGSTER_CLOUD_API_TOKEN"]
-    ) as client:
+    result.messages.append(f"Connecting to {url} using {TOKEN_ENV_VAR_NAME}")
+    with gql.graphql_client_from_url(url, os.environ[TOKEN_ENV_VAR_NAME]) as client:
         try:
             gql.get_organization_settings(client)
             result.messages.append("Connection successful")
         except Exception as err:
-            result.errors.append(f"Failed to connect to {os.environ['DAGSTER_CLOUD_URL']}: {err}")
+            result.errors.append(f"Failed to connect to {url}: {err}")
 
     return result
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/ci/state.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,37 @@
 from dagster_cloud_cli.core import pydantic_yaml
 
 
 class DockerBuildOutput(BaseModel, extra=Extra.forbid):
     strategy: Literal["docker"] = "docker"
     python_version: Optional[str] = None
     image: str
-    commit_hash: Optional[str] = None
 
 
 class PexBuildOutput(BaseModel, extra=Extra.forbid):
     strategy: Literal["python-executable"] = "python-executable"
     python_version: str
     image: str
-    # TBD: add more pex build specific fields
+    pex_tag: str
+
+
+class BuildMetadata(BaseModel):
+    git_url: Optional[str]
+    commit_hash: Optional[str]
+    build_config: Optional[pydantic_yaml.Build]  # copied from dagster_cloud.yaml
 
 
 class LocationState(BaseModel, extra=Extra.forbid):
     # we intentionally don't save api_token here for security reasons
     url: str
     deployment_name: str
     location_file: str
     location_name: str
     selected: bool = True
-    build: Optional[pydantic_yaml.Build]  # copied from dagster_cloud.yaml
+    build: BuildMetadata
     build_output: Optional[Union[DockerBuildOutput, PexBuildOutput]] = Field(
         None, discriminator="strategy"
     )
 
 
 class Store(metaclass=ABCMeta):
     @abstractmethod
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/config.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/job/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/run/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/config_utils.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/config_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,14 +161,20 @@
 def get_url(ctx: Optional[Context] = None) -> Optional[str]:
     """Gets the url passed in or from the environment."""
     if ctx and ctx.params.get(URL_CLI_ARGUMENT):
         return ctx.params[URL_CLI_ARGUMENT]
     return os.getenv(URL_ENV_VAR_NAME)
 
 
+def get_org_url(organization: str, dagster_env: Optional[str]):
+    if dagster_env:
+        return f"https://{organization}.{dagster_env}.dagster.cloud"
+    return f"https://{organization}.dagster.cloud"
+
+
 # Typer Option definitions for common CLI config options (organization, deployment, user token)
 ORGANIZATION_OPTION = Option(
     get_organization,
     "--organization",
     "-o",
     help="Organization to target.",
     show_default=get_organization(),  # type: ignore
@@ -177,14 +183,22 @@
     get_deployment,
     "--deployment",
     "-d",
     help="Deployment to target.",
     autocompletion=available_deployment_names,
     show_default=get_deployment(),  # type: ignore
 )
+
+DAGSTER_ENV_OPTION = Option(
+    None,
+    "--dagster-env",
+    hidden=True,
+    envvar="DAGSTER_CLOUD_ENV",
+)
+
 USER_TOKEN_OPTION = Option(
     get_user_token,
     "--api-token",
     "--user-token",
     "-u",
     help="Cloud user token.",
     show_default=ui.censor_token(get_user_token()) if get_user_token() else None,  # type: ignore
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/docker_runner.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/errors.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/graphql_client.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/headers/impl.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 
 def create_or_update_branch_deployment_from_github_context(
     dagster_cloud_org_url: str,
     dagster_cloud_api_token: str,
     github_event: github_context.GithubEvent,
 ) -> Optional[str]:
+    """Return the branch deployment associated with the github PR."""
     event = github_event
     logging.debug("Read github event GithubEvent(%r)", event.__dict__)
     if not event.branch_name:
         logging.info("Not in a branch, not creating branch deployment")
         return None
     else:
-        url = f"{dagster_cloud_org_url}/prod"
+        url = f"{dagster_cloud_org_url}"
         with gql.graphql_client_from_url(url, dagster_cloud_api_token) as client:
             deployment_name = gql.create_or_update_branch_deployment(
                 client,
                 repo_name=event.repo_name,
                 branch_name=event.branch_name,
                 commit_hash=event.github_sha,
                 timestamp=event.timestamp,
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/source.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pex_builder/util.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/core/workspace.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/docker_utils.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/entrypoint.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/gql.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/pex_utils.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/types.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/ui.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli/utils.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,11 +56,12 @@
 dagster_cloud_cli/core/pex_builder/github_context.py
 dagster_cloud_cli/core/pex_builder/parse_workspace.py
 dagster_cloud_cli/core/pex_builder/pex_registry.py
 dagster_cloud_cli/core/pex_builder/selftest.py
 dagster_cloud_cli/core/pex_builder/source.py
 dagster_cloud_cli/core/pex_builder/util.py
 dagster_cloud_cli_tests/__init__.py
+dagster_cloud_cli_tests/conftest.py
 dagster_cloud_cli_tests/test_check.py
+dagster_cloud_cli_tests/test_ci_commands.py
 dagster_cloud_cli_tests/test_gql.py
-dagster_cloud_cli_tests/test_metrics.py
-dagster_cloud_cli_tests/test_state.py
+dagster_cloud_cli_tests/test_metrics.py
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_gql.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_metrics.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         @metrics.instrument(CliEventType.DEPLOY, tags=[CliEventTags.server_strategy.pex])
         def instrumented_with_tags_command(api_token: str, url: str, raising: bool, **kwargs):
             frozen_datetime.tick()
             if raising:
                 raise ui.error("boom")
             else:
                 ui.print("ok")
+            metrics.instrument_add_tags([CliEventTags.source.bitbucket])
 
         env = {
             "DAGSTER_CLOUD_API_TOKEN": "fake-token",
             "DAGSTER_CLOUD_ORGANIZATION": "fake-organization",
             "DAGSTER_CLOUD_DEPLOYMENT": "fake-deployment",
         }
 
@@ -156,15 +157,16 @@
         gql.mark_cli_event.assert_has_calls(
             [
                 call(
                     client=ANY,
                     duration_seconds=1,
                     event_type=CliEventType.DEPLOY,
                     success=True,
-                    tags=["server-strategy:pex", "source:cli"],
+                    # 'source:bitbucket' expected from the instrument_add_tags() call
+                    tags=["server-strategy:pex", "source:cli", "source:bitbucket"],
                 ),
             ]
         )
 
         # env is checked when the decorator executes, so we need a new command for GITHUB_ACTION
         monkeypatch.setenv("GITHUB_ACTION", "test-action")
```

### Comparing `dagster_cloud_cli-1.3.3/dagster_cloud_cli_tests/test_state.py` & `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,101 +23,143 @@
           module_name: c
       image: docker/c
       working_directory: c
 """
 
 
 @contextmanager
-def with_dagtser_yaml(text):
+def with_dagster_yaml(text):
     pwd = os.curdir
     try:
         with tempfile.TemporaryDirectory() as tmpdir:
             os.mkdir(os.path.join(tmpdir, "subdir"))
             yaml_path = os.path.join(tmpdir, "dagster_cloud.yaml")
             with open(yaml_path, "w") as f:
                 f.write(text)
             os.chdir(tmpdir)
             yield tmpdir
     finally:
         os.chdir(pwd)
 
 
-def test_ci_init(monkeypatch) -> None:
-    monkeypatch.setenv("DAGSTER_CLOUD_URL", "http://some-url")
+def test_ci_init(monkeypatch, mocker, empty_config) -> None:
+    monkeypatch.setenv("DAGSTER_CLOUD_ORGANIZATION", "some-org")
+    monkeypatch.setenv("DAGSTER_CLOUD_API_TOKEN", "some-org:fake-token")
 
     with tempfile.TemporaryDirectory() as statedir:
-        with with_dagtser_yaml(DAGSTER_CLOUD_YAML) as project_dir:
+        with with_dagster_yaml(DAGSTER_CLOUD_YAML) as project_dir:
             runner = CliRunner()
             result = runner.invoke(app, ["ci", "init", f"--project-dir={project_dir}"])
             # statedir not specified
             assert result.exit_code
             monkeypatch.setenv("DAGSTER_BUILD_STATEDIR", statedir)
             result = runner.invoke(app, ["ci", "init", f"--project-dir={project_dir}"])
-            assert result.exit_code
+            assert result.exit_code, result.output
             assert "deployment" in result.output
 
             result = runner.invoke(
-                app, ["ci", "init", f"--project-dir={project_dir}", "--deployment=prod"]
+                app,
+                [
+                    "ci",
+                    "init",
+                    f"--project-dir={project_dir}",
+                    "--deployment=prod",
+                    "--commit-hash=hash-1234",
+                    "--git-url=http://some-git-url",
+                ],
             )
             assert not result.exit_code
 
             # 'status' should return a list of code locations
             result = runner.invoke(app, ["ci", "status"])
             assert not result.exit_code
             locations = [json.loads(line) for line in result.output.splitlines()]
             assert ["a", "b", "c"] == [loc["location_name"] for loc in locations]
             location_a = locations[0]
             assert location_a == {
-                "build": None,
+                "build": {
+                    "build_config": None,
+                    "commit_hash": "hash-1234",
+                    "git_url": "http://some-git-url",
+                },
                 "build_output": None,
                 "location_name": "a",
                 "deployment_name": "prod",
                 "location_file": f"{project_dir}/dagster_cloud.yaml",
                 "selected": True,
-                "url": "http://some-url",
+                "url": "https://some-org.dagster.cloud",
             }
 
-        with with_dagtser_yaml(DAGSTER_CLOUD_YAML) as project_dir:
+        with with_dagster_yaml(DAGSTER_CLOUD_YAML) as project_dir:
             runner = CliRunner()
             monkeypatch.setenv("DAGSTER_BUILD_STATEDIR", statedir)
             result = runner.invoke(
                 app,
                 [
                     "ci",
                     "init",
                     f"--project-dir={project_dir}",
                     "--location-name=a",
                     "--location-name=c",
-                    "--deployment=prod",
+                    "--deployment=prod-1",
                 ],
             )
             assert not result.exit_code, result.output
             result = runner.invoke(app, ["ci", "status"])
+            print(result.output)
             locations = [json.loads(line) for line in result.output.splitlines()]
             assert ["a", "c"] == [loc["location_name"] for loc in locations]
+            assert ["prod-1", "prod-1"] == [loc["deployment_name"] for loc in locations]
+
+            # ensure branch deployment is used if available
+            mocker.patch(
+                "dagster_cloud_cli.commands.ci.get_deployment_from_context",
+                return_value="branch-deployment",
+            )
+            result = runner.invoke(
+                app,
+                [
+                    "ci",
+                    "init",
+                    f"--project-dir={project_dir}",
+                    "--location-name=a",
+                    "--deployment=prod-2",
+                ],
+            )
+            assert not result.exit_code, result.output
+            result = runner.invoke(app, ["ci", "status"])
+            locations = [json.loads(line) for line in result.output.splitlines()]
+            assert ["branch-deployment"] == [loc["deployment_name"] for loc in locations]
 
 
 @pytest.fixture(params=["prod", "branch-deployment-1234"])
 def deployment_name(request):
     return request.param
 
 
 @pytest.fixture
 def initialized_runner(deployment_name, monkeypatch):
-    monkeypatch.setenv("DAGSTER_CLOUD_URL", "http://some-url")
+    monkeypatch.setenv("DAGSTER_CLOUD_ORGANIZATION", "some-org")
+    monkeypatch.setenv("DAGSTER_CLOUD_API_TOKEN", "some-org:some-token")
     with tempfile.TemporaryDirectory():
-        with with_dagtser_yaml(DAGSTER_CLOUD_YAML) as project_dir:
+        with with_dagster_yaml(DAGSTER_CLOUD_YAML) as project_dir:
             statedir = os.path.join(project_dir, "tmp")
             monkeypatch.setenv("DAGSTER_BUILD_STATEDIR", statedir)
 
             runner = CliRunner()
 
             result = runner.invoke(
                 app,
-                ["ci", "init", f"--project-dir={project_dir}", f"--deployment={deployment_name}"],
+                [
+                    "ci",
+                    "init",
+                    f"--project-dir={project_dir}",
+                    f"--deployment={deployment_name}",
+                    "--commit-hash=hash-4354",
+                ],
             )
             assert not result.exit_code, result.output
             yield runner
 
 
 def get_locations(runner):
     result = runner.invoke(app, ["ci", "status"])
@@ -179,15 +221,22 @@
     assert c_tag.startswith(f"{deployment_name}-c")
     assert c_build_dir == "subdir"
 
     # test overriding some defaults
     build_image.reset_mock()
     upload_image.reset_mock()
     result = initialized_runner.invoke(
-        app, ["ci", "build", "--base-image=custom-base-image", "--env=A=1", "--env=B=2"]
+        app,
+        [
+            "ci",
+            "build",
+            "--docker-base-image=custom-base-image",
+            "--docker-env=A=1",
+            "--docker-env=B=2",
+        ],
     )
     assert not result.exit_code, result.output
 
     (b_build_dir, b_tag, b_registry_info), b_kwargs = build_image.call_args_list[0]
     assert b_build_dir == "."
     assert b_registry_info["registry_url"] == "example.com/image-registry"
     assert b_kwargs["base_image"] == "custom-base-image"
@@ -204,15 +253,15 @@
     )
     mocker.patch("dagster_cloud_cli.docker_utils.build_image", return_value=0)
     mocker.patch("dagster_cloud_cli.docker_utils.upload_image", return_value=0)
     update_code_location = mocker.patch("dagster_cloud_cli.gql.add_or_update_code_location")
     wait_for_load = mocker.patch("dagster_cloud_cli.commands.ci.wait_for_load")
 
     initialized_runner.invoke(app, ["ci", "locations-deselect", "a"])
-    result = initialized_runner.invoke(app, ["ci", "build", "--commit-hash=hash-4354"])
+    result = initialized_runner.invoke(app, ["ci", "build"])
     assert not result.exit_code, result.output
     print(result.output)
     result = initialized_runner.invoke(app, ["ci", "deploy"])
     assert not result.exit_code, result.output
     print(result.output)
 
     assert len(update_code_location.call_args_list) == 2
@@ -222,38 +271,132 @@
     (_, c_update_args), _ = update_code_location.call_args_list[1]
     assert b_update_args == {
         "code_source": {"module_name": "b"},
         "git": {"commit_hash": "hash-4354"},
         "image": f"example.com/image-registry:{deployment_name}-b-hash-4354",
         "location_name": "b",
     }
-    assert gql_shim.url == f"http://some-url/{deployment_name}/graphql"
+    assert gql_shim.url == f"https://some-org.dagster.cloud/{deployment_name}/graphql"
     assert c_update_args == {
         "code_source": {"module_name": "c"},
         "git": {"commit_hash": "hash-4354"},
         "image": f"example.com/image-registry:{deployment_name}-c-hash-4354",
         "location_name": "c",
         "working_directory": "c",
     }
     (_, wait_location_args), wait_kwargs = wait_for_load.call_args_list[0]
     assert wait_location_args == ["b", "c"]
-    assert wait_kwargs["url"] == f"http://some-url/{deployment_name}"
+    assert wait_kwargs["url"] == f"https://some-org.dagster.cloud/{deployment_name}"
 
 
 def test_ci_set_build_output(initialized_runner: CliRunner):
     result = initialized_runner.invoke(app, ["ci", "set-build-output", "--image-tag=1234"])
     assert result.exit_code
     assert "Error: No build:registry:" in result.output
 
     initialized_runner.invoke(app, ["ci", "locations-deselect", "a", "b"])
-    result = initialized_runner.invoke(
-        app, ["ci", "set-build-output", "--image-tag=1234", "--commit-hash=abcd"]
-    )
+    result = initialized_runner.invoke(app, ["ci", "set-build-output", "--image-tag=1234"])
     assert not result.exit_code, result.output
     print(result.output)
     c_location = [
         location
         for location in get_locations(initialized_runner)
         if location["location_name"] == "c"
     ][0]
     assert c_location["build_output"]["image"] == "example.com/some-image-name:1234"
-    assert c_location["build_output"]["commit_hash"] == "abcd"
+
+
+def test_ci_deploy_pex(
+    mocker, monkeypatch, deployment_name: str, initialized_runner: CliRunner
+) -> None:
+    monkeypatch.setenv("DAGSTER_CLOUD_API_TOKEN", "fake-token")
+    build_upload_pex = mocker.patch(
+        "dagster_cloud_cli.pex_utils.build_upload_pex",
+        return_value={"image": "pex-base-image", "pex_tag": "deps-123.pex:source-456.pex"},
+    )
+    update_code_location = mocker.patch("dagster_cloud_cli.gql.add_or_update_code_location")
+    wait_for_load = mocker.patch("dagster_cloud_cli.commands.ci.wait_for_load")
+
+    initialized_runner.invoke(app, ["ci", "locations-deselect", "a"])
+    result = initialized_runner.invoke(
+        app,
+        [
+            "ci",
+            "build",
+            "--build-strategy=python-executable",
+            "--pex-deps-cache-from=from-cache",
+            "--pex-deps-cache-to=to-cache",
+        ],
+    )
+    assert not result.exit_code, result.output
+    print(result.output)
+    _, b_build_upload_pex_kwargs = build_upload_pex.call_args_list[0]
+    assert b_build_upload_pex_kwargs["kwargs"]["deps_cache_from"] == "from-cache"
+    assert b_build_upload_pex_kwargs["kwargs"]["deps_cache_to"] == "to-cache"
+
+    result = initialized_runner.invoke(app, ["ci", "deploy"])
+    assert not result.exit_code, result.output
+    print(result.output)
+
+    assert len(update_code_location.call_args_list) == 2
+    assert len(wait_for_load.call_args_list) == 1
+
+    (gql_shim, b_update_args), _ = update_code_location.call_args_list[0]
+    (_, c_update_args), _ = update_code_location.call_args_list[1]
+    assert b_update_args == {
+        "location_name": "b",
+        "code_source": {"module_name": "b"},
+        "git": {"commit_hash": "hash-4354"},
+        "image": "pex-base-image",
+        "pex_metadata": {"pex_tag": "deps-123.pex:source-456.pex"},
+    }
+    assert gql_shim.url == f"https://some-org.dagster.cloud/{deployment_name}/graphql"
+    assert c_update_args == {
+        "location_name": "c",
+        "code_source": {"module_name": "c"},
+        "git": {"commit_hash": "hash-4354"},
+        "image": "pex-base-image",
+        "pex_metadata": {"pex_tag": "deps-123.pex:source-456.pex"},
+        "working_directory": "c",
+    }
+    (_, wait_location_args), wait_kwargs = wait_for_load.call_args_list[0]
+    assert wait_location_args == ["b", "c"]
+    assert wait_kwargs["url"] == f"https://some-org.dagster.cloud/{deployment_name}"
+
+
+def test_ci_branch_deployment(
+    mocker,
+    monkeypatch,
+    empty_config,
+) -> None:
+    monkeypatch.setenv("DAGSTER_CLOUD_API_TOKEN", "fake-token")
+    mocker.patch(
+        "dagster_cloud_cli.commands.ci.get_deployment_from_context", return_value="branch-dep-name"
+    )
+    with with_dagster_yaml(DAGSTER_CLOUD_YAML) as project_dir:
+        runner = CliRunner()
+        result = runner.invoke(
+            app,
+            [
+                "ci",
+                "branch-deployment",
+                project_dir,
+            ],
+        )
+        assert result.exit_code
+
+        monkeypatch.setenv("DAGSTER_CLOUD_ORGANIZATION", "someorg")
+        result = runner.invoke(
+            app,
+            [
+                "ci",
+                "branch-deployment",
+                project_dir,
+            ],
+        )
+        assert not result.exit_code
+        assert result.output.strip() == "branch-dep-name"
+
+        monkeypatch.delenv("DAGSTER_CLOUD_ORGANIZATION")
+        monkeypatch.setenv("DAGSTER_CLOUD_URL", "https://someurl")
+        assert not result.exit_code
+        assert result.output.strip() == "branch-dep-name"
```

### Comparing `dagster_cloud_cli-1.3.3/setup.py` & `dagster_cloud_cli-1.3.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/runpod-0.9.4.tar.gz` & `tmp/runpod-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpod-0.9.4.tar", last modified: Thu May 11 01:33:20 2023, max compression
+gzip compressed data, was "runpod-0.9.5.tar", last modified: Thu May 11 05:09:23 2023, max compression
```

## Comparing `runpod-0.9.4.tar` & `runpod-0.9.5.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/CD_publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/CI_codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/CI_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/ci_pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-11 01:33:05.000000 runpod-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 01:33:05.000000 runpod-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 01:33:20.328328 runpod-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-11 01:33:05.000000 runpod-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.308328 runpod-0.9.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/api/quries.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/images/env_var_location.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/docs/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/local_testing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/docs/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_cleanup.md
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_download.md
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_upload.md
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/worker.md
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/worker_realtime.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-11 01:33:05.000000 runpod-0.9.4/examples/call_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-11 01:33:05.000000 runpod-0.9.4/examples/call_endpoint_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-11 01:33:05.000000 runpod-0.9.4/examples/graphql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-11 01:33:05.000000 runpod-0.9.4/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 01:33:05.000000 runpod-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 01:33:05.000000 runpod-0.9.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod/api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/ctl_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod/api_wrapper/mutations/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/mutations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/api_wrapper/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/queries/gpus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/endpoint/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/asyncio/asyncio_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/serverless/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/rp_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/rp_tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/worker_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/runpod/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/work_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 01:33:20.328328 runpod-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 01:33:05.000000 runpod-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/tests/test_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_endpoint/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/tests/test_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/test_module_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/test_pod_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/test_util_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_whatever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/whatever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.240259 runpod-0.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 05:09:04.000000 runpod-0.9.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 05:09:04.000000 runpod-0.9.5/.github/workflows/CD_publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 05:09:04.000000 runpod-0.9.5/.github/workflows/CI_codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-11 05:09:04.000000 runpod-0.9.5/.github/workflows/CI_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-11 05:09:04.000000 runpod-0.9.5/.github/workflows/ci_pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-11 05:09:04.000000 runpod-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 05:09:04.000000 runpod-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 05:09:23.240259 runpod-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-11 05:09:04.000000 runpod-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.228258 runpod-0.9.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/api/quries.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/images/env_var_location.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/docs/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/local_testing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/docs/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/utils/rp_cleanup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/utils/rp_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/utils/rp_upload.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/utils/rp_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/worker.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 05:09:04.000000 runpod-0.9.5/docs/serverless/worker_realtime.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-11 05:09:04.000000 runpod-0.9.5/examples/call_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-11 05:09:04.000000 runpod-0.9.5/examples/call_endpoint_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-11 05:09:04.000000 runpod-0.9.5/examples/graphql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-11 05:09:04.000000 runpod-0.9.5/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 05:09:04.000000 runpod-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 05:09:04.000000 runpod-0.9.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/runpod/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/runpod/api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/api_wrapper/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/mutations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/api_wrapper/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/api_wrapper/queries/gpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/endpoint/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/endpoint/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/endpoint/asyncio/asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/endpoint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/serverless/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/rp_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/rp_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/modules/worker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/runpod/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/utils/rp_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/utils/rp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/utils/rp_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/utils/rp_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 05:09:04.000000 runpod-0.9.5/runpod/serverless/work_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.232259 runpod-0.9.5/runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 05:09:23.000000 runpod-0.9.5/runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-11 05:09:23.000000 runpod-0.9.5/runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:09:23.000000 runpod-0.9.5/runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 05:09:23.000000 runpod-0.9.5/runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 05:09:23.000000 runpod-0.9.5/runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 05:09:23.240259 runpod-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 05:09:04.000000 runpod-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.236259 runpod-0.9.5/tests/test_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_endpoint/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:09:23.240259 runpod-0.9.5/tests/test_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_serverless/test_module_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_serverless/test_pod_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_serverless/test_util_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/test_whatever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-11 05:09:04.000000 runpod-0.9.5/tests/whatever.py
```

### Comparing `runpod-0.9.4/.github/workflows/CD_publish-to-pypi.yml` & `runpod-0.9.5/.github/workflows/CD_publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/.github/workflows/CI_codeql.yml` & `runpod-0.9.5/.github/workflows/CI_codeql.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/.github/workflows/CI_tests.yml` & `runpod-0.9.5/.github/workflows/CI_tests.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/.github/workflows/ci_pylint.yml` & `runpod-0.9.5/.github/workflows/ci_pylint.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/.gitignore` & `runpod-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/LICENSE` & `runpod-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/PKG-INFO` & `runpod-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.4
+Version: 0.9.5
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
```

### Comparing `runpod-0.9.4/README.md` & `runpod-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/api/quries.md` & `runpod-0.9.5/docs/api/quries.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/images/env_var_location.png` & `runpod-0.9.5/docs/images/env_var_location.png`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/serverless/local_testing.md` & `runpod-0.9.5/docs/serverless/local_testing.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/serverless/utils/rp_download.md` & `runpod-0.9.5/docs/serverless/utils/rp_download.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/serverless/utils/rp_upload.md` & `runpod-0.9.5/docs/serverless/utils/rp_upload.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/serverless/utils/rp_validator.md` & `runpod-0.9.5/docs/serverless/utils/rp_validator.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/serverless/worker.md` & `runpod-0.9.5/docs/serverless/worker.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/docs/serverless/worker_realtime.md` & `runpod-0.9.5/docs/serverless/worker_realtime.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/examples/call_endpoint_asyncio.py` & `runpod-0.9.5/examples/call_endpoint_asyncio.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/examples/graphql_wrapper.py` & `runpod-0.9.5/examples/graphql_wrapper.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/infer.py` & `runpod-0.9.5/infer.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/api_wrapper/ctl_commands.py` & `runpod-0.9.5/runpod/api_wrapper/ctl_commands.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/api_wrapper/graphql.py` & `runpod-0.9.5/runpod/api_wrapper/graphql.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/api_wrapper/mutations/pods.py` & `runpod-0.9.5/runpod/api_wrapper/mutations/pods.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/api_wrapper/queries/gpus.py` & `runpod-0.9.5/runpod/api_wrapper/queries/gpus.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/endpoint/asyncio/asyncio_runner.py` & `runpod-0.9.5/runpod/endpoint/asyncio/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/endpoint/runner.py` & `runpod-0.9.5/runpod/endpoint/runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/__init__.py` & `runpod-0.9.5/runpod/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/heartbeat.py` & `runpod-0.9.5/runpod/serverless/modules/heartbeat.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/job.py` & `runpod-0.9.5/runpod/serverless/modules/job.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/logging.py` & `runpod-0.9.5/runpod/serverless/modules/logging.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/retry.py` & `runpod-0.9.5/runpod/serverless/modules/retry.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/rp_fastapi.py` & `runpod-0.9.5/runpod/serverless/modules/rp_fastapi.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/rp_tips.py` & `runpod-0.9.5/runpod/serverless/modules/rp_tips.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/modules/worker_state.py` & `runpod-0.9.5/runpod/serverless/modules/worker_state.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/utils/rp_cleanup.py` & `runpod-0.9.5/runpod/serverless/utils/rp_cleanup.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/utils/rp_download.py` & `runpod-0.9.5/runpod/serverless/utils/rp_download.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/utils/rp_upload.py` & `runpod-0.9.5/runpod/serverless/utils/rp_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod/serverless/utils/rp_validator.py` & `runpod-0.9.5/runpod/serverless/utils/rp_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     for key, rules in schema.items():
         # Enforce floats to be floats.
         if rules['type'] is float and type(raw_input[key]) in [int, float]:
             validated_input[key] = float(raw_input[key])
 
         # Check for the correct type.
-        if not isinstance(raw_input[key], rules['type']) and raw_input[key] is not None:
+        if not isinstance(validated_input[key], rules['type']) and raw_input.get(key, False):
             _add_error(
                 error_list, f"{key} should be {rules['type']} type, not {type(raw_input[key])}.")
 
         # Check lambda constraints.
         if "constraints" in rules:
             if not rules['constraints'](raw_input[key]):
                 _add_error(error_list, CONSTRAINTS_ERROR.format(key))
```

### Comparing `runpod-0.9.4/runpod/serverless/work_loop.py` & `runpod-0.9.5/runpod/serverless/work_loop.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/runpod.egg-info/PKG-INFO` & `runpod-0.9.5/runpod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.4
+Version: 0.9.5
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
```

### Comparing `runpod-0.9.4/runpod.egg-info/SOURCES.txt` & `runpod-0.9.5/runpod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/setup.cfg` & `runpod-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/tests/test_endpoint/test_runner.py` & `runpod-0.9.5/tests/test_endpoint/test_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/tests/test_serverless/test_module_download.py` & `runpod-0.9.5/tests/test_serverless/test_module_download.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/tests/test_serverless/test_pod_worker.py` & `runpod-0.9.5/tests/test_serverless/test_pod_worker.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/tests/test_serverless/test_util_upload.py` & `runpod-0.9.5/tests/test_serverless/test_util_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/tests/test_whatever.py` & `runpod-0.9.5/tests/test_whatever.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.4/tests/whatever.py` & `runpod-0.9.5/tests/whatever.py`

 * *Files identical despite different names*


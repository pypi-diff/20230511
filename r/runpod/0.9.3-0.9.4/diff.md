# Comparing `tmp/runpod-0.9.3.tar.gz` & `tmp/runpod-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpod-0.9.3.tar", last modified: Thu Apr 20 18:46:34 2023, max compression
+gzip compressed data, was "runpod-0.9.4.tar", last modified: Thu May 11 01:33:20 2023, max compression
```

## Comparing `runpod-0.9.3.tar` & `runpod-0.9.4.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/CD_publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/CI_codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/CI_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-20 18:46:19.000000 runpod-0.9.3/.github/workflows/ci_pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-20 18:46:19.000000 runpod-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-20 18:46:19.000000 runpod-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-20 18:46:34.162383 runpod-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-20 18:46:19.000000 runpod-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.146382 runpod-0.9.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/api/quries.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.150383 runpod-0.9.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/images/env_var_location.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/docs/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/local_testing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/docs/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_cleanup.md
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_download.md
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_upload.md
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/utils/rp_validator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-20 18:46:19.000000 runpod-0.9.3/docs/serverless/worker.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-20 18:46:19.000000 runpod-0.9.3/examples/call_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-20 18:46:19.000000 runpod-0.9.3/examples/call_endpoint_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 18:46:19.000000 runpod-0.9.3/examples/graphql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-20 18:46:19.000000 runpod-0.9.3/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 18:46:19.000000 runpod-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-20 18:46:19.000000 runpod-0.9.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod/api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/ctl_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod/api_wrapper/mutations/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/mutations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/api_wrapper/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/api_wrapper/queries/gpus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/endpoint/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/asyncio/asyncio_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/endpoint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/serverless/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/rp_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/rp_tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/modules/worker_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.158383 runpod-0.9.3/runpod/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/utils/rp_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 18:46:19.000000 runpod-0.9.3/runpod/serverless/work_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.154383 runpod-0.9.3/runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 18:46:34.000000 runpod-0.9.3/runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-20 18:46:34.162383 runpod-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 18:46:19.000000 runpod-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/tests/test_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_endpoint/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:46:34.162383 runpod-0.9.3/tests/test_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/test_module_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/test_pod_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_serverless/test_util_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/test_whatever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-20 18:46:19.000000 runpod-0.9.3/tests/whatever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/CD_publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/CI_codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/CI_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-11 01:33:05.000000 runpod-0.9.4/.github/workflows/ci_pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-11 01:33:05.000000 runpod-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 01:33:05.000000 runpod-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 01:33:20.328328 runpod-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-11 01:33:05.000000 runpod-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.308328 runpod-0.9.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/api/quries.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.312328 runpod-0.9.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/images/env_var_location.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/docs/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/local_testing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/docs/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_cleanup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_upload.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/utils/rp_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/worker.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 01:33:05.000000 runpod-0.9.4/docs/serverless/worker_realtime.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-11 01:33:05.000000 runpod-0.9.4/examples/call_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-11 01:33:05.000000 runpod-0.9.4/examples/call_endpoint_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-11 01:33:05.000000 runpod-0.9.4/examples/graphql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-11 01:33:05.000000 runpod-0.9.4/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 01:33:05.000000 runpod-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 01:33:05.000000 runpod-0.9.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod/api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/ctl_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod/api_wrapper/mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/mutations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/api_wrapper/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/api_wrapper/queries/gpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/endpoint/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/asyncio/asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/endpoint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.324328 runpod-0.9.4/runpod/serverless/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/rp_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/rp_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/modules/worker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/runpod/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/utils/rp_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 01:33:05.000000 runpod-0.9.4/runpod/serverless/work_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.316328 runpod-0.9.4/runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 01:33:20.000000 runpod-0.9.4/runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 01:33:20.328328 runpod-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 01:33:05.000000 runpod-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/tests/test_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_endpoint/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:33:20.328328 runpod-0.9.4/tests/test_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/test_module_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/test_pod_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_serverless/test_util_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/test_whatever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-11 01:33:05.000000 runpod-0.9.4/tests/whatever.py
```

### Comparing `runpod-0.9.3/.github/workflows/CD_publish-to-pypi.yml` & `runpod-0.9.4/.github/workflows/CD_publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/.github/workflows/CI_codeql.yml` & `runpod-0.9.4/.github/workflows/CI_codeql.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/.github/workflows/CI_tests.yml` & `runpod-0.9.4/.github/workflows/CI_tests.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/.github/workflows/ci_pylint.yml` & `runpod-0.9.4/.github/workflows/ci_pylint.yml`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/.gitignore` & `runpod-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/LICENSE` & `runpod-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/PKG-INFO` & `runpod-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.3
+Version: 0.9.4
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
```

### Comparing `runpod-0.9.3/README.md` & `runpod-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/docs/api/quries.md` & `runpod-0.9.4/docs/api/quries.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/docs/images/env_var_location.png` & `runpod-0.9.4/docs/images/env_var_location.png`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/docs/serverless/utils/rp_download.md` & `runpod-0.9.4/docs/serverless/utils/rp_download.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/docs/serverless/utils/rp_upload.md` & `runpod-0.9.4/docs/serverless/utils/rp_upload.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/docs/serverless/utils/rp_validator.md` & `runpod-0.9.4/docs/serverless/utils/rp_validator.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/docs/serverless/worker.md` & `runpod-0.9.4/docs/serverless/worker.md`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/examples/call_endpoint_asyncio.py` & `runpod-0.9.4/examples/call_endpoint_asyncio.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/examples/graphql_wrapper.py` & `runpod-0.9.4/examples/graphql_wrapper.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/infer.py` & `runpod-0.9.4/infer.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/api_wrapper/ctl_commands.py` & `runpod-0.9.4/runpod/api_wrapper/ctl_commands.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/api_wrapper/graphql.py` & `runpod-0.9.4/runpod/api_wrapper/graphql.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/api_wrapper/mutations/pods.py` & `runpod-0.9.4/runpod/api_wrapper/mutations/pods.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/api_wrapper/queries/gpus.py` & `runpod-0.9.4/runpod/api_wrapper/queries/gpus.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/endpoint/asyncio/asyncio_runner.py` & `runpod-0.9.4/runpod/endpoint/asyncio/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/endpoint/runner.py` & `runpod-0.9.4/runpod/endpoint/runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/modules/heartbeat.py` & `runpod-0.9.4/runpod/serverless/modules/heartbeat.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/modules/job.py` & `runpod-0.9.4/runpod/serverless/modules/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,22 +29,26 @@
     if "id" not in test_inputs:
         test_inputs["id"] = "local_test"
 
     log.debug(f"Retrieved local job: {test_inputs}")
     return test_inputs
 
 
-async def get_job(session):
+async def get_job(session, config):
     """
     Get the job from the queue.
     """
     next_job = None
 
     try:
-        if _IS_LOCAL_TEST:
+        if config.get("test_input", None) is not None:
+            log.warn("test_input set, using test_input as job input")
+            next_job = config["test_input"]
+            next_job["id"] = "test_input_provided"
+        elif _IS_LOCAL_TEST:
             log.warn("RUNPOD_WEBHOOK_GET_JOB not set, switching to get_local")
             next_job = _get_local()
         else:
             async with session.get(JOB_GET_URL) as response:
                 next_job = await response.json()
                 log.debug(f"Retrieved remote job: {next_job}")
```

### Comparing `runpod-0.9.3/runpod/serverless/modules/logging.py` & `runpod-0.9.4/runpod/serverless/modules/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 load_dotenv(env_path)  # Load environment variables
 
 
 def log(message, level='INFO'):
     '''
     Log message to stdout if RUNPOD_DEBUG is true.
     '''
-    set_level = os.environ.get('RUNPOD_DEBUG_LEVEL', 'DEBUG').upper()
+    set_level = os.environ.get('RUNPOD_DEBUG_LEVEL', 'INFO').upper()
     level = level.ljust(7)
 
     if os.environ.get('RUNPOD_DEBUG', 'true').lower() != 'true':
         return
 
     if set_level == 'ERROR' and level != 'ERROR':
         return
```

### Comparing `runpod-0.9.3/runpod/serverless/modules/retry.py` & `runpod-0.9.4/runpod/serverless/modules/retry.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/modules/rp_fastapi.py` & `runpod-0.9.4/runpod/serverless/modules/rp_fastapi.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/modules/rp_tips.py` & `runpod-0.9.4/runpod/serverless/modules/rp_tips.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/modules/worker_state.py` & `runpod-0.9.4/runpod/serverless/modules/worker_state.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/utils/rp_cleanup.py` & `runpod-0.9.4/runpod/serverless/utils/rp_cleanup.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/utils/rp_download.py` & `runpod-0.9.4/runpod/serverless/utils/rp_download.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/utils/rp_upload.py` & `runpod-0.9.4/runpod/serverless/utils/rp_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/runpod/serverless/work_loop.py` & `runpod-0.9.4/runpod/serverless/work_loop.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 runpod | serverless | worker_loop.py
 Called to convert a container into a worker pod for the runpod serverless platform.
 """
 
 import os
+import sys
 
 import aiohttp
 
 import runpod.serverless.modules.logging as log
 from .modules.heartbeat import start_ping
 from .modules.job import get_job, run_job, send_result
 from .modules.worker_state import set_job_id
@@ -30,15 +31,15 @@
     auth_header = _get_auth_header()
 
     async with aiohttp.ClientSession(headers=auth_header, timeout=_TIMEOUT) as session:
 
         start_ping()
 
         while True:
-            job = await get_job(session)
+            job = await get_job(session, config)
 
             if job is None:
                 log.info("No job available, waiting for the next one.")
                 continue
 
             if job["input"] is None:
                 log.error(f"Job {job['id']} has no input parameter provided. Skipping this job.")
@@ -55,9 +56,13 @@
                 job_result["stopPod"] = True
 
             await send_result(session, job_result, job)
 
             set_job_id(None)
 
             if _is_local_testing():
-                log.info("Local testing complete, exiting.")
-                break
+                if "error" in job_result:
+                    log.error(f"Job {job['id']} failed with error: {job_result['error']}")
+                    sys.exit(1)
+                else:
+                    log.info("Local testing complete, exiting.")
+                    sys.exit(0)
```

### Comparing `runpod-0.9.3/runpod.egg-info/PKG-INFO` & `runpod-0.9.4/runpod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.3
+Version: 0.9.4
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
```

### Comparing `runpod-0.9.3/runpod.egg-info/SOURCES.txt` & `runpod-0.9.4/runpod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .github/workflows/CI_codeql.yml
 .github/workflows/CI_tests.yml
 .github/workflows/ci_pylint.yml
 docs/api/quries.md
 docs/images/env_var_location.png
 docs/serverless/local_testing.md
 docs/serverless/worker.md
+docs/serverless/worker_realtime.md
 docs/serverless/utils/rp_cleanup.md
 docs/serverless/utils/rp_download.md
 docs/serverless/utils/rp_upload.md
 docs/serverless/utils/rp_validator.md
 examples/call_endpoint.py
 examples/call_endpoint_asyncio.py
 examples/graphql_wrapper.py
```

### Comparing `runpod-0.9.3/setup.cfg` & `runpod-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/tests/test_endpoint/test_runner.py` & `runpod-0.9.4/tests/test_endpoint/test_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/tests/test_serverless/test_module_download.py` & `runpod-0.9.4/tests/test_serverless/test_module_download.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/tests/test_serverless/test_pod_worker.py` & `runpod-0.9.4/tests/test_serverless/test_pod_worker.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/tests/test_serverless/test_util_upload.py` & `runpod-0.9.4/tests/test_serverless/test_util_upload.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/tests/test_whatever.py` & `runpod-0.9.4/tests/test_whatever.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.3/tests/whatever.py` & `runpod-0.9.4/tests/whatever.py`

 * *Files identical despite different names*


# Comparing `tmp/clustaar.webhook-0.1.6.tar.gz` & `tmp/clustaar.webhook-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clustaar.webhook-0.1.6.tar", last modified: Tue May 26 02:36:38 2020, max compression
+gzip compressed data, was "clustaar.webhook-0.1.7.tar", last modified: Thu May 11 15:03:48 2023, max compression
```

## Comparing `clustaar.webhook-0.1.6.tar` & `clustaar.webhook-0.1.7.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      547 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/.coveragerc
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      431 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/.gitignore
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      124 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/.pre-commit-config.yaml
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       76 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/AUTHORS.rst
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       30 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/CHANGELOG.rst
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1075 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/LICENSE.txt
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     4588 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/PKG-INFO
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     3231 2020-05-26 02:33:50.000000 clustaar.webhook-0.1.6/README.md
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/docs/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     7608 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/Makefile
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/docs/_static/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       18 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/_static/.gitignore
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       41 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/authors.rst
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       43 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/changelog.rst
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     9132 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/conf.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     2036 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/index.rst
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       74 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/docs/license.rst
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/example/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      864 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/example/client.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       34 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/example/requirements.txt
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      387 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/example/webhook.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      501 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/goal.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       91 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/pyproject.toml
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1549 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/setup.cfg
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      594 2020-05-26 02:32:29.000000 clustaar.webhook-0.1.6/setup.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:37.000000 clustaar.webhook-0.1.6/src/
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/src/clustaar/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       80 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/__init__.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      389 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/__init__.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       21 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/constants.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       56 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/events.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1030 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/events_handler.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/falcon/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       78 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/falcon/__init__.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      649 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/falcon/http_request.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      595 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/falcon/http_response.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     3299 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/filters.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      146 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/__init__.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1355 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/authenticators.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1737 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/basic_authentication_middleware.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1004 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/replay_prevention_middleware.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     2522 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/validate_signature_middleware.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      684 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/monkey_patch.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/routing/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       52 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/routing/__init__.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1431 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/routing/route.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1101 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/routing/router.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     2439 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/src/clustaar/webhook/webhook.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     4588 2020-05-26 02:36:37.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/PKG-INFO
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     2173 2020-05-26 02:36:37.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/SOURCES.txt
--rw-rw-r--   0 depopper  (1000) depopper  (1000)        1 2020-05-26 02:36:37.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/dependency_links.txt
--rw-rw-r--   0 depopper  (1000) depopper  (1000)        1 2020-05-25 12:10:52.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/not-zip-safe
--rw-rw-r--   0 depopper  (1000) depopper  (1000)       90 2020-05-26 02:36:37.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/requires.txt
--rw-rw-r--   0 depopper  (1000) depopper  (1000)        9 2020-05-26 02:36:37.000000 clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/top_level.txt
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      106 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/test-requirements.txt
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      451 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/conftest.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/resources/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      636 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/resources/webhook_request.json
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/utils/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      641 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/utils/__init__.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      686 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/utils/factory.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/webhook/
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/webhook/falcon/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      426 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/falcon/test_http_request.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      439 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/falcon/test_http_response.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/webhook/filters/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      750 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/filters/test_json_key_equals.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      558 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/filters/test_json_key_exists.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      747 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/filters/test_json_key_in.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      536 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/filters/test_step_id.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/webhook/middlewares/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     2086 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/middlewares/test_basic_authentication_middleware.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1003 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/middlewares/test_replay_prevention_middleware.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      741 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/middlewares/test_static_authenticator.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     2775 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/middlewares/test_validate_signature_middleware.py
-drwxrwxr-x   0 depopper  (1000) depopper  (1000)        0 2020-05-26 02:36:38.000000 clustaar.webhook-0.1.6/tests/webhook/routing/
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1652 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/routing/test_route.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     1158 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/routing/test_router.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      766 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/test_events_handler.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)     3309 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tests/webhook/test_webhook.py
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      136 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/tox.ini
--rw-rw-r--   0 depopper  (1000) depopper  (1000)      622 2020-05-25 10:12:19.000000 clustaar.webhook-0.1.6/wercker.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.540554 clustaar.webhook-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/.github/workflows/build_package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/.github/workflows/launch_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/example/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/example/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-11 15:03:48.552554 clustaar.webhook-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.540554 clustaar.webhook-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/src/clustaar/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/src/clustaar/webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/events_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/src/clustaar/webhook/falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/falcon/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/falcon/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/basic_authentication_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/replay_prevention_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/validate_signature_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/monkey_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/src/clustaar/webhook/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/routing/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/routing/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/src/clustaar/webhook/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.544554 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-11 15:03:48.000000 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-11 15:03:48.000000 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:03:48.000000 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:03:48.000000 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 15:03:48.000000 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:03:48.000000 clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/resources/webhook_request.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/utils/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/webhook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/webhook/falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/falcon/test_http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/falcon/test_http_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/webhook/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/filters/test_json_key_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/filters/test_json_key_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/filters/test_json_key_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/filters/test_step_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/webhook/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/middlewares/test_basic_authentication_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/middlewares/test_replay_prevention_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/middlewares/test_static_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/middlewares/test_validate_signature_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:03:48.548554 clustaar.webhook-0.1.7/tests/webhook/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/routing/test_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/routing/test_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/test_events_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tests/webhook/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-11 15:03:35.000000 clustaar.webhook-0.1.7/wercker.yml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clustaar.webhook-0.1.6/.coveragerc` & `clustaar.webhook-0.1.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/LICENSE.txt` & `clustaar.webhook-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/README.md` & `clustaar.webhook-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/docs/Makefile` & `clustaar.webhook-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/docs/conf.py` & `clustaar.webhook-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/docs/index.rst` & `clustaar.webhook-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/example/client.py` & `clustaar.webhook-0.1.7/example/client.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/setup.cfg` & `clustaar.webhook-0.1.7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = clustaar.webhook
 description = Clustaar webhook framework
 author = Aurélien
-author-email = aurelien@clustaar.com
+author-email = axel.schafers@clustaar.com
 license = mit
 url = https://github.com/Clustaar/clustaar.webhook
 long-description = file: README.md
 long_description_content_type = text/markdown
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
@@ -15,18 +15,18 @@
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
-	falcon~=1.4.1
+	falcon~=3.0.1
 	ujson~=1.35
 	jmespath~=0.9.3
-	clustaar.schemas~=0.17.0
+	clustaar.schemas==1.0.9
 	python-dateutil~=2.7.3
 tests_require = pytest; pytest-cov
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `clustaar.webhook-0.1.6/setup.py` & `clustaar.webhook-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/events_handler.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/events_handler.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/falcon/http_request.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/falcon/http_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def body(self):
         """Keeps body available for future calls
 
         Returns:
             str: request body
         """
         if self._body is None:
-            self._body = self.stream.read()
+            self._body = self.stream.read(self.content_length or 0)
 
         return self._body
 
     @property
     def json(self):
         """Loads JSON object from body.
```

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/falcon/http_response.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/falcon/http_response.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/filters.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/filters.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/authenticators.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/authenticators.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/basic_authentication_middleware.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/basic_authentication_middleware.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/replay_prevention_middleware.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/replay_prevention_middleware.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/middlewares/validate_signature_middleware.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/middlewares/validate_signature_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
         signed_headers = ("date",)
         buffer = "\n".join(
             ["%s=%s" % (header, req.get_header(header)) for header in signed_headers]
         )
         buffer += "\n" + req.body.decode("utf-8")
         expected_signature = hmac.new(self._private_key, buffer.encode(), hash_function).hexdigest()
+
         if expected_signature != signature:
             self._raise("The request's signature is invalid.")
 
     def _raise(self, description):
         """Raises a HTTPInvalidHeader exception with descrition.
 
         Args:
```

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/monkey_patch.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/routing/route.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/routing/route.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/routing/router.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/routing/router.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar/webhook/webhook.py` & `clustaar.webhook-0.1.7/src/clustaar/webhook/webhook.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/src/clustaar.webhook.egg-info/SOURCES.txt` & `clustaar.webhook-0.1.7/src/clustaar.webhook.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 goal.py
 pyproject.toml
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 wercker.yml
+.github/workflows/build_package.yml
+.github/workflows/launch_tests.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
 docs/_static/.gitignore
```

### Comparing `clustaar.webhook-0.1.6/tests/resources/webhook_request.json` & `clustaar.webhook-0.1.7/tests/resources/webhook_request.json`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/utils/__init__.py` & `clustaar.webhook-0.1.7/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/utils/factory.py` & `clustaar.webhook-0.1.7/tests/utils/factory.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/filters/test_json_key_equals.py` & `clustaar.webhook-0.1.7/tests/webhook/filters/test_json_key_equals.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/filters/test_json_key_exists.py` & `clustaar.webhook-0.1.7/tests/webhook/filters/test_json_key_exists.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/filters/test_json_key_in.py` & `clustaar.webhook-0.1.7/tests/webhook/filters/test_json_key_in.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/filters/test_step_id.py` & `clustaar.webhook-0.1.7/tests/webhook/filters/test_step_id.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/middlewares/test_basic_authentication_middleware.py` & `clustaar.webhook-0.1.7/tests/webhook/middlewares/test_basic_authentication_middleware.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/middlewares/test_replay_prevention_middleware.py` & `clustaar.webhook-0.1.7/tests/webhook/middlewares/test_replay_prevention_middleware.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/middlewares/test_static_authenticator.py` & `clustaar.webhook-0.1.7/tests/webhook/middlewares/test_static_authenticator.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/middlewares/test_validate_signature_middleware.py` & `clustaar.webhook-0.1.7/tests/webhook/middlewares/test_validate_signature_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,49 +20,49 @@
     def test_raises_exception_if_no_signature(self, middleware, response):
         request = FACTORY.create_http_request()
         with pytest.raises(falcon.HTTPInvalidHeader) as excinfo:
             middleware.process_resource(request, response, Mock(), {})
 
         exception = excinfo.value
         assert exception.description == (
-            "The value provided for the X-Hub-Signature header is invalid. "
+            "The value provided for the \"X-Hub-Signature\" header is invalid. "
             "The request's signature is missing."
         )
 
     def test_raises_exception_if_invalid_signature(self, middleware, response):
         request = FACTORY.create_http_request(headers={"X-Hub-Signature": "sha1=invalid"})
         with pytest.raises(falcon.HTTPInvalidHeader) as excinfo:
             middleware.process_resource(request, response, Mock(), {})
 
         exception = excinfo.value
         assert exception.description == (
-            "The value provided for the X-Hub-Signature header"
+            "The value provided for the \"X-Hub-Signature\" header"
             " is invalid. The request's signature is invalid."
         )
 
     def test_raises_execption_if_invalid_hash_function(self, middleware, response):
         request = FACTORY.create_http_request(headers={"X-Hub-Signature": "md5=invalid"})
         with pytest.raises(falcon.HTTPInvalidHeader) as excinfo:
             middleware.process_resource(request, response, Mock(), {})
 
         exception = excinfo.value
         assert exception.description == (
-            "The value provided for the X-Hub-Signature header is invalid. "
+            "The value provided for the \"X-Hub-Signature\" header is invalid. "
             "The request's signature hash function is "
             "invalid (should be one of ['sha1'])."
         )
 
     def test_raises_execption_if_invalid_format(self, middleware, response):
         request = FACTORY.create_http_request(headers={"X-Hub-Signature": "invalid_format"})
         with pytest.raises(falcon.HTTPInvalidHeader) as excinfo:
             middleware.process_resource(request, response, Mock(), {})
 
         exception = excinfo.value
         assert exception.description == (
-            "The value provided for the X-Hub-Signature header is invalid. "
+            "The value provided for the \"X-Hub-Signature\" header is invalid. "
             "The request's signature format is invalid."
         )
 
     def test_does_not_raises_exception_if_valid(self, middleware, response):
         request = FACTORY.create_http_request(
             body="{}", headers={"X-Hub-Signature": "sha1=fc2bdea0e6a9e0dc333dece7568b5c3337a92342"}
         )
```

### Comparing `clustaar.webhook-0.1.6/tests/webhook/routing/test_route.py` & `clustaar.webhook-0.1.7/tests/webhook/routing/test_route.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/routing/test_router.py` & `clustaar.webhook-0.1.7/tests/webhook/routing/test_router.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/test_events_handler.py` & `clustaar.webhook-0.1.7/tests/webhook/test_events_handler.py`

 * *Files identical despite different names*

### Comparing `clustaar.webhook-0.1.6/tests/webhook/test_webhook.py` & `clustaar.webhook-0.1.7/tests/webhook/test_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from freezegun import freeze_time
-from unittest.mock import Mock
 from base64 import b64encode
+from unittest.mock import Mock
+
 import falcon
 import pytest
-from clustaar.webhook import Webhook
 from clustaar.schemas.models import StepReachedResponse
+from freezegun import freeze_time
+
+from clustaar.webhook import Webhook
 from tests.utils import resource_content
 
 
 @pytest.fixture
 def webhook():
     return Webhook(
         private_key="test", auth_username="admin", auth_password="p@ssword", request_max_age=None
@@ -26,15 +28,15 @@
 
 
 class TestCall(object):
     def test_handles_invalid_signature(self, client, auth_value):
         result = client.simulate_post("/", headers={"Authorization": "Basic " + auth_value})
         assert result.json == {
             "description": (
-                "The value provided for the X-Hub-Signature header is invalid. "
+                "The value provided for the \"X-Hub-Signature\" header is invalid. "
                 "The request's signature is missing."
             ),
             "title": "Invalid header value",
         }
 
     def test_handles_invalid_credentials(self, client):
         result = client.simulate_post(
```

### Comparing `clustaar.webhook-0.1.6/wercker.yml` & `clustaar.webhook-0.1.7/wercker.yml`

 * *Files identical despite different names*


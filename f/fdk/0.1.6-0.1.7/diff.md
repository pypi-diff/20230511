# Comparing `tmp/fdk-0.1.6.tar.gz` & `tmp/fdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fdk-0.1.6.tar", last modified: Fri Jun 21 21:13:10 2019, max compression
+gzip compressed data, was "dist/fdk-0.1.7.tar", last modified: Mon Jul  1 17:13:57 2019, max compression
```

## Comparing `fdk-0.1.6.tar` & `fdk-0.1.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/.circleci/
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/.circleci/.anchore/
--rw-r--r--   0 denismakogon   (501) staff       (20)      863 2019-06-21 21:09:59.000000 fdk-0.1.6/.circleci/.anchore/policy_bundle.json
--rw-r--r--   0 denismakogon   (501) staff       (20)     3070 2019-06-21 21:09:59.000000 fdk-0.1.6/.circleci/config.yml
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/.github/
--rw-r--r--   0 denismakogon   (501) staff       (20)     1716 2019-02-05 16:34:38.000000 fdk-0.1.6/.github/issue_template.md
--rw-r--r--   0 denismakogon   (501) staff       (20)      192 2019-02-05 16:34:38.000000 fdk-0.1.6/.github/pull_request_template.md
--rw-r--r--   0 denismakogon   (501) staff       (20)      460 2019-06-21 21:13:08.000000 fdk-0.1.6/AUTHORS
--rw-r--r--   0 denismakogon   (501) staff       (20)     3464 2019-06-21 21:13:08.000000 fdk-0.1.6/ChangeLog
--rw-r--r--   0 denismakogon   (501) staff       (20)    11357 2019-02-05 16:34:38.000000 fdk-0.1.6/LICENSE
--rw-r--r--   0 denismakogon   (501) staff       (20)      619 2019-06-21 21:13:10.000000 fdk-0.1.6/PKG-INFO
--rw-r--r--   0 denismakogon   (501) staff       (20)    11925 2019-02-06 17:11:32.000000 fdk-0.1.6/README.md
--rwxr-xr-x   0 denismakogon   (501) staff       (20)      249 2019-06-21 21:09:59.000000 fdk-0.1.6/build-images.sh
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/fdk/
--rw-r--r--   0 denismakogon   (501) staff       (20)     4121 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/__init__.py
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/fdk/async_http/
--rw-r--r--   0 denismakogon   (501) staff       (20)        0 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/__init__.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     4069 2019-02-25 17:21:24.000000 fdk-0.1.6/fdk/async_http/app.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     4655 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/error_handler.py
--rw-r--r--   0 denismakogon   (501) staff       (20)    11767 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/exceptions.py
--rw-r--r--   0 denismakogon   (501) staff       (20)    20081 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/protocol.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     4351 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/request.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     9389 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/response.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1726 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/async_http/router.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     6739 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/async_http/server.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1507 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/constants.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     4882 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/context.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     2708 2019-02-28 21:57:08.000000 fdk-0.1.6/fdk/customer_code.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1259 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/errors.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     2267 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/event_handler.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     2595 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/fixtures.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1499 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/headers.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1303 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/log.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1736 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/response.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     3425 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/runner.py
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/fdk/scripts/
--rw-r--r--   0 denismakogon   (501) staff       (20)     1129 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/scripts/fdk.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1197 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/scripts/fdk_tcp_debug.py
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/fdk/tests/
--rw-r--r--   0 denismakogon   (501) staff       (20)        0 2019-02-05 16:34:38.000000 fdk-0.1.6/fdk/tests/__init__.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     3030 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/tests/funcs.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1624 2019-02-06 17:11:32.000000 fdk-0.1.6/fdk/tests/tcp_debug.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     1607 2019-02-28 21:57:08.000000 fdk-0.1.6/fdk/tests/test_delayed_loader.py
--rw-r--r--   0 denismakogon   (501) staff       (20)     5385 2019-06-21 21:09:59.000000 fdk-0.1.6/fdk/tests/test_http_stream.py
--rw-r--r--   0 denismakogon   (501) staff       (20)       18 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk/version.py
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/fdk.egg-info/
--rw-r--r--   0 denismakogon   (501) staff       (20)      619 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk.egg-info/PKG-INFO
--rw-r--r--   0 denismakogon   (501) staff       (20)     1284 2019-06-21 21:13:09.000000 fdk-0.1.6/fdk.egg-info/SOURCES.txt
--rw-r--r--   0 denismakogon   (501) staff       (20)        1 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk.egg-info/dependency_links.txt
--rw-r--r--   0 denismakogon   (501) staff       (20)       93 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk.egg-info/entry_points.txt
--rw-r--r--   0 denismakogon   (501) staff       (20)        1 2019-03-05 11:46:37.000000 fdk-0.1.6/fdk.egg-info/not-zip-safe
--rw-r--r--   0 denismakogon   (501) staff       (20)       47 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk.egg-info/pbr.json
--rw-r--r--   0 denismakogon   (501) staff       (20)       89 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk.egg-info/requires.txt
--rw-r--r--   0 denismakogon   (501) staff       (20)        4 2019-06-21 21:13:08.000000 fdk-0.1.6/fdk.egg-info/top_level.txt
--rwxr-xr-x   0 denismakogon   (501) staff       (20)      800 2019-06-21 21:09:59.000000 fdk-0.1.6/generate_func.sh
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/images/
--rw-r--r--   0 denismakogon   (501) staff       (20)      570 2019-06-21 21:09:59.000000 fdk-0.1.6/images/README.md
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/images/build-stage/
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/images/build-stage/3.6/
--rw-r--r--   0 denismakogon   (501) staff       (20)      168 2019-06-21 21:09:59.000000 fdk-0.1.6/images/build-stage/3.6/Dockerfile
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/images/build-stage/3.7.1/
--rw-r--r--   0 denismakogon   (501) staff       (20)      170 2019-06-21 21:09:59.000000 fdk-0.1.6/images/build-stage/3.7.1/Dockerfile
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/images/runtime/
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/images/runtime/3.6/
--rw-r--r--   0 denismakogon   (501) staff       (20)      181 2019-06-21 21:09:59.000000 fdk-0.1.6/images/runtime/3.6/Dockerfile
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/images/runtime/3.7.1/
--rw-r--r--   0 denismakogon   (501) staff       (20)      184 2019-06-21 21:09:59.000000 fdk-0.1.6/images/runtime/3.7.1/Dockerfile
--rwxr-xr-x   0 denismakogon   (501) staff       (20)      858 2019-06-21 21:09:59.000000 fdk-0.1.6/release.sh
--rw-r--r--   0 denismakogon   (501) staff       (20)     1109 2019-02-05 16:34:38.000000 fdk-0.1.6/release_doc.md
--rwxr-xr-x   0 denismakogon   (501) staff       (20)      268 2019-06-21 21:09:59.000000 fdk-0.1.6/release_images.sh
--rw-r--r--   0 denismakogon   (501) staff       (20)      102 2019-02-06 17:11:32.000000 fdk-0.1.6/requirements.txt
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:09.000000 fdk-0.1.6/samples/
-drwxr-xr-x   0 denismakogon   (501) staff       (20)        0 2019-06-21 21:13:10.000000 fdk-0.1.6/samples/echo/
--rw-r--r--   0 denismakogon   (501) staff       (20)     1354 2019-02-25 17:21:24.000000 fdk-0.1.6/samples/echo/func.py
--rw-r--r--   0 denismakogon   (501) staff       (20)      786 2019-06-21 21:13:10.000000 fdk-0.1.6/setup.cfg
--rw-r--r--   0 denismakogon   (501) staff       (20)      685 2019-02-05 16:34:38.000000 fdk-0.1.6/setup.py
--rw-r--r--   0 denismakogon   (501) staff       (20)       68 2019-02-06 17:11:32.000000 fdk-0.1.6/test-requirements.txt
--rw-r--r--   0 denismakogon   (501) staff       (20)      877 2019-02-28 21:57:08.000000 fdk-0.1.6/tox.ini
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/.circleci/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/.circleci/.anchore/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      863 2019-07-01 17:12:22.000000 fdk-0.1.7/.circleci/.anchore/policy_bundle.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3139 2019-07-01 17:12:22.000000 fdk-0.1.7/.circleci/config.yml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/.github/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1716 2019-07-01 17:12:22.000000 fdk-0.1.7/.github/issue_template.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2019-07-01 17:12:22.000000 fdk-0.1.7/.github/pull_request_template.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      460 2019-07-01 17:13:57.000000 fdk-0.1.7/AUTHORS
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3675 2019-07-01 17:13:57.000000 fdk-0.1.7/ChangeLog
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2019-07-01 17:12:22.000000 fdk-0.1.7/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      687 2019-07-01 17:13:57.000000 fdk-0.1.7/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11925 2019-07-01 17:12:22.000000 fdk-0.1.7/README.md
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      249 2019-07-01 17:12:22.000000 fdk-0.1.7/build-images.sh
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4121 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk/async_http/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3996 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4655 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/error_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11767 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20081 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/protocol.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4351 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11117 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1726 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/router.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6739 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/async_http/server.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4882 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2708 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/customer_code.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2267 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/event_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2595 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/headers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1303 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1736 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3230 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk/scripts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/scripts/fdk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1197 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/scripts/fdk_tcp_debug.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3030 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/tests/funcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1624 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/tests/tcp_debug.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1607 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/tests/test_delayed_loader.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5493 2019-07-01 17:12:22.000000 fdk-0.1.7/fdk/tests/test_http_stream.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2019-07-01 17:13:56.000000 fdk-0.1.7/fdk/version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      687 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1284 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/pbr.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2019-07-01 17:13:57.000000 fdk-0.1.7/fdk.egg-info/top_level.txt
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      800 2019-07-01 17:12:22.000000 fdk-0.1.7/generate_func.sh
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      570 2019-07-01 17:12:22.000000 fdk-0.1.7/images/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/build-stage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/build-stage/3.6/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      168 2019-07-01 17:12:22.000000 fdk-0.1.7/images/build-stage/3.6/Dockerfile
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/build-stage/3.7.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      170 2019-07-01 17:12:22.000000 fdk-0.1.7/images/build-stage/3.7.1/Dockerfile
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/runtime/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/runtime/3.6/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2019-07-01 17:12:22.000000 fdk-0.1.7/images/runtime/3.6/Dockerfile
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/images/runtime/3.7.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2019-07-01 17:12:22.000000 fdk-0.1.7/images/runtime/3.7.1/Dockerfile
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      837 2019-07-01 17:12:22.000000 fdk-0.1.7/release.sh
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1109 2019-07-01 17:12:22.000000 fdk-0.1.7/release_doc.md
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      268 2019-07-01 17:12:22.000000 fdk-0.1.7/release_images.sh
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      102 2019-07-01 17:12:22.000000 fdk-0.1.7/requirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/samples/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-07-01 17:13:57.000000 fdk-0.1.7/samples/echo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1354 2019-07-01 17:12:22.000000 fdk-0.1.7/samples/echo/func.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      786 2019-07-01 17:13:57.000000 fdk-0.1.7/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      685 2019-07-01 17:12:22.000000 fdk-0.1.7/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2019-07-01 17:12:22.000000 fdk-0.1.7/test-requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2019-07-01 17:12:22.000000 fdk-0.1.7/tox.ini
```

### Comparing `fdk-0.1.6/.circleci/.anchore/policy_bundle.json` & `fdk-0.1.7/.circleci/.anchore/policy_bundle.json`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/.circleci/config.yml` & `fdk-0.1.7/.circleci/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,25 @@
     working_directory: ~/fdk-python
     steps:
       - checkout
       - restore_cache:
           key: deps1-{{ .Branch }}-{{ checksum "requirements.txt" }}
       - setup_remote_docker:
           docker_layer_caching: true
+      - run:
+          command: |
+            sudo pip install twine
       - deploy:
           command: |
             if [[ "${CIRCLE_BRANCH}" == "master" && -z "${CIRCLE_PR_REPONAME}" ]]; then
               printenv DOCKER_PASS | docker login -u $DOCKER_USER --password-stdin
               ./build-images.sh 3.6
               ./build-images.sh 3.7.1
-              ./release_images.sh
               ./release.sh
+              ./release_images.sh
             fi
 
   "python36_security_check":
     executor: anchore/anchore_engine
     working_directory: ~/fdk-python
     steps:
       - setup_remote_docker:
```

### Comparing `fdk-0.1.6/.github/issue_template.md` & `fdk-0.1.7/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/ChangeLog` & `fdk-0.1.7/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+* Enable docker images release (#92)
+* Fixing version placement command
+* properly grab content type (#90)
+* Disable image release procedure temporarily (#89)
+
+0.1.6
+-----
+
+* FDK Python: 0.1.6 release [skip ci]
 * fix gateway headers / headers casing (#88)
 * removing corresponding TODO
 * adding FDK release into the CI
 * New PBR release broke setup config
 * Automated releases + FDK version header (#82)
 * attempt fixing content type issue (#83)
 * Adding Anchore CI check (#77)
```

### Comparing `fdk-0.1.6/LICENSE` & `fdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/PKG-INFO` & `fdk-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Function Developer Kit for Python
 Home-page: https://fnproject.github.io
 Author: Denis Makogon
 Author-email: denys.makogon@oracle.com
 License: UNKNOWN
 Description: 
         README.md
@@ -12,7 +12,8 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

### Comparing `fdk-0.1.6/README.md` & `fdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/__init__.py` & `fdk-0.1.7/fdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/async_http/app.py` & `fdk-0.1.7/fdk/async_http/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
             response = handler(request)
             logger.info("got response from function")
             res = await response
             body = res.body
             headers = res.headers
             status = res.status
             response = HTTPResponse(
-                body=body, status=status,
-                headers=headers,
-                content_type=headers.get("Content-Type")
+                body=body, status=status, headers=headers,
             )
         except CancelledError:
             response = None
             cancelled = True
         except Exception as e:
             if isinstance(e, AsyncHTTPException):
                 response = self.error_handler.default(
```

### Comparing `fdk-0.1.6/fdk/async_http/error_handler.py` & `fdk-0.1.7/fdk/async_http/error_handler.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/async_http/exceptions.py` & `fdk-0.1.7/fdk/async_http/exceptions.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/async_http/protocol.py` & `fdk-0.1.7/fdk/async_http/protocol.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/async_http/request.py` & `fdk-0.1.7/fdk/async_http/request.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/async_http/response.py` & `fdk-0.1.7/fdk/async_http/response.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,14 +127,65 @@
             self.status,
             status,
             timeout_header,
             headers,
         )
 
 
+# CaseInsensitiveDict for headers. TODO should we let users use it in fdk too?
+class CaseInsensitiveDict(dict):
+    @classmethod
+    def _k(cls, key):
+        return key.lower() if isinstance(key, str) else key
+
+    def __init__(self, *args, **kwargs):
+        super(CaseInsensitiveDict, self).__init__(*args, **kwargs)
+        self._convert_keys()
+
+    def __getitem__(self, key):
+        return super(CaseInsensitiveDict, self).__getitem__(
+            self.__class__._k(key))
+
+    def __setitem__(self, key, value):
+        super(CaseInsensitiveDict, self).__setitem__(
+            self.__class__._k(key), value)
+
+    def __delitem__(self, key):
+        return super(CaseInsensitiveDict, self).__delitem__(
+            self.__class__._k(key))
+
+    def __contains__(self, key):
+        return super(CaseInsensitiveDict, self).__contains__(
+            self.__class__._k(key))
+
+    # DEPRECATED
+    # def has_key(self, key):
+
+    def pop(self, key, *args, **kwargs):
+        return super(CaseInsensitiveDict, self).pop(
+            self.__class__._k(key), *args, **kwargs)
+
+    def get(self, key, *args, **kwargs):
+        return super(CaseInsensitiveDict, self).get(
+            self.__class__._k(key), *args, **kwargs)
+
+    def setdefault(self, key, *args, **kwargs):
+        return super(CaseInsensitiveDict, self).setdefault(
+            self.__class__._k(key), *args, **kwargs)
+
+    def update(self, E={}, **F):
+        super(CaseInsensitiveDict, self).update(self.__class__(E))
+        super(CaseInsensitiveDict, self).update(self.__class__(**F))
+
+    def _convert_keys(self):
+        for k in list(self.keys()):
+            v = super(CaseInsensitiveDict, self).pop(k)
+            self.__setitem__(k, v)
+
+
 class HTTPResponse(BaseHTTPResponse):
     __slots__ = ("body", "status", "content_type", "headers", "_cookies")
 
     def __init__(
         self,
         body=None,
         status=200,
@@ -146,15 +197,15 @@
 
         if body is not None:
             self.body = self._encode_body(body)
         else:
             self.body = body_bytes
 
         self.status = status
-        self.headers = dict(headers or {})
+        self.headers = CaseInsensitiveDict(headers or {})
         self._cookies = None
 
     def output(self, version="1.1", keep_alive=False, keep_alive_timeout=None):
         # This is all returned in a kind-of funky way
         # We tried to make this as fast as possible in pure python
         timeout_header = b""
         if keep_alive and keep_alive_timeout is not None:
```

### Comparing `fdk-0.1.6/fdk/async_http/router.py` & `fdk-0.1.7/fdk/async_http/router.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/async_http/server.py` & `fdk-0.1.7/fdk/async_http/server.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/constants.py` & `fdk-0.1.7/fdk/constants.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/context.py` & `fdk-0.1.7/fdk/context.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/customer_code.py` & `fdk-0.1.7/fdk/customer_code.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/errors.py` & `fdk-0.1.7/fdk/errors.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/event_handler.py` & `fdk-0.1.7/fdk/event_handler.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/fixtures.py` & `fdk-0.1.7/fdk/fixtures.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/headers.py` & `fdk-0.1.7/fdk/headers.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/log.py` & `fdk-0.1.7/fdk/log.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/response.py` & `fdk-0.1.7/fdk/response.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/runner.py` & `fdk-0.1.7/fdk/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import traceback
 import signal
 import datetime as dt
 import iso8601
 import types
 
 from fdk import context
-from fdk import constants
 from fdk import customer_code
 from fdk import errors
 from fdk import log
 from fdk import response
 
 
 async def with_deadline(ctx: context.InvokeContext,
@@ -87,19 +86,14 @@
         response_data = await with_deadline(ctx, handler_code, body)
         log.log("function result obtained")
         if isinstance(response_data, response.Response):
             return response_data
 
         headers = ctx.GetResponseHeaders()
         log.log("response headers obtained")
-        response_content_type = headers.get(
-            constants.CONTENT_TYPE, "text/plain"
-        )
-        headers[constants.CONTENT_TYPE] = response_content_type
-
         return response.Response(
             ctx, response_data=response_data,
             headers=headers, status_code=200)
 
     except (Exception, TimeoutError) as ex:
         log.log("exception appeared: {0}".format(ex))
         traceback.print_exc(file=sys.stderr)
```

### Comparing `fdk-0.1.6/fdk/scripts/fdk.py` & `fdk-0.1.7/fdk/scripts/fdk.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/scripts/fdk_tcp_debug.py` & `fdk-0.1.7/fdk/scripts/fdk_tcp_debug.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/tests/funcs.py` & `fdk-0.1.7/fdk/tests/funcs.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/tests/tcp_debug.py` & `fdk-0.1.7/fdk/tests/tcp_debug.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/tests/test_delayed_loader.py` & `fdk-0.1.7/fdk/tests/test_delayed_loader.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/fdk/tests/test_http_stream.py` & `fdk-0.1.7/fdk/tests/test_http_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 async def test_override_content_type():
     call = await fixtures.setup_fn_call(
         funcs.content_type)
     content, status, headers = await call
 
     assert 200 == status
     assert "OK" == content
-    assert "application/json" in headers.get("content-type")
+    assert headers.get("content-type") == "application/json"
+    # we've had issues with 'Content-Type: None' slipping in
+    assert headers.get("Content-Type") is None
     assert version.VERSION == headers.get(constants.FN_FDK_VERSION)
 
 
 @pytest.mark.asyncio
 async def test_parse_request_without_data():
     call = await fixtures.setup_fn_call(funcs.dummy_func)
```

### Comparing `fdk-0.1.6/fdk.egg-info/PKG-INFO` & `fdk-0.1.7/fdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Function Developer Kit for Python
 Home-page: https://fnproject.github.io
 Author: Denis Makogon
 Author-email: denys.makogon@oracle.com
 License: UNKNOWN
 Description: 
         README.md
@@ -12,7 +12,8 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

### Comparing `fdk-0.1.6/fdk.egg-info/SOURCES.txt` & `fdk-0.1.7/fdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/generate_func.sh` & `fdk-0.1.7/generate_func.sh`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/images/README.md` & `fdk-0.1.7/images/README.md`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/release.sh` & `fdk-0.1.7/release.sh`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 version_file="fdk/version.py"
 current_version=$(grep -m1 -Eo "[0-9]+\.[0-9]+\.[0-9]+" ${version_file})
 new_version=$(docker run --rm marcelocorreia/semver semver -c -i patch ${current_version})
 
 echo "Current version: $current_version"
 echo "New version: $new_version"
 
-sed -i '' -e 's/'"$current_version"'/'"$new_version"'/g' fdk/version.py
+echo "VERSION = '${new_version}'" > fdk/version.py
 
 PBR_VERSION=${new_version} python setup.py sdist bdist_wheel
 twine upload -u ${FN_PYPI_USER} -p ${FN_PYPI_PSWD} dist/fdk-${new_version}*
 
 tag="$new_version"
 git add -u
 git commit -m "FDK Python: $new_version release [skip ci]"
```

### Comparing `fdk-0.1.6/release_doc.md` & `fdk-0.1.7/release_doc.md`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/samples/echo/func.py` & `fdk-0.1.7/samples/echo/func.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/setup.cfg` & `fdk-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/setup.py` & `fdk-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `fdk-0.1.6/tox.ini` & `fdk-0.1.7/tox.ini`

 * *Files identical despite different names*


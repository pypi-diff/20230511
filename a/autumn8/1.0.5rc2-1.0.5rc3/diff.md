# Comparing `tmp/autumn8-1.0.5rc2.tar.gz` & `tmp/autumn8-1.0.5rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc2.tar", last modified: Thu May 11 15:27:21 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc3.tar", last modified: Thu May 11 15:41:32 2023, max compression
```

## Comparing `autumn8-1.0.5rc2.tar` & `autumn8-1.0.5rc3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.529408 autumn8-1.0.5rc2/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-11 15:27:21.519416 autumn8-1.0.5rc2/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.489441 autumn8-1.0.5rc2/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.499432 autumn8-1.0.5rc2/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-09 16:01:44.000000 autumn8-1.0.5rc2/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-11 15:01:40.000000 autumn8-1.0.5rc2/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.499432 autumn8-1.0.5rc2/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     9136 2023-05-11 15:01:40.000000 autumn8-1.0.5rc2/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16161 2023-05-11 15:15:48.000000 autumn8-1.0.5rc2/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4094 2023-05-11 15:01:40.000000 autumn8-1.0.5rc2/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-11 15:01:40.000000 autumn8-1.0.5rc2/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-09 16:01:44.000000 autumn8-1.0.5rc2/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-05 17:40:41.000000 autumn8-1.0.5rc2/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.509424 autumn8-1.0.5rc2/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-11 15:26:22.000000 autumn8-1.0.5rc2/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.509424 autumn8-1.0.5rc2/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.5rc2/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.509424 autumn8-1.0.5rc2/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc2/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc2/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc2/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc2/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc2/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.519416 autumn8-1.0.5rc2/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc2/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.5rc2/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.5rc2/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.5rc2/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.5rc2/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.519416 autumn8-1.0.5rc2/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.5rc2/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.519416 autumn8-1.0.5rc2/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-11 15:01:40.000000 autumn8-1.0.5rc2/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-05 17:40:41.000000 autumn8-1.0.5rc2/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11804 2023-05-09 16:01:44.000000 autumn8-1.0.5rc2/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-11 15:01:40.000000 autumn8-1.0.5rc2/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1676 2023-05-11 15:25:39.000000 autumn8-1.0.5rc2/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-05 17:40:41.000000 autumn8-1.0.5rc2/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      107 2023-05-11 15:15:11.000000 autumn8-1.0.5rc2/autumn8/lib/exceptions.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-05 17:40:41.000000 autumn8-1.0.5rc2/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-05 17:40:41.000000 autumn8-1.0.5rc2/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.5rc2/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc2/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-09 16:01:44.000000 autumn8-1.0.5rc2/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.499432 autumn8-1.0.5rc2/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-11 15:27:21.000000 autumn8-1.0.5rc2/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1462 2023-05-11 15:27:21.000000 autumn8-1.0.5rc2/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-11 15:27:21.000000 autumn8-1.0.5rc2/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-11 15:27:21.000000 autumn8-1.0.5rc2/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-11 15:27:21.000000 autumn8-1.0.5rc2/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-11 15:27:21.000000 autumn8-1.0.5rc2/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-09 16:01:44.000000 autumn8-1.0.5rc2/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-11 15:27:21.529408 autumn8-1.0.5rc2/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.5rc2/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:27:21.519416 autumn8-1.0.5rc2/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-09 16:01:44.000000 autumn8-1.0.5rc2/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.5rc2/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.377173 autumn8-1.0.5rc3/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-11 15:41:32.377173 autumn8-1.0.5rc3/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.357173 autumn8-1.0.5rc3/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-09 16:01:44.000000 autumn8-1.0.5rc3/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-11 15:01:40.000000 autumn8-1.0.5rc3/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     9136 2023-05-11 15:01:40.000000 autumn8-1.0.5rc3/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16161 2023-05-11 15:40:12.000000 autumn8-1.0.5rc3/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4094 2023-05-11 15:01:40.000000 autumn8-1.0.5rc3/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-11 15:01:40.000000 autumn8-1.0.5rc3/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-09 16:01:44.000000 autumn8-1.0.5rc3/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-05 17:40:41.000000 autumn8-1.0.5rc3/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-11 15:40:44.000000 autumn8-1.0.5rc3/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.5rc3/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc3/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc3/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc3/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc3/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc3/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc3/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.5rc3/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.5rc3/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.5rc3/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.5rc3/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.377173 autumn8-1.0.5rc3/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.5rc3/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.377173 autumn8-1.0.5rc3/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-11 15:01:40.000000 autumn8-1.0.5rc3/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-05 17:40:41.000000 autumn8-1.0.5rc3/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11814 2023-05-11 15:36:13.000000 autumn8-1.0.5rc3/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-11 15:01:40.000000 autumn8-1.0.5rc3/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1676 2023-05-11 15:40:12.000000 autumn8-1.0.5rc3/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-05 17:40:41.000000 autumn8-1.0.5rc3/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      107 2023-05-11 15:40:12.000000 autumn8-1.0.5rc3/autumn8/lib/exceptions.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-05 17:40:41.000000 autumn8-1.0.5rc3/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-05 17:40:41.000000 autumn8-1.0.5rc3/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.5rc3/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc3/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-09 16:01:44.000000 autumn8-1.0.5rc3/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.367173 autumn8-1.0.5rc3/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-11 15:41:32.000000 autumn8-1.0.5rc3/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1462 2023-05-11 15:41:32.000000 autumn8-1.0.5rc3/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-11 15:41:32.000000 autumn8-1.0.5rc3/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-11 15:41:32.000000 autumn8-1.0.5rc3/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-11 15:41:32.000000 autumn8-1.0.5rc3/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-11 15:41:32.000000 autumn8-1.0.5rc3/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-09 16:01:44.000000 autumn8-1.0.5rc3/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-11 15:41:32.377173 autumn8-1.0.5rc3/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.5rc3/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-11 15:41:32.377173 autumn8-1.0.5rc3/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-09 16:01:44.000000 autumn8-1.0.5rc3/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.5rc3/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc2/PKG-INFO` & `autumn8-1.0.5rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc2
+Version: 1.0.5rc3
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc2/README.md` & `autumn8-1.0.5rc3/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/analyze.py` & `autumn8-1.0.5rc3/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc3/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc3/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc3/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/examples.py` & `autumn8-1.0.5rc3/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/interactive.py` & `autumn8-1.0.5rc3/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/main.py` & `autumn8-1.0.5rc3/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/options.py` & `autumn8-1.0.5rc3/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc3/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/cli/validation.py` & `autumn8-1.0.5rc3/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc3/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/common/config/settings.py` & `autumn8-1.0.5rc3/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc3/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/common/types.py` & `autumn8-1.0.5rc3/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/env/__init__.py` & `autumn8-1.0.5rc3/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/examples/mnist.py` & `autumn8-1.0.5rc3/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/examples/model.py` & `autumn8-1.0.5rc3/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc3/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc3/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/__init__.py` & `autumn8-1.0.5rc3/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/api/cloud.py` & `autumn8-1.0.5rc3/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc3/autumn8/lib/api/lab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import io
 import json
+import os
 from threading import Lock
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 import appdirs
 import boto3
 import httpx
 import requests
```

### Comparing `autumn8-1.0.5rc2/autumn8/lib/api/user.py` & `autumn8-1.0.5rc3/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc3/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/asyncio.py` & `autumn8-1.0.5rc3/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/http.py` & `autumn8-1.0.5rc3/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/logging.py` & `autumn8-1.0.5rc3/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc3/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc3/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8/lib/service.py` & `autumn8-1.0.5rc3/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc3/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc2
+Version: 1.0.5rc3
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc2/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc3/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/pyproject.toml` & `autumn8-1.0.5rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.5rc3/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc2/tests/test_settings.py` & `autumn8-1.0.5rc3/tests/test_settings.py`

 * *Files identical despite different names*


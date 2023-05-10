# Comparing `tmp/dev-gpt-0.18.37.dev52.tar.gz` & `tmp/dev-gpt-0.18.37.dev78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-gpt-0.18.37.dev52.tar", last modified: Fri May  5 01:25:23 2023, max compression
+gzip compressed data, was "dev-gpt-0.18.37.dev78.tar", last modified: Wed May 10 23:13:34 2023, max compression
```

## Comparing `dev-gpt-0.18.37.dev52.tar` & `dev-gpt-0.18.37.dev78.tar`

### file list

```diff
@@ -1,72 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 01:25:22.000000 dev-gpt-0.18.37.dev52/dev_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/apis/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/configure/key_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/deploy/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/base_image/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/base_image/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/app_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/generate/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/options/run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/options/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/dev_gpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/dev_gpt/utils/string_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.484175 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 01:25:23.000000 dev-gpt-0.18.37.dev52/dev_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/integration/test_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:23.488175 dev-gpt-0.18.37.dev52/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/test_response_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 01:25:17.000000 dev-gpt-0.18.37.dev52/test/unit/test_strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 23:13:33.000000 dev-gpt-0.18.37.dev78/dev_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/apis/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/apis/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/apis/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/options/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/configure/key_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/options/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/deploy/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/auto_refine_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/extract_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/get_user_input_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25847 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/pm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/pm/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/pm/task_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/prompt_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/base_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/base_image/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/app_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/custom_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/microservice/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/microservice/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/templates_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/templates_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/generate/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/options/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/options/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/dev_gpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/dev_gpt/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.211951 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-10 23:13:34.000000 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-10 23:13:34.000000 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:13:34.000000 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 23:13:34.000000 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 23:13:34.000000 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 23:13:34.000000 dev-gpt-0.18.37.dev78/dev_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/integration/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:34.215951 dev-gpt-0.18.37.dev78/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/unit/test_construct_sub_task_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/unit/test_response_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-10 23:13:30.000000 dev-gpt-0.18.37.dev78/test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.37.dev52/LICENSE` & `dev-gpt-0.18.37.dev78/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/PKG-INFO` & `dev-gpt-0.18.37.dev78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.37.dev52
+Version: 0.18.37.dev78
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev52 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev78 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.37.dev52/README.md` & `dev-gpt-0.18.37.dev78/README.md`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/apis/gpt.py` & `dev-gpt-0.18.37.dev78/dev_gpt/apis/gpt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,73 @@
+import json
 import os
 from copy import deepcopy
 from time import sleep
-
 from typing import List, Any
 
 import openai
 from langchain import PromptTemplate
 from langchain.callbacks import CallbackManager
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.chat_models import ChatOpenAI
-from openai.error import RateLimitError
 from langchain.schema import HumanMessage, SystemMessage, BaseMessage, AIMessage
-from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
+from openai.error import RateLimitError
 from requests.exceptions import ConnectionError, ChunkedEncodingError
 from urllib3.exceptions import InvalidChunkLength
 
 from dev_gpt.constants import PRICING_GPT4_PROMPT, PRICING_GPT4_GENERATION, PRICING_GPT3_5_TURBO_PROMPT, \
     PRICING_GPT3_5_TURBO_GENERATION, CHARS_PER_TOKEN
 from dev_gpt.options.generate.templates_system import template_system_message_base
-from dev_gpt.utils.string_tools import print_colored
+from dev_gpt.utils.string_tools import print_colored, get_template_parameters
 
 
 def configure_openai_api_key():
     if 'OPENAI_API_KEY' not in os.environ:
         print_colored('You need to set OPENAI_API_KEY in your environment.', '''
 Run:
 dev-gpt configure --key <your_openai_api_key>
 
 If you have updated it already, please restart your terminal.
 ''', 'red')
         exit(1)
     openai.api_key = os.environ['OPENAI_API_KEY']
 
+
 class GPTSession:
-    def __init__(self, task_description, model: str = 'gpt-4', ):
-        self.task_description = task_description
+    _instance = None
+    _initialized = False
+
+    def __new__(cls, *args, **kwargs):
+        if cls._instance is None:
+            cls._instance = super(GPTSession, cls).__new__(cls)
+        return cls._instance
+
+    def __init__(self, model: str = 'gpt-4', ):
+        if GPTSession._initialized:
+            return
         if model == 'gpt-4' and self.is_gpt4_available():
             self.pricing_prompt = PRICING_GPT4_PROMPT
             self.pricing_generation = PRICING_GPT4_GENERATION
         else:
             if model == 'gpt-4':
                 print_colored('GPT version info', 'GPT-4 is not available. Using GPT-3.5-turbo instead.', 'yellow')
             model = 'gpt-3.5-turbo'
             self.pricing_prompt = PRICING_GPT3_5_TURBO_PROMPT
             self.pricing_generation = PRICING_GPT3_5_TURBO_GENERATION
         self.model_name = model
         self.chars_prompt_so_far = 0
         self.chars_generation_so_far = 0
+        GPTSession._initialized = True
 
     def get_conversation(self, messages: List[BaseMessage] = [], print_stream: bool = True, print_costs: bool = True):
         messages = deepcopy(messages)
         return _GPTConversation(
             self.model_name, self.cost_callback, messages, print_stream, print_costs
         )
 
-
     @staticmethod
     def is_gpt4_available():
         try:
             for i in range(5):
                 try:
                     openai.ChatCompletion.create(
                         model="gpt-4",
@@ -105,15 +115,14 @@
             temperature=0,
         )
         self.cost_callback = cost_callback
         self.messages = messages
         self.print_stream = print_stream
         self.print_costs = print_costs
 
-
     def print_messages(self, messages):
         for i, message in enumerate(messages):
             if os.environ['VERBOSE'].lower() == 'true':
                 if isinstance(message, SystemMessage):
                     print_colored(f'({i}) system - prompt', message.content, 'magenta')
                 elif isinstance(message, HumanMessage):
                     print_colored(f'({i}) user - prompt', message.content, 'blue')
@@ -147,7 +156,27 @@
     @staticmethod
     def _create_system_message(task_description, test_description) -> SystemMessage:
         system_message = PromptTemplate.from_template(template_system_message_base).format(
             task_description=task_description,
             test_description=test_description,
         )
         return SystemMessage(content=system_message)
+
+
+def ask_gpt(prompt_template, parser, **kwargs):
+    template_parameters = get_template_parameters(prompt_template)
+    if set(template_parameters) != set(kwargs.keys()):
+        raise ValueError(
+            f'Prompt template parameters {set(template_parameters)} do not match provided parameters {set(kwargs.keys())}'
+        )
+    for key, value in kwargs.items():
+        if isinstance(value, dict):
+            kwargs[key] = json.dumps(value, indent=4)
+    prompt = prompt_template.format(**kwargs)
+    conversation = GPTSession().get_conversation(
+        [],
+        print_stream=os.environ['VERBOSE'].lower() == 'true',
+        print_costs=False
+    )
+    agent_response_raw = conversation.chat(prompt, role='user')
+    agent_response = parser(agent_response_raw)
+    return agent_response
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/apis/jina_cloud.py` & `dev-gpt-0.18.37.dev78/dev_gpt/apis/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/apis/pypi.py` & `dev-gpt-0.18.37.dev78/dev_gpt/apis/pypi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 import os
 import re
 from datetime import datetime
 
 import requests
 from packaging import version
 
-
 def is_package_on_pypi(package_name, version=None):
     """
     Returns True if the package is on PyPI, False if it is not, and None if the status code is not 200 or 404.
     """
     optional_version = f"/{version}" if version else ""
     url = f"https://pypi.org/pypi/{package_name}{optional_version}/json"
     response = requests.get(url)
-    if response.status_code == 200:
-        return True
-    elif response.status_code == 404:
-        return False
-    else:
-        return None
+    return response.status_code == 200 and len(response.json()['urls']) > 0
 
 
 def get_latest_package_version(package_name):
     """
     Returns the latest version of a package that is not older than 2021.
     """
     url = f'https://pypi.org/pypi/{package_name}/json'
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/cli.py` & `dev-gpt-0.18.37.dev78/dev_gpt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 def path_param(func):
     @click.option('--path', default='microservice', help='Path to the generated microservice.')
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         path = os.path.expanduser(kwargs['path'])
         path = os.path.abspath(path)
+        if os.path.exists(path) and os.listdir(path):
+                click.echo(f"Error: The path {path} you provided via --path is not empty. Please choose a directory that does not exist or is empty.")
+                exit(1)
         kwargs['path'] = path
         return func(*args, **kwargs)
     return wrapper
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/constants.py` & `dev-gpt-0.18.37.dev78/dev_gpt/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,13 @@
     'tika',  # because it needs java
 ]
 UNNECESSARY_PACKAGES = [
     'fastapi', 'uvicorn', 'starlette'  # because the wrappers are used instead
 ]
 
 LANGUAGE_PACKAGES = [
-    'allennlp', 'bertopic', 'fasttext', 'flair', 'gensim', 'nltk',
+    'allennlp', 'bertopic', 'fasttext', 'flair', 'gensim', 'nltk', 'openai',
     'pattern', 'polyglot', 'pytorch-transformers', 'rasa', 'sentence-transformers',
-    'spacy', 'stanza', 'summarizer', 'sumy', 'textblob', 'textstat', 'transformers'
+    'spacy', 'stanza', 'summarizer', 'sumy', 'textblob', 'textstat', 'transformers',
+    'vadersentiment'
 ]
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/__init__.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/configure/key_handling.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/configure/key_handling.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/generator.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,48 +3,45 @@
 import random
 import re
 import shutil
 from typing import Callable
 from typing import List, Text, Optional
 
 from langchain import PromptTemplate
-from langchain.schema import SystemMessage, HumanMessage, AIMessage
 from pydantic.dataclasses import dataclass
 
 from dev_gpt.apis import gpt
 from dev_gpt.apis.gpt import _GPTConversation
 from dev_gpt.apis.jina_cloud import process_error_message, push_executor, is_executor_in_hub
-from dev_gpt.apis.pypi import is_package_on_pypi, get_latest_package_version, clean_requirements_txt
+from dev_gpt.apis.pypi import is_package_on_pypi, clean_requirements_txt
 from dev_gpt.constants import FILE_AND_TAG_PAIRS, NUM_IMPLEMENTATION_STRATEGIES, MAX_DEBUGGING_ITERATIONS, \
     BLACKLISTED_PACKAGES, EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_NAME, TEST_EXECUTOR_FILE_TAG, \
     REQUIREMENTS_FILE_NAME, REQUIREMENTS_FILE_TAG, DOCKER_FILE_NAME, IMPLEMENTATION_FILE_NAME, \
     IMPLEMENTATION_FILE_TAG, LANGUAGE_PACKAGES, UNNECESSARY_PACKAGES, DOCKER_BASE_IMAGE_VERSION
-from dev_gpt.options.generate.templates_system import system_task_iteration, system_task_introduction, system_test_iteration
+from dev_gpt.options.generate.pm.pm import PM
 from dev_gpt.options.generate.templates_user import template_generate_microservice_name, \
     template_generate_possible_packages, \
     template_solve_code_issue, \
     template_solve_pip_dependency_issue, template_is_dependency_issue, template_generate_playground, \
     template_generate_function, template_generate_test, template_generate_requirements, \
     template_chain_of_thought, template_summarize_error, \
-    template_solve_apt_get_dependency_issue, template_pm_task_iteration, \
-    template_pm_test_iteration
-from dev_gpt.options.generate.ui import get_random_employee
+    template_solve_apt_get_dependency_issue
 from dev_gpt.utils.io import persist_file, get_all_microservice_files_with_content, get_microservice_path
 from dev_gpt.utils.string_tools import print_colored
 
 
 @dataclass
 class TaskSpecification:
     task: Optional[Text]
     test: Optional[Text]
 
 
 class Generator:
     def __init__(self, task_description, path, model='gpt-4'):
-        self.gpt_session = gpt.GPTSession(task_description, model=model)
+        self.gpt_session = gpt.GPTSession(model=model)
         self.microservice_specification = TaskSpecification(task=task_description, test=None)
         self.microservice_root_path = path
 
     @staticmethod
     def extract_content_from_result(plain_text, file_name, match_single_block=False, can_contain_code_block=True):
         optional_line_break = '\n' if can_contain_code_block else ''  # the \n at the end makes sure that ``` within the generated code is not matched because it is not right before a line break
         pattern = fr"(?:\*|\*\*| ){file_name}\*?\*?\n```(?:\w+\n)?([\s\S]*?){optional_line_break}```"
@@ -125,15 +122,15 @@
             template.format(
                 **template_kwargs
             )
         )
         content = parse_result_fn(content_raw)
         if content == {}:
             content_raw = conversation.chat(
-                'You must add the content' + (f' for {file_name_s[0]}' if len(file_name_s) == 1 else ''))
+                'You must add the content in the format shown above' + (f' for {file_name_s[0]}' if len(file_name_s) == 1 else ''))
             content = parse_result_fn(content_raw)
         for _file_name, _file_content in content.items():
             persist_file(_file_content, os.path.join(destination_folder, _file_name))
         return content
 
     def generate_microservice(
             self,
@@ -371,17 +368,14 @@
                     all_files_string=self.files_to_string(
                         {key: val for key, val in file_name_to_content.items() if key != EXECUTOR_FILE_NAME}),
                 )
 
     class MaxDebugTimeReachedException(BaseException):
         pass
 
-    class TaskRefinementException(BaseException):
-        pass
-
     def is_dependency_issue(self, summarized_error, dock_req_string: str, package_manager: str):
         # a few heuristics to quickly jump ahead
         if any([error_message in summarized_error for error_message in
                 ['AttributeError', 'NameError', 'AssertionError']]):
             return False
         if package_manager.lower() == 'pip' and any(
                 [em in summarized_error for em in ['ModuleNotFoundError', 'ImportError']]):
@@ -418,19 +412,21 @@
             description=self.microservice_specification.task
         )['strategies.json']
         packages_list = [[pkg.strip().lower() for pkg in packages] for packages in json.loads(packages_json_string)]
         packages_list = [[self.replace_with_gpt_3_5_turbo_if_possible(pkg) for pkg in packages] for packages in
                          packages_list]
 
         packages_list = self.filter_packages_list(packages_list)
+        packages_list = self.remove_duplicates_from_packages_list(packages_list)
         packages_list = packages_list[:NUM_IMPLEMENTATION_STRATEGIES]
         return packages_list
-
+    # '/private/var/folders/f5/whmffl4d7q79s29jpyb6719m0000gn/T/pytest-of-florianhonicke/pytest-128/test_generation_level_0_mock_i0'
+    # '/private/var/folders/f5/whmffl4d7q79s29jpyb6719m0000gn/T/pytest-of-florianhonicke/pytest-129/test_generation_level_0_mock_i0'
     def generate(self):
-        self.refine_specification()
+        self.microservice_specification.task, self.microservice_specification.test = PM().refine_specification(self.microservice_specification.task)
         os.makedirs(self.microservice_root_path)
         generated_name = self.generate_microservice_name(self.microservice_specification.task)
         microservice_name = f'{generated_name}{random.randint(0, 10_000_000)}'
         packages_list = self.get_possible_packages()
         for num_approach, packages in enumerate(packages_list):
             try:
                 self.generate_microservice(microservice_name, packages, num_approach)
@@ -453,112 +449,14 @@
             return 0
 
     def summarize_error(self, error):
         conversation = self.gpt_session.get_conversation()
         error_summary = conversation.chat(template_summarize_error.format(error=error))
         return error_summary
 
-    def refine_specification(self):
-        pm = get_random_employee('pm')
-        print(f'{pm.emoji}👋 Hi, I\'m {pm.name}, a PM at Jina AI. Gathering the requirements for our engineers.')
-        original_task = self.microservice_specification.task
-        while True:
-            try:
-                self.microservice_specification.test = None
-                if not original_task:
-                    self.microservice_specification.task = self.get_user_input(pm, 'What should your microservice do?')
-
-                self.refine_requirements(
-                    pm,
-                    [
-                        SystemMessage(content=system_task_introduction + system_task_iteration),
-                    ],
-                    'task',
-                    '',
-                    template_pm_task_iteration,
-                    micro_service_initial_description=f'''Microservice description:
-```
-{self.microservice_specification.task}
-```
-''',
-                )
-                self.refine_requirements(
-                    pm,
-                    [
-                        SystemMessage(content=system_task_introduction + system_test_iteration),
-                    ],
-                    'test',
-                    '''Note that the test scenario must not contain information that was already mentioned in the microservice description.
-Note that you must not ask for information that were already mentioned before.''',
-                    template_pm_test_iteration,
-                    micro_service_initial_description=f'''Microservice original description: 
-```
-{original_task}
-```
-Microservice refined description: 
-```
-{self.microservice_specification.task}
-```
-''',
-                )
-                break
-            except self.TaskRefinementException as e:
-
-                print_colored('', f'{pm.emoji} Could not refine your requirements. Please try again...', 'red')
-
-        print(f'''
-{pm.emoji} 👍 Great, I will handover the following requirements to our engineers:
-Description of the microservice:
-{self.microservice_specification.task}
-Test scenario:
-{self.microservice_specification.test}
-''')
-
-    def refine_requirements(self, pm, messages, refinement_type, custom_suffix, template_pm_iteration,
-                            micro_service_initial_description=None):
-        user_input = self.microservice_specification.task
-        num_parsing_tries = 0
-        while True:
-            conversation = self.gpt_session.get_conversation(messages,
-                                                             print_stream=os.environ['VERBOSE'].lower() == 'true',
-                                                             print_costs=False)
-            agent_response_raw = conversation.chat(
-                template_pm_iteration.format(
-                    custom_suffix=custom_suffix,
-                    micro_service_initial_description=micro_service_initial_description if len(messages) == 1 else '',
-                ),
-                role='user'
-            )
-            messages.append(HumanMessage(content=user_input))
-            agent_question = self.extract_content_from_result(agent_response_raw, 'prompt.json',
-                                                              can_contain_code_block=False)
-            final = self.extract_content_from_result(agent_response_raw, 'final.json', can_contain_code_block=False)
-            if final:
-                messages.append(AIMessage(content=final))
-                setattr(self.microservice_specification, refinement_type, final)
-                break
-            elif agent_question:
-                question_parsed = json.loads(agent_question)['question']
-                messages.append(AIMessage(content=question_parsed))
-                user_input = self.get_user_input(pm, question_parsed)
-            else:
-                if num_parsing_tries > 2:
-                    raise self.TaskRefinementException()
-                num_parsing_tries += 1
-                messages.append(AIMessage(content=agent_response_raw))
-                messages.append(
-                    SystemMessage(content='You did not put your answer into the right format using *** and ```.'))
-
-    @staticmethod
-    def get_user_input(employee, prompt_to_user):
-        val = input(f'{employee.emoji}❓ {prompt_to_user}\nyou: ')
-        print()
-        while not val:
-            val = input('you: ')
-        return val
 
     @staticmethod
     def replace_with_gpt_3_5_turbo_if_possible(pkg):
         if pkg in LANGUAGE_PACKAGES:
             return 'gpt_3_5_turbo'
         return pkg
 
@@ -579,7 +477,24 @@
                    and (  # all packages must be on pypi or it is gpt_3_5_turbo
                            is_package_on_pypi(package)
                            or package == 'gpt_3_5_turbo'
                    )
             ] for packages in packages_list
         ]
         return packages_list
+
+    @staticmethod
+    def remove_duplicates_from_packages_list(packages_list):
+        return [list(set(packages)) for packages in packages_list]
+
+#     def create_prototype_implementation(self):
+#         microservice_py_lines = ['''\
+# Class {microservice_name}:''']
+#         for sub_task in self.pm.iterate_over_sub_tasks_pydantic(self.sub_task_tree):
+#             microservice_py_lines.append(f'    {sub_task.python_fn_signature}')
+#             microservice_py_lines.append(f'        """')
+#             microservice_py_lines.append(f'        {sub_task.python_fn_docstring}')
+#             microservice_py_lines.append(f'        """')
+#             microservice_py_lines.append(f'        raise NotImplementedError')
+#         microservice_py_str = '\n'.join(microservice_py_lines)
+#         persist_file(os.path.join(self.microservice_root_path, 'microservice.py'), microservice_py_str)
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/custom_gateway.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/custom_gateway.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/gateway/nginx.conf` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/gateway/nginx.conf`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/static_files/microservice/apis.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/static_files/microservice/apis.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_system.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/templates_system.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/templates_user.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/templates_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 gpt_3_5_turbo = GPT_3_5_Turbo(
     system=\'\'\'
 You are a tv-reporter who is specialized in C-list celebrities.
 When you get asked something like 'Who was having a date with <X>?', then you answer with a json like '{{"dates": ["<Y>", "<Z>"]}}'. 
 You must not answer something else - only the json.
 \'\'\')
 
-response_string = gpt(prompt)  # fill-in the prompt (str); the output is a string
+generated_string = gpt(prompt)  # fill-in the prompt (str); the output is a string
 ```
 """
 
 
 template_generate_function = PromptTemplate.from_template(
     general_guidelines_string + '''
 
@@ -285,14 +285,15 @@
 The output is:
 **apt-get-packages.json**
 ```json
 {{"packages": [libgl1-mesa-glx]}}
 ```
 Note that you must not output the content of any other files like the Dockerfile or requirements.txt. 
 Only output the apt-get-packages.json file.
+Note that the first line you output must be: **apt-get-packages.json**
 '''
 )
 
 
 template_solve_code_issue = PromptTemplate.from_template(
     '''General rules:
 ''' + not_allowed_function_string + '''
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/options/generate/ui.py` & `dev-gpt-0.18.37.dev78/dev_gpt/options/generate/ui.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/utils/io.py` & `dev-gpt-0.18.37.dev78/dev_gpt/utils/io.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt/utils/string_tools.py` & `dev-gpt-0.18.37.dev78/dev_gpt/utils/string_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import platform
+import string
 
 if platform.system() == "Windows":
     os.system("color")
 
 def print_colored(headline, text, color_code, end='\n'):
     if color_code == 'black':
         color_code = '30'
@@ -23,7 +24,19 @@
         color_code = '37'
     color_start = f"\033[{color_code}m"
     reset = "\033[0m"
     bold_start = "\033[1m"
     if headline:
         print(f"{bold_start}{color_start}{headline}{reset}")
     print(f"{color_start}{text}{reset}", end=end)
+
+
+def get_template_parameters(formatted_string):
+    formatter = string.Formatter()
+    parsed = formatter.parse(formatted_string)
+    parameters = []
+
+    for literal_text, field_name, format_spec, conversion in parsed:
+        if field_name is not None:
+            parameters.append(field_name)
+
+    return parameters
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt.egg-info/PKG-INFO` & `dev-gpt-0.18.37.dev78/dev_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-gpt
-Version: 0.18.37.dev52
+Version: 0.18.37.dev78
 Summary: Use natural language interface to generate, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/dev-gpt
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev52 Summary: Use natural
+Metadata-Version: 2.1 Name: dev-gpt Version: 0.18.37.dev78 Summary: Use natural
 language interface to generate, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/dev-gpt Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dev-gpt-0.18.37.dev52/dev_gpt.egg-info/SOURCES.txt` & `dev-gpt-0.18.37.dev78/dev_gpt.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -21,17 +21,29 @@
 dev_gpt/options/__init__.py
 dev_gpt/options/configure/__init__.py
 dev_gpt/options/configure/key_handling.py
 dev_gpt/options/deploy/__init__.py
 dev_gpt/options/deploy/deployer.py
 dev_gpt/options/generate/__init__.py
 dev_gpt/options/generate/generator.py
+dev_gpt/options/generate/parser.py
+dev_gpt/options/generate/prompt_factory.py
 dev_gpt/options/generate/templates_system.py
 dev_gpt/options/generate/templates_user.py
 dev_gpt/options/generate/ui.py
+dev_gpt/options/generate/chains/__init__.py
+dev_gpt/options/generate/chains/auto_refine_description.py
+dev_gpt/options/generate/chains/extract_information.py
+dev_gpt/options/generate/chains/get_user_input_if_needed.py
+dev_gpt/options/generate/chains/question_answering.py
+dev_gpt/options/generate/chains/translation.py
+dev_gpt/options/generate/chains/user_confirmation_feedback_loop.py
+dev_gpt/options/generate/pm/__init__.py
+dev_gpt/options/generate/pm/pm.py
+dev_gpt/options/generate/pm/task_tree_schema.py
 dev_gpt/options/generate/static_files/base_image/Dockerfile
 dev_gpt/options/generate/static_files/gateway/Dockerfile
 dev_gpt/options/generate/static_files/gateway/__init__.py
 dev_gpt/options/generate/static_files/gateway/app_config.toml
 dev_gpt/options/generate/static_files/gateway/custom_gateway.py
 dev_gpt/options/generate/static_files/gateway/nginx.conf
 dev_gpt/options/generate/static_files/gateway/requirements.txt
@@ -41,13 +53,15 @@
 dev_gpt/options/generate/static_files/microservice/jina_wrapper.py
 dev_gpt/options/run/__init__.py
 dev_gpt/options/run/runner.py
 dev_gpt/utils/__init__.py
 dev_gpt/utils/io.py
 dev_gpt/utils/string_tools.py
 test/__init__.py
+test/conftest.py
 test/integration/__init__.py
 test/integration/test_generator.py
 test/unit/__init__.py
 test/unit/test_api.py
+test/unit/test_construct_sub_task_tree.py
 test/unit/test_response_parsing.py
 test/unit/test_strings.py
```

### Comparing `dev-gpt-0.18.37.dev52/setup.py` & `dev-gpt-0.18.37.dev78/setup.py`

 * *Files identical despite different names*

### Comparing `dev-gpt-0.18.37.dev52/test/unit/test_api.py` & `dev-gpt-0.18.37.dev78/test/unit/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 def test_is_package_on_pypi():
     assert is_package_on_pypi('jina') is True
     assert is_package_on_pypi('jina', '0.9.25') is True
     assert is_package_on_pypi('jina', '10.10.10') is False
     assert is_package_on_pypi('jina-jina-jina') is False
     assert is_package_on_pypi('jina-jina-jina', '0.9.25') is False
     assert is_package_on_pypi('jina-jina-jina', '10.10.10') is False
+    assert is_package_on_pypi('io', '0.0.1') is False
 
 
 def test_filter_packages_list():
     filtered_list = Generator.filter_packages_list([
         ["gpt_3_5_turbo", "requests", "base64", "gtts", "pydub"],
         ["requests", "base64", "gtts", "pydub"],
         ["gpt_3_5_turbo", "requests", "base64", "gtts"],
@@ -43,14 +44,16 @@
 docarray==111.222.333
 # package that actually exists in that version
 gtts~=2.2.3
 # package with non-existing version
 pydub~=123.123.123
 # non-existing package with correct version
 base64~=3.3.0
+# another non-existing package
+io~=0.0.1
 # not parsable version
 pdfminer.six>=20201018,<20211018
 # existing package without version
 requests
 # another existing package without version
 streamlit
 """
```

### Comparing `dev-gpt-0.18.37.dev52/test/unit/test_response_parsing.py` & `dev-gpt-0.18.37.dev78/test/unit/test_response_parsing.py`

 * *Files identical despite different names*


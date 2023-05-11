# Comparing `tmp/metaflow-netflixext-0.1.0rc5.tar.gz` & `tmp/metaflow-netflixext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-0.1.0rc5.tar", last modified: Thu Apr 13 08:36:25 2023, max compression
+gzip compressed data, was "metaflow-netflixext-0.1.1.tar", last modified: Thu May 11 09:19:03 2023, max compression
```

## Comparing `metaflow-netflixext-0.1.0rc5.tar` & `metaflow-netflixext-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32856 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   148709 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    44143 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.594170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 08:36:25.000000 metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:36:25.598170 metaflow-netflixext-0.1.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-13 08:36:17.000000 metaflow-netflixext-0.1.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.086420 metaflow-netflixext-0.1.1/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36386 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154121 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31238 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44671 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22711 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.090420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 09:19:03.000000 metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:19:03.094420 metaflow-netflixext-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-11 09:18:51.000000 metaflow-netflixext-0.1.1/setup.py
```

### Comparing `metaflow-netflixext-0.1.0rc5/LICENSE` & `metaflow-netflixext-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/PKG-INFO` & `metaflow-netflixext-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: metaflow-netflixext
-Version: 0.1.0rc5
-Summary: EXPERIMENTAL Metaflow extensions from Netflix
-Author: Netflix Metaflow Developers
-Author-email: metaflow-dev@netflix.com
-License: Apache Software License
-Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
-Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Metaflow Experimental Extensions from Netflix
 This repository contains *non-supported* extensions for Metaflow.
 - If you are within Netflix and are looking for the Netflix version of Metaflow,
   this is *not* it.
 - If you are looking for the community supported Metaflow package, this is also *not*
   it, please see [here](https://github.com/Netflix/metaflow) for that package.
 
@@ -123,16 +100,15 @@
 - `CONDA_ENVS_DIRNAME`: same thing a `CONDA_PACKAGES_DIRNAME` but for environments
   (defaults to `envs`)
 - `CONDA_LOCAL_DIST`: if set architecture specific tar ball in `CONDA_LOCAL_DIST_DIRNAME`.
 - `CONDA_LOCAL_PATH`: if set, installs the tarball in `CONDA_LOCAL_DIST` in this path.
 - `CONDA_PREFERRED_FORMAT`: `.tar.bz2` or `.conda`. Prefer `.conda` for speed gains; any
   package not available in the preferred format will be transmuted to it automatically.
   If left empty, whatever package is found will be used (ie: there is no preference)
-- `CONDA_DEFAULT_PIP_SOURCES`: list of additional mirrors to search for packages. Useful
-  if your company has an internal mirror.
+- `CONDA_DEFAULT_PIP_SOURCE`: mirror to use for PIP.
 
 ##### Azure specific setup
 For Azure, you need to do the following two steps once during setup:
 - Manually create the blob container specified in `CONDA_AZUREROOT`
 - Grant the `Storage Blob Data Contributor` role to the storage account to the service
   principal or user accounts that will be accessing as described
   [here](https://learn.microsoft.com/en-us/azure/storage/blobs/assign-azure-role-data-access?tabs=portal#assign-an-azure-role).
@@ -229,14 +205,21 @@
   dependencies.
 - a mixed environment with a mixture of pip and conda packages (specified via
   the `conda` decorator): in this case, `conda-lock` is used to resolve the
   entire environment. `conda-lock` uses a two phased approach to resolving, first
   resolving the conda environment and then using `poetry` to resolve the additional
   `pip` packages within the confines of the defined `conda` environment.
 
+Note that to support a bit more flexibility, you can have a pure Pip environment
+as well as non-Python conda packages. This is similar to the mixed environment
+but, in some cases, pip is more flexible than conda-lock in requirement specification
+(for example, pip supports GIT repositories) so it makes it possible to gain the
+flexibility of installing non python packages in your environment and still use
+pip to resolve your python dependencies.
+
 #### Additional command-line tool
 An additional `environment` command-line tool is available invoked as follows:
 `python myflow.py --environment=conda environment --help`.
 It provides the following two sub-commands:
 - `resolve`: will resolve one or more steps without executing the flow.
 - `show`: will show information about the environments for the flow (whether they exist,
   need to be resolved, etc.)
@@ -246,14 +229,41 @@
 - `create`: locally creates/instantiates an environment
 - `resolve`: resolves an environment using either a requirements.txt file (for pip only
   environments) or an environment.yml file (for conda or mixed environments)
 - `show`: shows information about an environment (packages, etc)
 - `alias`: aliases an environment giving it a name so it can be used later
 - `get`: fetches an environment from the remote environment store locally
 
+#### Supported format for requirements.txt
+
+The requirements.txt file, which can be used to specify a pip only environment, supports
+the following syntax (a subset of the full syntax supported by pip):
+- Comment lines starting with '#'
+- `--extra-index-url`: to spcify an additional repository to look at. Note that to
+  specify the `--index-url`, set it with the `METAFLOW_CONDA_DEFAULT_PIP_SOURCE
+  environment variable.
+- `-f`, `--find-links` and `--trusted-host`: passed directly to pip with the
+  corresponding argument
+- `--pre`, `--no-index`: passed directly to pip
+- `--conda-pkg`: extension allowing you to specify a conda package that does not
+  need Python
+- a requirement specification. This can include GIT repositories or local directories
+  as well as more classic package specification. Constraints and environment
+  markers are not supported.
+
+Note that GIT repositories, local directories and non wheel packages are not
+compatible with cross-architecture resolution. Metaflow will build the wheel on the fly
+when resolving the environment and this is only possible if the same architecture is used.
+
+If possible, it is best to specify pre-built packages.
+
+#### Supported format for environment.yml
+
+The environment.yml format is the same as the one for conda-lock.
+
 #### Named environments
 Environments can optionally be given aliases.
 
 Implicitly, the pathspec to a step that executed with a given Conda environment is
 an alias for that environment and you can refer to it using that pathspec. For
 example, if step `start` in run 456 of `MyFlow` executed within a certain
 environment, that environment can be referred to as `MyFlow/456/start`.
```

### Comparing `metaflow-netflixext-0.1.0rc5/README.md` & `metaflow-netflixext-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: metaflow-netflixext
+Version: 0.1.1
+Summary: EXPERIMENTAL Metaflow extensions from Netflix
+Author: Netflix Metaflow Developers
+Author-email: metaflow-dev@netflix.com
+License: Apache Software License
+Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
+Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Metaflow Experimental Extensions from Netflix
 This repository contains *non-supported* extensions for Metaflow.
 - If you are within Netflix and are looking for the Netflix version of Metaflow,
   this is *not* it.
 - If you are looking for the community supported Metaflow package, this is also *not*
   it, please see [here](https://github.com/Netflix/metaflow) for that package.
 
@@ -100,16 +123,15 @@
 - `CONDA_ENVS_DIRNAME`: same thing a `CONDA_PACKAGES_DIRNAME` but for environments
   (defaults to `envs`)
 - `CONDA_LOCAL_DIST`: if set architecture specific tar ball in `CONDA_LOCAL_DIST_DIRNAME`.
 - `CONDA_LOCAL_PATH`: if set, installs the tarball in `CONDA_LOCAL_DIST` in this path.
 - `CONDA_PREFERRED_FORMAT`: `.tar.bz2` or `.conda`. Prefer `.conda` for speed gains; any
   package not available in the preferred format will be transmuted to it automatically.
   If left empty, whatever package is found will be used (ie: there is no preference)
-- `CONDA_DEFAULT_PIP_SOURCES`: list of additional mirrors to search for packages. Useful
-  if your company has an internal mirror.
+- `CONDA_DEFAULT_PIP_SOURCE`: mirror to use for PIP.
 
 ##### Azure specific setup
 For Azure, you need to do the following two steps once during setup:
 - Manually create the blob container specified in `CONDA_AZUREROOT`
 - Grant the `Storage Blob Data Contributor` role to the storage account to the service
   principal or user accounts that will be accessing as described
   [here](https://learn.microsoft.com/en-us/azure/storage/blobs/assign-azure-role-data-access?tabs=portal#assign-an-azure-role).
@@ -206,14 +228,21 @@
   dependencies.
 - a mixed environment with a mixture of pip and conda packages (specified via
   the `conda` decorator): in this case, `conda-lock` is used to resolve the
   entire environment. `conda-lock` uses a two phased approach to resolving, first
   resolving the conda environment and then using `poetry` to resolve the additional
   `pip` packages within the confines of the defined `conda` environment.
 
+Note that to support a bit more flexibility, you can have a pure Pip environment
+as well as non-Python conda packages. This is similar to the mixed environment
+but, in some cases, pip is more flexible than conda-lock in requirement specification
+(for example, pip supports GIT repositories) so it makes it possible to gain the
+flexibility of installing non python packages in your environment and still use
+pip to resolve your python dependencies.
+
 #### Additional command-line tool
 An additional `environment` command-line tool is available invoked as follows:
 `python myflow.py --environment=conda environment --help`.
 It provides the following two sub-commands:
 - `resolve`: will resolve one or more steps without executing the flow.
 - `show`: will show information about the environments for the flow (whether they exist,
   need to be resolved, etc.)
@@ -223,14 +252,41 @@
 - `create`: locally creates/instantiates an environment
 - `resolve`: resolves an environment using either a requirements.txt file (for pip only
   environments) or an environment.yml file (for conda or mixed environments)
 - `show`: shows information about an environment (packages, etc)
 - `alias`: aliases an environment giving it a name so it can be used later
 - `get`: fetches an environment from the remote environment store locally
 
+#### Supported format for requirements.txt
+
+The requirements.txt file, which can be used to specify a pip only environment, supports
+the following syntax (a subset of the full syntax supported by pip):
+- Comment lines starting with '#'
+- `--extra-index-url`: to spcify an additional repository to look at. Note that to
+  specify the `--index-url`, set it with the `METAFLOW_CONDA_DEFAULT_PIP_SOURCE
+  environment variable.
+- `-f`, `--find-links` and `--trusted-host`: passed directly to pip with the
+  corresponding argument
+- `--pre`, `--no-index`: passed directly to pip
+- `--conda-pkg`: extension allowing you to specify a conda package that does not
+  need Python
+- a requirement specification. This can include GIT repositories or local directories
+  as well as more classic package specification. Constraints and environment
+  markers are not supported.
+
+Note that GIT repositories, local directories and non wheel packages are not
+compatible with cross-architecture resolution. Metaflow will build the wheel on the fly
+when resolving the environment and this is only possible if the same architecture is used.
+
+If possible, it is best to specify pre-built packages.
+
+#### Supported format for environment.yml
+
+The environment.yml format is the same as the one for conda-lock.
+
 #### Named environments
 Environments can optionally be given aliases.
 
 Implicitly, the pathspec to a step that executed with a given Conda environment is
 an alias for that environment and you can refer to it using that pathspec. For
 example, if step `start` in run 456 of `MyFlow` executed within a certain
 environment, that environment can be referred to as `MyFlow/456/start`.
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 import platform
+import re
 import shutil
 import subprocess
 import tempfile
 import time
 
 from functools import wraps
 from itertools import chain
@@ -44,14 +45,17 @@
 )
 
 from .utils import (
     download_mf_version,
 )
 
 
+REQ_SPLIT_LINE = re.compile(r"([^~<=>]*)([~<=>]+.*)?")
+
+
 class CommandObj:
     def __init__(self):
         pass
 
 
 def env_spec_options(func):
     @click.option(
@@ -289,32 +293,68 @@
             "Environment '%s' does not exist for this architecture" % (env_name)
         )
 
     if install_notebook:
         start = time.time()
         # We need to install ipykernel into the resolved environment
         obj.echo("    Resolving an environment compatible with Jupyter ...", nl=False)
-        # We don't pin to avoid issues with python versions -- it will take the
-        # best one it can.
-        env = cast(Conda, obj.conda).add_to_resolved_env(
+
+        # We use envsresolver to properly deal with builder environments and what not
+        ipy_env_id, ipy_sources, ipy_deps, _, _ = cast(
+            Conda, obj.conda
+        ).info_for_add_to_resolved_env(
             env,
             using_steps=["ipykernel"],
             deps=[
                 TStr(
                     category="pip" if env.env_type == EnvType.PIP_ONLY else "conda",
                     value="ipykernel",
                 )
             ],
             sources=[],
+            extras=[],
             architecture=arch_id(),
         )
-        # Cache this information for the next time around
-        cast(Conda, obj.conda).cache_environments([env])
-        cast(Conda, obj.conda).add_environments([env])
-        cast(Conda, obj.conda).set_default_environment(env.env_id)
+        resolver = EnvsResolver(obj.conda)
+        resolver.add_environment(
+            ipy_env_id, deps=ipy_deps, sources=ipy_sources, extras=[], base_env=env
+        )
+        resolver.resolve_environments(obj.echo)
+        update_envs = []  # type: List[ResolvedEnvironment]
+        if obj.datastore_type != "local":
+            # We may need to update caches
+            # Note that it is possible that something we needed to resolve, we don't need
+            # to cache (if we resolved to something already cached).
+            formats = set()  # type: Set[str]
+            for _, resolved_env, f, _ in resolver.need_caching_environments(
+                include_builder_envs=True
+            ):
+                update_envs.append(resolved_env)
+                formats.update(f)
+
+            cast(Conda, obj.conda).cache_environments(
+                update_envs, {"conda": list(formats)}
+            )
+        else:
+            update_envs = [
+                resolved_env
+                for _, resolved_env, _ in resolver.new_environments(
+                    include_builder_envs=True
+                )
+            ]
+        cast(Conda, obj.conda).add_environments(update_envs)
+
+        # Update the default environment
+        for env_id, resolved_env, _ in resolver.all_environments(
+            include_builder_envs=True
+        ):
+            obj.conda.set_default_environment(resolved_env.env_id)
+
+        cast(Conda, obj.conda).write_out_environments()
+
         delta_time = int(time.time() - start)
         obj.echo(" done in %d second%s." % (delta_time, plural_marker(delta_time)))
 
     name = name or "metaflowtmp_%s_%s" % (env.env_id.req_id, env.env_id.full_id)
 
     existing_env = obj.conda.created_environment(name)
     if existing_env:
@@ -466,30 +506,31 @@
             "--python",
             "Cannot specify a Python version if using --using-pathspec or --using",
         )
     resolver = EnvsResolver(obj.conda)
 
     new_conda_deps = {}  # type: Dict[str, str]
     new_pip_deps = {}  # type: Dict[str, str]
+    new_np_conda_deps = {}  # type: Dict[str, str]
     new_sources = []  # type: List[TStr]
     new_extras = []  # type: List[TStr]
 
     using_str = None  # type: Optional[str]
     if using:
         using_str = using
     if using_pathspec:
         using_str = "step:%s" % using_pathspec
 
     archs = list(arch) if arch else [arch_id()]
     base_env_id = None
     base_env_conda_deps = {}  # type: Dict[str, str]
+    base_env_np_conda_deps = {}  # type: Dict[str, str]
     base_env_pip_deps = {}  # type: Dict[str, str]
-    base_env_conda_channels = []  # type: List[str]
-    base_env_pip_sources = []  # type: List[str]
     base_env_extras = []  # type: List[TStr]
+    base_env_sources = []  # type: List[TStr]
     base_env_python = python
     base_env = None  # type: Optional[ResolvedEnvironment]
     if using_str:
         base_env_id = cast(Conda, obj.conda).env_id_from_alias(using_str, local_only)
         if base_env_id is None:
             raise CommandException("No known environment for '%s'" % using_str)
 
@@ -518,57 +559,57 @@
                 base_env_pip_deps[vals[0]] = vals[1]
             elif d.category == "conda":
                 if vals[0] == "python":
                     base_env_python = vals[1]
                 else:
                     # We will re-add python later
                     base_env_conda_deps[vals[0]] = vals[1]
+            elif d.category == "npconda":
+                base_env_np_conda_deps[vals[0]] = vals[1]
 
         # Now of channels/sources
-        all_sources = base_env.sources
-        base_env_conda_channels.extend(
-            [s.value for s in all_sources if s.category == "conda"]
-        )
-        base_env_pip_sources.extend(
-            [s.value for s in all_sources if s.category == "pip"]
-        )
+        base_env_sources = base_env.sources
 
         # Finally the extras
         base_env_extras = base_env.extras
 
     # Parse yaml first to put conda sources first to be consistent with step decorator
     if yml_file:
         _parse_yml_file(yml_file, new_extras, new_sources, new_conda_deps, new_pip_deps)
     if req_file:
-        _parse_req_file(req_file, new_extras, new_sources, new_pip_deps)
+        _parse_req_file(
+            req_file, new_extras, new_sources, new_pip_deps, new_np_conda_deps
+        )
 
     if base_env_python is None:
         base_env_python = platform.python_version()
 
     # Compute the deps
     if len(new_conda_deps) == 0 and (
         not base_env or base_env.env_type == EnvType.PIP_ONLY
     ):
         # Assume a pip environment for base deps
-        pip_deps = get_pinned_conda_libs(base_env_python, obj.datastore_type)
+        pip_deps = dict(get_pinned_conda_libs(base_env_python, obj.datastore_type))
         conda_deps = {}
     else:
-        conda_deps = get_pinned_conda_libs(base_env_python, obj.datastore_type)
+        conda_deps = dict(get_pinned_conda_libs(base_env_python, obj.datastore_type))
         pip_deps = {}
 
     pip_deps.update(base_env_pip_deps)
     pip_deps.update(new_pip_deps)
 
     conda_deps.update(base_env_conda_deps)
     conda_deps.update(new_conda_deps)
+    np_conda_deps = dict(base_env_np_conda_deps)
+    np_conda_deps.update(new_np_conda_deps)
 
     # Compute the sources
-    seen = set()
-    sources = []  # type: List[str]
-    for c in chain(base_env_conda_channels, base_env_pip_sources, new_sources):
+    seen = set()  # ttype: List[TStr]
+    sources = []  # type: List[TStr]
+    for c in chain(base_env_sources, new_sources):
         if c in seen:
             continue
         seen.add(c)
         sources.append(c)
 
     deps = list(
         chain(
@@ -577,14 +618,18 @@
                 TStr("conda", "%s==%s" % (name, ver) if ver else name)
                 for name, ver in conda_deps.items()
             ),
             (
                 TStr("pip", "%s==%s" % (name, ver) if ver else name)
                 for name, ver in pip_deps.items()
             ),
+            (
+                TStr("npconda", "%s==%s" % (name, ver) if ver else name)
+                for name, ver in np_conda_deps.items()
+            ),
         )
     )
 
     extras = base_env_extras + new_extras
 
     requested_req_id = ResolvedEnvironment.get_req_id(deps, sources, extras)
 
@@ -605,29 +650,34 @@
                 )
         resolver.add_environment(
             EnvID(requested_req_id, "_default", cur_arch),
             deps,
             sources,
             extras,
             base_env,
+            clean_base=(not new_extras)
+            and (not new_sources)
+            and (not new_np_conda_deps)
+            and (not new_conda_deps)
+            and (not new_pip_deps),
             local_only=local_only,
             force=force,
             force_co_resolve=len(archs) > 1,
         )
 
     has_something = False
     for _ in resolver.non_resolved_environments():
         has_something = True
         break
     if not has_something:
         # Nothing to do
         if alias and not dry_run:
             # We don't care about arch for aliasing so pick one
             obj.echo(
-                "Not environments to resolve, aliasing only. Use --force to force "
+                "No environments to resolve, aliasing only. Use --force to force "
                 "re-resolution"
             )
             obj.conda.alias_environment(
                 EnvID(
                     requested_req_id,
                     next(resolver.all_environments())[1].env_id.full_id,
                     arch=arch_id(),
@@ -668,29 +718,36 @@
     # information
     update_envs = []  # type: List[ResolvedEnvironment]
     if obj.datastore_type != "local":
         # We may need to update caches
         # Note that it is possible that something we needed to resolve, we don't need
         # to cache (if we resolved to something already cached).
         formats = set()  # type: Set[str]
-        for _, resolved_env, f, _ in resolver.need_caching_environments():
+        for _, resolved_env, f, _ in resolver.need_caching_environments(
+            include_builder_envs=True
+        ):
             update_envs.append(resolved_env)
             formats.update(f)
 
         cast(Conda, obj.conda).cache_environments(update_envs, {"conda": list(formats)})
     else:
         update_envs = [
-            resolved_env for _, resolved_env, _ in resolver.new_environments()
+            resolved_env
+            for _, resolved_env, _ in resolver.new_environments(
+                include_builder_envs=True
+            )
         ]
 
     cast(Conda, obj.conda).add_environments(update_envs)
 
     # Update the default environment
     if set_default:
-        for env_id, resolved_env, _ in resolver.all_environments():
+        for env_id, resolved_env, _ in resolver.all_environments(
+            include_builder_envs=True
+        ):
             obj.conda.set_default_environment(resolved_env.env_id)
 
     # We are done -- write back out the environments
     cast(Conda, obj.conda).write_out_environments()
 
 
 @environment.command(help="Show information about an environment")
@@ -702,26 +759,35 @@
 )
 @click.option(
     "--arch",
     show_default=True,
     default=arch_id(),
     help="Show environment for this architecture",
 )
+@click.option(
+    "--pathspec",
+    default=False,
+    is_flag=True,
+    show_default=True,
+    help="The environments given are pathspecs",
+)
 @click.argument("envs", required=True, nargs=-1)
 @click.pass_obj
-def show(obj, local_only: bool, arch: str, envs: Tuple[str]):
+def show(obj, local_only: bool, arch: str, pathspec: bool, envs: Tuple[str]):
     # req-id -> full-id -> List of paths
     all_envs = {}  # Dict[str, Dict[str, List[str]]]
     created_envs = cast(Conda, obj.conda).created_environments()
     for env_id, present_list in created_envs.items():
         all_envs.setdefault(env_id.req_id, {})[env_id.full_id] = [
             os.path.basename(p) for p in present_list
         ]
 
     for env_name in envs:
+        if pathspec:
+            env_name = "step:%s" % env_name
         resolved_env = cast(Conda, obj.conda).environment_from_alias(
             env_name, arch, local_only
         )
         if resolved_env is None:
             if obj.quiet:
                 obj.echo_always("%s@%s" % (env_name, arch))
                 obj.echo_always("NOT_FOUND")
@@ -755,19 +821,27 @@
 @environment.command(help="Alias an existing environment")
 @click.option(
     "--local-only/--non-local",
     show_default=True,
     default=False,
     help="Only resolve source env using local information",
 )
+@click.option(
+    "--pathspec",
+    default=False,
+    is_flag=True,
+    show_default=True,
+    help="The source environment given is a pathspec",
+)
 @click.argument("source_env")
 @click.argument("alias")
 @click.pass_obj
-def alias(obj, local_only: bool, source_env: str, alias: str):
-
+def alias(obj, local_only: bool, pathspec: bool, source_env: str, alias: str):
+    if pathspec:
+        source_env = "step:%s" % source_env
     env_id_for_alias = cast(Conda, obj.conda).env_id_from_alias(source_env, local_only)
     if env_id_for_alias is None:
         raise CommandException(
             "Environment '%s' does not refer to a known environment" % source_env
         )
     cast(Conda, obj.conda).alias_environment(env_id_for_alias, [alias])
     cast(Conda, obj.conda).write_out_environments()
@@ -784,17 +858,26 @@
 )
 @click.option(
     "--arch",
     default=None,
     show_default=True,
     help="Request this architecture -- defaults to current architecture if not specified",
 )
+@click.option(
+    "--pathspec",
+    default=False,
+    is_flag=True,
+    show_default=True,
+    help="The environment name given is a pathspec",
+)
 @click.argument("source_env")
 @click.pass_obj
-def get(obj, default: bool, arch: Optional[str], source_env: str):
+def get(obj, default: bool, arch: Optional[str], pathspec: bool, source_env: str):
+    if pathspec:
+        source_env = "step:%s" % source_env
     env = cast(Conda, obj.conda).environment_from_alias(source_env, arch)
     if env is None:
         raise CommandException(
             "Environment '%s' does not refer to a known environment for %s"
             % (source_env, arch or arch_id())
         )
     if default:
@@ -808,15 +891,19 @@
         obj.echo_always(env.quiet_print(existing_envs))
     else:
         obj.echo(env.pretty_print(existing_envs))
     cast(Conda, obj.conda).write_out_environments()
 
 
 def _parse_req_file(
-    file_name: str, extra_args: List[TStr], sources: List[TStr], deps: Dict[str, str]
+    file_name: str,
+    extra_args: List[TStr],
+    sources: List[TStr],
+    deps: Dict[str, str],
+    np_deps: Dict[str, str],
 ):
     with open(file_name, mode="r", encoding="utf-8") as f:
         for line in f:
             line = line.strip()
             if not line:
                 continue
             splits = line.split(maxsplit=1)
@@ -834,14 +921,26 @@
                 sources.append(TStr(category="pip", value=rem))
             elif first_word in ("-f", "--find-links", "--trusted-host") and rem:
                 extra_args.append(
                     TStr(category="pip", value=" ".join([first_word, rem]))
                 )
             elif first_word in ("--pre", "--no-index"):
                 extra_args.append(TStr(category="pip", value=first_word))
+            elif first_word == "--conda-pkg":
+                # Special extension to allow non-python conda package specification
+                split_res = REQ_SPLIT_LINE.match(splits[1])
+                if split_res is None:
+                    raise InvalidEnvironmentException(
+                        "Could not parse conda package '%s'" % splits[1]
+                    )
+                s = split_res.groups()
+                if s[1] is None:
+                    np_deps[s[0].replace(" ", "")] = ""
+                else:
+                    np_deps[s[0].replace(" ", "")] = s[1].replace(" ", "").lstrip("=")
             elif first_word.startswith("#"):
                 continue
             elif first_word.startswith("-"):
                 raise InvalidEnvironmentException(
                     "'%s' is not a supported line in a requirements.txt" % line
                 )
             elif (
@@ -851,19 +950,24 @@
                 or first_word.startswith("svn+")
                 or (rem and rem[0] == "@")
             ):
                 if rem and rem[0] == "@":
                     first_word = rem[1:].strip()
                 deps[first_word] = ""
             else:
-                splits = line.split("=", 1)
-                if len(splits) == 1:
-                    deps[line.strip()] = ""
+                split_res = REQ_SPLIT_LINE.match(line)
+                if split_res is None:
+                    raise InvalidEnvironmentException("Could not parse '%s'" % line)
+                splits = split_res.groups()
+                if splits[1] is None:
+                    deps[splits[0].replace(" ", "")] = ""
                 else:
-                    deps[splits[0].strip()] = splits[1].lstrip(" =").rstrip()
+                    deps[splits[0].replace(" ", "")] = (
+                        splits[1].replace(" ", "").lstrip("=")
+                    )
 
 
 def _parse_yml_file(
     file_name: str,
     _: List[TStr],
     sources: List[TStr],
     conda_deps: Dict[str, str],
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: strict, reportTypeCommentUsage=false, reportMissingTypeStubs=false
 
 import errno
 import json
 import os
 import platform
+import re
 import requests
 import shutil
 import socket
 import stat
 import subprocess
 import sys
 import tarfile
@@ -185,22 +186,35 @@
     def binary(self, binary: str) -> Optional[str]:
         if not self._found_binaries:
             self._find_conda_binary()
         if self._bins:
             return self._bins.get(binary)
         return None
 
+    @staticmethod
+    def env_type_for_deps(deps: Sequence[TStr]) -> EnvType:
+        conda_packages = [d for d in deps if d.category == "conda"]
+        pip_packages = [d for d in deps if d.category == "pip"]
+        env_type = EnvType.CONDA_ONLY
+        if len(conda_packages) == 1:
+            # This is a pip only mode
+            env_type = EnvType.PIP_ONLY
+        elif len(pip_packages) > 0:
+            env_type = EnvType.MIXED
+        return env_type
+
     def resolve(
         self,
         using_steps: Sequence[str],
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
         env_type: Optional[EnvType] = None,
+        builder_env: Optional[ResolvedEnvironment] = None,
     ) -> ResolvedEnvironment:
         if self._mode != "local":
             # TODO: Maybe relax this later but for now assume that the remote environment
             # is a "lighter" conda.
             raise CondaException("Cannot resolve environments in a remote environment")
 
         if not self._found_binaries:
@@ -209,22 +223,15 @@
         # We determine the resolver method based on what we have to resolve. There are
         # three cases:
         #  - only conda packages (conda-only resolver)
         #  - mix of conda packages and pip packages (mixed resolver)
         #  - a single conda package (the python version) and all pip packages
         #    (conda-only for the python version and pip-only for the rest)
         if env_type is None:
-            conda_packages = [d for d in deps if d.category == "conda"]
-            pip_packages = [d for d in deps if d.category == "pip"]
-            env_type = EnvType.CONDA_ONLY
-            if len(conda_packages) == 1:
-                # This is a pip only mode
-                env_type = EnvType.PIP_ONLY
-            elif len(pip_packages) > 0:
-                env_type = EnvType.MIXED
+            env_type = self.env_type_for_deps(deps)
         debug.conda_exec("Environment is of type %s" % env_type.value)
         # We now check we have a resolver
         resolver_bin = self._resolvers[env_type]
         if resolver_bin is None:
             raise InvalidEnvironmentException(
                 "Cannot resolve environments in %s mode because no resolver is configured"
                 % env_type.value
@@ -252,25 +259,94 @@
                     # Should never happen and be caught earlier but being clean
                     # add other mixed resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
                     )
             else:
                 # Pip only mode
-                packages = self._resolve_env_with_conda(deps, sources, architecture)
-                conda_only_deps = [d for d in deps if d.category == "conda"]
-                conda_only_sources = [s for s in sources if s.category == "conda"]
-                builder_resolved_env = ResolvedEnvironment(
-                    conda_only_deps,
-                    conda_only_sources,
-                    None,
-                    architecture,
-                    all_packages=packages,
-                    env_type=EnvType.CONDA_ONLY,
-                )
+                # In this mode, we also allow (as a workaround for poor support for
+                # more advanced options in conda-lock (like git repo, local support,
+                # etc)) the inclusion of conda packages that are *not* python packages.
+                # To ensure this, we check the npconda packages, create an environment
+                # for it and check if that environment doesn't contain python deps.
+                # If that is the case, we then create the actual environment including
+                # both conda and npconda packages and re-resolve. We could maybe
+                # optimize to not resolve from scratch twice but given this is a rare
+                # situation and the cost is only during resolution, it doesn't seem
+                # worth it.
+                npconda_deps = [d for d in deps if d.category == "npconda"]
+                if npconda_deps:
+                    npconda_pkgs = self._resolve_env_with_conda(
+                        npconda_deps, sources, architecture
+                    )
+                    if any((p.filename.startswith("python-") for p in npconda_pkgs)):
+                        raise InvalidEnvironmentException(
+                            "Cannot specify a non-python Conda dependency that uses "
+                            "python: %s. Please use the mixed mode instead."
+                            % ", ".join([d.value for d in npconda_deps])
+                        )
+
+                # We have two cases here with the builder envs because we actually
+                # need up to two builder environments:
+                #  - arch_id() == architecture:
+                #    - in this case, we can use the builder_env passed in if it exists
+                #      for both the environment to build PIP packages in and the
+                #      environment to resolve the PIP environment in
+                #  - arch_id() != architecture:
+                #    - in this case, we can use the builder_env passed in, if it
+                #      exists ONLY to resolve the PIP environment (the passed in
+                #      environment is always of arch arch_id()). We cannot, in this
+                #      case build PIP packages (cross arch build so we don't do that)
+                if arch_id() == architecture and builder_env:
+                    debug.conda_exec("Using builder_env passed in")
+                    packages = list(builder_env.packages)
+                else:
+                    debug.conda_exec("Building base conda env with %s" % str(deps))
+
+                    packages = self._resolve_env_with_conda(deps, sources, architecture)
+                    if arch_id() == architecture:
+                        debug.conda_exec("Using as builder env")
+                        conda_only_deps = [
+                            d for d in deps if d.category in ("conda", "npconda")
+                        ]
+                        conda_only_sources = [
+                            s for s in sources if s.category == "conda"
+                        ]
+
+                        builder_env = ResolvedEnvironment(
+                            conda_only_deps,
+                            conda_only_sources,
+                            None,
+                            architecture,
+                            all_packages=packages,
+                            env_type=EnvType.CONDA_ONLY,
+                        )
+                    elif not builder_env:
+                        python_only_dep = [
+                            d
+                            for d in deps
+                            if d.category == "conda" and d.value.startswith("python==")
+                        ]
+                        debug.conda_exec(
+                            "Building vanilla builder env with %s"
+                            % str(python_only_dep)
+                        )
+                        python_only_packages = self._resolve_env_with_conda(
+                            python_only_dep,
+                            sources,
+                            arch_id(),
+                        )
+                        builder_env = ResolvedEnvironment(
+                            python_only_dep,
+                            [s for s in sources if s.category == "conda"],
+                            None,
+                            arch_id(),
+                            all_packages=python_only_packages,
+                            env_type=EnvType.CONDA_ONLY,
+                        )
                 if resolver_bin == "pip":
                     # We need to get the python package to get the version
                     python_version = None  # type: Optional[str]
                     for p in packages:
                         if p.filename.startswith("python-"):
                             python_version = p.package_version
                             break
@@ -282,15 +358,15 @@
                     packages.extend(
                         self._resolve_env_with_pip(
                             python_version,
                             deps,
                             sources,
                             extras,
                             architecture,
-                            builder_resolved_env,
+                            builder_env,
                         )
                     )
                 else:
                     # Should also never happen and be caught earlier but being clean
                     # add other pip resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
@@ -303,25 +379,26 @@
                 architecture,
                 all_packages=packages,
                 env_type=env_type,
             )
         except CondaException as e:
             raise CondaStepException(e, using_steps)
 
-    def add_to_resolved_env(
+    def info_for_add_to_resolved_env(
         self,
         cur_env: ResolvedEnvironment,
         using_steps: Sequence[str],
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
         inputs_are_addl: bool = True,
-        cur_is_accurate: bool = True,
-    ) -> ResolvedEnvironment:
+    ) -> Tuple[EnvID, Sequence[TStr], Sequence[TStr], Sequence[TStr], Sequence[TStr]]:
+        # Computes the new information for a derived environment (built on top of cur_env)
+        # Returns the new EnvID, sources, user_deps, deps and extras
         if self._mode != "local":
             # TODO: Maybe relax this later but for now assume that the remote environment
             # is a "lighter" conda.
             raise CondaException("Cannot resolve environments in a remote environment")
 
         if not self._found_binaries:
             self._find_conda_binary()
@@ -353,42 +430,62 @@
         # We check if we already resolved this environment and bypass resolving for
         # if it we already have solved for it.
         new_env_id = EnvID(
             ResolvedEnvironment.get_req_id(user_deps, sources, extras),
             "_default",
             architecture,
         )
+
+        return new_env_id, sources, user_deps, deps, extras
+
+    def add_to_resolved_env(
+        self,
+        cur_env: ResolvedEnvironment,
+        using_steps: Sequence[str],
+        deps: Sequence[TStr],
+        sources: Sequence[TStr],
+        extras: Sequence[TStr],
+        architecture: str,
+        inputs_are_addl: bool = True,
+        cur_is_accurate: bool = True,
+        builder_env: Optional[ResolvedEnvironment] = None,
+    ) -> ResolvedEnvironment:
+        if self._mode != "local":
+            # TODO: Maybe relax this later but for now assume that the remote environment
+            # is a "lighter" conda.
+            raise CondaException("Cannot resolve environments in a remote environment")
+
+        if not self._found_binaries:
+            self._find_conda_binary()
+
+        (
+            new_env_id,
+            sources,
+            user_deps,
+            deps,
+            extras,
+        ) = self.info_for_add_to_resolved_env(
+            cur_env, using_steps, deps, sources, extras, architecture, inputs_are_addl
+        )
+
         new_resolved_env = self.environment(new_env_id)
         if new_resolved_env:
             return new_resolved_env
 
         # Figure out the env_type
         new_env_type = cur_env.env_type
-        if cur_env.env_type == EnvType.PIP_ONLY and any(
-            [d.value for d in deps if d.category == "conda"]
-        ):
-            self._echo(
-                "Upgrading an environment from %s to %s due to new Conda dependencies"
-                % (EnvType.PIP_ONLY, EnvType.MIXED)
-            )
-        elif cur_env.env_type == EnvType.CONDA_ONLY and any(
-            [d.value for d in deps if d.category == "pip"]
-        ):
-            self._echo(
-                "Upgrading an environment from %s to %s due to new Pip dependencies"
-                % (EnvType.CONDA_ONLY, EnvType.MIXED)
-            )
 
         new_resolved_env = self.resolve(
             using_steps,
             deps,
             sources,
             extras,
             architecture,
             env_type=new_env_type,
+            builder_env=builder_env,
         )
 
         # We now try to copy as much information as possible from the current environment
         # which includes information about cached packages
         cur_packages = {p.filename: p.to_dict() for p in cur_env.packages}
         merged_packages = []  # type: List[PackageSpecification]
         for p in new_resolved_env.packages:
@@ -1499,25 +1596,26 @@
                 "Could not fetch packages -- see pretty-printed errors above."
             )
 
     def _resolve_env_with_micromamba_server(
         self, deps: Sequence[TStr], channels: Sequence[TStr], architecture: str
     ) -> List[PackageSpecification]:
 
-        deps = [d for d in deps if d.category == "conda"]
+        deps = [d for d in deps if d.category in ("conda", "npconda")]
 
         if not self._have_micromamba_server:
             raise CondaException(
                 "Micromamba server not supported by installed version of micromamba"
             )
 
         self._start_micromamba_server()
         # Form the payload to send to the server
         req = {
-            "specs": [d.value for d in deps if d.category == "conda"] + ["pip"],
+            "specs": [d.value for d in deps if d.category in ("conda", "npconda")]
+            + ["pip"],
             "platform": architecture,
             "channels": [c.value for c in channels if c.category == "conda"],
         }
         if arch_id() == architecture:
             # Use the same virtual packages as the ones used for conda/mamba
             req["virtual_packages"] = [
                 "%s=%s=%s" % (pkg_name, pkg_version, pkg_id)
@@ -1556,15 +1654,15 @@
     def _resolve_env_with_conda(
         self,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         architecture: str,
     ) -> List[PackageSpecification]:
 
-        deps = [d for d in deps if d.category == "conda"]
+        deps = [d for d in deps if d.category in ("conda", "npconda")]
 
         result = []
         with tempfile.TemporaryDirectory() as mamba_dir:
             args = [
                 "create",
                 "--prefix",
                 os.path.join(mamba_dir, "prefix"),
@@ -1574,15 +1672,19 @@
             for c in sources:
                 if c.category == "conda":
                     have_channels = True
                     args.extend(["-c", c.value])
 
             if not have_channels:
                 have_channels = any(
-                    ["::" in d.value for d in deps if d.category == "conda"]
+                    [
+                        "::" in d.value
+                        for d in deps
+                        if d.category in ("conda", "npconda")
+                    ]
                 )
             if have_channels:
                 # Add no-channel-priority because otherwise if a version
                 # is present in the other channels but not in the higher
                 # priority channels, it is not found.
                 args.append("--no-channel-priority")
             args.extend([d.value for d in deps])
@@ -1677,17 +1779,35 @@
             chain.from_iterable(
                 map(
                     lambda x: x.split(maxsplit=1),
                     (e.value for e in extras if e.category == "pip"),
                 )
             )
         )
+
+        # Create the environment in which we will call pip
+        debug.conda_exec("Creating builder conda environment")
+        techo = self._echo
+        self._echo = self._no_echo
+        self.create_for_name(
+            self._env_builder_directory_from_envid(builder_env.env_id),
+            builder_env,
+        )
+        self._echo = techo
+
+        builder_python = cast(
+            str,
+            self.python(self._env_builder_directory_from_envid(builder_env.env_id)),
+        )
+
         result = []
         with tempfile.TemporaryDirectory() as pip_dir:
             args = [
+                "-m",
+                "pip",
                 "--isolated",
                 "install",
                 "--ignore-installed",
                 "--dry-run",
                 "--target",
                 pip_dir,
                 "--report",
@@ -1698,35 +1818,35 @@
                 args.extend(["-i", CONDA_DEFAULT_PIP_SOURCE])
             for c in chain(
                 (s.value for s in sources if s.category == "pip"),
             ):
                 args.extend(["--extra-index-url", c])
 
             supported_tags = pip_tags_from_arch(python_version, architecture)
-            if python_version != platform.python_version() or architecture != arch_id():
-                clean_version = ".".join(python_version.split(".")[:2])
-                args.extend(["--only-binary=:all:", "--python-version", clean_version])
 
             if architecture != arch_id():
+
                 implementations = []  # type: List[str]
                 abis = []  # type: List[str]
                 platforms = []  # type: List[str]
                 for tag in supported_tags:
                     implementations.append(tag.interpreter)
                     abis.append(tag.abi)
                     platforms.append(tag.platform)
                 implementations = [x.interpreter for x in supported_tags]
                 extra_args = (
-                    *(
-                        chain.from_iterable(
-                            product(["--implementation"], implementations)
-                        )
-                    ),
-                    *(chain.from_iterable(product(["--abi"], abis))),
-                    *(chain.from_iterable(product(["--platform"], platforms))),
+                    "--only-binary=:all:",
+                    # This seems to overly constrain things so skipping for now
+                    # *(
+                    #    chain.from_iterable(
+                    #        product(["--implementation"], set(implementations))
+                    #    )
+                    # ),
+                    *(chain.from_iterable(product(["--abi"], set(abis)))),
+                    *(chain.from_iterable(product(["--platform"], set(platforms)))),
                 )
 
                 args.extend(extra_args)
 
             # Unfortunately, pip doesn't like things like ==<= so we need to strip
             # the ==
             for d in deps:
@@ -1737,15 +1857,15 @@
                     if splits[1][0] in ("=", "<", ">"):
                         # Something originally like pkg==<=ver
                         args.append("".join(splits))
                     else:
                         # Something originally like pkg==ver
                         args.append(d.value)
 
-            self._call_binary(args, binary="pip")
+            self._call_binary(args, binary=builder_python)
 
             # We should now have a json blob in out.json
             result = []  # type: List[PackageSpecification]
             with open(
                 os.path.join(pip_dir, "out.json"), mode="r", encoding="utf-8"
             ) as f:
                 desc = json.load(f)
@@ -2027,29 +2147,14 @@
                     debug.conda_exec(
                         "Creating builder environment to build PIP packages"
                     )
 
                     target_directory = os.path.join(self._package_dirs[0], "pip")
                     os.makedirs(target_directory, exist_ok=True)
 
-                    techo = self._echo
-                    self._echo = self._no_echo
-                    self.create_for_name(
-                        self._env_builder_directory_from_envid(builder_env.env_id),
-                        builder_env,
-                    )
-                    self._echo = techo
-
-                    builder_python = cast(
-                        str,
-                        self.python(
-                            self._env_builder_directory_from_envid(builder_env.env_id)
-                        ),
-                    )
-
                     def _build_with_pip(identifier: int, key: str, url: str):
                         dest_path = os.path.join(pip_dir, "build_%d" % identifier)
                         debug.conda_exec(
                             "Building package '%s'  for '%s' in '%s'"
                             % (url, key, dest_path)
                         )
                         self._call_binary(
@@ -2125,15 +2230,15 @@
         self,
         deps: Sequence[TStr],
         channels: Sequence[TStr],
         architecture: str,
     ) -> List[PackageSpecification]:
         outfile_name = None
         my_arch = arch_id()
-        if any([d.category not in ("pip", "conda") for d in deps]):
+        if any([d.category not in ("pip", "conda", "npconda") for d in deps]):
             raise CondaException(
                 "Cannot resolve dependencies that include non-Conda/Pip dependencies: %s"
                 % "; ".join(map(str, deps))
             )
         self._start_micromamba_server()
 
         def _poetry_exec(cmd: str, *args: str):
@@ -2168,25 +2273,29 @@
                 raise CondaException(
                     "Could not manage poetry's dependency using '{cmd}' -- got error"
                     "code {code}'; see pretty-printed error above".format(
                         cmd=e.cmd, code=e.returncode
                     )
                 )
 
-        pip_channels = ([CONDA_DEFAULT_PIP_SOURCE] if CONDA_DEFAULT_PIP_SOURCE else []) + [
+        pip_channels = (
+            [CONDA_DEFAULT_PIP_SOURCE] if CONDA_DEFAULT_PIP_SOURCE else []
+        ) + [
             c.value for c in channels if c.category == "pip"
         ]  # type: List[str]
         try:
             # We resolve the environment using conda-lock
 
             # Write out the requirement yml file. It's easy enough so don't use a YAML
             # library to avoid adding another dep
 
             pip_deps = [d.value for d in deps if d.category == "pip"]
-            conda_deps = [d.value for d in deps if d.category == "conda"] + ["pip"]
+            conda_deps = [
+                d.value for d in deps if d.category in ("conda", "npconda")
+            ] + ["pip"]
             # Add channels
             lines = ["channels:\n"]
             lines.extend(
                 ["  - %s\n" % c.value for c in channels if c.category == "conda"]
             )
             for c in self._info["channels"]:
                 lines.append("  - %s\n" % c.replace(my_arch, architecture))
@@ -2868,29 +2977,39 @@
                     pip_paths.append("%s\n" % local_path)
                 else:
                     raise CondaException(
                         "Local file for package %s expected" % p.filename
                     )
             elif p.TYPE == "conda":
                 local_dir = p.local_dir
+                found_local_dir = False
                 if local_dir:
                     # If this is a local directory, we make sure we use the URL for that
                     # directory (so the conda system uses it properly)
                     debug.conda_exec(
                         "For %s, using local Conda directory at '%s'"
                         % (p.filename, local_dir)
                     )
                     with open(
                         os.path.join(local_dir, "info", "repodata_record.json"),
                         mode="r",
                         encoding="utf-8",
                     ) as f:
                         info = json.load(f)
-                        explicit_urls.append("%s#%s\n" % (info["url"], info["md5"]))
-                else:
+                        # Some packages don't have a repodata_record.json with url so
+                        # we will download again
+                        if "url" in info and "md5" in info:
+                            explicit_urls.append("%s#%s\n" % (info["url"], info["md5"]))
+                            found_local_dir = True
+                        else:
+                            debug.conda_exec(
+                                "Skipping local directory as no URL information"
+                            )
+
+                if not found_local_dir:
                     for f in CONDA_FORMATS:
                         cache_info = p.cached_version(f)
                         if cache_info:
                             debug.conda_exec(
                                 "For %s, using cached package from '%s'"
                                 % (p.filename, cache_info.url)
                             )
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
             ][0](self._flow)
 
     def init_environment(self, echo: Callable[..., None]):
         # Print a message for now
         echo("Bootstrapping Conda environment... (this could take a few minutes)")
 
         self._conda = cast(Conda, self._conda)
-
         resolver = EnvsResolver(self._conda)
 
         for step in self._flow:
             # Figure out the environments that we need to resolve for all steps
             # We will resolve all unique environments in parallel
             step_conda_dec = get_conda_decorator(self._flow, step.name)
             resolver.add_environment_for_step(step.name, step_conda_dec)
@@ -91,16 +90,16 @@
             update_envs = [
                 resolved_env for _, resolved_env, _ in resolver.new_environments()
             ]
 
         self._conda.add_environments(update_envs)
 
         # Update the default environment
-        for env_id, resolved_env, _ in resolver.resolved_environments():
-            if env_id.full_id == "_default":
+        for env_id, resolved_env, _ in resolver.all_environments():
+            if resolved_env and env_id.full_id == "_default":
                 self._conda.set_default_environment(resolved_env.env_id)
 
         # We are done -- write back out the environments.
         # TODO: Not great that this is manual
         self._conda.write_out_environments()
 
         # Delegate to whatever the base environment needs to do.
@@ -112,16 +111,17 @@
         self._local_root = cast(str, LocalStorage.get_datastore_root_from_config(echo))
         self._datastore_type = datastore_type
         self._conda = Conda(echo, datastore_type)
 
         return self.base_env.validate_environment(echo, datastore_type)
 
     def decospecs(self) -> Tuple[str, ...]:
-        # Apply conda decorator and base environment's decorators to all steps
-        return ("conda",) + self.base_env.decospecs()
+        # Apply conda and pip decorator and base environment's decorators to all steps.
+        # We will later resolve which to keep.
+        return ("conda", "pip") + self.base_env.decospecs()
 
     def _get_env_id(self, step_name: str) -> Optional[EnvID]:
         conda_decorator = get_conda_decorator(self._flow, step_name)
         if conda_decorator.is_enabled():
             resolved_env = cast(Conda, self._conda).environment(conda_decorator.env_id)
             if resolved_env:
                 return resolved_env.env_id
@@ -222,9 +222,9 @@
             }
             return new_info
         return {"type": "conda"}
 
     def get_package_commands(self, code_package_url: str, datastore_type: str):
         return self.base_env.get_package_commands(code_package_url, datastore_type)
 
-    def get_environment_info(self):
-        return self.base_env.get_environment_info()
+    def get_environment_info(self, include_ext_info=False):
+        return self.base_env.get_environment_info(include_ext_info)
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from metaflow.metaflow_environment import (
     InvalidEnvironmentException,
     MetaflowEnvironment,
 )
 from .env_descr import (
     TStr,
     EnvID,
+    EnvType,
     ResolvedEnvironment,
 )
 from metaflow.plugins.env_escape import generate_trampolines
 from metaflow.unbounded_foreach import UBF_CONTROL
 from metaflow.util import get_metaflow_root
 
 from .utils import AliasType, arch_id, resolve_env_alias
@@ -173,14 +174,18 @@
         else:
             deps = [TStr("conda", "python==%s" % self._python_version())]
         # Empty version will just be "I want this package with no version constraints"
         deps.extend(
             TStr("conda", "%s==%s" % (name, ver) if ver else name)
             for name, ver in self._conda_deps().items()
         )
+        deps.extend(
+            TStr("npconda", "%s==%s" % (name, ver) if ver else name)
+            for name, ver in self._np_conda_deps().items()
+        )
         # If we have an empty version, we consider that the name is a direct
         # link to a package like a URL
         deps.extend(
             TStr("pip", "%s==%s" % (name, ver) if ver else name)
             for name, ver in self._pip_deps().items()
         )
         return deps
@@ -216,29 +221,43 @@
             if self._from_env is None:
                 raise InvalidEnvironmentException(
                     "'%s' is a valid Conda environment but does not exist for %s"
                     % (from_alias, self._arch)
                 )
         return self._from_env
 
+    @property
+    def clean_from_env(self) -> bool:
+        if self.from_env:
+            # env_id forces the computation of all dependencies for this step which
+            # will update _clean_from_env if there is any update to the base env
+            self.env_id
+            return self._clean_from_env
+        return False
+
+    def set_conda(self, conda: Conda):
+        self.conda = conda
+
     def step_init(
         self,
         flow: FlowSpec,
         graph: FlowGraph,
         step_name: str,
-        decorators: Sequence[StepDecorator],
+        decorators: List[StepDecorator],
         environment: MetaflowEnvironment,
         flow_datastore: FlowDataStore,
         logger: Callable[..., None],
     ):
         if environment.TYPE != "conda":
             raise InvalidEnvironmentException(
                 "The *@%s* decorator requires " "--environment=conda" % self.name
             )
 
+        if not self._resolve_pip_or_conda_deco(flow, decorators):
+            return
         self._echo = logger
         self._env = environment
         self._flow = flow
         self._step_name = step_name
         self._flow_datastore_type = flow_datastore.TYPE  # type: str
         self._base_attributes = self._get_base_attributes()
 
@@ -253,18 +272,25 @@
         self.__class__._local_root = LocalStorage.get_datastore_root_from_config(
             self._echo
         )  # type: str
 
         # Information about the environment this environment is built from
         self._from_env = None  # type: Optional[ResolvedEnvironment]
         self._from_env_conda_deps = None  # type: Optional[Dict[str, str]]
+        self._from_env_np_conda_deps = None  # type: Optional[Dict[str, str]]
         self._from_env_conda_channels = None  # type: Optional[List[str]]
         self._from_env_pip_deps = None  # type: Optional[Dict[str, str]]
         self._from_env_pip_sources = None  # type: Optional[List[str]]
 
+        # This variable indicates if the environment is a pure "from" environment
+        # in which case we do not try to re-resolve. We only re-resolve if there
+        # are modifications to the environment (from either new user dependencies or
+        # potentially because Metaflow's dependencies have changed)
+        self._clean_from_env = True  # type: bool
+
         if (self.attributes["name"] or self.attributes["pathspec"]) and len(
             [
                 k
                 for k, v in self.attributes.items()
                 if v and k not in ("name", "pathspec")
             ]
         ):
@@ -293,15 +319,17 @@
             # the same way as outside conda (looking at distributions, etc). In a
             # Conda environment, as shown below (where we set self._addl_paths), all
             # EXT_PKG extensions are PYTHONPATH extensions. Instead of re-resolving,
             # we use the resolved information that is written out to the INFO file.
             with open(
                 os.path.join(self._metaflow_home, "INFO"), mode="wt", encoding="utf-8"
             ) as f:
-                f.write(json.dumps(self._env.get_environment_info()))
+                f.write(
+                    json.dumps(self._env.get_environment_info(include_ext_info=True))
+                )
 
         # Do the same for EXT_PKG
         try:
             m = importlib.import_module(EXT_PKG)
         except ImportError:
             # No additional check needed because if we are here, we already checked
             # for other issues when loading at the toplevel
@@ -430,24 +458,27 @@
                 "@conda decorator is not compatible with @pip_base decorator."
             )
         if "conda_base" in self._flow._flow_decorators:
             return self._flow._flow_decorators["conda_base"][0].attributes
         return self.defaults
 
     def _python_version(self) -> str:
-        return next(
+        s = next(
             x
             for x in [
                 self.attributes["python"],
                 self._base_attributes["python"],
                 self._from_env_python(),
                 platform.python_version(),
             ]
             if x is not None
         )
+        if self.from_env != None and s != self._from_env_python():
+            self._clean_from_env = False
+        return s
 
     def _from(self) -> Optional[str]:
         return (
             next(
                 x
                 for x in [
                     self.attributes["name"],
@@ -467,41 +498,48 @@
 
     def _compute_from_env(self):
         base = self.from_env
         if base and self._from_env_conda_deps is None:
             # We either compute all or nothing so it means we computed none
             self._from_env_conda_deps = {}
             self._from_env_pip_deps = {}
+            self._from_env_np_conda_deps = {}
             self._from_env_conda_channels = []
             self._from_env_pip_sources = []
 
             # Take care of dependencies first
             all_deps = base.deps
             for d in all_deps:
                 vals = d.value.split("==")
                 if len(vals) == 1:
                     vals.append("")
                 if d.category == "pip":
                     self._from_env_pip_deps[vals[0]] = vals[1]
                 elif d.category == "conda":
                     self._from_env_conda_deps[vals[0]] = vals[1]
+                elif d.category == "npconda":
+                    self._from_env_np_conda_deps[vals[0]] = vals[1]
 
             # Now of channels/sources
             all_sources = base.sources
             self._from_env_conda_channels = [
                 s.value for s in all_sources if s.category == "conda"
             ]
             self._from_env_pip_sources = [
                 s.value for s in all_sources if s.category == "pip"
             ]
 
     def _from_conda_deps(self) -> Optional[Dict[str, str]]:
         self._compute_from_env()
         return self._from_env_conda_deps
 
+    def _from_np_conda_deps(self) -> Optional[Dict[str, str]]:
+        self._compute_from_env()
+        return self._from_env_np_conda_deps
+
     def _from_pip_deps(self) -> Optional[Dict[str, str]]:
         self._compute_from_env()
         return self._from_env_pip_deps
 
     def _from_conda_channels(self) -> Optional[List[str]]:
         self._compute_from_env()
         return self._from_env_conda_channels
@@ -513,23 +551,43 @@
     def _from_env_python(self) -> Optional[str]:
         self._compute_from_env()
         conda_deps = self._from_conda_deps()
         if conda_deps:
             return conda_deps["python"]
         return None
 
-    def _conda_deps(self) -> Dict[str, str]:
-        deps = get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
+    def _np_conda_deps(self) -> Dict[str, str]:
+        if self.from_env:
+            return dict(cast(Dict[str, str], self._from_np_conda_deps()))
+        return {}
 
+    def _conda_deps(self) -> Dict[str, str]:
         if self.from_env:
-            deps.update(cast(Dict[str, str], self._from_conda_deps()))
+            if self.from_env.env_type == EnvType.PIP_ONLY:
+                # We don't get pinned deps here -- we will set them as pip ones to
+                # allow things like @conda_base(name=<piponlyenv>)
+                deps = dict(self._from_conda_deps())
+            else:
+                deps = dict(
+                    get_pinned_conda_libs(
+                        self._python_version(), self._flow_datastore_type
+                    )
+                )
+                deps.update(cast(Dict[str, str], self._from_conda_deps()))
+        else:
+            deps = dict(
+                get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
+            )
 
         deps.update(self._base_attributes["libraries"])
         deps.update(self.attributes["libraries"])
 
+        if self.from_env and self._from_conda_deps() != deps:
+            self._clean_from_env = False
+
         return deps
 
     def _conda_channels(self) -> List[str]:
         if self.from_env:
             from_channels = cast(List[str], self._from_conda_channels())
         else:
             from_channels = []
@@ -541,25 +599,39 @@
             self.attributes["channels"],
             self._base_attributes["channels"],
         ):
             if c in seen:
                 continue
             seen.add(c)
             result.append(c)
+
+        if self.from_env and sorted(from_channels) != sorted(result):
+            self._clean_from_env = False
         return result
 
     def _pip_deps(self) -> Dict[str, str]:
         if self.from_env:
-            deps = cast(Dict[str, str], self._from_pip_deps())
+            if self.from_env.env_type == EnvType.PIP_ONLY:
+                deps = dict(
+                    get_pinned_conda_libs(
+                        self._python_version(), self._flow_datastore_type
+                    )
+                )
+                deps.update(cast(Dict[str, str], self._from_pip_deps()))
+            else:
+                deps = dict(cast(Dict[str, str], self._from_pip_deps()))
         else:
             deps = {}
 
         deps.update(self._base_attributes["pip_packages"])
         deps.update(self.attributes["pip_packages"])
 
+        if self.from_env and self._from_pip_deps() != deps:
+            self._clean_from_env = False
+
         return deps
 
     def _pip_sources(self) -> List[str]:
         if self.from_env:
             from_sources = cast(List[str], self._from_pip_sources())
         else:
             from_sources = []
@@ -570,16 +642,74 @@
             self.attributes["pip_sources"],
             self._base_attributes["pip_sources"],
         ):
             if c in seen:
                 continue
             seen.add(c)
             result.append(c)
+
+        if self.from_env and sorted(from_sources) != sorted(result):
+            self._clean_from_env = False
+
         return result
 
+    def _resolve_pip_or_conda_deco(
+        self, flow: FlowSpec, decorators: List[StepDecorator]
+    ) -> bool:
+        has_pip_base = "pip_base" in flow._flow_decorators
+        has_conda_base = "conda_base" in flow._flow_decorators
+        conda_decs = [(d, idx) for idx, d in enumerate(decorators) if d.name == "conda"]
+        pip_decs = [(d, idx) for idx, d in enumerate(decorators) if d.name == "pip"]
+
+        # It is possible we don't have both if we call step_init twice (which can
+        # happen when deploying to schedulers since we attach an additional deco
+        # and then call step_init again. In that case, we just continue for the
+        # decorator and ignore this function -- we already properly checked the
+        # first time around since both conda and pip decorators are added to all
+        # steps
+        if len(conda_decs) == 0 or len(pip_decs) == 0:
+            return True
+
+        conda_step_decorator, conda_idx = conda_decs[0]
+        pip_step_decorator, pip_idx = pip_decs[0]
+
+        my_idx = pip_idx if self.name == "pip" else conda_idx
+
+        debug.conda_exec(
+            "In %s decorator: pip_base(%s), conda_base(%s), conda_idx(%d), pip_idx(%d)"
+            % (self.name, has_pip_base, has_conda_base, conda_idx, pip_idx)
+        )
+        if (
+            conda_step_decorator.statically_defined
+            and pip_step_decorator.statically_defined
+        ):
+            raise InvalidEnvironmentException(
+                "Cannot specify both @conda and @pip on a step. "
+                "If you need both pip and conda dependencies, use @conda and "
+                "pass in the pip dependencies as `pip_packages` and the sources as "
+                "`pip_sources`"
+            )
+        if has_pip_base and conda_step_decorator.statically_defined:
+            raise InvalidEnvironmentException("@pip_base is not compatible with @conda")
+        if has_conda_base and pip_step_decorator.statically_defined:
+            raise InvalidEnvironmentException("@conda_base is not compatible with @pip")
+
+        # At this point, we have at most one statically defined so we keep that one
+        # or the one derived from the base decorator.
+        # If we have none, we keep the conda one (base one). We remove only when
+        # we are the second decorator
+        # Return true if we should continue the function. False if we return (ie:
+        # we are going to be deleted)
+        del_idx = pip_idx
+        if pip_step_decorator.statically_defined or has_pip_base:
+            del_idx = conda_idx
+        if my_idx == max(pip_idx, conda_idx):
+            del decorators[del_idx]
+        return my_idx != del_idx
+
     @classmethod
     def _get_conda(cls, echo: Callable[..., None], datastore_type: str) -> None:
         if cls.conda is None:
             cls.conda = Conda(echo, datastore_type)
 
 
 class PipStepDecorator(CondaStepDecorator):
@@ -622,31 +752,55 @@
         "sources": [],
         "python": None,
         "disabled": None,
     }
 
     def _conda_deps(self) -> Dict[str, str]:
         if self.from_env:
+            if self.from_env.env_type != EnvType.PIP_ONLY:
+                deps = dict(
+                    get_pinned_conda_libs(
+                        self._python_version(), self._flow_datastore_type
+                    )
+                )
+                deps.update(cast(Dict[str, str], self._from_conda_deps()))
+
+                if deps != self._from_conda_deps():
+                    self._clean_from_env = False
+                return deps
             return cast(Dict[str, str], self._from_conda_deps())
         return {}
 
     def _conda_channels(self) -> List[str]:
         if self.from_env:
             return cast(List[str], self._from_conda_channels())
         return []
 
     def _pip_deps(self) -> Dict[str, str]:
-        deps = get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
-
         if self.from_env:
-            deps.update(cast(Dict[str, str], self._from_pip_deps()))
+            if self.from_env.env_type != EnvType.PIP_ONLY:
+                deps = dict(cast(Dict[str, str], self._from_pip_deps()))
+            else:
+                deps = dict(
+                    get_pinned_conda_libs(
+                        self._python_version(), self._flow_datastore_type
+                    )
+                )
+                deps.update(cast(Dict[str, str], self._from_pip_deps()))
+        else:
+            deps = dict(
+                get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
+            )
 
         deps.update(self._base_attributes["packages"])
         deps.update(self.attributes["packages"])
 
+        if self.from_env and self._from_pip_deps() != deps:
+            self._clean_from_env = False
+
         return deps
 
     def _pip_sources(self) -> List[str]:
         if self.from_env:
             from_sources = cast(List[str], self._from_pip_sources())
         else:
             from_sources = []
@@ -657,50 +811,29 @@
             self.attributes["sources"],
             self._base_attributes["sources"],
         ):
             if c in seen:
                 continue
             seen.add(c)
             result.append(c)
+
+        if self.from_env and sorted(from_sources) != sorted(result):
+            self._clean_from_env = False
+
         return result
 
     def _get_base_attributes(self) -> Dict[str, Any]:
         if "conda_base" in self._flow._flow_decorators:
             raise InvalidEnvironmentException(
                 "@pip decorator is not compatible with @conda_base decorator."
             )
         if "pip_base" in self._flow._flow_decorators:
-            return self._flow._flow_decorators["pip_base"].attributes
+            return self._flow._flow_decorators["pip_base"][0].attributes
         return self.defaults
 
-    def step_init(
-        self, flow, graph, step_name, decorators, environment, flow_datastore, logger
-    ):
-        if environment.TYPE != "conda":
-            raise InvalidEnvironmentException(
-                "@%s decorator requires --environment=conda" % self.name
-            )
-
-        for idx, deco in enumerate(decorators):
-            if deco.name == "conda":
-                if deco.statically_defined:
-                    raise InvalidEnvironmentException(
-                        "@pip decorator is not compatible with @conda. "
-                        "If you need both pip and conda dependencies, use @conda and "
-                        "pass in the pip dependencies as `pip_packages` and the "
-                        "sources as `pip_sources`"
-                    )
-                else:
-                    # Auto inserted decorator -- we remove since we replace it
-                    del decorators[idx]
-                    break
-        return super().step_init(
-            flow, graph, step_name, decorators, environment, flow_datastore, logger
-        )
-
 
 def get_conda_decorator(flow: FlowSpec, step_name: str) -> CondaStepDecorator:
     step = next(step for step in flow if step.name == step_name)
 
     decorator = next(
         deco for deco in step.decorators if isinstance(deco, CondaStepDecorator)
     )
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,14 +654,18 @@
             )
         new_full_id = ResolvedEnvironment._compute_hash(to_hash)
         for env in envs:
             env.set_coresolved(archs, new_full_id)
 
     @property
     def is_info_accurate(self) -> bool:
+        # Returns True if the requirements for this environment are accurate. This is
+        # currently always the case. This code was initially added in case we could
+        # get an environment from a FULL_ID which doesn't guarantee uniqueness of the
+        # requirements part (different requirements can resolve to the same environment)
         return not self._accurate_source
 
     @property
     def deps(self) -> List[TStr]:
         return self._user_dependencies
 
     @property
@@ -813,15 +817,19 @@
         lines.append("")
 
         if conda_packages:
             lines.append(
                 "*Conda Packages installed* %s"
                 % ", ".join(
                     [
-                        "%s==%s" % (p.package_name, p.package_version)
+                        "%s==%s"
+                        % (
+                            p.package_name,
+                            p.package_detailed_version,
+                        )
                         for p in conda_packages
                     ]
                 )
             )
 
         if pip_packages:
             lines.append(
@@ -872,15 +880,18 @@
             self.env_id.arch,
             self.resolved_on.isoformat(),
             self.resolved_by,
             ",".join(self.co_resolved_archs),
             ",".join([str(d) for d in self.deps]),
             ",".join([str(s) for s in self.sources]) if self.sources else "NONE",
             ",".join(
-                ["%s==%s" % (p.package_name, p.package_version) for p in conda_packages]
+                [
+                    "%s==%s" % (p.package_name, p.package_detailed_version)
+                    for p in conda_packages
+                ]
             ),
             ",".join(
                 ["%s==%s" % (p.package_name, p.package_version) for p in pip_packages]
             ),
             ",".join(local_instances) if local_instances else "NONE",
         )
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/markers.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/tags.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/utils.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_extensions/netflix_ext/vendor/packaging/version.py` & `metaflow-netflixext-0.1.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.1.0rc5
+Version: 0.1.1
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
@@ -123,16 +123,15 @@
 - `CONDA_ENVS_DIRNAME`: same thing a `CONDA_PACKAGES_DIRNAME` but for environments
   (defaults to `envs`)
 - `CONDA_LOCAL_DIST`: if set architecture specific tar ball in `CONDA_LOCAL_DIST_DIRNAME`.
 - `CONDA_LOCAL_PATH`: if set, installs the tarball in `CONDA_LOCAL_DIST` in this path.
 - `CONDA_PREFERRED_FORMAT`: `.tar.bz2` or `.conda`. Prefer `.conda` for speed gains; any
   package not available in the preferred format will be transmuted to it automatically.
   If left empty, whatever package is found will be used (ie: there is no preference)
-- `CONDA_DEFAULT_PIP_SOURCES`: list of additional mirrors to search for packages. Useful
-  if your company has an internal mirror.
+- `CONDA_DEFAULT_PIP_SOURCE`: mirror to use for PIP.
 
 ##### Azure specific setup
 For Azure, you need to do the following two steps once during setup:
 - Manually create the blob container specified in `CONDA_AZUREROOT`
 - Grant the `Storage Blob Data Contributor` role to the storage account to the service
   principal or user accounts that will be accessing as described
   [here](https://learn.microsoft.com/en-us/azure/storage/blobs/assign-azure-role-data-access?tabs=portal#assign-an-azure-role).
@@ -229,14 +228,21 @@
   dependencies.
 - a mixed environment with a mixture of pip and conda packages (specified via
   the `conda` decorator): in this case, `conda-lock` is used to resolve the
   entire environment. `conda-lock` uses a two phased approach to resolving, first
   resolving the conda environment and then using `poetry` to resolve the additional
   `pip` packages within the confines of the defined `conda` environment.
 
+Note that to support a bit more flexibility, you can have a pure Pip environment
+as well as non-Python conda packages. This is similar to the mixed environment
+but, in some cases, pip is more flexible than conda-lock in requirement specification
+(for example, pip supports GIT repositories) so it makes it possible to gain the
+flexibility of installing non python packages in your environment and still use
+pip to resolve your python dependencies.
+
 #### Additional command-line tool
 An additional `environment` command-line tool is available invoked as follows:
 `python myflow.py --environment=conda environment --help`.
 It provides the following two sub-commands:
 - `resolve`: will resolve one or more steps without executing the flow.
 - `show`: will show information about the environments for the flow (whether they exist,
   need to be resolved, etc.)
@@ -246,14 +252,41 @@
 - `create`: locally creates/instantiates an environment
 - `resolve`: resolves an environment using either a requirements.txt file (for pip only
   environments) or an environment.yml file (for conda or mixed environments)
 - `show`: shows information about an environment (packages, etc)
 - `alias`: aliases an environment giving it a name so it can be used later
 - `get`: fetches an environment from the remote environment store locally
 
+#### Supported format for requirements.txt
+
+The requirements.txt file, which can be used to specify a pip only environment, supports
+the following syntax (a subset of the full syntax supported by pip):
+- Comment lines starting with '#'
+- `--extra-index-url`: to spcify an additional repository to look at. Note that to
+  specify the `--index-url`, set it with the `METAFLOW_CONDA_DEFAULT_PIP_SOURCE
+  environment variable.
+- `-f`, `--find-links` and `--trusted-host`: passed directly to pip with the
+  corresponding argument
+- `--pre`, `--no-index`: passed directly to pip
+- `--conda-pkg`: extension allowing you to specify a conda package that does not
+  need Python
+- a requirement specification. This can include GIT repositories or local directories
+  as well as more classic package specification. Constraints and environment
+  markers are not supported.
+
+Note that GIT repositories, local directories and non wheel packages are not
+compatible with cross-architecture resolution. Metaflow will build the wheel on the fly
+when resolving the environment and this is only possible if the same architecture is used.
+
+If possible, it is best to specify pre-built packages.
+
+#### Supported format for environment.yml
+
+The environment.yml format is the same as the one for conda-lock.
+
 #### Named environments
 Environments can optionally be given aliases.
 
 Implicitly, the pathspec to a step that executed with a given Conda environment is
 an alias for that environment and you can refer to it using that pathspec. For
 example, if step `start` in run 456 of `MyFlow` executed within a certain
 environment, that environment can be referred to as `MyFlow/456/start`.
```

### Comparing `metaflow-netflixext-0.1.0rc5/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-0.1.1/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.1.0rc5/setup.py` & `metaflow-netflixext-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.1.0rc5"
+version = "0.1.1"
 
 setup(
     name="metaflow-netflixext",
     version=version,
     description="EXPERIMENTAL Metaflow extensions from Netflix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
@@ -31,9 +31,9 @@
     py_modules=[
         "metaflow_extensions",
     ],
     package_data={
         "metaflow_extensions.netflix_ext.plugins.conda.resources": ["*.png", "*.svg"]
     },
     python_requires=">=3.7.2",
-    install_requires=["metaflow>=2.7.22"],
+    install_requires=["metaflow>=2.8.3"],
 )
```


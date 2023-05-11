# Comparing `tmp/cliconfig-0.4.1.tar.gz` & `tmp/cliconfig-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.4.1.tar", last modified: Wed May 10 16:37:05 2023, max compression
+gzip compressed data, was "cliconfig-0.4.2.tar", last modified: Wed May 10 17:18:13 2023, max compression
```

## Comparing `cliconfig-0.4.1.tar` & `cliconfig-0.4.2.tar`

### file list

```diff
@@ -1,92 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.546070 cliconfig-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.530070 cliconfig-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.534070 cliconfig-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-10 16:36:45.000000 cliconfig-0.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-10 16:36:45.000000 cliconfig-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 16:36:45.000000 cliconfig-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-10 16:37:05.546070 cliconfig-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-05-10 16:36:45.000000 cliconfig-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.534070 cliconfig-0.4.1/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 16:37:05.000000 cliconfig-0.4.1/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.538070 cliconfig-0.4.1/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 16:36:45.000000 cliconfig-0.4.1/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.534070 cliconfig-0.4.1/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-10 16:37:05.000000 cliconfig-0.4.1/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-10 16:37:05.000000 cliconfig-0.4.1/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:37:05.000000 cliconfig-0.4.1/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 16:37:05.000000 cliconfig-0.4.1/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 16:37:05.000000 cliconfig-0.4.1/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.538070 cliconfig-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 16:36:45.000000 cliconfig-0.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.538070 cliconfig-0.4.1/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 16:36:45.000000 cliconfig-0.4.1/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 16:36:45.000000 cliconfig-0.4.1/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-10 16:36:45.000000 cliconfig-0.4.1/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 16:36:45.000000 cliconfig-0.4.1/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 16:36:45.000000 cliconfig-0.4.1/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.538070 cliconfig-0.4.1/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 16:36:45.000000 cliconfig-0.4.1/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 16:36:45.000000 cliconfig-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 16:36:45.000000 cliconfig-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 16:36:45.000000 cliconfig-0.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.542070 cliconfig-0.4.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-10 16:36:45.000000 cliconfig-0.4.1/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:37:05.546070 cliconfig-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 16:36:45.000000 cliconfig-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.542070 cliconfig-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.542070 cliconfig-0.4.1/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.542070 cliconfig-0.4.1/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:37:05.542070 cliconfig-0.4.1/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-10 16:36:45.000000 cliconfig-0.4.1/tests/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.322135 cliconfig-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.322135 cliconfig-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-10 17:17:54.000000 cliconfig-0.4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-10 17:17:54.000000 cliconfig-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 17:17:54.000000 cliconfig-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-05-10 17:18:13.330135 cliconfig-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-05-10 17:17:54.000000 cliconfig-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 17:18:13.000000 cliconfig-0.4.2/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 17:17:54.000000 cliconfig-0.4.2/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-05-10 17:18:13.000000 cliconfig-0.4.2/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-10 17:18:13.000000 cliconfig-0.4.2/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:18:13.000000 cliconfig-0.4.2/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 17:18:13.000000 cliconfig-0.4.2/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 17:18:13.000000 cliconfig-0.4.2/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/cliconfig.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 17:17:54.000000 cliconfig-0.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 17:17:54.000000 cliconfig-0.4.2/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 17:17:54.000000 cliconfig-0.4.2/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-10 17:17:54.000000 cliconfig-0.4.2/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 17:17:54.000000 cliconfig-0.4.2/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 17:17:54.000000 cliconfig-0.4.2/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 17:17:54.000000 cliconfig-0.4.2/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 17:17:54.000000 cliconfig-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 17:17:54.000000 cliconfig-0.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 17:17:54.000000 cliconfig-0.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-10 17:17:54.000000 cliconfig-0.4.2/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:18:13.330135 cliconfig-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 17:17:54.000000 cliconfig-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.326135 cliconfig-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/tests/configs/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/integration/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/integration/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/integration/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:18:13.330135 cliconfig-0.4.2/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-10 17:17:54.000000 cliconfig-0.4.2/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.4.1/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.4.2/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/.github/workflows/pydocstyle.yaml` & `cliconfig-0.4.2/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/.github/workflows/pylint.yaml` & `cliconfig-0.4.2/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/.github/workflows/tests.yaml` & `cliconfig-0.4.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/.pylintrc` & `cliconfig-0.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/CONTRIBUTING.md` & `cliconfig-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/LICENSE` & `cliconfig-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/PKG-INFO` & `cliconfig-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.1
+Version: 0.4.2
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -153,16 +153,17 @@
 You can also combine the tags, example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
-config1.param@copy@type:int: config1.param2
-config1.param2@type:int: 1
+config1:
+  param@copy@type:int: config1.param2
+  param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
@@ -220,14 +221,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
+* [ ] allow passing new arguments by CLI (with warning and no actual merge)
 * [ ] add a routine to check if a tag is in a key and robust to all other possible tags
 * [ ] add an integration test with all built-in processing (and more)
 
 Secondary:
 
 * [ ] add `make_processing_keep_status` to make a processing that keep the status of
   a parameter across merged configs. The status is any python object returned by
```

### Comparing `cliconfig-0.4.1/README.md` & `cliconfig-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,17 @@
 You can also combine the tags, example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
-config1.param@copy@type:int: config1.param2
-config1.param2@type:int: 1
+config1:
+  param@copy@type:int: config1.param2
+  param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
@@ -208,14 +209,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
+* [ ] allow passing new arguments by CLI (with warning and no actual merge)
 * [ ] add a routine to check if a tag is in a key and robust to all other possible tags
 * [ ] add an integration test with all built-in processing (and more)
 
 Secondary:
 
 * [ ] add `make_processing_keep_status` to make a processing that keep the status of
   a parameter across merged configs. The status is any python object returned by
```

### Comparing `cliconfig-0.4.1/cliconfig/__init__.py` & `cliconfig-0.4.2/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/build_config.py` & `cliconfig-0.4.2/cliconfig/build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/cli_parser.py` & `cliconfig-0.4.2/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/dict_routines.py` & `cliconfig-0.4.2/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/process_routines.py` & `cliconfig-0.4.2/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/processing/_type_parser.py` & `cliconfig-0.4.2/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/processing/base.py` & `cliconfig-0.4.2/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/processing/builtin.py` & `cliconfig-0.4.2/cliconfig/processing/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,22 +199,23 @@
         processing_list: list,  # noqa
     ) -> Dict[str, Any]:
         """Pre-merge processing."""
         items = list(flat_dict.items())
         for flat_key, val in items:
             key = flat_key.split(".")[-1]
             if "@copy" in key:
-                if not isinstance(val, str) or val not in flat_dict:
+                clean_dict, _ = dict_clean_tags(flat_dict)
+                if not isinstance(val, str) or val not in clean_dict:
                     raise ValueError(
                         "Key with '@copy' tag must be associated "
                         "to a string corresponding to an existing flat key. "
                         f"The problem occurs at key: {flat_key} with value: {val}"
                     )
                 # Remove the tag and update the dict
-                flat_dict[clean_tag(flat_key, "copy")] = flat_dict[val]
+                flat_dict[clean_tag(flat_key, "copy")] = clean_dict[val]
                 del flat_dict[flat_key]
         return flat_dict
 
 
 class ProcessTyping(Processing):
     """Force a type with '@type:mytype' tag. The type is preserved forever.
```

### Comparing `cliconfig-0.4.1/cliconfig/processing/create.py` & `cliconfig-0.4.2/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig/tag_routines.py` & `cliconfig-0.4.2/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.4.2/cliconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.1
+Version: 0.4.2
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -153,16 +153,17 @@
 You can also combine the tags, example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
-config1.param@copy@type:int: config1.param2
-config1.param2@type:int: 1
+config1:
+  param@copy@type:int: config1.param2
+  param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
@@ -220,14 +221,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
+* [ ] allow passing new arguments by CLI (with warning and no actual merge)
 * [ ] add a routine to check if a tag is in a key and robust to all other possible tags
 * [ ] add an integration test with all built-in processing (and more)
 
 Secondary:
 
 * [ ] add `make_processing_keep_status` to make a processing that keep the status of
   a parameter across merged configs. The status is any python object returned by
```

### Comparing `cliconfig-0.4.1/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.4.2/cliconfig.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -50,27 +50,31 @@
 github_actions_utils/pydocstyle_manager.py
 github_actions_utils/pylint_manager.py
 github_actions_utils/pytest_manager.py
 licenses_tier/FLATTEN_DICT_LICENSE
 scripts/pre-commit-checks.sh
 tests/__init__.py
 tests/conftest.py
-tests/test_build_config.py
-tests/test_cli_parser.py
-tests/test_dict_routines.py
-tests/test_process_routines.py
-tests/test_tag_routines.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
 tests/configs/configtag1.yaml
 tests/configs/configtag2.yaml
 tests/configs/default1.yaml
 tests/configs/default2.yaml
+tests/configs/integration/main.yaml
+tests/configs/integration/sub1.yaml
+tests/configs/integration/sub2.yaml
 tests/configs/merge/additional1.yaml
 tests/configs/merge/additional2.yaml
 tests/configs/merge/additional3.yaml
 tests/configs/merge/default1.yaml
 tests/configs/merge/default2.yaml
 tests/configs/merge/default3.yaml
-tests/processing/test_builtin.py
-tests/processing/test_create.py
-tests/processing/test_type_parser.py
+tests/integration/test_inte_multiple_tags.py
+tests/unit/test_build_config.py
+tests/unit/test_cli_parser.py
+tests/unit/test_dict_routines.py
+tests/unit/test_process_routines.py
+tests/unit/test_tag_routines.py
+tests/unit/processing/test_builtin.py
+tests/unit/processing/test_create.py
+tests/unit/processing/test_type_parser.py
```

### Comparing `cliconfig-0.4.1/docs/Makefile` & `cliconfig-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/cliconfig_api.rst` & `cliconfig-0.4.2/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/conf.py` & `cliconfig-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/edge_cases.md` & `cliconfig-0.4.2/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/index.rst` & `cliconfig-0.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/license.md` & `cliconfig-0.4.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/make.bat` & `cliconfig-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/processing.md` & `cliconfig-0.4.2/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/docs/quickstart.md` & `cliconfig-0.4.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.4.2/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/github_actions_utils/pylint_manager.py` & `cliconfig-0.4.2/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/github_actions_utils/pytest_manager.py` & `cliconfig-0.4.2/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.4.2/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/pyproject.toml` & `cliconfig-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/scripts/pre-commit-checks.sh` & `cliconfig-0.4.2/scripts/pre-commit-checks.sh`

 * *Files 0% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 
 echo "*********** Style evaluation ***********"
 score=$(pylint . | sed -n 's/^Your code has been rated at \([-0-9.]*\)\/.*/\1/p')
 
 echo "Pylint score: ${BOLD}$score/10.0${NORMAL} (details by running: pylint .)\nMinimum authorized score: 8.5\n"
 
 echo "************** Unit tests **************"
-pytest --cov-report term-missing --cov=./cliconfig tests/
+pytest --cov-report term-missing --cov=./cliconfig tests/unit
 check_output "Unit tests"
 
 printf "\n${GREEN}${BOLD}All checks pass${NORMAL}${WHITE}\n\n"
```

### Comparing `cliconfig-0.4.1/tests/conftest.py` & `cliconfig-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/processing/test_builtin.py` & `cliconfig-0.4.2/tests/unit/processing/test_builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/processing/test_create.py` & `cliconfig-0.4.2/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/processing/test_type_parser.py` & `cliconfig-0.4.2/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/test_build_config.py` & `cliconfig-0.4.2/tests/unit/test_build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/test_cli_parser.py` & `cliconfig-0.4.2/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/test_dict_routines.py` & `cliconfig-0.4.2/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/test_process_routines.py` & `cliconfig-0.4.2/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.1/tests/test_tag_routines.py` & `cliconfig-0.4.2/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*


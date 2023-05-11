# Comparing `tmp/cliconfig-0.4.3.tar.gz` & `tmp/cliconfig-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.4.3.tar", last modified: Thu May 11 00:41:44 2023, max compression
+gzip compressed data, was "cliconfig-0.4.4.tar", last modified: Thu May 11 01:24:46 2023, max compression
```

## Comparing `cliconfig-0.4.3.tar` & `cliconfig-0.4.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.465177 cliconfig-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.469177 cliconfig-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-11 00:41:21.000000 cliconfig-0.4.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 00:41:21.000000 cliconfig-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 00:41:21.000000 cliconfig-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-11 00:41:44.477177 cliconfig-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-05-11 00:41:21.000000 cliconfig-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.469177 cliconfig-0.4.3/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 00:41:44.000000 cliconfig-0.4.3/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 00:41:21.000000 cliconfig-0.4.3/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-11 00:41:44.000000 cliconfig-0.4.3/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-11 00:41:44.000000 cliconfig-0.4.3/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:41:44.000000 cliconfig-0.4.3/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 00:41:44.000000 cliconfig-0.4.3/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 00:41:44.000000 cliconfig-0.4.3/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 00:41:21.000000 cliconfig-0.4.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 00:41:21.000000 cliconfig-0.4.3/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-11 00:41:21.000000 cliconfig-0.4.3/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 00:41:21.000000 cliconfig-0.4.3/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 00:41:21.000000 cliconfig-0.4.3/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 00:41:21.000000 cliconfig-0.4.3/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 00:41:21.000000 cliconfig-0.4.3/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 00:41:21.000000 cliconfig-0.4.3/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-11 00:41:21.000000 cliconfig-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 00:41:21.000000 cliconfig-0.4.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 00:41:21.000000 cliconfig-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:41:44.477177 cliconfig-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 00:41:21.000000 cliconfig-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.473177 cliconfig-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/tests/configs/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/integration/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/integration/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/integration/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:41:44.477177 cliconfig-0.4.3/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/processing/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 00:41:21.000000 cliconfig-0.4.3/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.383058 cliconfig-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 01:24:24.000000 cliconfig-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 01:24:24.000000 cliconfig-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-11 01:24:46.399059 cliconfig-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-11 01:24:24.000000 cliconfig-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/cliconfig.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 01:24:24.000000 cliconfig-0.4.4/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 01:24:24.000000 cliconfig-0.4.4/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-11 01:24:24.000000 cliconfig-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 01:24:24.000000 cliconfig-0.4.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 01:24:24.000000 cliconfig-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:24:46.399059 cliconfig-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 01:24:24.000000 cliconfig-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/configs/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/integration/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/integration/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/integration/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.4.3/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.4.4/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/.github/workflows/pydocstyle.yaml` & `cliconfig-0.4.4/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/.github/workflows/pylint.yaml` & `cliconfig-0.4.4/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/.github/workflows/tests.yaml` & `cliconfig-0.4.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/.pylintrc` & `cliconfig-0.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/CONTRIBUTING.md` & `cliconfig-0.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/LICENSE` & `cliconfig-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/PKG-INFO` & `cliconfig-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.3
+Version: 0.4.4
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLI Config
 
 <p align="center">
-  <img src="docs/_static/logo.png" />
+  <img src="docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It is also provide processing functions
 that can change the whole config before and after each config merge, before config
 saving and after config loading. It also contains many routines to manipulate
 the config as flatten or nested dicts.
```

### Comparing `cliconfig-0.4.3/README.md` & `cliconfig-0.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CLI Config
 
 <p align="center">
-  <img src="docs/_static/logo.png" />
+  <img src="docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It is also provide processing functions
 that can change the whole config before and after each config merge, before config
 saving and after config loading. It also contains many routines to manipulate
 the config as flatten or nested dicts.
```

### Comparing `cliconfig-0.4.3/cliconfig/__init__.py` & `cliconfig-0.4.4/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/build_config.py` & `cliconfig-0.4.4/cliconfig/build_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         f"{len(config_paths)} additional configs and "
         f"{len(config_cli_params)} CLI parameter(s)."
     )
     if processing_list is None:
         processing_list_: List[Processing] = []
     if add_default_processing:
         processing_list_.extend([
-            ProcessTyping(),
             ProcessCheckTags(),
+            ProcessTyping(),
             ProcessCopy(),
             ProcessMerge(),
         ])
 
     for default_config_path in default_config_paths:
         # Allow new keys for default configs
         config, processing_list_ = merge_flat_paths_processing(
```

### Comparing `cliconfig-0.4.3/cliconfig/cli_parser.py` & `cliconfig-0.4.4/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/dict_routines.py` & `cliconfig-0.4.4/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/process_routines.py` & `cliconfig-0.4.4/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/processing/_type_parser.py` & `cliconfig-0.4.4/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/processing/base.py` & `cliconfig-0.4.4/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/processing/builtin.py` & `cliconfig-0.4.4/cliconfig/processing/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = 0.0
         self.postmerge_order = 10.0
         self.presave_order = 10.0
         self.keys_to_copy: Dict[str, str] = {}
+        self.current_value: Dict[str, Any] = {}
 
     def premerge(
         self,
         flat_dict: Dict[str, Any],
         processing_list: list,  # noqa ARG002
     ) -> Dict[str, Any]:
         """Pre-merge processing."""
@@ -231,16 +232,17 @@
                 if (clean_key in self.keys_to_copy
                         and self.keys_to_copy[clean_key] != val):
                     raise ValueError(
                         "Key with '@copy' has change its value to copy. Found key: "
                         f"{flat_key} with value: {val}, previous value to copy: "
                         f"{self.keys_to_copy[clean_key]}"
                     )
-                # Store the key to copy
+                # Store the key to copy and value
                 self.keys_to_copy[clean_key] = val
+                self.current_value[clean_key] = val
                 # Remove the tag and update the dict
                 flat_dict[clean_tag(flat_key, "copy")] = val
                 del flat_dict[flat_key]
         return flat_dict
 
     def postmerge(
         self,
@@ -251,23 +253,25 @@
         for key, val in self.keys_to_copy.items():
             if key in flat_dict:
                 if val not in flat_dict:
                     raise ValueError(
                         f"Key to copy not found in config: {val}. "
                         f"The problem occurs with key: {key}"
                     )
-                if flat_dict[key] not in (flat_dict[val], val):
+                if flat_dict[key] != self.current_value[key]:
                     # The key has been modified
                     raise ValueError(
                         "Found attempt to modify a key with '@copy' tag. The key is "
                         "then protected against updates (except the copied value or "
                         f"the original key to copy). Found key: {key} of value "
                         f"{flat_dict[key]} that copy {val} of value {flat_dict[val]}")
                 # Copy the value
                 flat_dict[key] = flat_dict[val]
+                # Update the current value
+                self.current_value[key] = flat_dict[val]
         return flat_dict
 
     def presave(
         self,
         flat_dict: Dict[str, Any],
         processing_list: list,  # noqa ARG002
     ) -> Dict[str, Any]:
```

### Comparing `cliconfig-0.4.3/cliconfig/processing/create.py` & `cliconfig-0.4.4/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig/tag_routines.py` & `cliconfig-0.4.4/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.4.4/cliconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.3
+Version: 0.4.4
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLI Config
 
 <p align="center">
-  <img src="docs/_static/logo.png" />
+  <img src="docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It is also provide processing functions
 that can change the whole config before and after each config merge, before config
 saving and after config loading. It also contains many routines to manipulate
 the config as flatten or nested dicts.
```

### Comparing `cliconfig-0.4.3/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.4.4/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/Makefile` & `cliconfig-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/_static/logo.png` & `cliconfig-0.4.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/_static/logo_extend.png` & `cliconfig-0.4.4/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/cliconfig_api.rst` & `cliconfig-0.4.4/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/conf.py` & `cliconfig-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/edge_cases.md` & `cliconfig-0.4.4/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/index.rst` & `cliconfig-0.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/license.md` & `cliconfig-0.4.4/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/make.bat` & `cliconfig-0.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/processing.md` & `cliconfig-0.4.4/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/docs/quickstart.md` & `cliconfig-0.4.4/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.4.4/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/github_actions_utils/pylint_manager.py` & `cliconfig-0.4.4/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/github_actions_utils/pytest_manager.py` & `cliconfig-0.4.4/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.4.4/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/pre-commit-checks.sh` & `cliconfig-0.4.4/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/pyproject.toml` & `cliconfig-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/conftest.py` & `cliconfig-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/integration/test_inte_multiple_tags.py` & `cliconfig-0.4.4/tests/integration/test_inte_multiple_tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,26 @@
     sys_argv = sys.argv.copy()
     sys.argv = ["test_inte_multiple_tags.py"]
     config, processing_list = make_config("tests/configs/integration/main.yaml")
     expected_config = {
         "path_1": "tests/configs/integration/sub1.yaml",
         "path_2": "tests/configs/integration/sub2.yaml",
         "config1": {
-            "param": 1,
+            "param": 2,
             "param2": 1,
         },
         "config2": {
             "param": 2,
         },
     }
     check.equal(config, expected_config)
     with pytest.raises(
         ValueError,
         match="Key previously tagged with '@type:None|int'.*"
     ):
-        merge_flat_processing(config, {'config2.param': 5.6}, processing_list)
+        merge_flat_processing(
+            config,
+            {'config2.param': 5.6},
+            processing_list,
+            preprocess_first=False,
+        )
     sys.argv = sys_argv
```

### Comparing `cliconfig-0.4.3/tests/unit/processing/test_base.py` & `cliconfig-0.4.4/tests/unit/processing/test_base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/processing/test_builtin.py` & `cliconfig-0.4.4/tests/unit/processing/test_builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,18 +99,20 @@
         "config2.param2@copy": 'config1.param1',
     }
     flat_dict = processing.premerge(flat_dict, [processing])
     check.equal(flat_dict, {"config1.param1": 1, "config2.param2": 'config1.param1'})
     flat_dict = processing.postmerge(flat_dict, [processing])
     check.equal(flat_dict, {"config1.param1": 1, "config2.param2": 1})
     flat_dict = processing.presave(flat_dict, [processing])
+    check.equal(processing.current_value, {"config2.param2": 1})
     check.equal(
         flat_dict,
         {"config1.param1": 1, "config2.param2@copy": 'config1.param1'}
     )
+    check.equal(processing.keys_to_copy, {"config2.param2": "config1.param1"})
     # Reset copy processing
     processing.keys_to_copy = {}
     # Case of wrong key
     with pytest.raises(
         ValueError,
         match=(
             "Key with '@copy' tag must be associated "
@@ -136,14 +138,15 @@
         match=(
             "Key to copy not found in config: b. "
             "The problem occurs with key: a"
         )
     ):
         flat_dict = processing.postmerge({"a": "b"}, [processing])
     # Case overwriting a key
+    processing.current_value = {"a": 2}
     with pytest.raises(
         ValueError,
         match=re.escape(
             "Found attempt to modify a key with '@copy' tag. The key is "
             "then protected against updates (except the copied value or "
             "the original key to copy). Found key: a of value c that copy "
             "b of value 1"
```

### Comparing `cliconfig-0.4.3/tests/unit/processing/test_create.py` & `cliconfig-0.4.4/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/processing/test_type_parser.py` & `cliconfig-0.4.4/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/test_build_config.py` & `cliconfig-0.4.4/tests/unit/test_build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/test_cli_parser.py` & `cliconfig-0.4.4/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/test_dict_routines.py` & `cliconfig-0.4.4/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/test_process_routines.py` & `cliconfig-0.4.4/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.3/tests/unit/test_tag_routines.py` & `cliconfig-0.4.4/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*


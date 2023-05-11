# Comparing `tmp/cliconfig-0.4.4.tar.gz` & `tmp/cliconfig-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.4.4.tar", last modified: Thu May 11 01:24:46 2023, max compression
+gzip compressed data, was "cliconfig-0.4.5.tar", last modified: Thu May 11 12:05:49 2023, max compression
```

## Comparing `cliconfig-0.4.4.tar` & `cliconfig-0.4.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.383058 cliconfig-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-11 01:24:24.000000 cliconfig-0.4.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 01:24:24.000000 cliconfig-0.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 01:24:24.000000 cliconfig-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-11 01:24:46.399059 cliconfig-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-11 01:24:24.000000 cliconfig-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 01:24:24.000000 cliconfig-0.4.4/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.391059 cliconfig-0.4.4/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 01:24:46.000000 cliconfig-0.4.4/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 01:24:24.000000 cliconfig-0.4.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 01:24:24.000000 cliconfig-0.4.4/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 01:24:24.000000 cliconfig-0.4.4/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 01:24:24.000000 cliconfig-0.4.4/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-11 01:24:24.000000 cliconfig-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 01:24:24.000000 cliconfig-0.4.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 01:24:24.000000 cliconfig-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:24:46.399059 cliconfig-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 01:24:24.000000 cliconfig-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.395059 cliconfig-0.4.4/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/configs/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/integration/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/integration/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/integration/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:46.399059 cliconfig-0.4.4/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 01:24:24.000000 cliconfig-0.4.4/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.885638 cliconfig-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.885638 cliconfig-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-11 12:05:32.000000 cliconfig-0.4.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 12:05:32.000000 cliconfig-0.4.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 12:05:32.000000 cliconfig-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-11 12:05:49.893638 cliconfig-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-05-11 12:05:32.000000 cliconfig-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 12:05:49.000000 cliconfig-0.4.5/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 12:05:32.000000 cliconfig-0.4.5/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-11 12:05:49.000000 cliconfig-0.4.5/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-11 12:05:49.000000 cliconfig-0.4.5/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:05:49.000000 cliconfig-0.4.5/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 12:05:49.000000 cliconfig-0.4.5/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 12:05:49.000000 cliconfig-0.4.5/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/cliconfig.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 12:05:32.000000 cliconfig-0.4.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 12:05:32.000000 cliconfig-0.4.5/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-11 12:05:32.000000 cliconfig-0.4.5/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 12:05:32.000000 cliconfig-0.4.5/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 12:05:32.000000 cliconfig-0.4.5/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 12:05:32.000000 cliconfig-0.4.5/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 12:05:32.000000 cliconfig-0.4.5/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 12:05:32.000000 cliconfig-0.4.5/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-11 12:05:32.000000 cliconfig-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 12:05:32.000000 cliconfig-0.4.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 12:05:32.000000 cliconfig-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:05:49.893638 cliconfig-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 12:05:32.000000 cliconfig-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.889638 cliconfig-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/tests/configs/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/integration/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/integration/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/integration/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:05:49.893638 cliconfig-0.4.5/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/processing/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 12:05:32.000000 cliconfig-0.4.5/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.4.4/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.4.5/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/.github/workflows/pydocstyle.yaml` & `cliconfig-0.4.5/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/.github/workflows/pylint.yaml` & `cliconfig-0.4.5/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/.github/workflows/tests.yaml` & `cliconfig-0.4.5/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/.pylintrc` & `cliconfig-0.4.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/CONTRIBUTING.md` & `cliconfig-0.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/LICENSE` & `cliconfig-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/PKG-INFO` & `cliconfig-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.4
+Version: 0.4.5
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -74,15 +74,15 @@
 Now you can set up your program to use the config:
 
 ```python
 # main.py
 from cliconfig import make_config, show_config
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)
+show_config(config)  # print the config to check it
 ```
 
 Then add one or multiple additional config files that will be passed on command line
 and that will override the default values.
 
 ```yaml
 ---  # first.yaml
@@ -90,32 +90,33 @@
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, The additional config files cannot add new parameters that are
+**Be careful, the additional config files cannot add new parameters that are
 not in default configs**. It is intended to prevent typos in the config files
 that would not be detected. It also improves the readability of the config
 files and the retro-compatibility.
 
 Now you can launch the program with additional configurations and parameters.
-The additional configuration paths are indicated with `--config` followed by a
-whitespace. If there are several paths, they should be separate with comma,
-without space. Then, you can set individual parameters with `--<subconfig.param_name>`
-(use dot for nested configs).
+The additional configs will be merged to the default configs, then the parameters
+will be merged.
 
-The default configuration will be merged to the default configs with the additional
-configurations (from left to right), then the parameters will be set. For example:
+For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
+*Note*: the additional configs are detected with `--config` followed by space
+and separated by a comma **without space**. It also possible to pass a list.
+The parameters are detected with the pattern `--<param>=<value>` without spaces.
+
 Will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
@@ -227,15 +228,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
-* [ ] allow passing new arguments by CLI (with warning and no actual merge)
+* [x] allow passing new arguments by CLI (with warning and no actual merge)
 * [ ] add a routine to check if a tag is in a key and robust to all other
   possible tags
 * [ ] add an integration test with all built-in processing (and more)
 
 Secondary:
 
 * [ ] add `make_processing_keep_status` to make a processing that keep the
```

### Comparing `cliconfig-0.4.4/README.md` & `cliconfig-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 Now you can set up your program to use the config:
 
 ```python
 # main.py
 from cliconfig import make_config, show_config
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)
+show_config(config)  # print the config to check it
 ```
 
 Then add one or multiple additional config files that will be passed on command line
 and that will override the default values.
 
 ```yaml
 ---  # first.yaml
@@ -78,32 +78,33 @@
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, The additional config files cannot add new parameters that are
+**Be careful, the additional config files cannot add new parameters that are
 not in default configs**. It is intended to prevent typos in the config files
 that would not be detected. It also improves the readability of the config
 files and the retro-compatibility.
 
 Now you can launch the program with additional configurations and parameters.
-The additional configuration paths are indicated with `--config` followed by a
-whitespace. If there are several paths, they should be separate with comma,
-without space. Then, you can set individual parameters with `--<subconfig.param_name>`
-(use dot for nested configs).
+The additional configs will be merged to the default configs, then the parameters
+will be merged.
 
-The default configuration will be merged to the default configs with the additional
-configurations (from left to right), then the parameters will be set. For example:
+For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
+*Note*: the additional configs are detected with `--config` followed by space
+and separated by a comma **without space**. It also possible to pass a list.
+The parameters are detected with the pattern `--<param>=<value>` without spaces.
+
 Will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
@@ -215,15 +216,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
-* [ ] allow passing new arguments by CLI (with warning and no actual merge)
+* [x] allow passing new arguments by CLI (with warning and no actual merge)
 * [ ] add a routine to check if a tag is in a key and robust to all other
   possible tags
 * [ ] add an integration test with all built-in processing (and more)
 
 Secondary:
 
 * [ ] add `make_processing_keep_status` to make a processing that keep the
```

### Comparing `cliconfig-0.4.4/cliconfig/__init__.py` & `cliconfig-0.4.5/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/build_config.py` & `cliconfig-0.4.5/cliconfig/build_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Functions to manipulate config as dict with yaml files and CLI."""
 import sys
 from typing import Any, Dict, List, Optional, Tuple
 
 from cliconfig.cli_parser import parse_cli
-from cliconfig.dict_routines import unflatten
+from cliconfig.dict_routines import flatten, unflatten
 from cliconfig.process_routines import (
     load_processing,
     merge_flat_paths_processing,
     merge_flat_processing,
 )
 from cliconfig.processing.base import Processing
 from cliconfig.processing.builtin import (
     ProcessCheckTags,
     ProcessCopy,
     ProcessMerge,
     ProcessTyping,
 )
+from cliconfig.tag_routines import clean_all_tags
 
 
 def make_config(
     *default_config_paths: str,
     processing_list: Optional[List[Processing]] = None,
     add_default_processing: bool = True,
 ) -> Tuple[Dict[str, Any], List[Processing]]:
@@ -60,24 +61,20 @@
 
         # main.py
         config, _ = make_config('data.yaml', 'model.yaml', 'train.yaml')
 
     .. code-block:: text
 
         python main.py -- config bestmodel.yaml,mydata.yaml \
-            --architecture.layers.hidden_dim 64
+            --architecture.layers.hidden_dim=64
 
     """
     config: Dict[str, Any] = {}
     config_paths, config_cli_params = parse_cli(sys.argv)
-    print(
-        f"[CONFIG] Merge {len(default_config_paths)} default configs, "
-        f"{len(config_paths)} additional configs and "
-        f"{len(config_cli_params)} CLI parameter(s)."
-    )
+    config_cli_params = flatten(config_cli_params)
     if processing_list is None:
         processing_list_: List[Processing] = []
     if add_default_processing:
         processing_list_.extend([
             ProcessCheckTags(),
             ProcessTyping(),
             ProcessCopy(),
@@ -99,21 +96,39 @@
         config, processing_list_ = merge_flat_paths_processing(
             config,
             config_path,
             processing_list_,
             allow_new_keys=False,
             preprocess_first=False,
         )
-    # Disallow new keys for CLI parameters
+    # Allow new keys for CLI parameters but do not merge them and raise
+    # warning.
+    new_keys, keys = [], list(config_cli_params.keys())
+    for key in keys:
+        if clean_all_tags(key) not in config:
+            new_keys.append(clean_all_tags(key))
+            del config_cli_params[key]
+    if new_keys:
+        new_keys_message = "  - " + "\n  - ".join(new_keys)
+        print(
+            "[CONFIG] Warning: New keys found in CLI parameters "
+            f"that will not be merged:\n{new_keys_message}"
+        )
     config, processing_list_ = merge_flat_processing(
         config,
         config_cli_params,
         processing_list_,
         allow_new_keys=False,
-        preprocess_first=False)
+        preprocess_first=False
+    )
+    print(
+        f"[CONFIG] Info: Merged {len(default_config_paths)} default config(s), "
+        f"{len(config_paths)} additional config(s) and "
+        f"{len(config_cli_params)} CLI parameter(s)."
+    )
     # Unflatten the config
     config = unflatten(config)
     return config, processing_list_
 
 
 def load_config(
     path: str,
```

### Comparing `cliconfig-0.4.4/cliconfig/cli_parser.py` & `cliconfig-0.4.5/cliconfig/cli_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,37 +3,41 @@
 
 import yaml
 
 
 def parse_cli(sys_argv: List[str]) -> Tuple[List[str], Dict[str, Any]]:
     """Parser for CLI commands.
 
+    Return list of config paths that are detected with `--config ` (with a space),
+    separated by commas without space (or in a list).
+    Return also a dictionary of parameters from CLI detected with --<key>=<value>
+    (with "=" and without spaces).
+
     Parameters
     ----------
     sys_argv : List[str]
         List of arguments from sys.argv.
 
+    Raises
+    ------
+    Value Error
+        If the '--config ' argument (with space) is used more than once.
+
     Returns
     -------
     config_paths : List[str]
         List of paths to config files to merge.
     config_cli_params : Dict[str, Any]
         Dictionary of parameters from CLI.
 
-    Warning
-    -------
-        The '--config' argument is used for config merging only if
-        **it is followed by a space**. If '--config=' is used, it will
-        be parsed as a regular parameter in the config called 'config'.
-
     Examples
     --------
     .. code-block:: text
 
-        $ python my_script.py --config config.yaml --foo.bar.param [1, 2, 3]
+        $ python my_script.py --config config.yaml --foo.bar.param=[1, 2, 3]
 
     Will be parsed as `config_paths=['config.yaml']`
     and `cli_params={'foo.bar.param': [1, 2, 3]}`.
     It is equivalent to: `{'foo': {'bar': {'param': [1, 2, 3]}}`
     for :func:`merge_config`.
     """
     config_cli_params: Dict[str, Any] = {}
@@ -41,26 +45,29 @@
     i = 0
     while i < len(sys_argv):
         elem = sys_argv[i]
         if elem == "--config":
             if config_paths:
                 raise ValueError(
                     "Only one '--config ' argument is allowed in CLI (used for "
-                    "config merging). If you have a subconfig called 'config', "
-                    "use '--config=<val>' (with an '=')."
+                    "config merging)."
                 )
-            config_paths = sys_argv[i + 1].split(",")
+            configs = yaml.safe_load(sys_argv[i + 1])
+            if isinstance(configs, list):
+                config_paths = configs
+            if isinstance(configs, str):
+                config_paths = sys_argv[i + 1].split(",")
             i += 2
-
         elif elem.startswith("--"):
-            if "=" in elem:
-                key, value_str = elem.split("=", maxsplit=1)
-                i += 1
+            splits = elem.split("=", maxsplit=1)
+            if len(splits) == 2:
+                key, value_str = splits
             else:
-                key, value_str = elem, sys_argv[i + 1]
-                i += 2
+                key = splits[0]
+                value_str = "null"
             key = key[2:]
             value = yaml.safe_load(value_str)
             config_cli_params[key] = value
-        else:
+            i += 1
+        else:  # Not a config parameter
             i += 1
     return config_paths, config_cli_params
```

### Comparing `cliconfig-0.4.4/cliconfig/dict_routines.py` & `cliconfig-0.4.5/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/process_routines.py` & `cliconfig-0.4.5/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/processing/_type_parser.py` & `cliconfig-0.4.5/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/processing/base.py` & `cliconfig-0.4.5/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/processing/builtin.py` & `cliconfig-0.4.5/cliconfig/processing/builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/processing/create.py` & `cliconfig-0.4.5/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig/tag_routines.py` & `cliconfig-0.4.5/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.4.5/cliconfig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.4
+Version: 0.4.5
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -74,15 +74,15 @@
 Now you can set up your program to use the config:
 
 ```python
 # main.py
 from cliconfig import make_config, show_config
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)
+show_config(config)  # print the config to check it
 ```
 
 Then add one or multiple additional config files that will be passed on command line
 and that will override the default values.
 
 ```yaml
 ---  # first.yaml
@@ -90,32 +90,33 @@
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, The additional config files cannot add new parameters that are
+**Be careful, the additional config files cannot add new parameters that are
 not in default configs**. It is intended to prevent typos in the config files
 that would not be detected. It also improves the readability of the config
 files and the retro-compatibility.
 
 Now you can launch the program with additional configurations and parameters.
-The additional configuration paths are indicated with `--config` followed by a
-whitespace. If there are several paths, they should be separate with comma,
-without space. Then, you can set individual parameters with `--<subconfig.param_name>`
-(use dot for nested configs).
+The additional configs will be merged to the default configs, then the parameters
+will be merged.
 
-The default configuration will be merged to the default configs with the additional
-configurations (from left to right), then the parameters will be set. For example:
+For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
+*Note*: the additional configs are detected with `--config` followed by space
+and separated by a comma **without space**. It also possible to pass a list.
+The parameters are detected with the pattern `--<param>=<value>` without spaces.
+
 Will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
@@ -227,15 +228,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
-* [ ] allow passing new arguments by CLI (with warning and no actual merge)
+* [x] allow passing new arguments by CLI (with warning and no actual merge)
 * [ ] add a routine to check if a tag is in a key and robust to all other
   possible tags
 * [ ] add an integration test with all built-in processing (and more)
 
 Secondary:
 
 * [ ] add `make_processing_keep_status` to make a processing that keep the
```

### Comparing `cliconfig-0.4.4/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.4.5/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/Makefile` & `cliconfig-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/_static/logo.png` & `cliconfig-0.4.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/_static/logo_extend.png` & `cliconfig-0.4.5/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/cliconfig_api.rst` & `cliconfig-0.4.5/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/conf.py` & `cliconfig-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/edge_cases.md` & `cliconfig-0.4.5/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/index.rst` & `cliconfig-0.4.5/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 Then launch your script with additional config(s) file(s) and parameters.
 By default, these additional configs cannot add new parameters to the default config
 (for security and retro-compatibility reasons).
 
 .. code:: bash
 
-   python main.py --config first.yaml,second.yaml --param1 1 --subconfig.param2 'foo'
+   python main.py --config first.yaml,second.yaml --param1=1 --subconfig.param2='foo'
 
 See *Quickstart* section for more details and *Processing* section for advanced usage.
 
 .. |PyPI version| image:: https://badge.fury.io/py/cliconfig.svg
    :target: https://badge.fury.io/py/cliconfig
 .. |PythonVersion| image:: https://img.shields.io/badge/python-3.7%20%7E%203.11-informational
 .. |License| image:: https://img.shields.io/github/license/valentingol/cliconfig?color=999
```

### Comparing `cliconfig-0.4.4/docs/license.md` & `cliconfig-0.4.5/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/make.bat` & `cliconfig-0.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/processing.md` & `cliconfig-0.4.5/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/docs/quickstart.md` & `cliconfig-0.4.5/docs/quickstart.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Now you can set up your program to use the config:
 
 ```python
 # main.py
 from cliconfig import make_config, show_config
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)
+show_config(config)  # print the config to check it
 ```
 
 Then add one or multiple additional config files that will be passed on command line
 and that will override the default values.
 
 ```yaml
 ---  # first.yaml
@@ -37,32 +37,33 @@
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, The additional config files cannot add new parameters that are not in
-default configs**. It is intended to prevent typos in the config files that would
-not be detected. It also improves the readability of the config files and the
-retro-compatibility.
+**Be careful, the additional config files cannot add new parameters that are
+not in default configs**. It is intended to prevent typos in the config files
+that would not be detected. It also improves the readability of the config
+files and the retro-compatibility.
 
 Now you can launch the program with additional configurations and parameters.
-The additional configuration paths are indicated with `--config` followed by a
-whitespace. If there are several paths, they should be separate with comma,
-without space. Then, you can set individual parameters with `--<subconfig.param_name>`
-(use dot for nested configs).
+The additional configs will be merged to the default configs, then the parameters
+will be merged.
 
-The default configuration will be merged to the default configs with the additional
-configurations (from left to right), then the parameters will be set. For example:
+For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
+*Note*: the additional configs are detected with `--config` followed by space
+and separated by a comma **without space**. It also possible to pass a list.
+The parameters are detected with the pattern `--<param>=<value>` without spaces.
+
 Will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
```

### Comparing `cliconfig-0.4.4/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.4.5/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/github_actions_utils/pylint_manager.py` & `cliconfig-0.4.5/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/github_actions_utils/pytest_manager.py` & `cliconfig-0.4.5/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.4.5/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/pre-commit-checks.sh` & `cliconfig-0.4.5/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/pyproject.toml` & `cliconfig-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/conftest.py` & `cliconfig-0.4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/integration/test_inte_multiple_tags.py` & `cliconfig-0.4.5/tests/integration/test_inte_multiple_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/unit/processing/test_base.py` & `cliconfig-0.4.5/tests/unit/processing/test_base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/unit/processing/test_builtin.py` & `cliconfig-0.4.5/tests/unit/processing/test_builtin.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,27 +202,23 @@
         )
     ):
         flat_dict = processing.postmerge({"param": "mystr"}, [processing])
 
 
 def test_process_check_tags() -> None:
     """Test ProcessCheckTags."""
-    from cliconfig.tag_routines import dict_clean_tags
     processing = ProcessCheckTags()
     flat_dict = {
         "config.param1": 1,
         "param1": 2,
     }
     check.equal(processing.premerge(flat_dict, [processing]), flat_dict)
 
     flat_dicts = [{'param1@tag': 1}, {'@foo': 2}, {'@': 3}]
     for flat_dict in flat_dicts:
-        _, tagged_keys = dict_clean_tags(flat_dict)
-        if tagged_keys:
-            print('**', tagged_keys, '**')
         with pytest.raises(
             ValueError,
             match=(
                 "Keys with tags are encountered at the end of "
                 "the pre-merge process.*"
             )
         ):
```

### Comparing `cliconfig-0.4.4/tests/unit/processing/test_create.py` & `cliconfig-0.4.5/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/unit/processing/test_type_parser.py` & `cliconfig-0.4.5/tests/unit/processing/test_type_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
         _parse_type(desc)
     desc = ("None||float")
     with pytest.raises(ValueError, match=f"Unknown type: '{desc}'"):
         _parse_type(desc)
     desc = ("Dict[str, Union[List[None|float], Dict[bool, Optional[int]]]]|List[Any]|"
             "Dict[List[int], Optional[Dict[str, float]]]|flsoat")  # flsoat != float
     with pytest.raises(ValueError, match=f"Unknown type: '{desc}'"):
-        print(_parse_type(desc))
+        _parse_type(desc)
```

### Comparing `cliconfig-0.4.4/tests/unit/test_build_config.py` & `cliconfig-0.4.5/tests/unit/test_build_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 def test_make_config(capsys: pytest.CaptureFixture) -> None:
     """Test make_config."""
     sys_argv = sys.argv.copy()
     sys.argv = [
         "tests/test_make_config.py.py",
         "--config",
         "tests/configs/config1.yaml,tests/configs/config2.yaml",
-        "--param2",
-        "6",
+        "--unknown",
+        "--param2=6",
+        "--unknown2=8",  # check that not error but a warning in console
     ]
     capsys.readouterr()  # Clear stdout and stderr
     config, _ = make_config(
         "tests/configs/default1.yaml",
         "tests/configs/default2.yaml"
     )
     captured = capsys.readouterr()
@@ -32,16 +33,19 @@
             "letter1": "f",
             "letter2": "e",
             "letter3": "c",
             "letter4": "d",
         },
     }
     expected_out = (
-        "[CONFIG] Merge 2 default configs, "
-        "2 additional configs and 1 CLI parameter(s).\n"
+        "[CONFIG] Warning: New keys found in CLI parameters that will not be merged:\n"
+        "  - unknown\n"
+        "  - unknown2\n"
+        "[CONFIG] Info: Merged 2 default config(s), "
+        "2 additional config(s) and 1 CLI parameter(s).\n"
     )
     check.equal(config, expected_config)
     check.equal(out, expected_out)
 
     # No additional configs
     sys.argv = [
         "tests/test_make_config.py.py",
```

### Comparing `cliconfig-0.4.4/tests/unit/test_dict_routines.py` & `cliconfig-0.4.5/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/unit/test_process_routines.py` & `cliconfig-0.4.5/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.4/tests/unit/test_tag_routines.py` & `cliconfig-0.4.5/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*


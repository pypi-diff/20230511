# Comparing `tmp/edulint-2.6.2.tar.gz` & `tmp/edulint-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-k_9gbewx/edulint-2.6.2.tar", last modified: Tue May  9 18:06:24 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-1lonfx5m/edulint-2.6.3.tar", last modified: Wed May 10 20:05:19 2023, max compression
```

## Comparing `edulint-2.6.2.tar` & `edulint-2.6.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 18:06:09.000000 edulint-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-09 18:06:24.000000 edulint-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-09 18:06:09.000000 edulint-2.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/config_translations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 18:06:09.000000 edulint-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 18:06:24.000000 edulint-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 18:06:09.000000 edulint-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 20:05:02.000000 edulint-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-10 20:05:19.000000 edulint-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-10 20:05:02.000000 edulint-2.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/config/config_translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-10 20:05:02.000000 edulint-2.6.3/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 20:05:19.000000 edulint-2.6.3/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 20:05:02.000000 edulint-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 20:05:19.000000 edulint-2.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-10 20:05:02.000000 edulint-2.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:05:19.000000 edulint-2.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-10 20:05:02.000000 edulint-2.6.3/tests/test_visitors.py
```

### Comparing `edulint-2.6.2/LICENSE` & `edulint-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/PKG-INFO` & `edulint-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.6.2
+Version: 2.6.3
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.6.2/README.md` & `edulint-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/config/config.py` & `edulint-2.6.3/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/config/config_translations.py` & `edulint-2.6.3/edulint/config/config_translations.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/edulint.py` & `edulint-2.6.3/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/explanations.toml` & `edulint-2.6.3/edulint/explanations.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8955,2317 +8955,2942 @@
 00022fa0: 5f64 6570 7468 2864 6570 7468 293a 0a20  _depth(depth):. 
 00022fb0: 2020 2020 2020 205c 225c 225c 2246 756e         \"\"\"Fun
 00022fc0: 6374 696f 6e20 6361 6c6c 6564 2077 6974  ction called wit
 00022fd0: 6820 2e62 6f72 655f 7769 7468 5f64 6570  h .bore_with_dep
 00022fe0: 7468 2864 6570 7468 292e 5c22 5c22 5c22  th(depth).\"\"\"
 00022ff0: 0a20 2020 2020 2020 2070 6173 730a 0a60  .        pass..`
 00023000: 6060 0a22 2222 0a0a 5b52 3631 3031 5d0a  ``."""..[R6101].
-00023010: 7768 7920 3d20 2249 7420 6c6f 6f6b 7320  why = "It looks 
-00023020: 6c69 6b65 2064 6963 7469 6f6e 6172 7920  like dictionary 
-00023030: 7661 6c75 6573 2063 616e 2062 6520 7265  values can be re
-00023040: 706c 6163 6564 2062 7920 6e61 6d65 6474  placed by namedt
-00023050: 7570 6c65 7320 6f72 2064 6174 6163 6c61  uples or datacla
-00023060: 7373 2069 6e73 7461 6e63 6573 2e22 0a65  ss instances.".e
-00023070: 7861 6d70 6c65 7320 3d20 223c 6120 6872  xamples = "<a hr
-00023080: 6566 3d5c 2268 7474 7073 3a2f 2f70 796c  ef=\"https://pyl
-00023090: 696e 742e 7079 6371 612e 6f72 672f 656e  int.pycqa.org/en
-000230a0: 2f6c 6174 6573 742f 7573 6572 5f67 7569  /latest/user_gui
-000230b0: 6465 2f6d 6573 7361 6765 732f 7265 6661  de/messages/refa
-000230c0: 6374 6f72 2f63 6f6e 7369 6465 722d 7573  ctor/consider-us
-000230d0: 696e 672d 6e61 6d65 6474 7570 6c65 2d6f  ing-namedtuple-o
-000230e0: 722d 6461 7461 636c 6173 732e 6874 6d6c  r-dataclass.html
-000230f0: 5c22 3e41 6464 6974 696f 6e61 6c20 696e  \">Additional in
-00023100: 666f 726d 6174 696f 6e3c 2f61 3e22 0a0a  formation</a>"..
-00023110: 5b52 3631 3032 5d0a 7768 7920 3d20 224f  [R6102].why = "O
-00023120: 6e6c 7920 666f 7220 7374 796c 6520 636f  nly for style co
-00023130: 6e73 6973 7465 6e63 7921 2045 6d69 7474  nsistency! Emitt
-00023140: 6564 2077 6865 7265 2061 6e20 696e 2d70  ed where an in-p
-00023150: 6c61 6365 2064 6566 696e 6564 2060 606c  lace defined ``l
-00023160: 6973 7460 6020 6361 6e20 6265 2072 6570  ist`` can be rep
-00023170: 6c61 6365 6420 6279 2061 2060 6074 7570  laced by a ``tup
-00023180: 6c65 6060 2e20 4475 6520 746f 206f 7074  le``. Due to opt
-00023190: 696d 697a 6174 696f 6e73 2062 7920 4350  imizations by CP
-000231a0: 7974 686f 6e2c 2074 6865 7265 2069 7320  ython, there is 
-000231b0: 6e6f 2070 6572 666f 726d 616e 6365 2062  no performance b
-000231c0: 656e 6566 6974 2066 726f 6d20 6974 2e22  enefit from it."
-000231d0: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
-000231e0: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
-000231f0: 6465 2a2a 0a0a 6060 6070 790a 666f 7220  de**..```py.for 
-00023200: 6920 696e 205b 312c 2032 2c20 335d 3a20  i in [1, 2, 3]: 
-00023210: 2023 205b 636f 6e73 6964 6572 2d75 7369   # [consider-usi
-00023220: 6e67 2d74 7570 6c65 5d0a 2020 2020 7072  ng-tuple].    pr
-00023230: 696e 7428 6929 0a0a 6060 600a 0a2a 2a48  int(i)..```..**H
-00023240: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
-00023250: 6060 6070 790a 666f 7220 6920 696e 2028  ```py.for i in (
-00023260: 312c 2032 2c20 3329 3a0a 2020 2020 7072  1, 2, 3):.    pr
-00023270: 696e 7428 6929 0a0a 6060 600a 2222 220a  int(i)..```.""".
-00023280: 0a5b 5236 3130 335d 0a77 6879 203d 2022  .[R6103].why = "
-00023290: 4974 206c 6f6f 6b73 206c 696b 6520 7468  It looks like th
-000232a0: 6520 6966 2061 7373 6967 6e6d 656e 7420  e if assignment 
-000232b0: 6973 2064 6972 6563 746c 7920 666f 6c6c  is directly foll
-000232c0: 6f77 6564 2062 7920 616e 2069 6620 7374  owed by an if st
-000232d0: 6174 656d 656e 7420 616e 6420 626f 7468  atement and both
-000232e0: 2063 616e 2062 6520 636f 6d62 696e 6564   can be combined
-000232f0: 2062 7920 7573 696e 6720 616e 2061 7373   by using an ass
-00023300: 6967 6e6d 656e 7420 6578 7072 6573 7369  ignment expressi
-00023310: 6f6e 2060 603a 3d60 602e 2052 6571 7569  on ``:=``. Requi
-00023320: 7265 7320 5079 7468 6f6e 2033 2e38 2061  res Python 3.8 a
-00023330: 6e64 2060 6070 792d 7665 7273 696f 6e20  nd ``py-version 
-00023340: 3e3d 2033 2e38 6060 2e22 0a65 7861 6d70  >= 3.8``.".examp
-00023350: 6c65 7320 3d20 2222 220a 2a2a 5072 6f62  les = """.**Prob
-00023360: 6c65 6d61 7469 6320 636f 6465 2a2a 0a0a  lematic code**..
-00023370: 6060 6070 790a 6170 706c 6573 203d 2032  ```py.apples = 2
-00023380: 0a0a 6966 2061 7070 6c65 733a 2020 2320  ..if apples:  # 
-00023390: 5b63 6f6e 7369 6465 722d 7573 696e 672d  [consider-using-
-000233a0: 6173 7369 676e 6d65 6e74 2d65 7870 725d  assignment-expr]
-000233b0: 0a20 2020 2070 7269 6e74 285c 2247 6f64  .    print(\"God
-000233c0: 2061 7070 6c65 7321 5c22 290a 0a60 6060   apples!\")..```
-000233d0: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
-000233e0: 742a 2a0a 0a60 6060 7079 0a69 6620 6170  t**..```py.if ap
-000233f0: 706c 6573 203a 3d20 323a 0a20 2020 2070  ples := 2:.    p
-00023400: 7269 6e74 285c 2247 6f64 2061 7070 6c65  rint(\"God apple
-00023410: 7321 5c22 290a 0a60 6060 0a22 2222 0a0a  s!\")..```."""..
-00023420: 5b52 3536 3031 5d0a 7768 7920 3d20 2249  [R5601].why = "I
-00023430: 7420 6c6f 6f6b 7320 6c69 6b65 2074 6865  t looks like the
-00023440: 2065 6c69 6620 7374 6174 656d 656e 7420   elif statement 
-00023450: 666f 6c6c 6f77 7320 7269 6768 7420 6166  follows right af
-00023460: 7465 7220 616e 2069 6e64 656e 7465 6420  ter an indented 
-00023470: 626c 6f63 6b20 7768 6963 6820 6974 7365  block which itse
-00023480: 6c66 2065 6e64 7320 7769 7468 2069 6620  lf ends with if 
-00023490: 6f72 2065 6c69 662e 2049 7420 6d61 7920  or elif. It may 
-000234a0: 6e6f 7420 6265 206f 7669 6f75 7320 6966  not be ovious if
-000234b0: 2074 6865 2065 6c69 6620 7374 6174 656d   the elif statem
-000234c0: 656e 7420 7761 7320 7769 6c6c 696e 676c  ent was willingl
-000234d0: 7920 6f72 206d 6973 7461 6b65 6e6c 7920  y or mistakenly 
-000234e0: 756e 696e 6465 6e74 6564 2e20 4578 7472  unindented. Extr
-000234f0: 6163 7469 6e67 2074 6865 2069 6e64 656e  acting the inden
-00023500: 7465 6420 6966 2073 7461 7465 6d65 6e74  ted if statement
-00023510: 2069 6e74 6f20 6120 7365 7061 7261 7465   into a separate
-00023520: 2066 756e 6374 696f 6e20 6d69 6768 7420   function might 
-00023530: 6176 6f69 6420 636f 6e66 7573 696f 6e20  avoid confusion 
-00023540: 616e 6420 7072 6576 656e 7420 6572 726f  and prevent erro
-00023550: 7273 2e22 0a65 7861 6d70 6c65 7320 3d20  rs.".examples = 
-00023560: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
-00023570: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
-00023580: 6465 6620 6d79 6675 6e63 2873 6861 6c6c  def myfunc(shall
-00023590: 5f63 6f6e 7469 6e75 653a 2062 6f6f 6c2c  _continue: bool,
-000235a0: 2073 6861 6c6c 5f65 7869 743a 2062 6f6f   shall_exit: boo
-000235b0: 6c29 3a0a 2020 2020 6966 2073 6861 6c6c  l):.    if shall
-000235c0: 5f63 6f6e 7469 6e75 653a 0a20 2020 2020  _continue:.     
-000235d0: 2020 2069 6620 696e 7075 7428 5c22 4172     if input(\"Ar
-000235e0: 6520 796f 7520 7375 7265 3f5c 2229 203d  e you sure?\") =
-000235f0: 3d20 5c22 795c 223a 0a20 2020 2020 2020  = \"y\":.       
-00023600: 2020 2020 2070 7269 6e74 285c 224d 6f76       print(\"Mov
-00023610: 696e 6720 6f6e 2e5c 2229 0a20 2020 2065  ing on.\").    e
-00023620: 6c69 6620 7368 616c 6c5f 6578 6974 3a20  lif shall_exit: 
-00023630: 2023 205b 636f 6e66 7573 696e 672d 636f   # [confusing-co
-00023640: 6e73 6563 7574 6976 652d 656c 6966 5d0a  nsecutive-elif].
-00023650: 2020 2020 2020 2020 7072 696e 7428 5c22          print(\"
-00023660: 4578 6974 696e 672e 5c22 290a 0a60 6060  Exiting.\")..```
-00023670: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
-00023680: 742a 2a0a 0a60 6060 7079 0a23 204f 7074  t**..```py.# Opt
-00023690: 696f 6e20 313a 2061 6464 2065 7870 6c69  ion 1: add expli
-000236a0: 6369 7420 2765 6c73 6527 0a64 6566 206d  cit 'else'.def m
-000236b0: 7966 756e 6328 7368 616c 6c5f 636f 6e74  yfunc(shall_cont
-000236c0: 696e 7565 3a20 626f 6f6c 2c20 7368 616c  inue: bool, shal
-000236d0: 6c5f 6578 6974 3a20 626f 6f6c 293a 0a20  l_exit: bool):. 
-000236e0: 2020 2069 6620 7368 616c 6c5f 636f 6e74     if shall_cont
-000236f0: 696e 7565 3a0a 2020 2020 2020 2020 6966  inue:.        if
-00023700: 2069 6e70 7574 285c 2241 7265 2079 6f75   input(\"Are you
-00023710: 2073 7572 653f 5c22 2920 3d3d 205c 2279   sure?\") == \"y
-00023720: 5c22 3a0a 2020 2020 2020 2020 2020 2020  \":.            
-00023730: 7072 696e 7428 5c22 4d6f 7669 6e67 206f  print(\"Moving o
-00023740: 6e2e 5c22 290a 2020 2020 2020 2020 656c  n.\").        el
-00023750: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00023760: 7061 7373 0a20 2020 2065 6c69 6620 7368  pass.    elif sh
-00023770: 616c 6c5f 6578 6974 3a0a 2020 2020 2020  all_exit:.      
-00023780: 2020 7072 696e 7428 5c22 4578 6974 696e    print(\"Exitin
-00023790: 672e 5c22 290a 0a0a 2320 4f70 7469 6f6e  g.\")...# Option
-000237a0: 2032 3a20 6578 7472 6163 7420 6675 6e63   2: extract func
-000237b0: 7469 6f6e 0a64 6566 2075 7365 725f 636f  tion.def user_co
-000237c0: 6e66 6972 6d61 7469 6f6e 2829 3a0a 2020  nfirmation():.  
-000237d0: 2020 6966 2069 6e70 7574 285c 2241 7265    if input(\"Are
-000237e0: 2079 6f75 2073 7572 653f 5c22 2920 3d3d   you sure?\") ==
-000237f0: 205c 2279 5c22 3a0a 2020 2020 2020 2020   \"y\":.        
-00023800: 7072 696e 7428 5c22 4d6f 7669 6e67 206f  print(\"Moving o
-00023810: 6e2e 5c22 290a 0a0a 6465 6620 6d79 6675  n.\")...def myfu
-00023820: 6e63 3228 7368 616c 6c5f 636f 6e74 696e  nc2(shall_contin
-00023830: 7565 3a20 626f 6f6c 2c20 7368 616c 6c5f  ue: bool, shall_
-00023840: 6578 6974 3a20 626f 6f6c 293a 0a20 2020  exit: bool):.   
-00023850: 2069 6620 7368 616c 6c5f 636f 6e74 696e   if shall_contin
-00023860: 7565 3a0a 2020 2020 2020 2020 7573 6572  ue:.        user
-00023870: 5f63 6f6e 6669 726d 6174 696f 6e28 290a  _confirmation().
-00023880: 2020 2020 656c 6966 2073 6861 6c6c 5f65      elif shall_e
-00023890: 7869 743a 0a20 2020 2020 2020 2070 7269  xit:.        pri
-000238a0: 6e74 285c 2245 7869 7469 6e67 2e5c 2229  nt(\"Exiting.\")
-000238b0: 0a0a 6060 600a 0a3c 6120 6872 6566 3d5c  ..```..<a href=\
-000238c0: 2268 7474 7073 3a2f 2f70 796c 696e 742e  "https://pylint.
-000238d0: 7079 6371 612e 6f72 672f 656e 2f6c 6174  pycqa.org/en/lat
-000238e0: 6573 742f 7573 6572 5f67 7569 6465 2f6d  est/user_guide/m
-000238f0: 6573 7361 6765 732f 7265 6661 6374 6f72  essages/refactor
-00023900: 2f63 6f6e 6675 7369 6e67 2d63 6f6e 7365  /confusing-conse
-00023910: 6375 7469 7665 2d65 6c69 662e 6874 6d6c  cutive-elif.html
-00023920: 5c22 3e41 6464 6974 696f 6e61 6c20 696e  \">Additional in
-00023930: 666f 726d 6174 696f 6e3c 2f61 3e22 2222  formation</a>"""
-00023940: 0a0a 5b52 3535 3031 5d0a 7768 7920 3d20  ..[R5501].why = 
-00023950: 2249 7420 6c6f 6f6b 7320 6c69 6b65 2074  "It looks like t
-00023960: 6865 2065 6c73 6520 7374 6174 656d 656e  he else statemen
-00023970: 7420 6973 2069 6d6d 6564 6961 7465 6c79  t is immediately
-00023980: 2066 6f6c 6c6f 7765 6420 6279 2061 6e20   followed by an 
-00023990: 6966 2073 7461 7465 6d65 6e74 2061 6e64  if statement and
-000239a0: 2064 6f65 7320 6e6f 7420 636f 6e74 6169   does not contai
-000239b0: 6e20 7374 6174 656d 656e 7473 2074 6861  n statements tha
-000239c0: 7420 776f 756c 6420 6265 2075 6e72 656c  t would be unrel
-000239d0: 6174 6564 2074 6f20 6974 2e22 0a65 7861  ated to it.".exa
-000239e0: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
-000239f0: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
-00023a00: 0a0a 6060 6070 790a 6966 2069 6e70 7574  ..```py.if input
-00023a10: 2829 3a0a 2020 2020 7061 7373 0a65 6c73  ():.    pass.els
-00023a20: 653a 0a20 2020 2069 6620 6c65 6e28 696e  e:.    if len(in
-00023a30: 7075 7428 2929 203e 3d20 3130 3a20 2023  put()) >= 10:  #
-00023a40: 205b 656c 7365 2d69 662d 7573 6564 5d0a   [else-if-used].
-00023a50: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00023a60: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
-00023a70: 6173 730a 0a60 6060 0a0a 2a2a 486f 7720  ass..```..**How 
-00023a80: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
-00023a90: 7079 0a69 6620 696e 7075 7428 293a 0a20  py.if input():. 
-00023aa0: 2020 2070 6173 730a 656c 6966 206c 656e     pass.elif len
-00023ab0: 2869 6e70 7574 2829 2920 3e3d 2031 303a  (input()) >= 10:
-00023ac0: 0a20 2020 2070 6173 730a 656c 7365 3a0a  .    pass.else:.
-00023ad0: 2020 2020 7061 7373 0a0a 6060 600a 2222      pass..```.""
-00023ae0: 220a 0a5b 5230 3430 315d 0a77 6879 203d  "..[R0401].why =
-00023af0: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
-00023b00: 7468 6520 6379 636c 6963 2069 6d70 6f72  the cyclic impor
-00023b10: 7420 6265 7477 6565 6e20 7477 6f20 6f72  t between two or
-00023b20: 206d 6f72 6520 6d6f 6475 6c65 7320 6973   more modules is
-00023b30: 2064 6574 6563 7465 642e 220a 6578 616d   detected.".exam
-00023b40: 706c 6573 203d 2022 3c61 2068 7265 663d  ples = "<a href=
-00023b50: 5c22 6874 7470 733a 2f2f 7079 6c69 6e74  \"https://pylint
-00023b60: 2e70 7963 7161 2e6f 7267 2f65 6e2f 6c61  .pycqa.org/en/la
-00023b70: 7465 7374 2f75 7365 725f 6775 6964 652f  test/user_guide/
-00023b80: 6d65 7373 6167 6573 2f72 6566 6163 746f  messages/refacto
-00023b90: 722f 6379 636c 6963 2d69 6d70 6f72 742e  r/cyclic-import.
-00023ba0: 6874 6d6c 5c22 3e41 6464 6974 696f 6e61  html\">Additiona
-00023bb0: 6c20 696e 666f 726d 6174 696f 6e3c 2f61  l information</a
-00023bc0: 3e22 0a0a 5b52 3034 3032 5d0a 7768 7920  >"..[R0402].why 
-00023bd0: 3d20 2249 7420 6c6f 6f6b 7320 6c69 6b65  = "It looks like
-00023be0: 2074 6865 2073 7562 6d6f 6475 6c65 206f   the submodule o
-00023bf0: 6620 6120 7061 636b 6167 6520 6973 2069  f a package is i
-00023c00: 6d70 6f72 7465 6420 616e 6420 616c 6961  mported and alia
-00023c10: 7365 6420 7769 7468 2074 6865 2073 616d  sed with the sam
-00023c20: 6520 6e61 6d65 2e20 452e 672e 2c20 696e  e name. E.g., in
-00023c30: 7374 6561 6420 6f66 2060 6069 6d70 6f72  stead of ``impor
-00023c40: 7420 636f 6e63 7572 7265 6e74 2e66 7574  t concurrent.fut
-00023c50: 7572 6573 2061 7320 6675 7475 7265 7360  ures as futures`
-00023c60: 6020 7573 6520 6060 6672 6f6d 2063 6f6e  ` use ``from con
-00023c70: 6375 7272 656e 7420 696d 706f 7274 2066  current import f
-00023c80: 7574 7572 6573 6060 220a 6578 616d 706c  utures``".exampl
-00023c90: 6573 203d 2022 2222 0a2a 2a50 726f 626c  es = """.**Probl
-00023ca0: 656d 6174 6963 2063 6f64 652a 2a0a 0a60  ematic code**..`
-00023cb0: 6060 7079 0a69 6d70 6f72 7420 6f73 2e70  ``py.import os.p
-00023cc0: 6174 6820 6173 2070 6174 6820 2023 205b  ath as path  # [
-00023cd0: 636f 6e73 6964 6572 2d75 7369 6e67 2d66  consider-using-f
-00023ce0: 726f 6d2d 696d 706f 7274 5d0a 0a60 6060  rom-import]..```
-00023cf0: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
-00023d00: 742a 2a0a 0a60 6060 7079 0a66 726f 6d20  t**..```py.from 
-00023d10: 6f73 2069 6d70 6f72 7420 7061 7468 0a0a  os import path..
-00023d20: 6060 600a 2222 220a 0a5b 5230 3230 345d  ```."""..[R0204]
-00023d30: 0a77 6879 203d 2022 4974 206c 6f6f 6b73  .why = "It looks
-00023d40: 206c 696b 6520 7468 6520 7479 7065 206f   like the type o
-00023d50: 6620 6120 7661 7269 6162 6c65 2063 6861  f a variable cha
-00023d60: 6e67 6573 2069 6e73 6964 6520 6120 6d65  nges inside a me
-00023d70: 7468 6f64 206f 7220 6120 6675 6e63 7469  thod or a functi
-00023d80: 6f6e 2e22 0a65 7861 6d70 6c65 7320 3d20  on.".examples = 
+00023010: 7768 7920 3d20 2259 6f75 2073 686f 756c  why = "You shoul
+00023020: 6420 7573 6520 5079 7468 6f6e 2066 6f72  d use Python for
+00023030: 6561 6368 2d73 7479 6c65 206c 6f6f 7020  each-style loop 
+00023040: 696e 7374 6561 6420 6f66 2069 7465 7261  instead of itera
+00023050: 7469 6e67 2074 6872 6f75 6768 2069 6e64  ting through ind
+00023060: 6963 6573 2062 6563 6175 7365 2069 7427  ices because it'
+00023070: 7320 6561 7369 6572 2074 6f20 7265 6164  s easier to read
+00023080: 2c20 616e 6420 6c65 7373 2070 726f 6e65  , and less prone
+00023090: 2074 6f20 6f66 662d 6279 2d6f 6e65 2065   to off-by-one e
+000230a0: 7272 6f72 732e 2041 6c73 6f2c 2079 6f75  rrors. Also, you
+000230b0: 2064 6f20 6e6f 7420 6861 7665 2074 6f20   do not have to 
+000230c0: 696e 6465 7820 7468 6520 6c69 7374 2c20  index the list, 
+000230d0: 7369 6e63 6520 796f 7520 6361 6e20 7573  since you can us
+000230e0: 6520 7468 6520 7661 6c75 6520 6469 7265  e the value dire
+000230f0: 6374 6c79 2e22 0a65 7861 6d70 6c65 7320  ctly.".examples 
+00023100: 3d20 2222 220a 6060 6070 790a 6672 7569  = """.```py.frui
+00023110: 7473 203d 205b 2761 7070 6c65 272c 2027  ts = ['apple', '
+00023120: 6261 6e61 6e61 272c 2027 6368 6572 7279  banana', 'cherry
+00023130: 275d 0a0a 6465 6620 7072 6f62 6c65 6d61  ']..def problema
+00023140: 7469 6328 6672 7569 7473 293a 0a20 2020  tic(fruits):.   
+00023150: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00023160: 6c65 6e28 6672 7569 7473 2929 3a0a 2020  len(fruits)):.  
+00023170: 2020 2020 2020 7072 696e 7428 6672 7569        print(frui
+00023180: 7473 5b69 5d29 0a0a 6465 6620 676f 6f64  ts[i])..def good
+00023190: 2866 7275 6974 7329 3a0a 2020 2020 666f  (fruits):.    fo
+000231a0: 7220 6672 7569 7420 696e 2066 7275 6974  r fruit in fruit
+000231b0: 733a 0a20 2020 2020 2020 2070 7269 6e74  s:.        print
+000231c0: 2866 7275 6974 290a 6060 600a 2222 220a  (fruit).```.""".
+000231d0: 0a5b 5236 3130 325d 0a77 6879 203d 2022  .[R6102].why = "
+000231e0: 596f 7520 7368 6f75 6c64 2075 7365 2065  You should use e
+000231f0: 6e75 6d65 7261 7465 2069 6e73 7465 6164  numerate instead
+00023200: 206f 6620 6974 6572 6174 696e 6720 7468   of iterating th
+00023210: 726f 7567 6820 696e 6469 6365 7320 6265  rough indices be
+00023220: 6361 7573 6520 6974 2773 206d 6f72 6520  cause it's more 
+00023230: 636f 6e63 6973 652e 2049 7420 7072 6576  concise. It prev
+00023240: 656e 7473 2079 6f75 2066 726f 6d20 696e  ents you from in
+00023250: 7472 6f64 7563 696e 6720 6f66 662d 6279  troducing off-by
+00023260: 2d6f 6e65 2065 7272 6f72 7320 616e 6420  -one errors and 
+00023270: 616c 6c6f 7773 2079 6f75 2074 6f20 6e61  allows you to na
+00023280: 6d65 2074 6865 2069 7465 6d73 220a 6578  me the items".ex
+00023290: 616d 706c 6573 203d 2022 2222 0a60 6060  amples = """.```
+000232a0: 7079 0a66 7275 6974 7320 3d20 5b27 6170  py.fruits = ['ap
+000232b0: 706c 6527 2c20 2762 616e 616e 6127 2c20  ple', 'banana', 
+000232c0: 2763 6865 7272 7927 5d0a 0a64 6566 2070  'cherry']..def p
+000232d0: 726f 626c 656d 6174 6963 2866 7275 6974  roblematic(fruit
+000232e0: 7329 3a0a 2020 2020 666f 7220 6920 696e  s):.    for i in
+000232f0: 2072 616e 6765 286c 656e 2866 7275 6974   range(len(fruit
+00023300: 7329 293a 0a20 2020 2020 2020 2070 7269  s)):.        pri
+00023310: 6e74 2869 2c20 6672 7569 7473 5b69 5d29  nt(i, fruits[i])
+00023320: 0a0a 6465 6620 676f 6f64 2866 7275 6974  ..def good(fruit
+00023330: 7329 3a0a 2020 2020 666f 7220 692c 2066  s):.    for i, f
+00023340: 7275 6974 2069 6e20 656e 756d 6572 6174  ruit in enumerat
+00023350: 6528 6672 7569 7473 293a 0a20 2020 2020  e(fruits):.     
+00023360: 2020 2070 7269 6e74 2869 2c20 6672 7569     print(i, frui
+00023370: 7429 0a60 6060 0a22 2222 0a0a 5b52 3631  t).```."""..[R61
+00023380: 3033 5d0a 7768 7920 3d20 2249 7420 6c6f  03].why = "It lo
+00023390: 6f6b 7320 6c69 6b65 2074 6865 2069 6620  oks like the if 
+000233a0: 6173 7369 676e 6d65 6e74 2069 7320 6469  assignment is di
+000233b0: 7265 6374 6c79 2066 6f6c 6c6f 7765 6420  rectly followed 
+000233c0: 6279 2061 6e20 6966 2073 7461 7465 6d65  by an if stateme
+000233d0: 6e74 2061 6e64 2062 6f74 6820 6361 6e20  nt and both can 
+000233e0: 6265 2063 6f6d 6269 6e65 6420 6279 2075  be combined by u
+000233f0: 7369 6e67 2061 6e20 6173 7369 676e 6d65  sing an assignme
+00023400: 6e74 2065 7870 7265 7373 696f 6e20 6060  nt expression ``
+00023410: 3a3d 6060 2e20 5265 7175 6972 6573 2050  :=``. Requires P
+00023420: 7974 686f 6e20 332e 3820 616e 6420 6060  ython 3.8 and ``
+00023430: 7079 2d76 6572 7369 6f6e 203e 3d20 332e  py-version >= 3.
+00023440: 3860 602e 220a 6578 616d 706c 6573 203d  8``.".examples =
+00023450: 2022 2222 0a2a 2a50 726f 626c 656d 6174   """.**Problemat
+00023460: 6963 2063 6f64 652a 2a0a 0a60 6060 7079  ic code**..```py
+00023470: 0a61 7070 6c65 7320 3d20 320a 0a69 6620  .apples = 2..if 
+00023480: 6170 706c 6573 3a20 2023 205b 636f 6e73  apples:  # [cons
+00023490: 6964 6572 2d75 7369 6e67 2d61 7373 6967  ider-using-assig
+000234a0: 6e6d 656e 742d 6578 7072 5d0a 2020 2020  nment-expr].    
+000234b0: 7072 696e 7428 5c22 476f 6420 6170 706c  print(\"God appl
+000234c0: 6573 215c 2229 0a0a 6060 600a 0a2a 2a48  es!\")..```..**H
+000234d0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+000234e0: 6060 6070 790a 6966 2061 7070 6c65 7320  ```py.if apples 
+000234f0: 3a3d 2032 3a0a 2020 2020 7072 696e 7428  := 2:.    print(
+00023500: 5c22 476f 6420 6170 706c 6573 215c 2229  \"God apples!\")
+00023510: 0a0a 6060 600a 2222 220a 0a5b 5235 3630  ..```."""..[R560
+00023520: 315d 0a77 6879 203d 2022 4974 206c 6f6f  1].why = "It loo
+00023530: 6b73 206c 696b 6520 7468 6520 656c 6966  ks like the elif
+00023540: 2073 7461 7465 6d65 6e74 2066 6f6c 6c6f   statement follo
+00023550: 7773 2072 6967 6874 2061 6674 6572 2061  ws right after a
+00023560: 6e20 696e 6465 6e74 6564 2062 6c6f 636b  n indented block
+00023570: 2077 6869 6368 2069 7473 656c 6620 656e   which itself en
+00023580: 6473 2077 6974 6820 6966 206f 7220 656c  ds with if or el
+00023590: 6966 2e20 4974 206d 6179 206e 6f74 2062  if. It may not b
+000235a0: 6520 6f76 696f 7573 2069 6620 7468 6520  e ovious if the 
+000235b0: 656c 6966 2073 7461 7465 6d65 6e74 2077  elif statement w
+000235c0: 6173 2077 696c 6c69 6e67 6c79 206f 7220  as willingly or 
+000235d0: 6d69 7374 616b 656e 6c79 2075 6e69 6e64  mistakenly unind
+000235e0: 656e 7465 642e 2045 7874 7261 6374 696e  ented. Extractin
+000235f0: 6720 7468 6520 696e 6465 6e74 6564 2069  g the indented i
+00023600: 6620 7374 6174 656d 656e 7420 696e 746f  f statement into
+00023610: 2061 2073 6570 6172 6174 6520 6675 6e63   a separate func
+00023620: 7469 6f6e 206d 6967 6874 2061 766f 6964  tion might avoid
+00023630: 2063 6f6e 6675 7369 6f6e 2061 6e64 2070   confusion and p
+00023640: 7265 7665 6e74 2065 7272 6f72 732e 220a  revent errors.".
+00023650: 6578 616d 706c 6573 203d 2022 2222 0a2a  examples = """.*
+00023660: 2a50 726f 626c 656d 6174 6963 2063 6f64  *Problematic cod
+00023670: 652a 2a0a 0a60 6060 7079 0a64 6566 206d  e**..```py.def m
+00023680: 7966 756e 6328 7368 616c 6c5f 636f 6e74  yfunc(shall_cont
+00023690: 696e 7565 3a20 626f 6f6c 2c20 7368 616c  inue: bool, shal
+000236a0: 6c5f 6578 6974 3a20 626f 6f6c 293a 0a20  l_exit: bool):. 
+000236b0: 2020 2069 6620 7368 616c 6c5f 636f 6e74     if shall_cont
+000236c0: 696e 7565 3a0a 2020 2020 2020 2020 6966  inue:.        if
+000236d0: 2069 6e70 7574 285c 2241 7265 2079 6f75   input(\"Are you
+000236e0: 2073 7572 653f 5c22 2920 3d3d 205c 2279   sure?\") == \"y
+000236f0: 5c22 3a0a 2020 2020 2020 2020 2020 2020  \":.            
+00023700: 7072 696e 7428 5c22 4d6f 7669 6e67 206f  print(\"Moving o
+00023710: 6e2e 5c22 290a 2020 2020 656c 6966 2073  n.\").    elif s
+00023720: 6861 6c6c 5f65 7869 743a 2020 2320 5b63  hall_exit:  # [c
+00023730: 6f6e 6675 7369 6e67 2d63 6f6e 7365 6375  onfusing-consecu
+00023740: 7469 7665 2d65 6c69 665d 0a20 2020 2020  tive-elif].     
+00023750: 2020 2070 7269 6e74 285c 2245 7869 7469     print(\"Exiti
+00023760: 6e67 2e5c 2229 0a0a 6060 600a 0a2a 2a48  ng.\")..```..**H
+00023770: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00023780: 6060 6070 790a 2320 4f70 7469 6f6e 2031  ```py.# Option 1
+00023790: 3a20 6164 6420 6578 706c 6963 6974 2027  : add explicit '
+000237a0: 656c 7365 270a 6465 6620 6d79 6675 6e63  else'.def myfunc
+000237b0: 2873 6861 6c6c 5f63 6f6e 7469 6e75 653a  (shall_continue:
+000237c0: 2062 6f6f 6c2c 2073 6861 6c6c 5f65 7869   bool, shall_exi
+000237d0: 743a 2062 6f6f 6c29 3a0a 2020 2020 6966  t: bool):.    if
+000237e0: 2073 6861 6c6c 5f63 6f6e 7469 6e75 653a   shall_continue:
+000237f0: 0a20 2020 2020 2020 2069 6620 696e 7075  .        if inpu
+00023800: 7428 5c22 4172 6520 796f 7520 7375 7265  t(\"Are you sure
+00023810: 3f5c 2229 203d 3d20 5c22 795c 223a 0a20  ?\") == \"y\":. 
+00023820: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00023830: 285c 224d 6f76 696e 6720 6f6e 2e5c 2229  (\"Moving on.\")
+00023840: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00023850: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00023860: 2020 2020 656c 6966 2073 6861 6c6c 5f65      elif shall_e
+00023870: 7869 743a 0a20 2020 2020 2020 2070 7269  xit:.        pri
+00023880: 6e74 285c 2245 7869 7469 6e67 2e5c 2229  nt(\"Exiting.\")
+00023890: 0a0a 0a23 204f 7074 696f 6e20 323a 2065  ...# Option 2: e
+000238a0: 7874 7261 6374 2066 756e 6374 696f 6e0a  xtract function.
+000238b0: 6465 6620 7573 6572 5f63 6f6e 6669 726d  def user_confirm
+000238c0: 6174 696f 6e28 293a 0a20 2020 2069 6620  ation():.    if 
+000238d0: 696e 7075 7428 5c22 4172 6520 796f 7520  input(\"Are you 
+000238e0: 7375 7265 3f5c 2229 203d 3d20 5c22 795c  sure?\") == \"y\
+000238f0: 223a 0a20 2020 2020 2020 2070 7269 6e74  ":.        print
+00023900: 285c 224d 6f76 696e 6720 6f6e 2e5c 2229  (\"Moving on.\")
+00023910: 0a0a 0a64 6566 206d 7966 756e 6332 2873  ...def myfunc2(s
+00023920: 6861 6c6c 5f63 6f6e 7469 6e75 653a 2062  hall_continue: b
+00023930: 6f6f 6c2c 2073 6861 6c6c 5f65 7869 743a  ool, shall_exit:
+00023940: 2062 6f6f 6c29 3a0a 2020 2020 6966 2073   bool):.    if s
+00023950: 6861 6c6c 5f63 6f6e 7469 6e75 653a 0a20  hall_continue:. 
+00023960: 2020 2020 2020 2075 7365 725f 636f 6e66         user_conf
+00023970: 6972 6d61 7469 6f6e 2829 0a20 2020 2065  irmation().    e
+00023980: 6c69 6620 7368 616c 6c5f 6578 6974 3a0a  lif shall_exit:.
+00023990: 2020 2020 2020 2020 7072 696e 7428 5c22          print(\"
+000239a0: 4578 6974 696e 672e 5c22 290a 0a60 6060  Exiting.\")..```
+000239b0: 0a0a 3c61 2068 7265 663d 5c22 6874 7470  ..<a href=\"http
+000239c0: 733a 2f2f 7079 6c69 6e74 2e70 7963 7161  s://pylint.pycqa
+000239d0: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f75  .org/en/latest/u
+000239e0: 7365 725f 6775 6964 652f 6d65 7373 6167  ser_guide/messag
+000239f0: 6573 2f72 6566 6163 746f 722f 636f 6e66  es/refactor/conf
+00023a00: 7573 696e 672d 636f 6e73 6563 7574 6976  using-consecutiv
+00023a10: 652d 656c 6966 2e68 746d 6c5c 223e 4164  e-elif.html\">Ad
+00023a20: 6469 7469 6f6e 616c 2069 6e66 6f72 6d61  ditional informa
+00023a30: 7469 6f6e 3c2f 613e 2222 220a 0a5b 5235  tion</a>"""..[R5
+00023a40: 3530 315d 0a77 6879 203d 2022 4974 206c  501].why = "It l
+00023a50: 6f6f 6b73 206c 696b 6520 7468 6520 656c  ooks like the el
+00023a60: 7365 2073 7461 7465 6d65 6e74 2069 7320  se statement is 
+00023a70: 696d 6d65 6469 6174 656c 7920 666f 6c6c  immediately foll
+00023a80: 6f77 6564 2062 7920 616e 2069 6620 7374  owed by an if st
+00023a90: 6174 656d 656e 7420 616e 6420 646f 6573  atement and does
+00023aa0: 206e 6f74 2063 6f6e 7461 696e 2073 7461   not contain sta
+00023ab0: 7465 6d65 6e74 7320 7468 6174 2077 6f75  tements that wou
+00023ac0: 6c64 2062 6520 756e 7265 6c61 7465 6420  ld be unrelated 
+00023ad0: 746f 2069 742e 220a 6578 616d 706c 6573  to it.".examples
+00023ae0: 203d 2022 2222 0a2a 2a50 726f 626c 656d   = """.**Problem
+00023af0: 6174 6963 2063 6f64 652a 2a0a 0a60 6060  atic code**..```
+00023b00: 7079 0a69 6620 696e 7075 7428 293a 0a20  py.if input():. 
+00023b10: 2020 2070 6173 730a 656c 7365 3a0a 2020     pass.else:.  
+00023b20: 2020 6966 206c 656e 2869 6e70 7574 2829    if len(input()
+00023b30: 2920 3e3d 2031 303a 2020 2320 5b65 6c73  ) >= 10:  # [els
+00023b40: 652d 6966 2d75 7365 645d 0a20 2020 2020  e-if-used].     
+00023b50: 2020 2070 6173 730a 2020 2020 656c 7365     pass.    else
+00023b60: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00023b70: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
+00023b80: 7820 6974 2a2a 0a0a 6060 6070 790a 6966  x it**..```py.if
+00023b90: 2069 6e70 7574 2829 3a0a 2020 2020 7061   input():.    pa
+00023ba0: 7373 0a65 6c69 6620 6c65 6e28 696e 7075  ss.elif len(inpu
+00023bb0: 7428 2929 203e 3d20 3130 3a0a 2020 2020  t()) >= 10:.    
+00023bc0: 7061 7373 0a65 6c73 653a 0a20 2020 2070  pass.else:.    p
+00023bd0: 6173 730a 0a60 6060 0a22 2222 0a0a 5b52  ass..```."""..[R
+00023be0: 3034 3031 5d0a 7768 7920 3d20 2249 7420  0401].why = "It 
+00023bf0: 6c6f 6f6b 7320 6c69 6b65 2074 6865 2063  looks like the c
+00023c00: 7963 6c69 6320 696d 706f 7274 2062 6574  yclic import bet
+00023c10: 7765 656e 2074 776f 206f 7220 6d6f 7265  ween two or more
+00023c20: 206d 6f64 756c 6573 2069 7320 6465 7465   modules is dete
+00023c30: 6374 6564 2e22 0a65 7861 6d70 6c65 7320  cted.".examples 
+00023c40: 3d20 223c 6120 6872 6566 3d5c 2268 7474  = "<a href=\"htt
+00023c50: 7073 3a2f 2f70 796c 696e 742e 7079 6371  ps://pylint.pycq
+00023c60: 612e 6f72 672f 656e 2f6c 6174 6573 742f  a.org/en/latest/
+00023c70: 7573 6572 5f67 7569 6465 2f6d 6573 7361  user_guide/messa
+00023c80: 6765 732f 7265 6661 6374 6f72 2f63 7963  ges/refactor/cyc
+00023c90: 6c69 632d 696d 706f 7274 2e68 746d 6c5c  lic-import.html\
+00023ca0: 223e 4164 6469 7469 6f6e 616c 2069 6e66  ">Additional inf
+00023cb0: 6f72 6d61 7469 6f6e 3c2f 613e 220a 0a5b  ormation</a>"..[
+00023cc0: 5230 3430 325d 0a77 6879 203d 2022 4974  R0402].why = "It
+00023cd0: 206c 6f6f 6b73 206c 696b 6520 7468 6520   looks like the 
+00023ce0: 7375 626d 6f64 756c 6520 6f66 2061 2070  submodule of a p
+00023cf0: 6163 6b61 6765 2069 7320 696d 706f 7274  ackage is import
+00023d00: 6564 2061 6e64 2061 6c69 6173 6564 2077  ed and aliased w
+00023d10: 6974 6820 7468 6520 7361 6d65 206e 616d  ith the same nam
+00023d20: 652e 2045 2e67 2e2c 2069 6e73 7465 6164  e. E.g., instead
+00023d30: 206f 6620 6060 696d 706f 7274 2063 6f6e   of ``import con
+00023d40: 6375 7272 656e 742e 6675 7475 7265 7320  current.futures 
+00023d50: 6173 2066 7574 7572 6573 6060 2075 7365  as futures`` use
+00023d60: 2060 6066 726f 6d20 636f 6e63 7572 7265   ``from concurre
+00023d70: 6e74 2069 6d70 6f72 7420 6675 7475 7265  nt import future
+00023d80: 7360 6022 0a65 7861 6d70 6c65 7320 3d20  s``".examples = 
 00023d90: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
 00023da0: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
-00023db0: 7820 3d20 310a 7820 3d20 5c22 325c 2220  x = 1.x = \"2\" 
-00023dc0: 2023 205b 7265 6465 6669 6e65 642d 7661   # [redefined-va
-00023dd0: 7269 6162 6c65 2d74 7970 655d 0a0a 6060  riable-type]..``
-00023de0: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
-00023df0: 6974 2a2a 0a0a 6060 6070 790a 7820 3d20  it**..```py.x = 
-00023e00: 310a 7820 3d20 320a 0a60 6060 0a22 2222  1.x = 2..```."""
-00023e10: 0a0a 5b52 3633 3031 5d0a 7768 7920 3d20  ..[R6301].why = 
-00023e20: 2249 7420 6c6f 6f6b 7320 6c69 6b65 2074  "It looks like t
-00023e30: 6865 206d 6574 686f 6420 646f 6573 6e27  he method doesn'
-00023e40: 7420 7573 6520 6974 7320 626f 756e 6420  t use its bound 
-00023e50: 696e 7374 616e 6365 2c20 616e 6420 736f  instance, and so
-00023e60: 2063 6f75 6c64 2062 6520 7772 6974 7465   could be writte
-00023e70: 6e20 6173 2061 2066 756e 6374 696f 6e2e  n as a function.
-00023e80: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
-00023e90: 0a2a 2a50 726f 626c 656d 6174 6963 2063  .**Problematic c
-00023ea0: 6f64 652a 2a0a 0a60 6060 7079 0a63 6c61  ode**..```py.cla
-00023eb0: 7373 2050 6572 736f 6e3a 0a0a 2020 2020  ss Person:..    
-00023ec0: 6465 6620 6465 7665 6c6f 7065 725f 6772  def developer_gr
-00023ed0: 6565 7469 6e67 2873 656c 6629 3a20 2023  eeting(self):  #
-00023ee0: 205b 6e6f 2d73 656c 662d 7573 655d 0a20   [no-self-use]. 
-00023ef0: 2020 2020 2020 2070 7269 6e74 285c 2247         print(\"G
-00023f00: 7265 6574 696e 6773 2064 6576 656c 6f70  reetings develop
-00023f10: 6572 215c 2229 0a0a 2020 2020 6465 6620  er!\")..    def 
-00023f20: 6772 6565 7469 6e67 5f31 2873 656c 6629  greeting_1(self)
-00023f30: 3a20 2023 205b 6e6f 2d73 656c 662d 7573  :  # [no-self-us
-00023f40: 655d 0a20 2020 2020 2020 2070 7269 6e74  e].        print
-00023f50: 285c 2248 656c 6c6f 215c 2229 0a0a 2020  (\"Hello!\")..  
-00023f60: 2020 6465 6620 6772 6565 7469 6e67 5f32    def greeting_2
-00023f70: 2873 656c 6629 3a20 2023 205b 6e6f 2d73  (self):  # [no-s
-00023f80: 656c 662d 7573 655d 0a20 2020 2020 2020  elf-use].       
-00023f90: 2070 7269 6e74 285c 2248 6921 5c22 290a   print(\"Hi!\").
-00023fa0: 0a60 6060 0a0a 2a2a 486f 7720 746f 2066  .```..**How to f
-00023fb0: 6978 2069 742a 2a0a 0a60 6060 7079 0a64  ix it**..```py.d
-00023fc0: 6566 2064 6576 656c 6f70 6572 5f67 7265  ef developer_gre
-00023fd0: 6574 696e 6728 293a 0a20 2020 2070 7269  eting():.    pri
-00023fe0: 6e74 285c 2247 7265 6574 696e 6773 2064  nt(\"Greetings d
-00023ff0: 6576 656c 6f70 6572 215c 2229 0a0a 0a63  eveloper!\")...c
-00024000: 6c61 7373 2050 6572 736f 6e3a 0a20 2020  lass Person:.   
-00024010: 206e 616d 6520 3d20 5c22 5061 7269 735c   name = \"Paris\
-00024020: 220a 0a20 2020 2064 6566 2067 7265 6574  "..    def greet
-00024030: 696e 675f 3128 7365 6c66 293a 0a20 2020  ing_1(self):.   
-00024040: 2020 2020 2070 7269 6e74 2866 5c22 4865       print(f\"He
-00024050: 6c6c 6f20 6672 6f6d 207b 7365 6c66 2e6e  llo from {self.n
-00024060: 616d 657d 2021 5c22 290a 0a20 2020 2040  ame} !\")..    @
-00024070: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-00024080: 2064 6566 2067 7265 6574 696e 675f 3228   def greeting_2(
-00024090: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-000240a0: 285c 2248 6921 5c22 290a 0a60 6060 0a0a  (\"Hi!\")..```..
-000240b0: 3c61 2068 7265 663d 5c22 6874 7470 733a  <a href=\"https:
-000240c0: 2f2f 7079 6c69 6e74 2e70 7963 7161 2e6f  //pylint.pycqa.o
-000240d0: 7267 2f65 6e2f 6c61 7465 7374 2f75 7365  rg/en/latest/use
-000240e0: 725f 6775 6964 652f 6d65 7373 6167 6573  r_guide/messages
-000240f0: 2f72 6566 6163 746f 722f 6e6f 2d73 656c  /refactor/no-sel
-00024100: 662d 7573 652e 6874 6d6c 5c22 3e41 6464  f-use.html\">Add
-00024110: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-00024120: 696f 6e3c 2f61 3e22 2222 0a0a 5b52 3632  ion</a>"""..[R62
-00024130: 3031 5d0a 7768 7920 3d20 2248 6176 696e  01].why = "Havin
-00024140: 6720 756e 6e65 6365 7373 6172 7920 636f  g unnecessary co
-00024150: 6e64 6974 696f 6e73 2069 6e20 636f 6465  nditions in code
-00024160: 206d 616b 6573 2074 6865 2063 6f64 6520   makes the code 
-00024170: 6861 7264 6572 2074 6f20 756e 6465 7273  harder to unders
-00024180: 7461 6e64 2e22 0a65 7861 6d70 6c65 7320  tand.".examples 
-00024190: 3d20 2222 220a 4120 636f 6e64 6974 696f  = """.A conditio
-000241a0: 6e20 7468 6174 2072 6574 7572 6e73 2062  n that returns b
-000241b0: 6f6f 6c20 696e 2062 6f74 6820 6272 616e  ool in both bran
-000241c0: 6368 6573 2063 616e 2062 6520 7369 6d70  ches can be simp
-000241d0: 6c69 6669 6564 2065 7665 6e20 6966 2069  lified even if i
-000241e0: 7420 636f 6e74 6169 6e73 2061 206c 6f67  t contains a log
-000241f0: 6963 616c 2073 7461 7465 6d65 6e74 2e0a  ical statement..
-00024200: 0a60 6060 7079 0a64 6566 2070 726f 626c  .```py.def probl
-00024210: 656d 6174 6963 2861 3a20 626f 6f6c 2c20  ematic(a: bool, 
-00024220: 623a 2062 6f6f 6c29 202d 3e20 626f 6f6c  b: bool) -> bool
-00024230: 3a0a 2020 2020 6966 2061 206f 7220 623a  :.    if a or b:
-00024240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00024250: 5472 7565 0a20 2020 2065 6c73 653a 0a20  True.    else:. 
-00024260: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00024270: 6c73 650a 6060 600a 0a60 6060 7079 0a64  lse.```..```py.d
-00024280: 6566 2067 6f6f 6428 613a 2062 6f6f 6c2c  ef good(a: bool,
-00024290: 2062 3a20 626f 6f6c 2920 2d3e 2062 6f6f   b: bool) -> boo
-000242a0: 6c3a 0a20 2020 2072 6574 7572 6e20 6120  l:.    return a 
-000242b0: 6f72 2062 0a60 6060 0a22 2222 0a0a 5b52  or b.```."""..[R
-000242c0: 3230 3434 5d0a 7768 7920 3d20 2249 7420  2044].why = "It 
-000242d0: 6c6f 6f6b 7320 6c69 6b65 2074 6865 2023  looks like the #
-000242e0: 2073 796d 626f 6c20 6170 7065 6172 7320   symbol appears 
-000242f0: 6f6e 2061 206c 696e 6520 6e6f 7420 666f  on a line not fo
-00024300: 6c6c 6f77 6564 2062 7920 616e 2061 6374  llowed by an act
-00024310: 7561 6c20 636f 6d6d 656e 7422 0a65 7861  ual comment".exa
-00024320: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
-00024330: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
-00024340: 0a0a 6060 6070 790a 2320 2b31 3a5b 656d  ..```py.# +1:[em
-00024350: 7074 792d 636f 6d6d 656e 745d 0a23 0a0a  pty-comment].#..
-00024360: 2320 2b31 3a5b 656d 7074 792d 636f 6d6d  # +1:[empty-comm
-00024370: 656e 745d 0a78 203d 2030 2020 230a 0a60  ent].x = 0  #..`
-00024380: 6060 0a0a 2a2a 486f 7720 746f 2066 6978  ``..**How to fix
-00024390: 2069 742a 2a0a 0a60 6060 7079 0a23 2063   it**..```py.# c
-000243a0: 6f6d 6d65 6e74 0a0a 7820 3d20 3020 2023  omment..x = 0  #
-000243b0: 2063 6f6d 6d65 6e74 0a0a 6060 600a 2222   comment..```.""
-000243c0: 220a 0a5b 5231 3730 315d 0a77 6879 203d  "..[R1701].why =
-000243d0: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
-000243e0: 6d75 6c74 6970 6c65 2063 6f6e 7365 6375  multiple consecu
-000243f0: 7469 7665 2069 7369 6e73 7461 6e63 6520  tive isinstance 
-00024400: 6361 6c6c 7320 6361 6e20 6265 206d 6572  calls can be mer
-00024410: 6765 6420 696e 746f 206f 6e65 2e22 0a65  ged into one.".e
-00024420: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
-00024430: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
-00024440: 2a2a 0a0a 6060 6070 790a 6672 6f6d 2074  **..```py.from t
-00024450: 7970 696e 6720 696d 706f 7274 2041 6e79  yping import Any
-00024460: 0a0a 0a64 6566 2069 735f 6e75 6d62 6572  ...def is_number
-00024470: 2876 616c 7565 3a20 416e 7929 202d 3e20  (value: Any) -> 
-00024480: 626f 6f6c 3a0a 2020 2020 7265 7475 726e  bool:.    return
-00024490: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
-000244a0: 652c 2069 6e74 2920 6f72 2069 7369 6e73  e, int) or isins
-000244b0: 7461 6e63 6528 7661 6c75 652c 2066 6c6f  tance(value, flo
-000244c0: 6174 2920 2023 205b 636f 6e73 6964 6572  at)  # [consider
-000244d0: 2d6d 6572 6769 6e67 2d69 7369 6e73 7461  -merging-isinsta
-000244e0: 6e63 655d 0a0a 6060 600a 0a2a 2a48 6f77  nce]..```..**How
-000244f0: 2074 6f20 6669 7820 6974 2a2a 0a0a 6060   to fix it**..``
-00024500: 6070 790a 6672 6f6d 2074 7970 696e 6720  `py.from typing 
-00024510: 696d 706f 7274 2041 6e79 0a0a 0a64 6566  import Any...def
-00024520: 2069 735f 6e75 6d62 6572 2876 616c 7565   is_number(value
-00024530: 3a20 416e 7929 202d 3e20 626f 6f6c 3a0a  : Any) -> bool:.
-00024540: 2020 2020 7265 7475 726e 2069 7369 6e73      return isins
-00024550: 7461 6e63 6528 7661 6c75 652c 2028 696e  tance(value, (in
-00024560: 742c 2066 6c6f 6174 2929 0a0a 6060 600a  t, float))..```.
-00024570: 2222 220a 0a5b 5231 3730 325d 0a77 6879  """..[R1702].why
-00024580: 203d 2022 436f 6e73 6964 6572 206d 6f76   = "Consider mov
-00024590: 696e 6720 736f 6d65 206f 6620 7468 6520  ing some of the 
-000245a0: 636f 6465 2074 6f20 6865 6c70 6572 2066  code to helper f
-000245b0: 756e 6374 696f 6e73 2e22 0a65 7861 6d70  unctions.".examp
-000245c0: 6c65 7320 3d20 2222 220a 2a2a 5072 6f62  les = """.**Prob
-000245d0: 6c65 6d61 7469 6320 636f 6465 2a2a 0a0a  lematic code**..
-000245e0: 6060 6070 790a 6465 6620 636f 7272 6563  ```py.def correc
-000245f0: 745f 6672 7569 7473 2866 7275 6974 7329  t_fruits(fruits)
-00024600: 3a0a 2020 2020 6966 206c 656e 2866 7275  :.    if len(fru
-00024610: 6974 7329 203e 2031 3a20 2023 205b 746f  its) > 1:  # [to
-00024620: 6f2d 6d61 6e79 2d6e 6573 7465 642d 626c  o-many-nested-bl
-00024630: 6f63 6b73 5d0a 2020 2020 2020 2020 6966  ocks].        if
-00024640: 205c 2261 7070 6c65 5c22 2069 6e20 6672   \"apple\" in fr
-00024650: 7569 7473 3a0a 2020 2020 2020 2020 2020  uits:.          
-00024660: 2020 6966 205c 226f 7261 6e67 655c 2220    if \"orange\" 
-00024670: 696e 2066 7275 6974 733a 0a20 2020 2020  in fruits:.     
-00024680: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-00024690: 203d 2066 7275 6974 735b 5c22 6f72 616e   = fruits[\"oran
-000246a0: 6765 5c22 5d0a 2020 2020 2020 2020 2020  ge\"].          
-000246b0: 2020 2020 2020 6966 2063 6f75 6e74 2025        if count %
-000246c0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-000246d0: 2020 2020 2020 2020 6966 205c 226b 6977          if \"kiw
-000246e0: 695c 2220 696e 2066 7275 6974 733a 0a20  i\" in fruits:. 
-000246f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024700: 2020 2020 2020 2069 6620 636f 756e 7420         if count 
-00024710: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
-00024720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024730: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-00024740: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00024750: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
-00024760: 7820 6974 2a2a 0a0a 6060 6070 790a 6465  x it**..```py.de
-00024770: 6620 636f 7272 6563 745f 6672 7569 7473  f correct_fruits
-00024780: 2866 7275 6974 7329 3a0a 2020 2020 6966  (fruits):.    if
-00024790: 206c 656e 2866 7275 6974 7329 203e 2031   len(fruits) > 1
-000247a0: 2061 6e64 205c 2261 7070 6c65 5c22 2069   and \"apple\" i
-000247b0: 6e20 6672 7569 7473 2061 6e64 205c 226f  n fruits and \"o
-000247c0: 7261 6e67 655c 2220 696e 2066 7275 6974  range\" in fruit
-000247d0: 733a 0a20 2020 2020 2020 2063 6f75 6e74  s:.        count
-000247e0: 203d 2066 7275 6974 735b 5c22 6f72 616e   = fruits[\"oran
-000247f0: 6765 5c22 5d0a 2020 2020 2020 2020 6966  ge\"].        if
-00024800: 2063 6f75 6e74 2025 2032 2061 6e64 205c   count % 2 and \
-00024810: 226b 6977 695c 2220 696e 2066 7275 6974  "kiwi\" in fruit
-00024820: 7320 616e 6420 636f 756e 7420 3d3d 2032  s and count == 2
-00024830: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00024840: 7475 726e 2054 7275 650a 2020 2020 7265  turn True.    re
-00024850: 7475 726e 2046 616c 7365 0a0a 6060 600a  turn False..```.
-00024860: 2222 220a 0a5b 5231 3730 335d 0a77 6879  """..[R1703].why
-00024870: 203d 2022 4974 206c 6f6f 6b73 206c 696b   = "It looks lik
-00024880: 6520 7468 6520 6966 2073 7461 7465 6d65  e the if stateme
-00024890: 6e74 2063 616e 2062 6520 7265 706c 6163  nt can be replac
-000248a0: 6564 2077 6974 6820 2762 6f6f 6c28 7465  ed with 'bool(te
-000248b0: 7374 2927 2e22 0a65 7861 6d70 6c65 7320  st)'.".examples 
-000248c0: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-000248d0: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-000248e0: 790a 464c 5949 4e47 5f54 4849 4e47 5320  y.FLYING_THINGS 
-000248f0: 3d20 5b5c 2262 6972 645c 222c 205c 2270  = [\"bird\", \"p
-00024900: 6c61 6e65 5c22 2c20 5c22 7375 7065 726d  lane\", \"superm
-00024910: 616e 5c22 2c20 5c22 7468 6973 2065 7861  an\", \"this exa
-00024920: 6d70 6c65 5c22 5d0a 0a0a 6465 6620 6973  mple\"]...def is
-00024930: 5f66 6c79 696e 675f 616e 696d 616c 2861  _flying_animal(a
-00024940: 6e5f 6f62 6a65 6374 293a 0a20 2020 2069  n_object):.    i
-00024950: 6620 6973 696e 7374 616e 6365 2861 6e5f  f isinstance(an_
-00024960: 6f62 6a65 6374 2c20 416e 696d 616c 2920  object, Animal) 
-00024970: 616e 6420 616e 5f6f 626a 6563 7420 696e  and an_object in
-00024980: 2046 4c59 494e 475f 5448 494e 4753 3a20   FLYING_THINGS: 
-00024990: 2023 205b 7369 6d70 6c69 6669 6162 6c65   # [simplifiable
-000249a0: 2d69 662d 7374 6174 656d 656e 745d 0a20  -if-statement]. 
-000249b0: 2020 2020 2020 2069 735f 666c 7969 6e67         is_flying
-000249c0: 203d 2054 7275 650a 2020 2020 656c 7365   = True.    else
-000249d0: 3a0a 2020 2020 2020 2020 6973 5f66 6c79  :.        is_fly
-000249e0: 696e 6720 3d20 4661 6c73 650a 2020 2020  ing = False.    
-000249f0: 7265 7475 726e 2069 735f 666c 7969 6e67  return is_flying
-00024a00: 0a0a 6060 600a 0a2a 2a48 6f77 2074 6f20  ..```..**How to 
-00024a10: 6669 7820 6974 2a2a 0a0a 6060 6070 790a  fix it**..```py.
-00024a20: 464c 5949 4e47 5f54 4849 4e47 5320 3d20  FLYING_THINGS = 
-00024a30: 5b5c 2262 6972 645c 222c 205c 2270 6c61  [\"bird\", \"pla
-00024a40: 6e65 5c22 2c20 5c22 7375 7065 726d 616e  ne\", \"superman
-00024a50: 5c22 2c20 5c22 7468 6973 2065 7861 6d70  \", \"this examp
-00024a60: 6c65 5c22 5d0a 0a0a 6465 6620 6973 5f66  le\"]...def is_f
-00024a70: 6c79 696e 675f 616e 696d 616c 2861 6e5f  lying_animal(an_
-00024a80: 6f62 6a65 6374 293a 0a20 2020 2069 735f  object):.    is_
-00024a90: 666c 7969 6e67 203d 2069 7369 6e73 7461  flying = isinsta
-00024aa0: 6e63 6528 616e 5f6f 626a 6563 742c 2041  nce(an_object, A
-00024ab0: 6e69 6d61 6c29 2061 6e64 2061 6e5f 6f62  nimal) and an_ob
-00024ac0: 6a65 6374 2e6e 616d 6520 696e 2046 4c59  ject.name in FLY
-00024ad0: 494e 475f 5448 494e 4753 0a20 2020 2072  ING_THINGS.    r
-00024ae0: 6574 7572 6e20 6973 5f66 6c79 696e 670a  eturn is_flying.
-00024af0: 0a60 6060 0a22 2222 0a0a 5b52 3137 3034  .```."""..[R1704
-00024b00: 5d0a 7768 7920 3d20 2244 6964 2079 6f75  ].why = "Did you
-00024b10: 206e 6f74 6963 6520 7468 6174 2061 6e20   notice that an 
-00024b20: 6172 6775 6d65 6e74 2067 6574 7320 6f76  argument gets ov
-00024b30: 6572 7772 6974 7465 6e20 6865 7265 3f22  erwritten here?"
-00024b40: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
-00024b50: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
-00024b60: 6465 2a2a 0a0a 6060 6070 790a 6465 6620  de**..```py.def 
-00024b70: 7368 6f77 2868 6f73 745f 6964 3d31 302e  show(host_id=10.
-00024b80: 3131 293a 0a20 2020 2066 6f72 2068 6f73  11):.    for hos
-00024b90: 745f 6964 2c20 686f 7374 2069 6e20 5b5b  t_id, host in [[
-00024ba0: 3132 2e31 332c 2027 5665 6e75 7327 5d2c  12.13, 'Venus'],
-00024bb0: 205b 3134 2e31 352c 2027 4d61 7273 275d   [14.15, 'Mars']
-00024bc0: 5d3a 2020 2320 5b72 6564 6566 696e 6564  ]:  # [redefined
-00024bd0: 2d61 7267 756d 656e 742d 6672 6f6d 2d6c  -argument-from-l
-00024be0: 6f63 616c 5d0a 2020 2020 2020 2020 7072  ocal].        pr
-00024bf0: 696e 7428 686f 7374 5f69 642c 2068 6f73  int(host_id, hos
-00024c00: 7429 0a0a 6060 600a 0a2a 2a48 6f77 2074  t)..```..**How t
-00024c10: 6f20 6669 7820 6974 2a2a 0a0a 6060 6070  o fix it**..```p
-00024c20: 790a 6465 6620 7368 6f77 2868 6f73 745f  y.def show(host_
-00024c30: 6964 3d31 302e 3131 293a 0a20 2020 2066  id=10.11):.    f
-00024c40: 6f72 2069 6e6e 6572 5f68 6f73 745f 6964  or inner_host_id
-00024c50: 2c20 686f 7374 2069 6e20 5b5b 3132 2e31  , host in [[12.1
-00024c60: 332c 2027 5665 6e75 7327 5d2c 205b 3134  3, 'Venus'], [14
-00024c70: 2e31 352c 2027 4d61 7273 275d 5d3a 0a20  .15, 'Mars']]:. 
-00024c80: 2020 2020 2020 2070 7269 6e74 2868 6f73         print(hos
-00024c90: 745f 6964 2c20 696e 6e65 725f 686f 7374  t_id, inner_host
-00024ca0: 5f69 642c 2068 6f73 7429 0a0a 6060 600a  _id, host)..```.
-00024cb0: 2222 220a 0a5b 5231 3730 355d 0a77 6879  """..[R1705].why
-00024cc0: 203d 2022 5573 6564 2069 6e20 6f72 6465   = "Used in orde
-00024cd0: 7220 746f 2068 6967 686c 6967 6874 2061  r to highlight a
-00024ce0: 6e20 756e 6e65 6365 7373 6172 7920 626c  n unnecessary bl
-00024cf0: 6f63 6b20 6f66 2063 6f64 6520 666f 6c6c  ock of code foll
-00024d00: 6f77 696e 6720 616e 2069 6620 636f 6e74  owing an if cont
-00024d10: 6169 6e69 6e67 2061 2072 6574 7572 6e20  aining a return 
-00024d20: 7374 6174 656d 656e 742e 2041 7320 7375  statement. As su
-00024d30: 6368 2c20 6974 2077 696c 6c20 7761 726e  ch, it will warn
-00024d40: 2077 6865 6e20 6974 2065 6e63 6f75 6e74   when it encount
-00024d50: 6572 7320 616e 2065 6c73 6520 666f 6c6c  ers an else foll
-00024d60: 6f77 696e 6720 6120 6368 6169 6e20 6f66  owing a chain of
-00024d70: 2069 6673 2c20 616c 6c20 6f66 2074 6865   ifs, all of the
-00024d80: 6d20 636f 6e74 6169 6e69 6e67 2061 2072  m containing a r
-00024d90: 6574 7572 6e20 7374 6174 656d 656e 742e  eturn statement.
-00024da0: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
-00024db0: 0a2a 2a50 726f 626c 656d 6174 6963 2063  .**Problematic c
-00024dc0: 6f64 652a 2a0a 0a60 6060 7079 0a64 6566  ode**..```py.def
-00024dd0: 2063 6f6d 7061 7265 5f6e 756d 6265 7273   compare_numbers
-00024de0: 2861 3a20 696e 742c 2062 3a20 696e 7429  (a: int, b: int)
-00024df0: 202d 3e20 696e 743a 0a20 2020 2069 6620   -> int:.    if 
-00024e00: 6120 3d3d 2062 3a20 2023 205b 6e6f 2d65  a == b:  # [no-e
-00024e10: 6c73 652d 7265 7475 726e 5d0a 2020 2020  lse-return].    
-00024e20: 2020 2020 7265 7475 726e 2030 0a20 2020      return 0.   
-00024e30: 2065 6c69 6620 6120 3c20 623a 0a20 2020   elif a < b:.   
-00024e40: 2020 2020 2072 6574 7572 6e20 2d31 0a20       return -1. 
-00024e50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00024e60: 2072 6574 7572 6e20 310a 0a60 6060 0a0a   return 1..```..
-00024e70: 2a2a 486f 7720 746f 2066 6978 2069 742a  **How to fix it*
-00024e80: 2a0a 0a60 6060 7079 0a64 6566 2063 6f6d  *..```py.def com
-00024e90: 7061 7265 5f6e 756d 6265 7273 2861 3a20  pare_numbers(a: 
-00024ea0: 696e 742c 2062 3a20 696e 7429 202d 3e20  int, b: int) -> 
-00024eb0: 696e 743a 0a20 2020 2069 6620 6120 3d3d  int:.    if a ==
-00024ec0: 2062 3a0a 2020 2020 2020 2020 7265 7475   b:.        retu
-00024ed0: 726e 2030 0a20 2020 2069 6620 6120 3c20  rn 0.    if a < 
-00024ee0: 623a 0a20 2020 2020 2020 2072 6574 7572  b:.        retur
-00024ef0: 6e20 2d31 0a20 2020 2072 6574 7572 6e20  n -1.    return 
-00024f00: 310a 0a60 6060 0a22 2222 0a0a 5b52 3137  1..```."""..[R17
-00024f10: 3036 5d0a 7768 7920 3d20 2249 7420 6c6f  06].why = "It lo
-00024f20: 6f6b 7320 6c69 6b65 206f 6e65 206f 6620  oks like one of 
-00024f30: 6b6e 6f77 6e20 7072 652d 7079 7468 6f6e  known pre-python
-00024f40: 2032 2e35 2074 6572 6e61 7279 2073 796e   2.5 ternary syn
-00024f50: 7461 7820 6973 2075 7365 642e 220a 6578  tax is used.".ex
-00024f60: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
-00024f70: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
-00024f80: 2a0a 0a60 6060 7079 0a78 2c20 7920 3d20  *..```py.x, y = 
-00024f90: 312c 2032 0a6d 6178 696d 756d 203d 2078  1, 2.maximum = x
-00024fa0: 203e 3d20 7920 616e 6420 7820 6f72 2079   >= y and x or y
-00024fb0: 2020 2320 5b63 6f6e 7369 6465 722d 7573    # [consider-us
-00024fc0: 696e 672d 7465 726e 6172 795d 0a0a 6060  ing-ternary]..``
-00024fd0: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
-00024fe0: 6974 2a2a 0a0a 6060 6070 790a 782c 2079  it**..```py.x, y
-00024ff0: 203d 2031 2c20 320a 6d61 7869 6d75 6d20   = 1, 2.maximum 
-00025000: 3d20 7820 6966 2078 203e 3d20 7920 656c  = x if x >= y el
-00025010: 7365 2079 0a0a 6060 600a 2222 220a 0a5b  se y..```."""..[
-00025020: 5231 3730 375d 0a77 6879 203d 2022 496e  R1707].why = "In
-00025030: 2050 7974 686f 6e2c 2061 2074 7570 6c65   Python, a tuple
-00025040: 2069 7320 6163 7475 616c 6c79 2063 7265   is actually cre
-00025050: 6174 6564 2062 7920 7468 6520 636f 6d6d  ated by the comm
-00025060: 6120 7379 6d62 6f6c 2c20 6e6f 7420 6279  a symbol, not by
-00025070: 2074 6865 2070 6172 656e 7468 6573 6573   the parentheses
-00025080: 2e20 556e 666f 7274 756e 6174 656c 792c  . Unfortunately,
-00025090: 206f 6e65 2063 616e 2061 6374 7561 6c6c   one can actuall
-000250a0: 7920 6372 6561 7465 2061 2074 7570 6c65  y create a tuple
-000250b0: 2062 7920 6d69 7370 6c61 6369 6e67 2061   by misplacing a
-000250c0: 2074 7261 696c 696e 6720 636f 6d6d 612c   trailing comma,
-000250d0: 2077 6869 6368 2063 616e 206c 6561 6420   which can lead 
-000250e0: 746f 2070 6f74 656e 7469 616c 2077 6569  to potential wei
-000250f0: 7264 2062 7567 7320 696e 2079 6f75 7220  rd bugs in your 
-00025100: 636f 6465 2e20 596f 7520 7368 6f75 6c64  code. You should
-00025110: 2061 6c77 6179 7320 7573 6520 7061 7265   always use pare
-00025120: 6e74 6865 7365 7320 6578 706c 6963 6974  ntheses explicit
-00025130: 6c79 2066 6f72 2063 7265 6174 696e 6720  ly for creating 
-00025140: 6120 7475 706c 652e 220a 6578 616d 706c  a tuple.".exampl
-00025150: 6573 203d 2022 2222 0a2a 2a50 726f 626c  es = """.**Probl
-00025160: 656d 6174 6963 2063 6f64 652a 2a0a 0a60  ematic code**..`
-00025170: 6060 7079 0a43 4f4d 5041 5353 203d 205c  ``py.COMPASS = \
-00025180: 226e 6f72 7468 5c22 2c20 5c22 736f 7574  "north\", \"sout
-00025190: 685c 222c 205c 2265 6173 745c 222c 205c  h\", \"east\", \
-000251a0: 2277 6573 745c 222c 2020 2320 5b74 7261  "west\",  # [tra
-000251b0: 696c 696e 672d 636f 6d6d 612d 7475 706c  iling-comma-tupl
-000251c0: 655d 0a0a 6060 600a 0a2a 2a48 6f77 2074  e]..```..**How t
-000251d0: 6f20 6669 7820 6974 2a2a 0a0a 6060 6070  o fix it**..```p
-000251e0: 790a 434f 4d50 4153 5320 3d20 285c 226e  y.COMPASS = (\"n
-000251f0: 6f72 7468 5c22 2c20 5c22 736f 7574 685c  orth\", \"south\
-00025200: 222c 205c 2265 6173 745c 222c 205c 2277  ", \"east\", \"w
-00025210: 6573 745c 2229 0a0a 6060 600a 2222 220a  est\")..```.""".
-00025220: 0a5b 5231 3730 385d 0a77 6879 203d 2022  .[R1708].why = "
-00025230: 4163 636f 7264 696e 6720 746f 2050 4550  According to PEP
-00025240: 3437 392c 2074 6865 2072 6169 7365 206f  479, the raise o
-00025250: 6620 5374 6f70 4974 6572 6174 696f 6e20  f StopIteration 
-00025260: 746f 2065 6e64 2074 6865 206c 6f6f 7020  to end the loop 
-00025270: 6f66 2061 2067 656e 6572 6174 6f72 206d  of a generator m
-00025280: 6179 206c 6561 6420 746f 2068 6172 6420  ay lead to hard 
-00025290: 746f 2066 696e 6420 6275 6773 2e20 5468  to find bugs. Th
-000252a0: 6973 2050 4550 2073 7065 6369 6679 2074  is PEP specify t
-000252b0: 6861 7420 7261 6973 6520 5374 6f70 4974  hat raise StopIt
-000252c0: 6572 6174 696f 6e20 6861 7320 746f 2062  eration has to b
-000252d0: 6520 7265 706c 6163 6564 2062 7920 6120  e replaced by a 
-000252e0: 7369 6d70 6c65 2072 6574 7572 6e20 7374  simple return st
-000252f0: 6174 656d 656e 7422 0a65 7861 6d70 6c65  atement".example
-00025300: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
-00025310: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
-00025320: 6070 790a 6465 6620 6672 7569 745f 6765  `py.def fruit_ge
-00025330: 6e65 7261 746f 7228 293a 0a20 2020 2066  nerator():.    f
-00025340: 6f72 2066 7275 6974 2069 6e20 5b5c 2261  or fruit in [\"a
-00025350: 7070 6c65 5c22 2c20 5c22 6261 6e61 6e61  pple\", \"banana
-00025360: 5c22 5d3a 0a20 2020 2020 2020 2079 6965  \"]:.        yie
-00025370: 6c64 2066 7275 6974 0a20 2020 2072 6169  ld fruit.    rai
-00025380: 7365 2053 746f 7049 7465 7261 7469 6f6e  se StopIteration
-00025390: 2020 2320 5b73 746f 702d 6974 6572 6174    # [stop-iterat
-000253a0: 696f 6e2d 7265 7475 726e 5d0a 0a0a 6465  ion-return]...de
-000253b0: 6620 7477 6f5f 6672 7569 7473 5f67 656e  f two_fruits_gen
-000253c0: 6572 6174 6f72 2866 7275 6974 7329 3a0a  erator(fruits):.
-000253d0: 2020 2020 666f 7220 6672 7569 7420 696e      for fruit in
-000253e0: 2066 7275 6974 733a 0a20 2020 2020 2020   fruits:.       
-000253f0: 2079 6965 6c64 2066 7275 6974 2c20 6e65   yield fruit, ne
-00025400: 7874 2866 7275 6974 7329 2020 2320 5b73  xt(fruits)  # [s
-00025410: 746f 702d 6974 6572 6174 696f 6e2d 7265  top-iteration-re
-00025420: 7475 726e 5d0a 0a0a 6465 6620 7477 6f5f  turn]...def two_
-00025430: 676f 6f64 5f66 7275 6974 735f 6765 6e65  good_fruits_gene
-00025440: 7261 746f 7228 6672 7569 7473 293a 0a20  rator(fruits):. 
-00025450: 2020 2066 6f72 2066 7275 6974 2069 6e20     for fruit in 
-00025460: 6672 7569 7473 3a0a 2020 2020 2020 2020  fruits:.        
-00025470: 6966 206e 6f74 2066 7275 6974 2e69 735f  if not fruit.is_
-00025480: 7461 7374 7928 293a 0a20 2020 2020 2020  tasty():.       
-00025490: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-000254a0: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-000254b0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-000254c0: 7874 5f66 7275 6974 203d 206e 6578 7428  xt_fruit = next(
-000254d0: 6672 7569 7473 2920 2023 205b 7374 6f70  fruits)  # [stop
-000254e0: 2d69 7465 7261 7469 6f6e 2d72 6574 7572  -iteration-retur
-000254f0: 6e5d 0a20 2020 2020 2020 2020 2020 2069  n].            i
-00025500: 6620 6e65 7874 5f66 7275 6974 2e69 735f  f next_fruit.is_
-00025510: 7461 7374 7928 293a 0a20 2020 2020 2020  tasty():.       
-00025520: 2020 2020 2020 2020 2079 6965 6c64 2066           yield f
-00025530: 7275 6974 2c20 6e65 7874 5f66 7275 6974  ruit, next_fruit
-00025540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025550: 2062 7265 616b 0a0a 6060 600a 0a2a 2a48   break..```..**H
-00025560: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
-00025570: 6060 6070 790a 6465 6620 6672 7569 745f  ```py.def fruit_
-00025580: 6765 6e65 7261 746f 7228 293a 0a20 2020  generator():.   
-00025590: 205c 225c 225c 2254 6865 2065 7861 6d70   \"\"\"The examp
-000255a0: 6c65 2069 7320 7369 6d70 6c65 2065 6e6f  le is simple eno
-000255b0: 7567 6820 796f 7520 646f 6e27 7420 6e65  ugh you don't ne
-000255c0: 6564 2061 6e20 6578 706c 6963 6974 2072  ed an explicit r
-000255d0: 6574 7572 6e2e 5c22 5c22 5c22 0a20 2020  eturn.\"\"\".   
-000255e0: 2066 6f72 2066 7275 6974 2069 6e20 5b5c   for fruit in [\
-000255f0: 2261 7070 6c65 5c22 2c20 5c22 6261 6e61  "apple\", \"bana
-00025600: 6e61 5c22 5d3a 0a20 2020 2020 2020 2079  na\"]:.        y
-00025610: 6965 6c64 2066 7275 6974 0a0a 0a64 6566  ield fruit...def
-00025620: 2074 776f 5f66 7275 6974 735f 6765 6e65   two_fruits_gene
-00025630: 7261 746f 7228 6672 7569 7473 293a 0a20  rator(fruits):. 
-00025640: 2020 205c 225c 225c 2243 6174 6368 696e     \"\"\"Catchin
-00025650: 6720 7468 6520 5374 6f70 4974 6572 6174  g the StopIterat
-00025660: 696f 6e2e 5c22 5c22 5c22 0a20 2020 2066  ion.\"\"\".    f
-00025670: 6f72 2066 7275 6974 2069 6e20 6672 7569  or fruit in frui
-00025680: 7473 3a0a 2020 2020 2020 2020 7472 793a  ts:.        try:
-00025690: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-000256a0: 6c64 2066 7275 6974 2c20 6e65 7874 2866  ld fruit, next(f
-000256b0: 7275 6974 7329 0a20 2020 2020 2020 2065  ruits).        e
-000256c0: 7863 6570 7420 5374 6f70 4974 6572 6174  xcept StopIterat
-000256d0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-000256e0: 2070 7269 6e74 285c 2253 6f72 7279 2074   print(\"Sorry t
-000256f0: 6865 7265 2069 7320 6f6e 6c79 206f 6e65  here is only one
-00025700: 2066 7275 6974 206c 6566 742e 5c22 290a   fruit left.\").
-00025710: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00025720: 6420 6672 7569 742c 204e 6f6e 650a 0a0a  d fruit, None...
-00025730: 6465 6620 7477 6f5f 676f 6f64 5f66 7275  def two_good_fru
-00025740: 6974 735f 6765 6e65 7261 746f 7228 6672  its_generator(fr
-00025750: 7569 7473 293a 0a20 2020 205c 225c 225c  uits):.    \"\"\
-00025760: 2241 2072 6574 7572 6e20 6361 6e20 6265  "A return can be
-00025770: 2075 7365 6420 746f 2065 6e64 2074 6865   used to end the
-00025780: 2069 7465 7261 746f 7220 6561 726c 792c   iterator early,
-00025790: 2062 7574 206e 6f74 2061 2053 746f 7049   but not a StopI
-000257a0: 7465 7261 7469 6f6e 2e5c 225c 225c 220a  teration.\"\"\".
-000257b0: 2020 2020 666f 7220 6672 7569 7420 696e      for fruit in
-000257c0: 2066 7275 6974 733a 0a20 2020 2020 2020   fruits:.       
-000257d0: 2069 6620 6e6f 7420 6672 7569 742e 6973   if not fruit.is
-000257e0: 5f74 6173 7479 2829 3a0a 2020 2020 2020  _tasty():.      
-000257f0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00025800: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-00025810: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-00025820: 6578 745f 6672 7569 7420 3d20 6e65 7874  ext_fruit = next
-00025830: 2866 7275 6974 732c 204e 6f6e 6529 0a20  (fruits, None). 
-00025840: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
-00025850: 7874 5f66 7275 6974 2069 7320 4e6f 6e65  xt_fruit is None
-00025860: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00025870: 2020 7072 696e 7428 5c22 536f 7272 7920    print(\"Sorry 
-00025880: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
-00025890: 6520 6672 7569 7420 6c65 6674 2e5c 2229  e fruit left.\")
-000258a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000258b0: 2079 6965 6c64 2066 7275 6974 2c20 4e6f   yield fruit, No
-000258c0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-000258d0: 2020 2023 2057 6520 7265 6163 6865 6420     # We reached 
-000258e0: 7468 6520 656e 6420 6f66 2074 6865 2027  the end of the '
-000258f0: 6672 7569 7473 2720 6765 6e65 7261 746f  fruits' generato
-00025900: 7220 6275 7420 7261 6973 696e 6720 610a  r but raising a.
-00025910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025920: 2320 5374 6f70 4974 6572 6174 696f 6e20  # StopIteration 
-00025930: 696e 7374 6561 6420 6f66 2072 6574 7572  instead of retur
-00025940: 6e69 6e67 2077 6f75 6c64 2063 7265 6174  ning would creat
-00025950: 6520 6120 5275 6e74 696d 6545 7272 6f72  e a RuntimeError
-00025960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025970: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00025980: 2020 2020 6966 206e 6578 745f 6672 7569      if next_frui
-00025990: 742e 6973 5f74 6173 7479 2829 3a0a 2020  t.is_tasty():.  
-000259a0: 2020 2020 2020 2020 2020 2020 2020 7969                yi
-000259b0: 656c 6420 6672 7569 742c 206e 6578 745f  eld fruit, next_
-000259c0: 6672 7569 740a 2020 2020 2020 2020 2020  fruit.          
-000259d0: 2020 2020 2020 6272 6561 6b0a 0a60 6060        break..```
-000259e0: 0a0a 3c61 2068 7265 663d 5c22 6874 7470  ..<a href=\"http
-000259f0: 733a 2f2f 7079 6c69 6e74 2e70 7963 7161  s://pylint.pycqa
-00025a00: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f75  .org/en/latest/u
-00025a10: 7365 725f 6775 6964 652f 6d65 7373 6167  ser_guide/messag
-00025a20: 6573 2f72 6566 6163 746f 722f 7374 6f70  es/refactor/stop
-00025a30: 2d69 7465 7261 7469 6f6e 2d72 6574 7572  -iteration-retur
-00025a40: 6e2e 6874 6d6c 5c22 3e41 6464 6974 696f  n.html\">Additio
-00025a50: 6e61 6c20 696e 666f 726d 6174 696f 6e3c  nal information<
-00025a60: 2f61 3e22 2222 0a0a 5b52 3137 3039 5d0a  /a>"""..[R1709].
-00025a70: 7768 7920 3d20 2249 7420 6c6f 6f6b 7320  why = "It looks 
-00025a80: 6c69 6b65 2072 6564 756e 6461 6e74 2070  like redundant p
-00025a90: 7265 2d70 7974 686f 6e20 322e 3520 7465  re-python 2.5 te
-00025aa0: 726e 6172 7920 7379 6e74 6178 2069 7320  rnary syntax is 
-00025ab0: 7573 6564 2e22 0a65 7861 6d70 6c65 7320  used.".examples 
-00025ac0: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-00025ad0: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-00025ae0: 790a 6465 6620 6861 735f 6f72 616e 6765  y.def has_orange
-00025af0: 7328 6f72 616e 6765 732c 2061 7070 6c65  s(oranges, apple
-00025b00: 733d 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a  s=None) -> bool:
-00025b10: 0a20 2020 2072 6574 7572 6e20 6170 706c  .    return appl
-00025b20: 6573 2061 6e64 2046 616c 7365 206f 7220  es and False or 
-00025b30: 6f72 616e 6765 7320 2023 205b 7369 6d70  oranges  # [simp
-00025b40: 6c69 6679 2d62 6f6f 6c65 616e 2d65 7870  lify-boolean-exp
-00025b50: 7265 7373 696f 6e5d 0a0a 6060 600a 0a2a  ression]..```..*
-00025b60: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
-00025b70: 0a0a 6060 6070 790a 6465 6620 6861 735f  ..```py.def has_
-00025b80: 6f72 616e 6765 7328 6f72 616e 6765 732c  oranges(oranges,
-00025b90: 2061 7070 6c65 733d 4e6f 6e65 2920 2d3e   apples=None) ->
-00025ba0: 2062 6f6f 6c3a 0a20 2020 2072 6574 7572   bool:.    retur
-00025bb0: 6e20 6f72 616e 6765 730a 0a60 6060 0a22  n oranges..```."
-00025bc0: 2222 0a0a 5b52 3137 3130 5d0a 7768 7920  ""..[R1710].why 
-00025bd0: 3d20 2241 6363 6f72 6469 6e67 2074 6f20  = "According to 
-00025be0: 5045 5038 2c20 6966 2061 6e79 2072 6574  PEP8, if any ret
-00025bf0: 7572 6e20 7374 6174 656d 656e 7420 7265  urn statement re
-00025c00: 7475 726e 7320 616e 2065 7870 7265 7373  turns an express
-00025c10: 696f 6e2c 2061 6e79 2072 6574 7572 6e20  ion, any return 
-00025c20: 7374 6174 656d 656e 7473 2077 6865 7265  statements where
-00025c30: 206e 6f20 7661 6c75 6520 6973 2072 6574   no value is ret
-00025c40: 7572 6e65 6420 7368 6f75 6c64 2065 7870  urned should exp
-00025c50: 6c69 6369 746c 7920 7374 6174 6520 7468  licitly state th
-00025c60: 6973 2061 7320 7265 7475 726e 204e 6f6e  is as return Non
-00025c70: 652c 2061 6e64 2061 6e20 6578 706c 6963  e, and an explic
-00025c80: 6974 2072 6574 7572 6e20 7374 6174 656d  it return statem
-00025c90: 656e 7420 7368 6f75 6c64 2062 6520 7072  ent should be pr
-00025ca0: 6573 656e 7420 6174 2074 6865 2065 6e64  esent at the end
-00025cb0: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
-00025cc0: 2028 6966 2072 6561 6368 6162 6c65 2922   (if reachable)"
-00025cd0: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
-00025ce0: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
-00025cf0: 6465 2a2a 0a0a 6060 6070 790a 6465 6620  de**..```py.def 
-00025d00: 6765 745f 7468 655f 616e 7377 6572 2876  get_the_answer(v
-00025d10: 616c 7565 3a20 7374 7229 202d 3e20 7374  alue: str) -> st
-00025d20: 7220 7c20 4e6f 6e65 3a20 2023 205b 696e  r | None:  # [in
-00025d30: 636f 6e73 6973 7465 6e74 2d72 6574 7572  consistent-retur
-00025d40: 6e2d 7374 6174 656d 656e 7473 5d0a 2020  n-statements].  
-00025d50: 2020 6966 2076 616c 7565 3a0a 2020 2020    if value:.    
-00025d60: 2020 2020 7265 7475 726e 2076 616c 7565      return value
-00025d70: 0a0a 6060 600a 0a2a 2a48 6f77 2074 6f20  ..```..**How to 
-00025d80: 6669 7820 6974 2a2a 0a0a 6060 6070 790a  fix it**..```py.
-00025d90: 6465 6620 6765 745f 7468 655f 616e 7377  def get_the_answ
-00025da0: 6572 2876 616c 7565 3a20 7374 7229 202d  er(value: str) -
-00025db0: 3e20 7374 7220 7c20 4e6f 6e65 3a0a 2020  > str | None:.  
-00025dc0: 2020 6966 2076 616c 7565 3a0a 2020 2020    if value:.    
-00025dd0: 2020 2020 7265 7475 726e 2076 616c 7565      return value
-00025de0: 0a20 2020 2072 6574 7572 6e20 4e6f 6e65  .    return None
-00025df0: 0a0a 6060 600a 2222 220a 0a5b 5231 3731  ..```."""..[R171
-00025e00: 315d 0a77 6879 203d 2022 4974 206c 6f6f  1].why = "It loo
-00025e10: 6b73 206c 696b 6520 7468 6520 7369 6e67  ks like the sing
-00025e20: 6c65 205c 2272 6574 7572 6e5c 2220 6f72  le \"return\" or
-00025e30: 205c 2272 6574 7572 6e20 4e6f 6e65 5c22   \"return None\"
-00025e40: 2073 7461 7465 6d65 6e74 2069 7320 666f   statement is fo
-00025e50: 756e 6420 6174 2074 6865 2065 6e64 206f  und at the end o
-00025e60: 6620 6675 6e63 7469 6f6e 206f 7220 6d65  f function or me
-00025e70: 7468 6f64 2064 6566 696e 6974 696f 6e2e  thod definition.
-00025e80: 2054 6869 7320 7374 6174 656d 656e 7420   This statement 
-00025e90: 6361 6e20 7361 6665 6c79 2062 6520 7265  can safely be re
-00025ea0: 6d6f 7665 6420 6265 6361 7573 6520 5079  moved because Py
-00025eb0: 7468 6f6e 2077 696c 6c20 696d 706c 6963  thon will implic
-00025ec0: 6974 6c79 2072 6574 7572 6e20 4e6f 6e65  itly return None
-00025ed0: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
-00025ee0: 0a2a 2a50 726f 626c 656d 6174 6963 2063  .**Problematic c
-00025ef0: 6f64 652a 2a0a 0a60 6060 7079 0a69 6d70  ode**..```py.imp
-00025f00: 6f72 7420 7379 730a 0a0a 6465 6620 7072  ort sys...def pr
-00025f10: 696e 745f 7079 7468 6f6e 5f76 6572 7369  int_python_versi
-00025f20: 6f6e 2829 3a20 2023 205b 7573 656c 6573  on():  # [useles
-00025f30: 732d 7265 7475 726e 5d0a 2020 2020 7072  s-return].    pr
-00025f40: 696e 7428 7379 732e 7665 7273 696f 6e29  int(sys.version)
-00025f50: 0a20 2020 2072 6574 7572 6e20 4e6f 6e65  .    return None
-00025f60: 0a0a 6060 600a 0a2a 2a48 6f77 2074 6f20  ..```..**How to 
-00025f70: 6669 7820 6974 2a2a 0a0a 6060 6070 790a  fix it**..```py.
-00025f80: 696d 706f 7274 2073 7973 0a0a 0a64 6566  import sys...def
-00025f90: 2070 7269 6e74 5f70 7974 686f 6e5f 7665   print_python_ve
-00025fa0: 7273 696f 6e28 293a 0a20 2020 2070 7269  rsion():.    pri
-00025fb0: 6e74 2873 7973 2e76 6572 7369 6f6e 290a  nt(sys.version).
-00025fc0: 0a60 6060 0a22 2222 0a0a 5b52 3137 3132  .```."""..[R1712
-00025fd0: 5d0a 7768 7920 3d20 2259 6f75 2064 6f20  ].why = "You do 
-00025fe0: 6e6f 7420 6861 7665 2074 6f20 7573 6520  not have to use 
-00025ff0: 6120 7465 6d70 6f72 6172 7920 7661 7269  a temporary vari
-00026000: 6162 6c65 2069 6e20 6f72 6465 7220 746f  able in order to
-00026010: 2073 7761 7020 7661 7269 6162 6c65 732e   swap variables.
-00026020: 2055 7369 6e67 205c 2274 7570 6c65 2075   Using \"tuple u
-00026030: 6e70 6163 6b69 6e67 5c22 2074 6f20 6469  npacking\" to di
-00026040: 7265 6374 6c79 2073 7761 7020 7661 7269  rectly swap vari
-00026050: 6162 6c65 7320 6d61 6b65 7320 7468 6520  ables makes the 
-00026060: 696e 7465 6e74 696f 6e20 6d6f 7265 2063  intention more c
-00026070: 6c65 6172 2e20 4578 616d 706c 653a 205c  lear. Example: \
-00026080: 2261 2c20 6220 3d20 622c 2061 5c22 2e22  "a, b = b, a\"."
-00026090: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
-000260a0: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
-000260b0: 6465 2a2a 0a0a 6060 6070 790a 6120 3d20  de**..```py.a = 
-000260c0: 310a 6220 3d20 320a 0a74 656d 7020 3d20  1.b = 2..temp = 
-000260d0: 6120 2023 205b 636f 6e73 6964 6572 2d73  a  # [consider-s
-000260e0: 7761 702d 7661 7269 6162 6c65 735d 0a61  wap-variables].a
-000260f0: 203d 2062 0a62 203d 2074 656d 700a 0a60   = b.b = temp..`
-00026100: 6060 0a0a 2a2a 486f 7720 746f 2066 6978  ``..**How to fix
-00026110: 2069 742a 2a0a 0a60 6060 7079 0a61 203d   it**..```py.a =
-00026120: 2031 0a62 203d 2032 0a0a 612c 2062 203d   1.b = 2..a, b =
-00026130: 2062 2c20 610a 0a60 6060 0a22 2222 0a0a   b, a..```."""..
-00026140: 5b52 3137 3133 5d0a 7768 7920 3d20 2255  [R1713].why = "U
-00026150: 7369 6e67 2073 7472 2e6a 6f69 6e28 7365  sing str.join(se
-00026160: 7175 656e 6365 2920 6973 2066 6173 7465  quence) is faste
-00026170: 722c 2075 7365 7320 6c65 7373 206d 656d  r, uses less mem
-00026180: 6f72 7920 616e 6420 696e 6372 6561 7365  ory and increase
-00026190: 7320 7265 6164 6162 696c 6974 7920 636f  s readability co
-000261a0: 6d70 6172 6564 2074 6f20 666f 722d 6c6f  mpared to for-lo
-000261b0: 6f70 2069 7465 7261 7469 6f6e 2e22 0a65  op iteration.".e
-000261c0: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
-000261d0: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
-000261e0: 2a2a 0a0a 6060 6070 790a 6465 6620 6672  **..```py.def fr
-000261f0: 7569 7473 5f74 6f5f 7374 7269 6e67 2866  uits_to_string(f
-00026200: 7275 6974 7329 3a0a 2020 2020 666f 726d  ruits):.    form
-00026210: 6174 7465 645f 6672 7569 7420 3d20 5c22  atted_fruit = \"
-00026220: 5c22 0a20 2020 2066 6f72 2066 7275 6974  \".    for fruit
-00026230: 2069 6e20 6672 7569 7473 3a0a 2020 2020   in fruits:.    
-00026240: 2020 2020 666f 726d 6174 7465 645f 6672      formatted_fr
-00026250: 7569 7420 2b3d 2066 7275 6974 2020 2320  uit += fruit  # 
-00026260: 5b63 6f6e 7369 6465 722d 7573 696e 672d  [consider-using-
-00026270: 6a6f 696e 5d0a 2020 2020 7265 7475 726e  join].    return
-00026280: 2066 6f72 6d61 7474 6564 5f66 7275 6974   formatted_fruit
-00026290: 0a0a 7072 696e 7428 6672 7569 7473 5f74  ..print(fruits_t
-000262a0: 6f5f 7374 7269 6e67 285b 5c22 6170 706c  o_string([\"appl
-000262b0: 655c 222c 205c 2270 6561 725c 222c 205c  e\", \"pear\", \
-000262c0: 2270 6561 6368 5c22 5d29 290a 0a60 6060  "peach\"]))..```
-000262d0: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
-000262e0: 742a 2a0a 0a60 6060 7079 0a70 7269 6e74  t**..```py.print
-000262f0: 285c 225c 222e 6a6f 696e 285b 5c22 6170  (\"\".join([\"ap
-00026300: 706c 655c 222c 205c 2270 6561 725c 222c  ple\", \"pear\",
-00026310: 205c 2270 6561 6368 5c22 5d29 290a 0a60   \"peach\"]))..`
-00026320: 6060 0a22 2222 0a0a 5b52 3137 3134 5d0a  ``."""..[R1714].
-00026330: 7768 7920 3d20 2253 686f 7274 6572 2063  why = "Shorter c
-00026340: 6f6e 6469 7469 6f6e 7320 6172 6520 7573  onditions are us
-00026350: 7375 616c 6c79 2065 6173 6965 7220 746f  sually easier to
-00026360: 2072 6561 642e 220a 6578 616d 706c 6573   read.".examples
-00026370: 203d 2022 2222 0a43 6f6d 7061 7269 736f   = """.Compariso
-00026380: 6e20 6f66 2061 2076 6172 6961 626c 6520  n of a variable 
-00026390: 746f 2074 776f 2076 616c 7565 7320 6361  to two values ca
-000263a0: 6e20 6265 2073 696d 706c 6966 6965 6420  n be simplified 
-000263b0: 7573 696e 6720 7468 6520 6069 6e60 206f  using the `in` o
-000263c0: 7065 7261 746f 722e 0a54 6869 7320 6973  perator..This is
-000263d0: 206d 6f72 6520 7265 6164 6162 6c65 2061   more readable a
-000263e0: 6e64 2061 6c73 6f20 7361 6665 7220 6167  nd also safer ag
-000263f0: 6169 6e73 7420 636f 7079 2d70 6173 7465  ainst copy-paste
-00026400: 2065 7272 6f72 732e 0a0a 6060 6070 790a   errors...```py.
-00026410: 6465 6620 7072 6f62 6c65 6d61 7469 6328  def problematic(
-00026420: 7465 7874 3a20 7374 7229 3a0a 2020 2020  text: str):.    
-00026430: 6966 2074 6578 7420 3d3d 2027 6127 206f  if text == 'a' o
-00026440: 7220 7465 7874 203d 3d20 2762 273a 0a20  r text == 'b':. 
-00026450: 2020 2020 2020 2072 6574 7572 6e0a 6060         return.``
-00026460: 600a 0a60 6060 7079 0a64 6566 2067 6f6f  `..```py.def goo
-00026470: 6428 7465 7874 3a20 7374 7229 3a0a 2020  d(text: str):.  
-00026480: 2020 6966 2074 6578 7420 696e 2028 2761    if text in ('a
-00026490: 272c 2027 6227 293a 0a20 2020 2020 2020  ', 'b'):.       
-000264a0: 2072 6574 7572 6e0a 6060 600a 0a49 6620   return.```..If 
-000264b0: 796f 7520 6172 6520 636f 6d70 6172 696e  you are comparin
-000264c0: 6720 6120 7369 6e67 6c65 2063 6861 7261  g a single chara
-000264d0: 6374 6572 2c20 796f 7520 6361 6e20 616c  cter, you can al
-000264e0: 736f 2064 6f20 7468 6973 3a0a 0a60 6060  so do this:..```
-000264f0: 7079 0a64 6566 2067 6f6f 6428 6368 6172  py.def good(char
-00026500: 3a20 7374 7229 3a0a 2020 2020 6966 2063  : str):.    if c
-00026510: 6861 7220 696e 2027 6162 273a 0a20 2020  har in 'ab':.   
-00026520: 2020 2020 2072 6574 7572 6e0a 6060 600a       return.```.
-00026530: 2222 220a 0a5b 5231 3731 355d 0a77 6879  """..[R1715].why
-00026540: 203d 2022 5573 696e 6720 7468 6520 6275   = "Using the bu
-00026550: 696c 7469 6e20 6469 6374 2e67 6574 2066  iltin dict.get f
-00026560: 6f72 2067 6574 7469 6e67 2061 2076 616c  or getting a val
-00026570: 7565 2066 726f 6d20 6120 6469 6374 696f  ue from a dictio
-00026580: 6e61 7279 2069 6620 6120 6b65 7920 6973  nary if a key is
-00026590: 2070 7265 7365 6e74 206f 7220 6120 6465   present or a de
-000265a0: 6661 756c 7420 6966 206e 6f74 2c20 6973  fault if not, is
-000265b0: 2073 696d 706c 6572 2061 6e64 2063 6f6e   simpler and con
-000265c0: 7369 6465 7265 6420 6d6f 7265 2069 6469  sidered more idi
-000265d0: 6f6d 6174 6963 2c20 616c 7468 6f75 6768  omatic, although
-000265e0: 2073 6f6d 6574 696d 6573 2061 2062 6974   sometimes a bit
-000265f0: 2073 6c6f 7765 7222 0a65 7861 6d70 6c65   slower".example
-00026600: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
-00026610: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
-00026620: 6070 790a 6b6e 6967 6874 7320 3d20 7b5c  `py.knights = {\
-00026630: 2247 616c 6c61 6861 645c 223a 205c 2274  "Gallahad\": \"t
-00026640: 6865 2070 7572 655c 222c 205c 2252 6f62  he pure\", \"Rob
-00026650: 696e 5c22 3a20 5c22 7468 6520 6272 6176  in\": \"the brav
-00026660: 655c 227d 0a0a 6966 205c 2247 616c 6c61  e\"}..if \"Galla
-00026670: 6861 645c 2220 696e 206b 6e69 6768 7473  had\" in knights
-00026680: 3a20 2023 205b 636f 6e73 6964 6572 2d75  :  # [consider-u
-00026690: 7369 6e67 2d67 6574 5d0a 2020 2020 4445  sing-get].    DE
-000266a0: 5343 5249 5054 494f 4e20 3d20 6b6e 6967  SCRIPTION = knig
-000266b0: 6874 735b 5c22 4761 6c6c 6168 6164 5c22  hts[\"Gallahad\"
-000266c0: 5d0a 656c 7365 3a0a 2020 2020 4445 5343  ].else:.    DESC
-000266d0: 5249 5054 494f 4e20 3d20 5c22 5c22 0a0a  RIPTION = \"\"..
-000266e0: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
-000266f0: 7820 6974 2a2a 0a0a 6060 6070 790a 6b6e  x it**..```py.kn
-00026700: 6967 6874 7320 3d20 7b5c 2247 616c 6c61  ights = {\"Galla
-00026710: 6861 645c 223a 205c 2274 6865 2070 7572  had\": \"the pur
-00026720: 655c 222c 205c 2252 6f62 696e 5c22 3a20  e\", \"Robin\": 
-00026730: 5c22 7468 6520 6272 6176 655c 227d 0a0a  \"the brave\"}..
-00026740: 6465 7363 7269 7074 696f 6e20 3d20 6b6e  description = kn
-00026750: 6967 6874 732e 6765 7428 5c22 4761 6c6c  ights.get(\"Gall
-00026760: 6168 6164 5c22 2c20 5c22 5c22 290a 0a60  ahad\", \"\")..`
-00026770: 6060 0a22 2222 0a0a 5b52 3137 3136 5d0a  ``."""..[R1716].
-00026780: 7768 7920 3d20 2254 6869 7320 6d65 7373  why = "This mess
-00026790: 6167 6520 6973 2065 6d69 7474 6564 2077  age is emitted w
-000267a0: 6865 6e20 7079 6c69 6e74 2065 6e63 6f75  hen pylint encou
-000267b0: 6e74 6572 7320 626f 6f6c 6561 6e20 6f70  nters boolean op
-000267c0: 6572 6174 696f 6e20 6c69 6b65 5c22 6120  eration like\"a 
-000267d0: 3c20 6220 616e 6420 6220 3c20 635c 222c  < b and b < c\",
-000267e0: 2073 7567 6765 7374 696e 6720 696e 7374   suggesting inst
-000267f0: 6561 6420 746f 2072 6566 6163 746f 7220  ead to refactor 
-00026800: 6974 2074 6f20 5c22 6120 3c20 6220 3c20  it to \"a < b < 
-00026810: 635c 2222 0a65 7861 6d70 6c65 7320 3d20  c\"".examples = 
-00026820: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
-00026830: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
-00026840: 6120 3d20 696e 7428 696e 7075 7428 2929  a = int(input())
-00026850: 0a62 203d 2069 6e74 2869 6e70 7574 2829  .b = int(input()
-00026860: 290a 6320 3d20 696e 7428 696e 7075 7428  ).c = int(input(
-00026870: 2929 0a69 6620 6120 3c20 6220 616e 6420  )).if a < b and 
-00026880: 6220 3c20 633a 2020 2320 5b63 6861 696e  b < c:  # [chain
-00026890: 6564 2d63 6f6d 7061 7269 736f 6e5d 0a20  ed-comparison]. 
-000268a0: 2020 2070 6173 730a 0a60 6060 0a0a 2a2a     pass..```..**
-000268b0: 486f 7720 746f 2066 6978 2069 742a 2a0a  How to fix it**.
-000268c0: 0a60 6060 7079 0a61 203d 2069 6e74 2869  .```py.a = int(i
-000268d0: 6e70 7574 2829 290a 6220 3d20 696e 7428  nput()).b = int(
-000268e0: 696e 7075 7428 2929 0a63 203d 2069 6e74  input()).c = int
-000268f0: 2869 6e70 7574 2829 290a 6966 2061 203c  (input()).if a <
-00026900: 2062 203c 2063 3a0a 2020 2020 7061 7373   b < c:.    pass
-00026910: 0a0a 6060 600a 2222 220a 0a5b 5231 3731  ..```."""..[R171
-00026920: 375d 0a77 6879 203d 2022 4974 206c 6f6f  7].why = "It loo
-00026930: 6b73 206c 696b 6520 7765 2064 6574 6563  ks like we detec
-00026940: 7420 7468 6520 6372 6561 7469 6f6e 206f  t the creation o
-00026950: 6620 6120 6469 6374 696f 6e61 7279 2075  f a dictionary u
-00026960: 7369 6e67 2074 6865 2064 6963 7428 2920  sing the dict() 
-00026970: 6361 6c6c 6162 6c65 2061 6e64 2061 2074  callable and a t
-00026980: 7261 6e73 6965 6e74 206c 6973 742e 2041  ransient list. A
-00026990: 6c74 686f 7567 6820 7468 6572 6520 6973  lthough there is
-000269a0: 206e 6f74 6869 6e67 2073 796e 7461 6374   nothing syntact
-000269b0: 6963 616c 6c79 2077 726f 6e67 2077 6974  ically wrong wit
-000269c0: 6820 7468 6973 2063 6f64 652c 2069 7420  h this code, it 
-000269d0: 6973 2068 6172 6420 746f 2072 6561 6420  is hard to read 
-000269e0: 616e 6420 6361 6e20 6265 2073 696d 706c  and can be simpl
-000269f0: 6966 6965 6420 746f 2061 2064 6963 7420  ified to a dict 
-00026a00: 636f 6d70 7265 6865 6e73 696f 6e2e 416c  comprehension.Al
-00026a10: 736f 2069 7420 6973 2066 6173 7465 7220  so it is faster 
-00026a20: 7369 6e63 6520 796f 7520 646f 6e27 7420  since you don't 
-00026a30: 6e65 6564 2074 6f20 6372 6561 7465 2061  need to create a
-00026a40: 6e6f 7468 6572 2074 7261 6e73 6965 6e74  nother transient
-00026a50: 206c 6973 7422 0a65 7861 6d70 6c65 7320   list".examples 
-00026a60: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-00026a70: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-00026a80: 790a 4e55 4d42 4552 5320 3d20 5b31 2c20  y.NUMBERS = [1, 
-00026a90: 322c 2033 5d0a 0a23 202b 313a 205b 636f  2, 3]..# +1: [co
-00026aa0: 6e73 6964 6572 2d75 7369 6e67 2d64 6963  nsider-using-dic
-00026ab0: 742d 636f 6d70 7265 6865 6e73 696f 6e5d  t-comprehension]
-00026ac0: 0a44 4f55 424c 4544 5f4e 554d 4245 5253  .DOUBLED_NUMBERS
-00026ad0: 203d 2064 6963 7428 5b28 6e75 6d62 6572   = dict([(number
-00026ae0: 2c20 6e75 6d62 6572 202a 2032 2920 666f  , number * 2) fo
-00026af0: 7220 6e75 6d62 6572 2069 6e20 4e55 4d42  r number in NUMB
-00026b00: 4552 535d 290a 0a60 6060 0a0a 2a2a 486f  ERS])..```..**Ho
-00026b10: 7720 746f 2066 6978 2069 742a 2a0a 0a60  w to fix it**..`
-00026b20: 6060 7079 0a4e 554d 4245 5253 203d 205b  ``py.NUMBERS = [
-00026b30: 312c 2032 2c20 335d 0a0a 444f 5542 4c45  1, 2, 3]..DOUBLE
-00026b40: 445f 4e55 4d42 4552 5320 3d20 7b6e 756d  D_NUMBERS = {num
-00026b50: 6265 723a 206e 756d 6265 7220 2a20 3220  ber: number * 2 
-00026b60: 666f 7220 6e75 6d62 6572 2069 6e20 4e55  for number in NU
-00026b70: 4d42 4552 537d 0a0a 6060 600a 0a3c 6120  MBERS}..```..<a 
-00026b80: 6872 6566 3d5c 2268 7474 7073 3a2f 2f70  href=\"https://p
-00026b90: 796c 696e 742e 7079 6371 612e 6f72 672f  ylint.pycqa.org/
-00026ba0: 656e 2f6c 6174 6573 742f 7573 6572 5f67  en/latest/user_g
-00026bb0: 7569 6465 2f6d 6573 7361 6765 732f 7265  uide/messages/re
-00026bc0: 6661 6374 6f72 2f63 6f6e 7369 6465 722d  factor/consider-
-00026bd0: 7573 696e 672d 6469 6374 2d63 6f6d 7072  using-dict-compr
-00026be0: 6568 656e 7369 6f6e 2e68 746d 6c5c 223e  ehension.html\">
-00026bf0: 4164 6469 7469 6f6e 616c 2069 6e66 6f72  Additional infor
-00026c00: 6d61 7469 6f6e 3c2f 613e 2222 220a 0a5b  mation</a>"""..[
-00026c10: 5231 3731 385d 0a77 6879 203d 2022 416c  R1718].why = "Al
-00026c20: 7468 6f75 6768 2074 6865 7265 2069 7320  though there is 
-00026c30: 6e6f 7468 696e 6720 7379 6e74 6163 7469  nothing syntacti
-00026c40: 6361 6c6c 7920 7772 6f6e 6720 7769 7468  cally wrong with
-00026c50: 2074 6869 7320 636f 6465 2c20 6974 2069   this code, it i
-00026c60: 7320 6861 7264 2074 6f20 7265 6164 2061  s hard to read a
-00026c70: 6e64 2063 616e 2062 6520 7369 6d70 6c69  nd can be simpli
-00026c80: 6669 6564 2074 6f20 6120 7365 7420 636f  fied to a set co
-00026c90: 6d70 7265 6865 6e73 696f 6e2e 416c 736f  mprehension.Also
-00026ca0: 2069 7420 6973 2066 6173 7465 7220 7369   it is faster si
-00026cb0: 6e63 6520 796f 7520 646f 6e27 7420 6e65  nce you don't ne
-00026cc0: 6564 2074 6f20 6372 6561 7465 2061 6e6f  ed to create ano
-00026cd0: 7468 6572 2074 7261 6e73 6965 6e74 206c  ther transient l
-00026ce0: 6973 7422 0a65 7861 6d70 6c65 7320 3d20  ist".examples = 
-00026cf0: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
-00026d00: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
-00026d10: 4e55 4d42 4552 5320 3d20 5b31 2c20 322c  NUMBERS = [1, 2,
-00026d20: 2032 2c20 332c 2034 2c20 345d 0a0a 2320   2, 3, 4, 4]..# 
-00026d30: 2b31 3a20 5b63 6f6e 7369 6465 722d 7573  +1: [consider-us
-00026d40: 696e 672d 7365 742d 636f 6d70 7265 6865  ing-set-comprehe
-00026d50: 6e73 696f 6e5d 0a55 4e49 5155 455f 4556  nsion].UNIQUE_EV
-00026d60: 454e 5f4e 554d 4245 5253 203d 2073 6574  EN_NUMBERS = set
-00026d70: 285b 6e75 6d62 6572 2066 6f72 206e 756d  ([number for num
-00026d80: 6265 7220 696e 204e 554d 4245 5253 2069  ber in NUMBERS i
-00026d90: 6620 6e75 6d62 6572 2025 2032 203d 3d20  f number % 2 == 
-00026da0: 305d 290a 0a60 6060 0a0a 2a2a 486f 7720  0])..```..**How 
-00026db0: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
-00026dc0: 7079 0a4e 554d 4245 5253 203d 205b 312c  py.NUMBERS = [1,
-00026dd0: 2032 2c20 322c 2033 2c20 342c 2034 5d0a   2, 2, 3, 4, 4].
-00026de0: 0a55 4e49 5155 455f 4556 454e 5f4e 554d  .UNIQUE_EVEN_NUM
-00026df0: 4245 5253 203d 207b 6e75 6d62 6572 2066  BERS = {number f
-00026e00: 6f72 206e 756d 6265 7220 696e 204e 554d  or number in NUM
-00026e10: 4245 5253 2069 6620 6e75 6d62 6572 2025  BERS if number %
-00026e20: 2032 203d 3d20 307d 0a0a 6060 600a 0a3c   2 == 0}..```..<
-00026e30: 6120 6872 6566 3d5c 2268 7474 7073 3a2f  a href=\"https:/
-00026e40: 2f70 796c 696e 742e 7079 6371 612e 6f72  /pylint.pycqa.or
-00026e50: 672f 656e 2f6c 6174 6573 742f 7573 6572  g/en/latest/user
-00026e60: 5f67 7569 6465 2f6d 6573 7361 6765 732f  _guide/messages/
-00026e70: 7265 6661 6374 6f72 2f63 6f6e 7369 6465  refactor/conside
-00026e80: 722d 7573 696e 672d 7365 742d 636f 6d70  r-using-set-comp
-00026e90: 7265 6865 6e73 696f 6e2e 6874 6d6c 5c22  rehension.html\"
-00026ea0: 3e41 6464 6974 696f 6e61 6c20 696e 666f  >Additional info
-00026eb0: 726d 6174 696f 6e3c 2f61 3e22 2222 0a0a  rmation</a>"""..
-00026ec0: 5b52 3137 3139 5d0a 7768 7920 3d20 2249  [R1719].why = "I
-00026ed0: 7420 6c6f 6f6b 7320 6c69 6b65 2074 6865  t looks like the
-00026ee0: 2069 6620 6578 7072 6573 7369 6f6e 2063   if expression c
-00026ef0: 616e 2062 6520 7265 706c 6163 6564 2077  an be replaced w
-00026f00: 6974 6820 2762 6f6f 6c28 7465 7374 2927  ith 'bool(test)'
-00026f10: 206f 7220 7369 6d70 6c79 2027 7465 7374   or simply 'test
-00026f20: 2720 6966 2074 6865 2062 6f6f 6c65 616e  ' if the boolean
-00026f30: 2063 6173 7420 6973 2069 6d70 6c69 6369   cast is implici
-00026f40: 742e 220a 6578 616d 706c 6573 203d 2022  t.".examples = "
-00026f50: 2222 0a2a 2a50 726f 626c 656d 6174 6963  "".**Problematic
-00026f60: 2063 6f64 652a 2a0a 0a60 6060 7079 0a46   code**..```py.F
-00026f70: 4c59 494e 475f 5448 494e 4753 203d 205b  LYING_THINGS = [
-00026f80: 5c22 6269 7264 5c22 2c20 5c22 706c 616e  \"bird\", \"plan
-00026f90: 655c 222c 205c 2273 7570 6572 6d61 6e5c  e\", \"superman\
-00026fa0: 222c 205c 2274 6869 7320 6578 616d 706c  ", \"this exampl
-00026fb0: 655c 225d 0a0a 0a64 6566 2069 735f 666c  e\"]...def is_fl
-00026fc0: 7969 6e67 5f74 6869 6e67 2861 6e5f 6f62  ying_thing(an_ob
-00026fd0: 6a65 6374 293a 0a20 2020 2072 6574 7572  ject):.    retur
-00026fe0: 6e20 5472 7565 2069 6620 616e 5f6f 626a  n True if an_obj
-00026ff0: 6563 7420 696e 2046 4c59 494e 475f 5448  ect in FLYING_TH
-00027000: 494e 4753 2065 6c73 6520 4661 6c73 6520  INGS else False 
-00027010: 2023 205b 7369 6d70 6c69 6669 6162 6c65   # [simplifiable
-00027020: 2d69 662d 6578 7072 6573 7369 6f6e 5d0a  -if-expression].
-00027030: 0a0a 6465 6620 6973 5f6e 6f74 5f66 6c79  ..def is_not_fly
-00027040: 696e 675f 7468 696e 6728 616e 5f6f 626a  ing_thing(an_obj
-00027050: 6563 7429 3a0a 2020 2020 7265 7475 726e  ect):.    return
-00027060: 2046 616c 7365 2069 6620 616e 5f6f 626a   False if an_obj
-00027070: 6563 7420 696e 2046 4c59 494e 475f 5448  ect in FLYING_TH
-00027080: 494e 4753 2065 6c73 6520 5472 7565 2020  INGS else True  
-00027090: 2320 5b73 696d 706c 6966 6961 626c 652d  # [simplifiable-
-000270a0: 6966 2d65 7870 7265 7373 696f 6e5d 0a0a  if-expression]..
-000270b0: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
-000270c0: 7820 6974 2a2a 0a0a 6060 6070 790a 464c  x it**..```py.FL
-000270d0: 5949 4e47 5f54 4849 4e47 5320 3d20 5b5c  YING_THINGS = [\
-000270e0: 2262 6972 645c 222c 205c 2270 6c61 6e65  "bird\", \"plane
-000270f0: 5c22 2c20 5c22 7375 7065 726d 616e 5c22  \", \"superman\"
-00027100: 2c20 5c22 7468 6973 2065 7861 6d70 6c65  , \"this example
-00027110: 5c22 5d0a 0a0a 6465 6620 6973 5f66 6c79  \"]...def is_fly
-00027120: 696e 675f 7468 696e 6728 616e 5f6f 626a  ing_thing(an_obj
-00027130: 6563 7429 3a0a 2020 2020 7265 7475 726e  ect):.    return
-00027140: 2061 6e5f 6f62 6a65 6374 2069 6e20 464c   an_object in FL
-00027150: 5949 4e47 5f54 4849 4e47 530a 0a0a 6465  YING_THINGS...de
-00027160: 6620 6973 5f6e 6f74 5f66 6c79 696e 675f  f is_not_flying_
-00027170: 7468 696e 6728 616e 5f6f 626a 6563 7429  thing(an_object)
-00027180: 3a0a 2020 2020 7265 7475 726e 2061 6e5f  :.    return an_
-00027190: 6f62 6a65 6374 206e 6f74 2069 6e20 464c  object not in FL
-000271a0: 5949 4e47 5f54 4849 4e47 530a 0a60 6060  YING_THINGS..```
-000271b0: 0a22 2222 0a0a 5b52 3137 3230 5d0a 7768  ."""..[R1720].wh
-000271c0: 7920 3d20 2255 7365 6420 696e 206f 7264  y = "Used in ord
-000271d0: 6572 2074 6f20 6869 6768 6c69 6768 7420  er to highlight 
-000271e0: 616e 2075 6e6e 6563 6573 7361 7279 2062  an unnecessary b
-000271f0: 6c6f 636b 206f 6620 636f 6465 2066 6f6c  lock of code fol
-00027200: 6c6f 7769 6e67 2061 6e20 6966 2063 6f6e  lowing an if con
-00027210: 7461 696e 696e 6720 6120 7261 6973 6520  taining a raise 
-00027220: 7374 6174 656d 656e 742e 2041 7320 7375  statement. As su
-00027230: 6368 2c20 6974 2077 696c 6c20 7761 726e  ch, it will warn
-00027240: 2077 6865 6e20 6974 2065 6e63 6f75 6e74   when it encount
-00027250: 6572 7320 616e 2065 6c73 6520 666f 6c6c  ers an else foll
-00027260: 6f77 696e 6720 6120 6368 6169 6e20 6f66  owing a chain of
-00027270: 2069 6673 2c20 616c 6c20 6f66 2074 6865   ifs, all of the
-00027280: 6d20 636f 6e74 6169 6e69 6e67 2061 2072  m containing a r
-00027290: 6169 7365 2073 7461 7465 6d65 6e74 2e22  aise statement."
-000272a0: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
-000272b0: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
-000272c0: 6465 2a2a 0a0a 6060 6070 790a 6465 6620  de**..```py.def 
-000272d0: 696e 7465 6765 725f 7375 6d28 613a 2069  integer_sum(a: i
-000272e0: 6e74 2c20 623a 2069 6e74 2920 2d3e 2069  nt, b: int) -> i
-000272f0: 6e74 3a0a 2020 2020 6966 206e 6f74 2028  nt:.    if not (
-00027300: 6973 696e 7374 616e 6365 2861 2c20 696e  isinstance(a, in
-00027310: 7429 2061 6e64 2069 7369 6e73 7461 6e63  t) and isinstanc
-00027320: 6528 622c 2069 6e74 2929 3a20 2020 2023  e(b, int)):    #
-00027330: 205b 6e6f 2d65 6c73 652d 7261 6973 655d   [no-else-raise]
-00027340: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00027350: 616c 7565 4572 726f 7228 2746 756e 6374  alueError('Funct
-00027360: 696f 6e20 7375 7070 6f72 7473 206f 6e6c  ion supports onl
-00027370: 7920 696e 7465 6765 7220 7061 7261 6d65  y integer parame
-00027380: 7465 7273 2e27 290a 2020 2020 656c 7365  ters.').    else
-00027390: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000273a0: 2061 202b 2062 0a0a 6060 600a 0a2a 2a48   a + b..```..**H
-000273b0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
-000273c0: 6060 6070 790a 6465 6620 696e 7465 6765  ```py.def intege
-000273d0: 725f 7375 6d28 613a 2069 6e74 2c20 623a  r_sum(a: int, b:
-000273e0: 2069 6e74 2920 2d3e 2069 6e74 3a0a 2020   int) -> int:.  
-000273f0: 2020 6966 206e 6f74 2028 6973 696e 7374    if not (isinst
-00027400: 616e 6365 2861 2c20 696e 7429 2061 6e64  ance(a, int) and
-00027410: 2069 7369 6e73 7461 6e63 6528 622c 2069   isinstance(b, i
-00027420: 6e74 2929 3a0a 2020 2020 2020 2020 7261  nt)):.        ra
-00027430: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-00027440: 4675 6e63 7469 6f6e 2073 7570 706f 7274  Function support
-00027450: 7320 6f6e 6c79 2069 6e74 6567 6572 2070  s only integer p
-00027460: 6172 616d 6574 6572 732e 2729 0a20 2020  arameters.').   
-00027470: 2072 6574 7572 6e20 6120 2b20 620a 0a60   return a + b..`
-00027480: 6060 0a22 2222 0a0a 5b52 3137 3231 5d0a  ``."""..[R1721].
-00027490: 7768 7920 3d20 2249 6e73 7465 6164 206f  why = "Instead o
-000274a0: 6620 7573 696e 6720 616e 2069 6465 6e74  f using an ident
-000274b0: 6974 7920 636f 6d70 7265 6865 6e73 696f  ity comprehensio
-000274c0: 6e2c 2063 6f6e 7369 6465 7220 7573 696e  n, consider usin
-000274d0: 6720 7468 6520 6c69 7374 2c20 6469 6374  g the list, dict
-000274e0: 206f 7220 7365 7420 636f 6e73 7472 7563   or set construc
-000274f0: 746f 722e 2049 7420 6973 2066 6173 7465  tor. It is faste
-00027500: 7220 616e 6420 7369 6d70 6c65 722e 220a  r and simpler.".
-00027510: 6578 616d 706c 6573 203d 2022 2222 0a2a  examples = """.*
-00027520: 2a50 726f 626c 656d 6174 6963 2063 6f64  *Problematic cod
-00027530: 652a 2a0a 0a60 6060 7079 0a4e 554d 4245  e**..```py.NUMBE
-00027540: 5253 203d 205b 312c 2031 2c20 322c 2032  RS = [1, 1, 2, 2
-00027550: 2c20 332c 2033 5d0a 0a55 4e49 5155 455f  , 3, 3]..UNIQUE_
-00027560: 4e55 4d42 4552 5320 3d20 7b6e 756d 6265  NUMBERS = {numbe
-00027570: 7220 666f 7220 6e75 6d62 6572 2069 6e20  r for number in 
-00027580: 4e55 4d42 4552 537d 2020 2320 5b75 6e6e  NUMBERS}  # [unn
-00027590: 6563 6573 7361 7279 2d63 6f6d 7072 6568  ecessary-compreh
-000275a0: 656e 7369 6f6e 5d0a 0a60 6060 0a0a 2a2a  ension]..```..**
-000275b0: 486f 7720 746f 2066 6978 2069 742a 2a0a  How to fix it**.
-000275c0: 0a60 6060 7079 0a4e 554d 4245 5253 203d  .```py.NUMBERS =
-000275d0: 205b 312c 2031 2c20 322c 2032 2c20 332c   [1, 1, 2, 2, 3,
-000275e0: 2033 5d0a 0a55 4e49 5155 455f 4e55 4d42   3]..UNIQUE_NUMB
-000275f0: 4552 5320 3d20 7365 7428 4e55 4d42 4552  ERS = set(NUMBER
-00027600: 5329 0a0a 6060 600a 2222 220a 0a5b 5231  S)..```."""..[R1
-00027610: 3732 325d 0a77 6879 203d 2022 496e 7374  722].why = "Inst
-00027620: 6561 6420 6f66 2075 7369 6e67 2065 7869  ead of using exi
-00027630: 7428 2920 6f72 2071 7569 7428 292c 2063  t() or quit(), c
-00027640: 6f6e 7369 6465 7220 7573 696e 6720 7468  onsider using th
-00027650: 6520 7379 732e 6578 6974 2829 2e22 0a65  e sys.exit().".e
-00027660: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
-00027670: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
-00027680: 2a2a 0a0a 6060 6070 790a 6966 205f 5f6e  **..```py.if __n
-00027690: 616d 655f 5f20 3d3d 205c 225f 5f6d 6169  ame__ == \"__mai
-000276a0: 6e5f 5f5c 223a 0a20 2020 2075 7365 7220  n__\":.    user 
-000276b0: 3d20 696e 7075 7428 5c22 456e 7465 7220  = input(\"Enter 
-000276c0: 7573 6572 206e 616d 653a 205c 2229 0a20  user name: \"). 
-000276d0: 2020 2070 7269 6e74 2866 5c22 4865 6c6c     print(f\"Hell
-000276e0: 6f2c 207b 7573 6572 7d5c 2229 0a20 2020  o, {user}\").   
-000276f0: 2065 7869 7428 3029 2020 2320 5b63 6f6e   exit(0)  # [con
-00027700: 7369 6465 722d 7573 696e 672d 7379 732d  sider-using-sys-
-00027710: 6578 6974 5d0a 0a60 6060 0a0a 2a2a 486f  exit]..```..**Ho
-00027720: 7720 746f 2066 6978 2069 742a 2a0a 0a60  w to fix it**..`
-00027730: 6060 7079 0a69 6d70 6f72 7420 7379 730a  ``py.import sys.
-00027740: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00027750: 5c22 5f5f 6d61 696e 5f5f 5c22 3a0a 2020  \"__main__\":.  
-00027760: 2020 7573 6572 203d 2069 6e70 7574 285c    user = input(\
-00027770: 2245 6e74 6572 2075 7365 7220 6e61 6d65  "Enter user name
-00027780: 3a20 5c22 290a 2020 2020 7072 696e 7428  : \").    print(
-00027790: 665c 2248 656c 6c6f 2c20 7b75 7365 727d  f\"Hello, {user}
-000277a0: 5c22 290a 2020 2020 7379 732e 6578 6974  \").    sys.exit
-000277b0: 2830 290a 0a60 6060 0a22 2222 0a0a 5b52  (0)..```."""..[R
-000277c0: 3137 3233 5d0a 7768 7920 3d20 2255 7365  1723].why = "Use
-000277d0: 6420 696e 206f 7264 6572 2074 6f20 6869  d in order to hi
-000277e0: 6768 6c69 6768 7420 616e 2075 6e6e 6563  ghlight an unnec
-000277f0: 6573 7361 7279 2062 6c6f 636b 206f 6620  essary block of 
-00027800: 636f 6465 2066 6f6c 6c6f 7769 6e67 2061  code following a
-00027810: 6e20 6966 2063 6f6e 7461 696e 696e 6720  n if containing 
-00027820: 6120 6272 6561 6b20 7374 6174 656d 656e  a break statemen
-00027830: 742e 2041 7320 7375 6368 2c20 6974 2077  t. As such, it w
-00027840: 696c 6c20 7761 726e 2077 6865 6e20 6974  ill warn when it
-00027850: 2065 6e63 6f75 6e74 6572 7320 616e 2065   encounters an e
-00027860: 6c73 6520 666f 6c6c 6f77 696e 6720 6120  lse following a 
-00027870: 6368 6169 6e20 6f66 2069 6673 2c20 616c  chain of ifs, al
-00027880: 6c20 6f66 2074 6865 6d20 636f 6e74 6169  l of them contai
-00027890: 6e69 6e67 2061 2062 7265 616b 2073 7461  ning a break sta
-000278a0: 7465 6d65 6e74 2e22 0a65 7861 6d70 6c65  tement.".example
-000278b0: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
-000278c0: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
-000278d0: 6070 790a 6465 6620 6e65 7874 5f73 6576  `py.def next_sev
-000278e0: 656e 5f65 6c65 6d65 6e74 7328 6974 6572  en_elements(iter
-000278f0: 6174 6f72 293a 0a20 2020 2066 6f72 2069  ator):.    for i
-00027900: 2c20 6974 656d 2069 6e20 656e 756d 6572  , item in enumer
-00027910: 6174 6528 6974 6572 6174 6f72 293a 0a20  ate(iterator):. 
-00027920: 2020 2020 2020 2069 6620 6920 3d3d 2037         if i == 7
-00027930: 3a20 2023 205b 6e6f 2d65 6c73 652d 6272  :  # [no-else-br
-00027940: 6561 6b5d 0a20 2020 2020 2020 2020 2020  eak].           
-00027950: 2062 7265 616b 0a20 2020 2020 2020 2065   break.        e
-00027960: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00027970: 2079 6965 6c64 2069 7465 6d0a 0a60 6060   yield item..```
-00027980: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
-00027990: 742a 2a0a 0a60 6060 7079 0a64 6566 206e  t**..```py.def n
-000279a0: 6578 745f 7365 7665 6e5f 656c 656d 656e  ext_seven_elemen
-000279b0: 7473 2869 7465 7261 746f 7229 3a0a 2020  ts(iterator):.  
-000279c0: 2020 666f 7220 692c 2069 7465 6d20 696e    for i, item in
-000279d0: 2065 6e75 6d65 7261 7465 2869 7465 7261   enumerate(itera
-000279e0: 746f 7229 3a0a 2020 2020 2020 2020 6966  tor):.        if
-000279f0: 2069 203d 3d20 373a 0a20 2020 2020 2020   i == 7:.       
-00027a00: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00027a10: 2020 2079 6965 6c64 2069 7465 6d0a 0a60     yield item..`
-00027a20: 6060 0a22 2222 0a0a 5b52 3137 3234 5d0a  ``."""..[R1724].
-00027a30: 7768 7920 3d20 2255 7365 6420 696e 206f  why = "Used in o
-00027a40: 7264 6572 2074 6f20 6869 6768 6c69 6768  rder to highligh
-00027a50: 7420 616e 2075 6e6e 6563 6573 7361 7279  t an unnecessary
-00027a60: 2062 6c6f 636b 206f 6620 636f 6465 2066   block of code f
-00027a70: 6f6c 6c6f 7769 6e67 2061 6e20 6966 2063  ollowing an if c
-00027a80: 6f6e 7461 696e 696e 6720 6120 636f 6e74  ontaining a cont
-00027a90: 696e 7565 2073 7461 7465 6d65 6e74 2e20  inue statement. 
-00027aa0: 4173 2073 7563 682c 2069 7420 7769 6c6c  As such, it will
-00027ab0: 2077 6172 6e20 7768 656e 2069 7420 656e   warn when it en
-00027ac0: 636f 756e 7465 7273 2061 6e20 656c 7365  counters an else
-00027ad0: 2066 6f6c 6c6f 7769 6e67 2061 2063 6861   following a cha
-00027ae0: 696e 206f 6620 6966 732c 2061 6c6c 206f  in of ifs, all o
-00027af0: 6620 7468 656d 2063 6f6e 7461 696e 696e  f them containin
-00027b00: 6720 6120 636f 6e74 696e 7565 2073 7461  g a continue sta
-00027b10: 7465 6d65 6e74 2e22 0a65 7861 6d70 6c65  tement.".example
-00027b20: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
-00027b30: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
-00027b40: 6070 790a 6465 6620 6576 656e 5f6e 756d  `py.def even_num
-00027b50: 6265 725f 756e 6465 7228 6e3a 2069 6e74  ber_under(n: int
-00027b60: 293a 0a20 2020 2066 6f72 2069 2069 6e20  ):.    for i in 
-00027b70: 7261 6e67 6528 6e29 3a0a 2020 2020 2020  range(n):.      
-00027b80: 2020 6966 2069 2532 203d 3d20 313a 2020    if i%2 == 1:  
-00027b90: 2320 5b6e 6f2d 656c 7365 2d63 6f6e 7469  # [no-else-conti
-00027ba0: 6e75 655d 0a20 2020 2020 2020 2020 2020  nue].           
-00027bb0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00027bc0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00027bd0: 2020 2020 7969 656c 6420 690a 0a60 6060      yield i..```
-00027be0: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
-00027bf0: 742a 2a0a 0a60 6060 7079 0a64 6566 2065  t**..```py.def e
-00027c00: 7665 6e5f 6e75 6d62 6572 5f75 6e64 6572  ven_number_under
-00027c10: 286e 3a20 696e 7429 3a0a 2020 2020 666f  (n: int):.    fo
-00027c20: 7220 6920 696e 2072 616e 6765 286e 293a  r i in range(n):
-00027c30: 0a20 2020 2020 2020 2069 6620 6925 3220  .        if i%2 
-00027c40: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00027c50: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-00027c60: 2020 2079 6965 6c64 2069 0a0a 6060 600a     yield i..```.
-00027c70: 2222 220a 0a5b 5231 3732 355d 0a77 6879  """..[R1725].why
-00027c80: 203d 2022 4974 206c 6f6f 6b73 206c 696b   = "It looks lik
-00027c90: 6520 6361 6c6c 696e 6720 7468 6520 7375  e calling the su
-00027ca0: 7065 7228 2920 6275 696c 7469 6e20 7769  per() builtin wi
-00027cb0: 7468 2074 6865 2063 7572 7265 6e74 2063  th the current c
-00027cc0: 6c61 7373 2061 6e64 2069 6e73 7461 6e63  lass and instanc
-00027cd0: 652e 204f 6e20 5079 7468 6f6e 2033 2074  e. On Python 3 t
-00027ce0: 6865 7365 2061 7267 756d 656e 7473 2061  hese arguments a
-00027cf0: 7265 2074 6865 2064 6566 6175 6c74 2061  re the default a
-00027d00: 6e64 2074 6865 7920 6361 6e20 6265 206f  nd they can be o
-00027d10: 6d69 7474 6564 2e22 0a65 7861 6d70 6c65  mitted.".example
-00027d20: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
-00027d30: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
-00027d40: 6070 790a 636c 6173 7320 4672 7569 743a  `py.class Fruit:
-00027d50: 0a20 2020 2070 6173 730a 0a0a 636c 6173  .    pass...clas
-00027d60: 7320 4f72 616e 6765 2846 7275 6974 293a  s Orange(Fruit):
-00027d70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00027d80: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00027d90: 2073 7570 6572 284f 7261 6e67 652c 2073   super(Orange, s
-00027da0: 656c 6629 2e5f 5f69 6e69 745f 5f28 2920  elf).__init__() 
-00027db0: 2023 205b 7375 7065 722d 7769 7468 2d61   # [super-with-a
-00027dc0: 7267 756d 656e 7473 5d0a 0a60 6060 0a0a  rguments]..```..
-00027dd0: 2a2a 486f 7720 746f 2066 6978 2069 742a  **How to fix it*
-00027de0: 2a0a 0a60 6060 7079 0a63 6c61 7373 2046  *..```py.class F
-00027df0: 7275 6974 3a0a 2020 2020 7061 7373 0a0a  ruit:.    pass..
-00027e00: 0a63 6c61 7373 204f 7261 6e67 6528 4672  .class Orange(Fr
-00027e10: 7569 7429 3a0a 2020 2020 6465 6620 5f5f  uit):.    def __
-00027e20: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-00027e30: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-00027e40: 696e 6974 5f5f 2829 0a0a 6060 600a 2222  init__()..```.""
-00027e50: 220a 0a5b 5231 3732 365d 0a77 6879 203d  "..[R1726].why =
-00027e60: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
-00027e70: 7468 6520 626f 6f6c 6561 6e20 636f 6e64  the boolean cond
-00027e80: 6974 696f 6e20 6973 2061 626c 6520 746f  ition is able to
-00027e90: 2062 6520 7369 6d70 6c69 6669 6564 2e22   be simplified."
-00027ea0: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
-00027eb0: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
-00027ec0: 6465 2a2a 0a0a 6060 6070 790a 6465 6620  de**..```py.def 
-00027ed0: 6861 735f 6170 706c 6573 2861 7070 6c65  has_apples(apple
-00027ee0: 7329 202d 3e20 626f 6f6c 3a0a 2020 2020  s) -> bool:.    
-00027ef0: 7265 7475 726e 2062 6f6f 6c28 6170 706c  return bool(appl
-00027f00: 6573 206f 7220 4661 6c73 6529 2020 2320  es or False)  # 
-00027f10: 5b73 696d 706c 6966 6961 626c 652d 636f  [simplifiable-co
-00027f20: 6e64 6974 696f 6e5d 0a0a 6060 600a 0a2a  ndition]..```..*
-00027f30: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
-00027f40: 0a0a 6060 6070 790a 6465 6620 6861 735f  ..```py.def has_
-00027f50: 6170 706c 6573 2861 7070 6c65 7329 202d  apples(apples) -
-00027f60: 3e20 626f 6f6c 3a0a 2020 2020 7265 7475  > bool:.    retu
-00027f70: 726e 2062 6f6f 6c28 6170 706c 6573 290a  rn bool(apples).
-00027f80: 0a60 6060 0a22 2222 0a0a 5b52 3137 3237  .```."""..[R1727
-00027f90: 5d0a 7768 7920 3d20 2249 7420 6c6f 6f6b  ].why = "It look
-00027fa0: 7320 6c69 6b65 2074 6865 2062 6f6f 6c65  s like the boole
-00027fb0: 616e 2063 6f6e 6469 7469 6f6e 2063 616e  an condition can
-00027fc0: 2062 6520 7369 6d70 6c69 6669 6564 2074   be simplified t
-00027fd0: 6f20 6120 636f 6e73 7461 6e74 2076 616c  o a constant val
-00027fe0: 7565 2e22 0a65 7861 6d70 6c65 7320 3d20  ue.".examples = 
-00027ff0: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
-00028000: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
-00028010: 6465 6620 6973 5f61 5f66 7275 6974 2866  def is_a_fruit(f
-00028020: 7275 6974 293a 0a20 2020 2072 6574 7572  ruit):.    retur
-00028030: 6e20 626f 6f6c 2866 7275 6974 2069 6e20  n bool(fruit in 
-00028040: 7b5c 2261 7070 6c65 5c22 2c20 5c22 6f72  {\"apple\", \"or
-00028050: 616e 6765 5c22 7d20 6f72 2054 7275 6529  ange\"} or True)
-00028060: 2020 2320 5b63 6f6e 6469 7469 6f6e 2d65    # [condition-e
-00028070: 7661 6c73 2d74 6f2d 636f 6e73 7461 6e74  vals-to-constant
-00028080: 5d0a 0a60 6060 0a0a 2a2a 486f 7720 746f  ]..```..**How to
-00028090: 2066 6978 2069 742a 2a0a 0a60 6060 7079   fix it**..```py
-000280a0: 0a64 6566 2069 735f 615f 6672 7569 7428  .def is_a_fruit(
-000280b0: 6672 7569 7429 3a0a 2020 2020 7265 7475  fruit):.    retu
-000280c0: 726e 2066 7275 6974 2069 6e20 7b5c 2261  rn fruit in {\"a
-000280d0: 7070 6c65 5c22 2c20 5c22 6f72 616e 6765  pple\", \"orange
-000280e0: 5c22 7d0a 0a60 6060 0a22 2222 0a0a 5b52  \"}..```."""..[R
-000280f0: 3137 3238 5d0a 7768 7920 3d20 2249 6620  1728].why = "If 
-00028100: 796f 7572 2063 6f6e 7461 696e 6572 2063  your container c
-00028110: 616e 2062 6520 6c61 7267 6520 7573 696e  an be large usin
-00028120: 6720 6120 6765 6e65 7261 746f 7220 7769  g a generator wi
-00028130: 6c6c 2062 7269 6e67 2062 6574 7465 7220  ll bring better 
-00028140: 7065 7266 6f72 6d61 6e63 652e 220a 6578  performance.".ex
-00028150: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
-00028160: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
-00028170: 2a0a 0a60 6060 7079 0a6c 6973 7428 5b30  *..```py.list([0
-00028180: 2066 6f72 2079 2069 6e20 6c69 7374 2872   for y in list(r
-00028190: 616e 6765 2831 3029 295d 2920 2023 205b  ange(10))])  # [
-000281a0: 636f 6e73 6964 6572 2d75 7369 6e67 2d67  consider-using-g
-000281b0: 656e 6572 6174 6f72 5d0a 7475 706c 6528  enerator].tuple(
-000281c0: 5b30 2066 6f72 2079 2069 6e20 6c69 7374  [0 for y in list
-000281d0: 2872 616e 6765 2831 3029 295d 2920 2023  (range(10))])  #
-000281e0: 205b 636f 6e73 6964 6572 2d75 7369 6e67   [consider-using
-000281f0: 2d67 656e 6572 6174 6f72 5d0a 7375 6d28  -generator].sum(
-00028200: 5b79 2a2a 3220 666f 7220 7920 696e 206c  [y**2 for y in l
-00028210: 6973 7428 7261 6e67 6528 3130 2929 5d29  ist(range(10))])
-00028220: 2020 2320 5b63 6f6e 7369 6465 722d 7573    # [consider-us
-00028230: 696e 672d 6765 6e65 7261 746f 725d 0a6d  ing-generator].m
-00028240: 6178 285b 792a 2a32 2066 6f72 2079 2069  ax([y**2 for y i
-00028250: 6e20 6c69 7374 2872 616e 6765 2831 3029  n list(range(10)
-00028260: 295d 2920 2023 205b 636f 6e73 6964 6572  )])  # [consider
-00028270: 2d75 7369 6e67 2d67 656e 6572 6174 6f72  -using-generator
-00028280: 5d0a 6d69 6e28 5b79 2a2a 3220 666f 7220  ].min([y**2 for 
-00028290: 7920 696e 206c 6973 7428 7261 6e67 6528  y in list(range(
-000282a0: 3130 2929 5d29 2020 2320 5b63 6f6e 7369  10))])  # [consi
-000282b0: 6465 722d 7573 696e 672d 6765 6e65 7261  der-using-genera
-000282c0: 746f 725d 0a0a 6060 600a 0a2a 2a48 6f77  tor]..```..**How
-000282d0: 2074 6f20 6669 7820 6974 2a2a 0a0a 6060   to fix it**..``
-000282e0: 6070 790a 6c69 7374 2830 2066 6f72 2079  `py.list(0 for y
-000282f0: 2069 6e20 6c69 7374 2872 616e 6765 2831   in list(range(1
-00028300: 3029 2929 0a74 7570 6c65 2830 2066 6f72  0))).tuple(0 for
-00028310: 2079 2069 6e20 6c69 7374 2872 616e 6765   y in list(range
-00028320: 2831 3029 2929 0a73 756d 2879 2a2a 3220  (10))).sum(y**2 
-00028330: 666f 7220 7920 696e 206c 6973 7428 7261  for y in list(ra
-00028340: 6e67 6528 3130 2929 290a 6d61 7828 792a  nge(10))).max(y*
-00028350: 2a32 2066 6f72 2079 2069 6e20 6c69 7374  *2 for y in list
-00028360: 2872 616e 6765 2831 3029 2929 0a6d 696e  (range(10))).min
-00028370: 2879 2a2a 3220 666f 7220 7920 696e 206c  (y**2 for y in l
-00028380: 6973 7428 7261 6e67 6528 3130 2929 290a  ist(range(10))).
-00028390: 0a60 6060 0a0a 3c61 2068 7265 663d 5c22  .```..<a href=\"
-000283a0: 6874 7470 733a 2f2f 7079 6c69 6e74 2e70  https://pylint.p
-000283b0: 7963 7161 2e6f 7267 2f65 6e2f 6c61 7465  ycqa.org/en/late
-000283c0: 7374 2f75 7365 725f 6775 6964 652f 6d65  st/user_guide/me
-000283d0: 7373 6167 6573 2f72 6566 6163 746f 722f  ssages/refactor/
-000283e0: 636f 6e73 6964 6572 2d75 7369 6e67 2d67  consider-using-g
-000283f0: 656e 6572 6174 6f72 2e68 746d 6c5c 223e  enerator.html\">
-00028400: 4164 6469 7469 6f6e 616c 2069 6e66 6f72  Additional infor
-00028410: 6d61 7469 6f6e 3c2f 613e 2222 220a 0a5b  mation</a>"""..[
-00028420: 5231 3732 395d 0a77 6879 203d 2022 436f  R1729].why = "Co
-00028430: 6d70 7265 6865 6e73 696f 6e20 696e 7369  mprehension insi
-00028440: 6465 206f 6620 2761 6e79 272c 2027 616c  de of 'any', 'al
-00028450: 6c27 2c20 276d 6178 272c 2027 6d69 6e27  l', 'max', 'min'
-00028460: 206f 7220 2773 756d 2720 6973 2075 6e6e   or 'sum' is unn
-00028470: 6563 6573 7361 7279 2e20 4120 6765 6e65  ecessary. A gene
-00028480: 7261 746f 7220 776f 756c 6420 6265 2073  rator would be s
-00028490: 7566 6669 6369 656e 7420 616e 6420 6661  ufficient and fa
-000284a0: 7374 6572 2e22 0a65 7861 6d70 6c65 7320  ster.".examples 
-000284b0: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-000284c0: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-000284d0: 790a 6672 6f6d 2072 616e 646f 6d20 696d  y.from random im
-000284e0: 706f 7274 2072 616e 6469 6e74 0a0a 616c  port randint..al
-000284f0: 6c28 5b72 616e 6469 6e74 282d 352c 2035  l([randint(-5, 5
-00028500: 2920 3e20 3020 666f 7220 5f20 696e 2072  ) > 0 for _ in r
-00028510: 616e 6765 2831 3029 5d29 2020 2320 5b75  ange(10)])  # [u
-00028520: 7365 2d61 2d67 656e 6572 6174 6f72 5d0a  se-a-generator].
-00028530: 616e 7928 5b72 616e 6469 6e74 282d 352c  any([randint(-5,
-00028540: 2035 2920 3e20 3020 666f 7220 5f20 696e   5) > 0 for _ in
-00028550: 2072 616e 6765 2831 3029 5d29 2020 2320   range(10)])  # 
-00028560: 5b75 7365 2d61 2d67 656e 6572 6174 6f72  [use-a-generator
-00028570: 5d0a 0a60 6060 0a0a 2a2a 486f 7720 746f  ]..```..**How to
-00028580: 2066 6978 2069 742a 2a0a 0a60 6060 7079   fix it**..```py
-00028590: 0a66 726f 6d20 7261 6e64 6f6d 2069 6d70  .from random imp
-000285a0: 6f72 7420 7261 6e64 696e 740a 0a61 6c6c  ort randint..all
-000285b0: 2872 616e 6469 6e74 282d 352c 2035 2920  (randint(-5, 5) 
-000285c0: 3e20 3020 666f 7220 5f20 696e 2072 616e  > 0 for _ in ran
-000285d0: 6765 2831 3029 290a 616e 7928 7261 6e64  ge(10)).any(rand
-000285e0: 696e 7428 2d35 2c20 3529 203e 2030 2066  int(-5, 5) > 0 f
-000285f0: 6f72 205f 2069 6e20 7261 6e67 6528 3130  or _ in range(10
-00028600: 2929 0a0a 6060 600a 0a3c 6120 6872 6566  ))..```..<a href
-00028610: 3d5c 2268 7474 7073 3a2f 2f70 796c 696e  =\"https://pylin
-00028620: 742e 7079 6371 612e 6f72 672f 656e 2f6c  t.pycqa.org/en/l
-00028630: 6174 6573 742f 7573 6572 5f67 7569 6465  atest/user_guide
-00028640: 2f6d 6573 7361 6765 732f 7265 6661 6374  /messages/refact
-00028650: 6f72 2f75 7365 2d61 2d67 656e 6572 6174  or/use-a-generat
-00028660: 6f72 2e68 746d 6c5c 223e 4164 6469 7469  or.html\">Additi
-00028670: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
-00028680: 3c2f 613e 2222 220a 0a5b 5231 3733 305d  </a>"""..[R1730]
-00028690: 0a77 6879 203d 2022 5573 696e 6720 7468  .why = "Using th
-000286a0: 6520 6d69 6e20 6275 696c 7469 6e20 696e  e min builtin in
-000286b0: 7374 6561 6420 6f66 2061 2063 6f6e 6469  stead of a condi
-000286c0: 7469 6f6e 616c 2069 6d70 726f 7665 7320  tional improves 
-000286d0: 7265 6164 6162 696c 6974 7920 616e 6420  readability and 
-000286e0: 636f 6e63 6973 656e 6573 732e 220a 6578  conciseness.".ex
-000286f0: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
-00028700: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
-00028710: 2a0a 0a60 6060 7079 0a64 6566 2067 6574  *..```py.def get
-00028720: 5f6d 696e 2876 616c 7565 312c 2076 616c  _min(value1, val
-00028730: 7565 3229 3a0a 2020 2020 6966 2076 616c  ue2):.    if val
-00028740: 7565 3120 3e20 7661 6c75 6532 3a20 2023  ue1 > value2:  #
-00028750: 205b 636f 6e73 6964 6572 2d75 7369 6e67   [consider-using
-00028760: 2d6d 696e 2d62 7569 6c74 696e 5d0a 2020  -min-builtin].  
-00028770: 2020 2020 2020 7661 6c75 6531 203d 2076        value1 = v
-00028780: 616c 7565 320a 2020 2020 7265 7475 726e  alue2.    return
-00028790: 2076 616c 7565 310a 0a0a 7072 696e 7428   value1...print(
-000287a0: 6765 745f 6d69 6e28 312c 2032 2929 0a0a  get_min(1, 2))..
-000287b0: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
-000287c0: 7820 6974 2a2a 0a0a 6060 6070 790a 7072  x it**..```py.pr
-000287d0: 696e 7428 6d69 6e28 312c 2032 2929 0a0a  int(min(1, 2))..
-000287e0: 6060 600a 2222 220a 0a5b 5231 3733 315d  ```."""..[R1731]
-000287f0: 0a77 6879 203d 2022 5573 696e 6720 7468  .why = "Using th
-00028800: 6520 6d61 7820 6275 696c 7469 6e20 696e  e max builtin in
-00028810: 7374 6561 6420 6f66 2061 2063 6f6e 6469  stead of a condi
-00028820: 7469 6f6e 616c 2069 6d70 726f 7665 7320  tional improves 
-00028830: 7265 6164 6162 696c 6974 7920 616e 6420  readability and 
-00028840: 636f 6e63 6973 656e 6573 732e 220a 6578  conciseness.".ex
-00028850: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
-00028860: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
-00028870: 2a0a 0a60 6060 7079 0a64 6566 2067 6574  *..```py.def get
-00028880: 5f6d 6178 2876 616c 7565 312c 2076 616c  _max(value1, val
-00028890: 7565 3229 3a0a 2020 2020 6966 2076 616c  ue2):.    if val
-000288a0: 7565 3120 3c20 7661 6c75 6532 3a20 2023  ue1 < value2:  #
-000288b0: 205b 636f 6e73 6964 6572 2d75 7369 6e67   [consider-using
-000288c0: 2d6d 6178 2d62 7569 6c74 696e 5d0a 2020  -max-builtin].  
-000288d0: 2020 2020 2020 7661 6c75 6531 203d 2076        value1 = v
-000288e0: 616c 7565 320a 2020 2020 7265 7475 726e  alue2.    return
-000288f0: 2076 616c 7565 310a 0a0a 7072 696e 7428   value1...print(
-00028900: 6765 745f 6d61 7828 312c 2032 2929 0a0a  get_max(1, 2))..
-00028910: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
-00028920: 7820 6974 2a2a 0a0a 6060 6070 790a 7072  x it**..```py.pr
-00028930: 696e 7428 6d61 7828 312c 2032 2929 0a0a  int(max(1, 2))..
-00028940: 6060 600a 2222 220a 0a5b 5231 3733 325d  ```."""..[R1732]
-00028950: 0a77 6879 203d 2022 456d 6974 7465 6420  .why = "Emitted 
-00028960: 6966 2061 2072 6573 6f75 7263 652d 616c  if a resource-al
-00028970: 6c6f 6361 7469 6e67 2061 7373 6967 6e6d  locating assignm
-00028980: 656e 7420 6f72 2063 616c 6c20 6d61 7920  ent or call may 
-00028990: 6265 2072 6570 6c61 6365 6420 6279 2061  be replaced by a
-000289a0: 2027 7769 7468 2720 626c 6f63 6b2e 2042   'with' block. B
-000289b0: 7920 7573 696e 6720 2777 6974 6827 2074  y using 'with' t
-000289c0: 6865 2072 656c 6561 7365 206f 6620 7468  he release of th
-000289d0: 6520 616c 6c6f 6361 7465 6420 7265 736f  e allocated reso
-000289e0: 7572 6365 7320 6973 2065 6e73 7572 6564  urces is ensured
-000289f0: 2065 7665 6e20 696e 2074 6865 2063 6173   even in the cas
-00028a00: 6520 6f66 2061 6e20 6578 6365 7074 696f  e of an exceptio
-00028a10: 6e2e 220a 6578 616d 706c 6573 203d 2022  n.".examples = "
-00028a20: 2222 0a2a 2a50 726f 626c 656d 6174 6963  "".**Problematic
-00028a30: 2063 6f64 652a 2a0a 0a60 6060 7079 0a66   code**..```py.f
-00028a40: 696c 6520 3d20 6f70 656e 285c 2261 7070  ile = open(\"app
-00028a50: 6c65 2e74 7874 5c22 2c20 5c22 725c 222c  le.txt\", \"r\",
-00028a60: 2065 6e63 6f64 696e 673d 5c22 7574 6638   encoding=\"utf8
-00028a70: 5c22 2920 2023 205b 636f 6e73 6964 6572  \")  # [consider
-00028a80: 2d75 7369 6e67 2d77 6974 685d 0a63 6f6e  -using-with].con
-00028a90: 7465 6e74 7320 3d20 6669 6c65 2e72 6561  tents = file.rea
-00028aa0: 6428 290a 6669 6c65 2e63 6c6f 7365 2829  d().file.close()
-00028ab0: 0a0a 776f 7273 7420 3d20 6f70 656e 285c  ..worst = open(\
+00023db0: 696d 706f 7274 206f 732e 7061 7468 2061  import os.path a
+00023dc0: 7320 7061 7468 2020 2320 5b63 6f6e 7369  s path  # [consi
+00023dd0: 6465 722d 7573 696e 672d 6672 6f6d 2d69  der-using-from-i
+00023de0: 6d70 6f72 745d 0a0a 6060 600a 0a2a 2a48  mport]..```..**H
+00023df0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00023e00: 6060 6070 790a 6672 6f6d 206f 7320 696d  ```py.from os im
+00023e10: 706f 7274 2070 6174 680a 0a60 6060 0a22  port path..```."
+00023e20: 2222 0a0a 5b52 3032 3034 5d0a 7768 7920  ""..[R0204].why 
+00023e30: 3d20 2249 7420 6c6f 6f6b 7320 6c69 6b65  = "It looks like
+00023e40: 2074 6865 2074 7970 6520 6f66 2061 2076   the type of a v
+00023e50: 6172 6961 626c 6520 6368 616e 6765 7320  ariable changes 
+00023e60: 696e 7369 6465 2061 206d 6574 686f 6420  inside a method 
+00023e70: 6f72 2061 2066 756e 6374 696f 6e2e 220a  or a function.".
+00023e80: 6578 616d 706c 6573 203d 2022 2222 0a2a  examples = """.*
+00023e90: 2a50 726f 626c 656d 6174 6963 2063 6f64  *Problematic cod
+00023ea0: 652a 2a0a 0a60 6060 7079 0a78 203d 2031  e**..```py.x = 1
+00023eb0: 0a78 203d 205c 2232 5c22 2020 2320 5b72  .x = \"2\"  # [r
+00023ec0: 6564 6566 696e 6564 2d76 6172 6961 626c  edefined-variabl
+00023ed0: 652d 7479 7065 5d0a 0a60 6060 0a0a 2a2a  e-type]..```..**
+00023ee0: 486f 7720 746f 2066 6978 2069 742a 2a0a  How to fix it**.
+00023ef0: 0a60 6060 7079 0a78 203d 2031 0a78 203d  .```py.x = 1.x =
+00023f00: 2032 0a0a 6060 600a 2222 220a 0a5b 5236   2..```."""..[R6
+00023f10: 3330 315d 0a77 6879 203d 2022 5468 6520  301].why = "The 
+00023f20: 636f 6e64 6974 696f 6e20 6f66 2061 2060  condition of a `
+00023f30: 7768 696c 6560 206c 6f6f 7020 7361 7973  while` loop says
+00023f40: 2061 206c 6f74 2061 626f 7574 2077 6861   a lot about wha
+00023f50: 7420 7468 6520 6c6f 6f70 2064 6f65 732e  t the loop does.
+00023f60: 2049 7420 6973 2061 6c73 6f20 6561 7369   It is also easi
+00023f70: 6572 2074 6f20 7665 7269 6679 2074 6861  er to verify tha
+00023f80: 7420 7468 6520 6c6f 6f70 2077 696c 6c20  t the loop will 
+00023f90: 656e 642e 220a 6578 616d 706c 6573 203d  end.".examples =
+00023fa0: 2022 2222 0a60 6060 7079 0a64 6566 2070   """.```py.def p
+00023fb0: 726f 626c 656d 6174 6963 286e 293a 0a20  roblematic(n):. 
+00023fc0: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
+00023fd0: 2020 2020 2020 2069 6620 6e20 3d3d 2031         if n == 1
+00023fe0: 3a0a 2020 2020 2020 2020 2020 2020 6272  :.            br
+00023ff0: 6561 6b0a 2020 2020 2020 2020 2320 736f  eak.        # so
+00024000: 6d65 2063 6f64 650a 0a64 6566 2067 6f6f  me code..def goo
+00024010: 6428 6e29 3a0a 2020 2020 7768 696c 6520  d(n):.    while 
+00024020: 6e20 213d 2031 3a0a 2020 2020 2020 2020  n != 1:.        
+00024030: 2320 736f 6d65 2063 6f64 650a 6060 600a  # some code.```.
+00024040: 2222 220a 0a5b 5236 3230 315d 0a77 6879  """..[R6201].why
+00024050: 203d 2022 4861 7669 6e67 2075 6e6e 6563   = "Having unnec
+00024060: 6573 7361 7279 2063 6f6e 6469 7469 6f6e  essary condition
+00024070: 7320 696e 2063 6f64 6520 6d61 6b65 7320  s in code makes 
+00024080: 7468 6520 636f 6465 206d 6f72 6520 636c  the code more cl
+00024090: 7574 7465 7265 6420 616e 6420 7468 6572  uttered and ther
+000240a0: 6566 6f72 6520 6861 7264 6572 2074 6f20  efore harder to 
+000240b0: 756e 6465 7273 7461 6e64 2e22 0a65 7861  understand.".exa
+000240c0: 6d70 6c65 7320 3d20 2222 220a 4120 636f  mples = """.A co
+000240d0: 6e64 6974 696f 6e20 7468 6174 2072 6574  ndition that ret
+000240e0: 7572 6e73 2062 6f6f 6c20 696e 2062 6f74  urns bool in bot
+000240f0: 6820 6272 616e 6368 6573 2063 616e 2062  h branches can b
+00024100: 6520 7369 6d70 6c69 6669 6564 2065 7665  e simplified eve
+00024110: 6e20 6966 2069 7420 636f 6e74 6169 6e73  n if it contains
+00024120: 2061 206c 6f67 6963 616c 2073 7461 7465   a logical state
+00024130: 6d65 6e74 2e0a 0a60 6060 7079 0a64 6566  ment...```py.def
+00024140: 2070 726f 626c 656d 6174 6963 2861 3a20   problematic(a: 
+00024150: 626f 6f6c 2c20 623a 2062 6f6f 6c29 202d  bool, b: bool) -
+00024160: 3e20 626f 6f6c 3a0a 2020 2020 6966 2061  > bool:.    if a
+00024170: 206f 7220 623a 0a20 2020 2020 2020 2072   or b:.        r
+00024180: 6574 7572 6e20 5472 7565 0a20 2020 2065  eturn True.    e
+00024190: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+000241a0: 7572 6e20 4661 6c73 650a 6060 600a 0a60  urn False.```..`
+000241b0: 6060 7079 0a64 6566 2067 6f6f 6428 613a  ``py.def good(a:
+000241c0: 2062 6f6f 6c2c 2062 3a20 626f 6f6c 2920   bool, b: bool) 
+000241d0: 2d3e 2062 6f6f 6c3a 0a20 2020 2072 6574  -> bool:.    ret
+000241e0: 7572 6e20 6120 6f72 2062 0a60 6060 0a22  urn a or b.```."
+000241f0: 2222 0a0a 5b52 3230 3434 5d0a 7768 7920  ""..[R2044].why 
+00024200: 3d20 2249 7420 6c6f 6f6b 7320 6c69 6b65  = "It looks like
+00024210: 2074 6865 2023 2073 796d 626f 6c20 6170   the # symbol ap
+00024220: 7065 6172 7320 6f6e 2061 206c 696e 6520  pears on a line 
+00024230: 6e6f 7420 666f 6c6c 6f77 6564 2062 7920  not followed by 
+00024240: 616e 2061 6374 7561 6c20 636f 6d6d 656e  an actual commen
+00024250: 7422 0a65 7861 6d70 6c65 7320 3d20 2222  t".examples = ""
+00024260: 220a 2a2a 5072 6f62 6c65 6d61 7469 6320  ".**Problematic 
+00024270: 636f 6465 2a2a 0a0a 6060 6070 790a 2320  code**..```py.# 
+00024280: 2b31 3a5b 656d 7074 792d 636f 6d6d 656e  +1:[empty-commen
+00024290: 745d 0a23 0a0a 2320 2b31 3a5b 656d 7074  t].#..# +1:[empt
+000242a0: 792d 636f 6d6d 656e 745d 0a78 203d 2030  y-comment].x = 0
+000242b0: 2020 230a 0a60 6060 0a0a 2a2a 486f 7720    #..```..**How 
+000242c0: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
+000242d0: 7079 0a23 2063 6f6d 6d65 6e74 0a0a 7820  py.# comment..x 
+000242e0: 3d20 3020 2023 2063 6f6d 6d65 6e74 0a0a  = 0  # comment..
+000242f0: 6060 600a 2222 220a 0a5b 5231 3730 315d  ```."""..[R1701]
+00024300: 0a77 6879 203d 2022 4974 206c 6f6f 6b73  .why = "It looks
+00024310: 206c 696b 6520 6d75 6c74 6970 6c65 2063   like multiple c
+00024320: 6f6e 7365 6375 7469 7665 2069 7369 6e73  onsecutive isins
+00024330: 7461 6e63 6520 6361 6c6c 7320 6361 6e20  tance calls can 
+00024340: 6265 206d 6572 6765 6420 696e 746f 206f  be merged into o
+00024350: 6e65 2e22 0a65 7861 6d70 6c65 7320 3d20  ne.".examples = 
+00024360: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
+00024370: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
+00024380: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00024390: 7274 2041 6e79 0a0a 0a64 6566 2069 735f  rt Any...def is_
+000243a0: 6e75 6d62 6572 2876 616c 7565 3a20 416e  number(value: An
+000243b0: 7929 202d 3e20 626f 6f6c 3a0a 2020 2020  y) -> bool:.    
+000243c0: 7265 7475 726e 2069 7369 6e73 7461 6e63  return isinstanc
+000243d0: 6528 7661 6c75 652c 2069 6e74 2920 6f72  e(value, int) or
+000243e0: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
+000243f0: 652c 2066 6c6f 6174 2920 2023 205b 636f  e, float)  # [co
+00024400: 6e73 6964 6572 2d6d 6572 6769 6e67 2d69  nsider-merging-i
+00024410: 7369 6e73 7461 6e63 655d 0a0a 6060 600a  sinstance]..```.
+00024420: 0a2a 2a48 6f77 2074 6f20 6669 7820 6974  .**How to fix it
+00024430: 2a2a 0a0a 6060 6070 790a 6672 6f6d 2074  **..```py.from t
+00024440: 7970 696e 6720 696d 706f 7274 2041 6e79  yping import Any
+00024450: 0a0a 0a64 6566 2069 735f 6e75 6d62 6572  ...def is_number
+00024460: 2876 616c 7565 3a20 416e 7929 202d 3e20  (value: Any) -> 
+00024470: 626f 6f6c 3a0a 2020 2020 7265 7475 726e  bool:.    return
+00024480: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
+00024490: 652c 2028 696e 742c 2066 6c6f 6174 2929  e, (int, float))
+000244a0: 0a0a 6060 600a 2222 220a 0a5b 5231 3730  ..```."""..[R170
+000244b0: 325d 0a77 6879 203d 2022 436f 6e73 6964  2].why = "Consid
+000244c0: 6572 206d 6f76 696e 6720 736f 6d65 206f  er moving some o
+000244d0: 6620 7468 6520 636f 6465 2074 6f20 6865  f the code to he
+000244e0: 6c70 6572 2066 756e 6374 696f 6e73 2e22  lper functions."
+000244f0: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
+00024500: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
+00024510: 6465 2a2a 0a0a 6060 6070 790a 6465 6620  de**..```py.def 
+00024520: 636f 7272 6563 745f 6672 7569 7473 2866  correct_fruits(f
+00024530: 7275 6974 7329 3a0a 2020 2020 6966 206c  ruits):.    if l
+00024540: 656e 2866 7275 6974 7329 203e 2031 3a20  en(fruits) > 1: 
+00024550: 2023 205b 746f 6f2d 6d61 6e79 2d6e 6573   # [too-many-nes
+00024560: 7465 642d 626c 6f63 6b73 5d0a 2020 2020  ted-blocks].    
+00024570: 2020 2020 6966 205c 2261 7070 6c65 5c22      if \"apple\"
+00024580: 2069 6e20 6672 7569 7473 3a0a 2020 2020   in fruits:.    
+00024590: 2020 2020 2020 2020 6966 205c 226f 7261          if \"ora
+000245a0: 6e67 655c 2220 696e 2066 7275 6974 733a  nge\" in fruits:
+000245b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000245c0: 2063 6f75 6e74 203d 2066 7275 6974 735b   count = fruits[
+000245d0: 5c22 6f72 616e 6765 5c22 5d0a 2020 2020  \"orange\"].    
+000245e0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+000245f0: 6f75 6e74 2025 2032 3a0a 2020 2020 2020  ount % 2:.      
+00024600: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00024610: 205c 226b 6977 695c 2220 696e 2066 7275   \"kiwi\" in fru
+00024620: 6974 733a 0a20 2020 2020 2020 2020 2020  its:.           
+00024630: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00024640: 636f 756e 7420 3d3d 2032 3a0a 2020 2020  count == 2:.    
+00024650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024660: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00024670: 7275 650a 2020 2020 7265 7475 726e 2046  rue.    return F
+00024680: 616c 7365 0a0a 6060 600a 0a2a 2a48 6f77  alse..```..**How
+00024690: 2074 6f20 6669 7820 6974 2a2a 0a0a 6060   to fix it**..``
+000246a0: 6070 790a 6465 6620 636f 7272 6563 745f  `py.def correct_
+000246b0: 6672 7569 7473 2866 7275 6974 7329 3a0a  fruits(fruits):.
+000246c0: 2020 2020 6966 206c 656e 2866 7275 6974      if len(fruit
+000246d0: 7329 203e 2031 2061 6e64 205c 2261 7070  s) > 1 and \"app
+000246e0: 6c65 5c22 2069 6e20 6672 7569 7473 2061  le\" in fruits a
+000246f0: 6e64 205c 226f 7261 6e67 655c 2220 696e  nd \"orange\" in
+00024700: 2066 7275 6974 733a 0a20 2020 2020 2020   fruits:.       
+00024710: 2063 6f75 6e74 203d 2066 7275 6974 735b   count = fruits[
+00024720: 5c22 6f72 616e 6765 5c22 5d0a 2020 2020  \"orange\"].    
+00024730: 2020 2020 6966 2063 6f75 6e74 2025 2032      if count % 2
+00024740: 2061 6e64 205c 226b 6977 695c 2220 696e   and \"kiwi\" in
+00024750: 2066 7275 6974 7320 616e 6420 636f 756e   fruits and coun
+00024760: 7420 3d3d 2032 3a0a 2020 2020 2020 2020  t == 2:.        
+00024770: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00024780: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00024790: 0a0a 6060 600a 2222 220a 0a5b 5231 3730  ..```."""..[R170
+000247a0: 335d 0a77 6879 203d 2022 4974 206c 6f6f  3].why = "It loo
+000247b0: 6b73 206c 696b 6520 7468 6520 6966 2073  ks like the if s
+000247c0: 7461 7465 6d65 6e74 2063 616e 2062 6520  tatement can be 
+000247d0: 7265 706c 6163 6564 2077 6974 6820 2762  replaced with 'b
+000247e0: 6f6f 6c28 7465 7374 2927 2e22 0a65 7861  ool(test)'.".exa
+000247f0: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
+00024800: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
+00024810: 0a0a 6060 6070 790a 464c 5949 4e47 5f54  ..```py.FLYING_T
+00024820: 4849 4e47 5320 3d20 5b5c 2262 6972 645c  HINGS = [\"bird\
+00024830: 222c 205c 2270 6c61 6e65 5c22 2c20 5c22  ", \"plane\", \"
+00024840: 7375 7065 726d 616e 5c22 2c20 5c22 7468  superman\", \"th
+00024850: 6973 2065 7861 6d70 6c65 5c22 5d0a 0a0a  is example\"]...
+00024860: 6465 6620 6973 5f66 6c79 696e 675f 616e  def is_flying_an
+00024870: 696d 616c 2861 6e5f 6f62 6a65 6374 293a  imal(an_object):
+00024880: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00024890: 6365 2861 6e5f 6f62 6a65 6374 2c20 416e  ce(an_object, An
+000248a0: 696d 616c 2920 616e 6420 616e 5f6f 626a  imal) and an_obj
+000248b0: 6563 7420 696e 2046 4c59 494e 475f 5448  ect in FLYING_TH
+000248c0: 494e 4753 3a20 2023 205b 7369 6d70 6c69  INGS:  # [simpli
+000248d0: 6669 6162 6c65 2d69 662d 7374 6174 656d  fiable-if-statem
+000248e0: 656e 745d 0a20 2020 2020 2020 2069 735f  ent].        is_
+000248f0: 666c 7969 6e67 203d 2054 7275 650a 2020  flying = True.  
+00024900: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00024910: 6973 5f66 6c79 696e 6720 3d20 4661 6c73  is_flying = Fals
+00024920: 650a 2020 2020 7265 7475 726e 2069 735f  e.    return is_
+00024930: 666c 7969 6e67 0a0a 6060 600a 0a2a 2a48  flying..```..**H
+00024940: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00024950: 6060 6070 790a 464c 5949 4e47 5f54 4849  ```py.FLYING_THI
+00024960: 4e47 5320 3d20 5b5c 2262 6972 645c 222c  NGS = [\"bird\",
+00024970: 205c 2270 6c61 6e65 5c22 2c20 5c22 7375   \"plane\", \"su
+00024980: 7065 726d 616e 5c22 2c20 5c22 7468 6973  perman\", \"this
+00024990: 2065 7861 6d70 6c65 5c22 5d0a 0a0a 6465   example\"]...de
+000249a0: 6620 6973 5f66 6c79 696e 675f 616e 696d  f is_flying_anim
+000249b0: 616c 2861 6e5f 6f62 6a65 6374 293a 0a20  al(an_object):. 
+000249c0: 2020 2069 735f 666c 7969 6e67 203d 2069     is_flying = i
+000249d0: 7369 6e73 7461 6e63 6528 616e 5f6f 626a  sinstance(an_obj
+000249e0: 6563 742c 2041 6e69 6d61 6c29 2061 6e64  ect, Animal) and
+000249f0: 2061 6e5f 6f62 6a65 6374 2e6e 616d 6520   an_object.name 
+00024a00: 696e 2046 4c59 494e 475f 5448 494e 4753  in FLYING_THINGS
+00024a10: 0a20 2020 2072 6574 7572 6e20 6973 5f66  .    return is_f
+00024a20: 6c79 696e 670a 0a60 6060 0a22 2222 0a0a  lying..```."""..
+00024a30: 5b52 3137 3034 5d0a 7768 7920 3d20 2244  [R1704].why = "D
+00024a40: 6964 2079 6f75 206e 6f74 6963 6520 7468  id you notice th
+00024a50: 6174 2061 6e20 6172 6775 6d65 6e74 2067  at an argument g
+00024a60: 6574 7320 6f76 6572 7772 6974 7465 6e20  ets overwritten 
+00024a70: 6865 7265 3f22 0a65 7861 6d70 6c65 7320  here?".examples 
+00024a80: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
+00024a90: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
+00024aa0: 790a 6465 6620 7368 6f77 2868 6f73 745f  y.def show(host_
+00024ab0: 6964 3d31 302e 3131 293a 0a20 2020 2066  id=10.11):.    f
+00024ac0: 6f72 2068 6f73 745f 6964 2c20 686f 7374  or host_id, host
+00024ad0: 2069 6e20 5b5b 3132 2e31 332c 2027 5665   in [[12.13, 'Ve
+00024ae0: 6e75 7327 5d2c 205b 3134 2e31 352c 2027  nus'], [14.15, '
+00024af0: 4d61 7273 275d 5d3a 2020 2320 5b72 6564  Mars']]:  # [red
+00024b00: 6566 696e 6564 2d61 7267 756d 656e 742d  efined-argument-
+00024b10: 6672 6f6d 2d6c 6f63 616c 5d0a 2020 2020  from-local].    
+00024b20: 2020 2020 7072 696e 7428 686f 7374 5f69      print(host_i
+00024b30: 642c 2068 6f73 7429 0a0a 6060 600a 0a2a  d, host)..```..*
+00024b40: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
+00024b50: 0a0a 6060 6070 790a 6465 6620 7368 6f77  ..```py.def show
+00024b60: 2868 6f73 745f 6964 3d31 302e 3131 293a  (host_id=10.11):
+00024b70: 0a20 2020 2066 6f72 2069 6e6e 6572 5f68  .    for inner_h
+00024b80: 6f73 745f 6964 2c20 686f 7374 2069 6e20  ost_id, host in 
+00024b90: 5b5b 3132 2e31 332c 2027 5665 6e75 7327  [[12.13, 'Venus'
+00024ba0: 5d2c 205b 3134 2e31 352c 2027 4d61 7273  ], [14.15, 'Mars
+00024bb0: 275d 5d3a 0a20 2020 2020 2020 2070 7269  ']]:.        pri
+00024bc0: 6e74 2868 6f73 745f 6964 2c20 696e 6e65  nt(host_id, inne
+00024bd0: 725f 686f 7374 5f69 642c 2068 6f73 7429  r_host_id, host)
+00024be0: 0a0a 6060 600a 2222 220a 0a5b 5231 3730  ..```."""..[R170
+00024bf0: 355d 0a77 6879 203d 2022 5573 6564 2069  5].why = "Used i
+00024c00: 6e20 6f72 6465 7220 746f 2068 6967 686c  n order to highl
+00024c10: 6967 6874 2061 6e20 756e 6e65 6365 7373  ight an unnecess
+00024c20: 6172 7920 626c 6f63 6b20 6f66 2063 6f64  ary block of cod
+00024c30: 6520 666f 6c6c 6f77 696e 6720 616e 2069  e following an i
+00024c40: 6620 636f 6e74 6169 6e69 6e67 2061 2072  f containing a r
+00024c50: 6574 7572 6e20 7374 6174 656d 656e 742e  eturn statement.
+00024c60: 2041 7320 7375 6368 2c20 6974 2077 696c   As such, it wil
+00024c70: 6c20 7761 726e 2077 6865 6e20 6974 2065  l warn when it e
+00024c80: 6e63 6f75 6e74 6572 7320 616e 2065 6c73  ncounters an els
+00024c90: 6520 666f 6c6c 6f77 696e 6720 6120 6368  e following a ch
+00024ca0: 6169 6e20 6f66 2069 6673 2c20 616c 6c20  ain of ifs, all 
+00024cb0: 6f66 2074 6865 6d20 636f 6e74 6169 6e69  of them containi
+00024cc0: 6e67 2061 2072 6574 7572 6e20 7374 6174  ng a return stat
+00024cd0: 656d 656e 742e 220a 6578 616d 706c 6573  ement.".examples
+00024ce0: 203d 2022 2222 0a2a 2a50 726f 626c 656d   = """.**Problem
+00024cf0: 6174 6963 2063 6f64 652a 2a0a 0a60 6060  atic code**..```
+00024d00: 7079 0a64 6566 2063 6f6d 7061 7265 5f6e  py.def compare_n
+00024d10: 756d 6265 7273 2861 3a20 696e 742c 2062  umbers(a: int, b
+00024d20: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
+00024d30: 2020 2069 6620 6120 3d3d 2062 3a20 2023     if a == b:  #
+00024d40: 205b 6e6f 2d65 6c73 652d 7265 7475 726e   [no-else-return
+00024d50: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+00024d60: 2030 0a20 2020 2065 6c69 6620 6120 3c20   0.    elif a < 
+00024d70: 623a 0a20 2020 2020 2020 2072 6574 7572  b:.        retur
+00024d80: 6e20 2d31 0a20 2020 2065 6c73 653a 0a20  n -1.    else:. 
+00024d90: 2020 2020 2020 2072 6574 7572 6e20 310a         return 1.
+00024da0: 0a60 6060 0a0a 2a2a 486f 7720 746f 2066  .```..**How to f
+00024db0: 6978 2069 742a 2a0a 0a60 6060 7079 0a64  ix it**..```py.d
+00024dc0: 6566 2063 6f6d 7061 7265 5f6e 756d 6265  ef compare_numbe
+00024dd0: 7273 2861 3a20 696e 742c 2062 3a20 696e  rs(a: int, b: in
+00024de0: 7429 202d 3e20 696e 743a 0a20 2020 2069  t) -> int:.    i
+00024df0: 6620 6120 3d3d 2062 3a0a 2020 2020 2020  f a == b:.      
+00024e00: 2020 7265 7475 726e 2030 0a20 2020 2069    return 0.    i
+00024e10: 6620 6120 3c20 623a 0a20 2020 2020 2020  f a < b:.       
+00024e20: 2072 6574 7572 6e20 2d31 0a20 2020 2072   return -1.    r
+00024e30: 6574 7572 6e20 310a 0a60 6060 0a22 2222  eturn 1..```."""
+00024e40: 0a0a 5b52 3137 3036 5d0a 7768 7920 3d20  ..[R1706].why = 
+00024e50: 2249 7420 6c6f 6f6b 7320 6c69 6b65 206f  "It looks like o
+00024e60: 6e65 206f 6620 6b6e 6f77 6e20 7072 652d  ne of known pre-
+00024e70: 7079 7468 6f6e 2032 2e35 2074 6572 6e61  python 2.5 terna
+00024e80: 7279 2073 796e 7461 7820 6973 2075 7365  ry syntax is use
+00024e90: 642e 220a 6578 616d 706c 6573 203d 2022  d.".examples = "
+00024ea0: 2222 0a2a 2a50 726f 626c 656d 6174 6963  "".**Problematic
+00024eb0: 2063 6f64 652a 2a0a 0a60 6060 7079 0a78   code**..```py.x
+00024ec0: 2c20 7920 3d20 312c 2032 0a6d 6178 696d  , y = 1, 2.maxim
+00024ed0: 756d 203d 2078 203e 3d20 7920 616e 6420  um = x >= y and 
+00024ee0: 7820 6f72 2079 2020 2320 5b63 6f6e 7369  x or y  # [consi
+00024ef0: 6465 722d 7573 696e 672d 7465 726e 6172  der-using-ternar
+00024f00: 795d 0a0a 6060 600a 0a2a 2a48 6f77 2074  y]..```..**How t
+00024f10: 6f20 6669 7820 6974 2a2a 0a0a 6060 6070  o fix it**..```p
+00024f20: 790a 782c 2079 203d 2031 2c20 320a 6d61  y.x, y = 1, 2.ma
+00024f30: 7869 6d75 6d20 3d20 7820 6966 2078 203e  ximum = x if x >
+00024f40: 3d20 7920 656c 7365 2079 0a0a 6060 600a  = y else y..```.
+00024f50: 2222 220a 0a5b 5231 3730 375d 0a77 6879  """..[R1707].why
+00024f60: 203d 2022 496e 2050 7974 686f 6e2c 2061   = "In Python, a
+00024f70: 2074 7570 6c65 2069 7320 6163 7475 616c   tuple is actual
+00024f80: 6c79 2063 7265 6174 6564 2062 7920 7468  ly created by th
+00024f90: 6520 636f 6d6d 6120 7379 6d62 6f6c 2c20  e comma symbol, 
+00024fa0: 6e6f 7420 6279 2074 6865 2070 6172 656e  not by the paren
+00024fb0: 7468 6573 6573 2e20 556e 666f 7274 756e  theses. Unfortun
+00024fc0: 6174 656c 792c 206f 6e65 2063 616e 2061  ately, one can a
+00024fd0: 6374 7561 6c6c 7920 6372 6561 7465 2061  ctually create a
+00024fe0: 2074 7570 6c65 2062 7920 6d69 7370 6c61   tuple by mispla
+00024ff0: 6369 6e67 2061 2074 7261 696c 696e 6720  cing a trailing 
+00025000: 636f 6d6d 612c 2077 6869 6368 2063 616e  comma, which can
+00025010: 206c 6561 6420 746f 2070 6f74 656e 7469   lead to potenti
+00025020: 616c 2077 6569 7264 2062 7567 7320 696e  al weird bugs in
+00025030: 2079 6f75 7220 636f 6465 2e20 596f 7520   your code. You 
+00025040: 7368 6f75 6c64 2061 6c77 6179 7320 7573  should always us
+00025050: 6520 7061 7265 6e74 6865 7365 7320 6578  e parentheses ex
+00025060: 706c 6963 6974 6c79 2066 6f72 2063 7265  plicitly for cre
+00025070: 6174 696e 6720 6120 7475 706c 652e 220a  ating a tuple.".
+00025080: 6578 616d 706c 6573 203d 2022 2222 0a2a  examples = """.*
+00025090: 2a50 726f 626c 656d 6174 6963 2063 6f64  *Problematic cod
+000250a0: 652a 2a0a 0a60 6060 7079 0a43 4f4d 5041  e**..```py.COMPA
+000250b0: 5353 203d 205c 226e 6f72 7468 5c22 2c20  SS = \"north\", 
+000250c0: 5c22 736f 7574 685c 222c 205c 2265 6173  \"south\", \"eas
+000250d0: 745c 222c 205c 2277 6573 745c 222c 2020  t\", \"west\",  
+000250e0: 2320 5b74 7261 696c 696e 672d 636f 6d6d  # [trailing-comm
+000250f0: 612d 7475 706c 655d 0a0a 6060 600a 0a2a  a-tuple]..```..*
+00025100: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
+00025110: 0a0a 6060 6070 790a 434f 4d50 4153 5320  ..```py.COMPASS 
+00025120: 3d20 285c 226e 6f72 7468 5c22 2c20 5c22  = (\"north\", \"
+00025130: 736f 7574 685c 222c 205c 2265 6173 745c  south\", \"east\
+00025140: 222c 205c 2277 6573 745c 2229 0a0a 6060  ", \"west\")..``
+00025150: 600a 2222 220a 0a5b 5231 3730 385d 0a77  `."""..[R1708].w
+00025160: 6879 203d 2022 4163 636f 7264 696e 6720  hy = "According 
+00025170: 746f 2050 4550 3437 392c 2074 6865 2072  to PEP479, the r
+00025180: 6169 7365 206f 6620 5374 6f70 4974 6572  aise of StopIter
+00025190: 6174 696f 6e20 746f 2065 6e64 2074 6865  ation to end the
+000251a0: 206c 6f6f 7020 6f66 2061 2067 656e 6572   loop of a gener
+000251b0: 6174 6f72 206d 6179 206c 6561 6420 746f  ator may lead to
+000251c0: 2068 6172 6420 746f 2066 696e 6420 6275   hard to find bu
+000251d0: 6773 2e20 5468 6973 2050 4550 2073 7065  gs. This PEP spe
+000251e0: 6369 6679 2074 6861 7420 7261 6973 6520  cify that raise 
+000251f0: 5374 6f70 4974 6572 6174 696f 6e20 6861  StopIteration ha
+00025200: 7320 746f 2062 6520 7265 706c 6163 6564  s to be replaced
+00025210: 2062 7920 6120 7369 6d70 6c65 2072 6574   by a simple ret
+00025220: 7572 6e20 7374 6174 656d 656e 7422 0a65  urn statement".e
+00025230: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
+00025240: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
+00025250: 2a2a 0a0a 6060 6070 790a 6465 6620 6672  **..```py.def fr
+00025260: 7569 745f 6765 6e65 7261 746f 7228 293a  uit_generator():
+00025270: 0a20 2020 2066 6f72 2066 7275 6974 2069  .    for fruit i
+00025280: 6e20 5b5c 2261 7070 6c65 5c22 2c20 5c22  n [\"apple\", \"
+00025290: 6261 6e61 6e61 5c22 5d3a 0a20 2020 2020  banana\"]:.     
+000252a0: 2020 2079 6965 6c64 2066 7275 6974 0a20     yield fruit. 
+000252b0: 2020 2072 6169 7365 2053 746f 7049 7465     raise StopIte
+000252c0: 7261 7469 6f6e 2020 2320 5b73 746f 702d  ration  # [stop-
+000252d0: 6974 6572 6174 696f 6e2d 7265 7475 726e  iteration-return
+000252e0: 5d0a 0a0a 6465 6620 7477 6f5f 6672 7569  ]...def two_frui
+000252f0: 7473 5f67 656e 6572 6174 6f72 2866 7275  ts_generator(fru
+00025300: 6974 7329 3a0a 2020 2020 666f 7220 6672  its):.    for fr
+00025310: 7569 7420 696e 2066 7275 6974 733a 0a20  uit in fruits:. 
+00025320: 2020 2020 2020 2079 6965 6c64 2066 7275         yield fru
+00025330: 6974 2c20 6e65 7874 2866 7275 6974 7329  it, next(fruits)
+00025340: 2020 2320 5b73 746f 702d 6974 6572 6174    # [stop-iterat
+00025350: 696f 6e2d 7265 7475 726e 5d0a 0a0a 6465  ion-return]...de
+00025360: 6620 7477 6f5f 676f 6f64 5f66 7275 6974  f two_good_fruit
+00025370: 735f 6765 6e65 7261 746f 7228 6672 7569  s_generator(frui
+00025380: 7473 293a 0a20 2020 2066 6f72 2066 7275  ts):.    for fru
+00025390: 6974 2069 6e20 6672 7569 7473 3a0a 2020  it in fruits:.  
+000253a0: 2020 2020 2020 6966 206e 6f74 2066 7275        if not fru
+000253b0: 6974 2e69 735f 7461 7374 7928 293a 0a20  it.is_tasty():. 
+000253c0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+000253d0: 6e75 650a 2020 2020 2020 2020 7768 696c  nue.        whil
+000253e0: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
+000253f0: 2020 2020 6e65 7874 5f66 7275 6974 203d      next_fruit =
+00025400: 206e 6578 7428 6672 7569 7473 2920 2023   next(fruits)  #
+00025410: 205b 7374 6f70 2d69 7465 7261 7469 6f6e   [stop-iteration
+00025420: 2d72 6574 7572 6e5d 0a20 2020 2020 2020  -return].       
+00025430: 2020 2020 2069 6620 6e65 7874 5f66 7275       if next_fru
+00025440: 6974 2e69 735f 7461 7374 7928 293a 0a20  it.is_tasty():. 
+00025450: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00025460: 6965 6c64 2066 7275 6974 2c20 6e65 7874  ield fruit, next
+00025470: 5f66 7275 6974 0a20 2020 2020 2020 2020  _fruit.         
+00025480: 2020 2020 2020 2062 7265 616b 0a0a 6060         break..``
+00025490: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
+000254a0: 6974 2a2a 0a0a 6060 6070 790a 6465 6620  it**..```py.def 
+000254b0: 6672 7569 745f 6765 6e65 7261 746f 7228  fruit_generator(
+000254c0: 293a 0a20 2020 205c 225c 225c 2254 6865  ):.    \"\"\"The
+000254d0: 2065 7861 6d70 6c65 2069 7320 7369 6d70   example is simp
+000254e0: 6c65 2065 6e6f 7567 6820 796f 7520 646f  le enough you do
+000254f0: 6e27 7420 6e65 6564 2061 6e20 6578 706c  n't need an expl
+00025500: 6963 6974 2072 6574 7572 6e2e 5c22 5c22  icit return.\"\"
+00025510: 5c22 0a20 2020 2066 6f72 2066 7275 6974  \".    for fruit
+00025520: 2069 6e20 5b5c 2261 7070 6c65 5c22 2c20   in [\"apple\", 
+00025530: 5c22 6261 6e61 6e61 5c22 5d3a 0a20 2020  \"banana\"]:.   
+00025540: 2020 2020 2079 6965 6c64 2066 7275 6974       yield fruit
+00025550: 0a0a 0a64 6566 2074 776f 5f66 7275 6974  ...def two_fruit
+00025560: 735f 6765 6e65 7261 746f 7228 6672 7569  s_generator(frui
+00025570: 7473 293a 0a20 2020 205c 225c 225c 2243  ts):.    \"\"\"C
+00025580: 6174 6368 696e 6720 7468 6520 5374 6f70  atching the Stop
+00025590: 4974 6572 6174 696f 6e2e 5c22 5c22 5c22  Iteration.\"\"\"
+000255a0: 0a20 2020 2066 6f72 2066 7275 6974 2069  .    for fruit i
+000255b0: 6e20 6672 7569 7473 3a0a 2020 2020 2020  n fruits:.      
+000255c0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000255d0: 2020 2079 6965 6c64 2066 7275 6974 2c20     yield fruit, 
+000255e0: 6e65 7874 2866 7275 6974 7329 0a20 2020  next(fruits).   
+000255f0: 2020 2020 2065 7863 6570 7420 5374 6f70       except Stop
+00025600: 4974 6572 6174 696f 6e3a 0a20 2020 2020  Iteration:.     
+00025610: 2020 2020 2020 2070 7269 6e74 285c 2253         print(\"S
+00025620: 6f72 7279 2074 6865 7265 2069 7320 6f6e  orry there is on
+00025630: 6c79 206f 6e65 2066 7275 6974 206c 6566  ly one fruit lef
+00025640: 742e 5c22 290a 2020 2020 2020 2020 2020  t.\").          
+00025650: 2020 7969 656c 6420 6672 7569 742c 204e    yield fruit, N
+00025660: 6f6e 650a 0a0a 6465 6620 7477 6f5f 676f  one...def two_go
+00025670: 6f64 5f66 7275 6974 735f 6765 6e65 7261  od_fruits_genera
+00025680: 746f 7228 6672 7569 7473 293a 0a20 2020  tor(fruits):.   
+00025690: 205c 225c 225c 2241 2072 6574 7572 6e20   \"\"\"A return 
+000256a0: 6361 6e20 6265 2075 7365 6420 746f 2065  can be used to e
+000256b0: 6e64 2074 6865 2069 7465 7261 746f 7220  nd the iterator 
+000256c0: 6561 726c 792c 2062 7574 206e 6f74 2061  early, but not a
+000256d0: 2053 746f 7049 7465 7261 7469 6f6e 2e5c   StopIteration.\
+000256e0: 225c 225c 220a 2020 2020 666f 7220 6672  "\"\".    for fr
+000256f0: 7569 7420 696e 2066 7275 6974 733a 0a20  uit in fruits:. 
+00025700: 2020 2020 2020 2069 6620 6e6f 7420 6672         if not fr
+00025710: 7569 742e 6973 5f74 6173 7479 2829 3a0a  uit.is_tasty():.
+00025720: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00025730: 696e 7565 0a20 2020 2020 2020 2077 6869  inue.        whi
+00025740: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+00025750: 2020 2020 206e 6578 745f 6672 7569 7420       next_fruit 
+00025760: 3d20 6e65 7874 2866 7275 6974 732c 204e  = next(fruits, N
+00025770: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+00025780: 2069 6620 6e65 7874 5f66 7275 6974 2069   if next_fruit i
+00025790: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000257a0: 2020 2020 2020 2020 7072 696e 7428 5c22          print(\"
+000257b0: 536f 7272 7920 7468 6572 6520 6973 206f  Sorry there is o
+000257c0: 6e6c 7920 6f6e 6520 6672 7569 7420 6c65  nly one fruit le
+000257d0: 6674 2e5c 2229 0a20 2020 2020 2020 2020  ft.\").         
+000257e0: 2020 2020 2020 2079 6965 6c64 2066 7275         yield fru
+000257f0: 6974 2c20 4e6f 6e65 0a20 2020 2020 2020  it, None.       
+00025800: 2020 2020 2020 2020 2023 2057 6520 7265           # We re
+00025810: 6163 6865 6420 7468 6520 656e 6420 6f66  ached the end of
+00025820: 2074 6865 2027 6672 7569 7473 2720 6765   the 'fruits' ge
+00025830: 6e65 7261 746f 7220 6275 7420 7261 6973  nerator but rais
+00025840: 696e 6720 610a 2020 2020 2020 2020 2020  ing a.          
+00025850: 2020 2020 2020 2320 5374 6f70 4974 6572        # StopIter
+00025860: 6174 696f 6e20 696e 7374 6561 6420 6f66  ation instead of
+00025870: 2072 6574 7572 6e69 6e67 2077 6f75 6c64   returning would
+00025880: 2063 7265 6174 6520 6120 5275 6e74 696d   create a Runtim
+00025890: 6545 7272 6f72 0a20 2020 2020 2020 2020  eError.         
+000258a0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000258b0: 2020 2020 2020 2020 2020 6966 206e 6578            if nex
+000258c0: 745f 6672 7569 742e 6973 5f74 6173 7479  t_fruit.is_tasty
+000258d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000258e0: 2020 2020 7969 656c 6420 6672 7569 742c      yield fruit,
+000258f0: 206e 6578 745f 6672 7569 740a 2020 2020   next_fruit.    
+00025900: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00025910: 6b0a 0a60 6060 0a0a 3c61 2068 7265 663d  k..```..<a href=
+00025920: 5c22 6874 7470 733a 2f2f 7079 6c69 6e74  \"https://pylint
+00025930: 2e70 7963 7161 2e6f 7267 2f65 6e2f 6c61  .pycqa.org/en/la
+00025940: 7465 7374 2f75 7365 725f 6775 6964 652f  test/user_guide/
+00025950: 6d65 7373 6167 6573 2f72 6566 6163 746f  messages/refacto
+00025960: 722f 7374 6f70 2d69 7465 7261 7469 6f6e  r/stop-iteration
+00025970: 2d72 6574 7572 6e2e 6874 6d6c 5c22 3e41  -return.html\">A
+00025980: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
+00025990: 6174 696f 6e3c 2f61 3e22 2222 0a0a 5b52  ation</a>"""..[R
+000259a0: 3137 3039 5d0a 7768 7920 3d20 2249 7420  1709].why = "It 
+000259b0: 6c6f 6f6b 7320 6c69 6b65 2072 6564 756e  looks like redun
+000259c0: 6461 6e74 2070 7265 2d70 7974 686f 6e20  dant pre-python 
+000259d0: 322e 3520 7465 726e 6172 7920 7379 6e74  2.5 ternary synt
+000259e0: 6178 2069 7320 7573 6564 2e22 0a65 7861  ax is used.".exa
+000259f0: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
+00025a00: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
+00025a10: 0a0a 6060 6070 790a 6465 6620 6861 735f  ..```py.def has_
+00025a20: 6f72 616e 6765 7328 6f72 616e 6765 732c  oranges(oranges,
+00025a30: 2061 7070 6c65 733d 4e6f 6e65 2920 2d3e   apples=None) ->
+00025a40: 2062 6f6f 6c3a 0a20 2020 2072 6574 7572   bool:.    retur
+00025a50: 6e20 6170 706c 6573 2061 6e64 2046 616c  n apples and Fal
+00025a60: 7365 206f 7220 6f72 616e 6765 7320 2023  se or oranges  #
+00025a70: 205b 7369 6d70 6c69 6679 2d62 6f6f 6c65   [simplify-boole
+00025a80: 616e 2d65 7870 7265 7373 696f 6e5d 0a0a  an-expression]..
+00025a90: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
+00025aa0: 7820 6974 2a2a 0a0a 6060 6070 790a 6465  x it**..```py.de
+00025ab0: 6620 6861 735f 6f72 616e 6765 7328 6f72  f has_oranges(or
+00025ac0: 616e 6765 732c 2061 7070 6c65 733d 4e6f  anges, apples=No
+00025ad0: 6e65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ne) -> bool:.   
+00025ae0: 2072 6574 7572 6e20 6f72 616e 6765 730a   return oranges.
+00025af0: 0a60 6060 0a22 2222 0a0a 5b52 3137 3130  .```."""..[R1710
+00025b00: 5d0a 7768 7920 3d20 2241 6363 6f72 6469  ].why = "Accordi
+00025b10: 6e67 2074 6f20 5045 5038 2c20 6966 2061  ng to PEP8, if a
+00025b20: 6e79 2072 6574 7572 6e20 7374 6174 656d  ny return statem
+00025b30: 656e 7420 7265 7475 726e 7320 616e 2065  ent returns an e
+00025b40: 7870 7265 7373 696f 6e2c 2061 6e79 2072  xpression, any r
+00025b50: 6574 7572 6e20 7374 6174 656d 656e 7473  eturn statements
+00025b60: 2077 6865 7265 206e 6f20 7661 6c75 6520   where no value 
+00025b70: 6973 2072 6574 7572 6e65 6420 7368 6f75  is returned shou
+00025b80: 6c64 2065 7870 6c69 6369 746c 7920 7374  ld explicitly st
+00025b90: 6174 6520 7468 6973 2061 7320 7265 7475  ate this as retu
+00025ba0: 726e 204e 6f6e 652c 2061 6e64 2061 6e20  rn None, and an 
+00025bb0: 6578 706c 6963 6974 2072 6574 7572 6e20  explicit return 
+00025bc0: 7374 6174 656d 656e 7420 7368 6f75 6c64  statement should
+00025bd0: 2062 6520 7072 6573 656e 7420 6174 2074   be present at t
+00025be0: 6865 2065 6e64 206f 6620 7468 6520 6675  he end of the fu
+00025bf0: 6e63 7469 6f6e 2028 6966 2072 6561 6368  nction (if reach
+00025c00: 6162 6c65 2922 0a65 7861 6d70 6c65 7320  able)".examples 
+00025c10: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
+00025c20: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
+00025c30: 790a 6465 6620 6765 745f 7468 655f 616e  y.def get_the_an
+00025c40: 7377 6572 2876 616c 7565 3a20 7374 7229  swer(value: str)
+00025c50: 202d 3e20 7374 7220 7c20 4e6f 6e65 3a20   -> str | None: 
+00025c60: 2023 205b 696e 636f 6e73 6973 7465 6e74   # [inconsistent
+00025c70: 2d72 6574 7572 6e2d 7374 6174 656d 656e  -return-statemen
+00025c80: 7473 5d0a 2020 2020 6966 2076 616c 7565  ts].    if value
+00025c90: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00025ca0: 2076 616c 7565 0a0a 6060 600a 0a2a 2a48   value..```..**H
+00025cb0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00025cc0: 6060 6070 790a 6465 6620 6765 745f 7468  ```py.def get_th
+00025cd0: 655f 616e 7377 6572 2876 616c 7565 3a20  e_answer(value: 
+00025ce0: 7374 7229 202d 3e20 7374 7220 7c20 4e6f  str) -> str | No
+00025cf0: 6e65 3a0a 2020 2020 6966 2076 616c 7565  ne:.    if value
+00025d00: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00025d10: 2076 616c 7565 0a20 2020 2072 6574 7572   value.    retur
+00025d20: 6e20 4e6f 6e65 0a0a 6060 600a 2222 220a  n None..```.""".
+00025d30: 0a5b 5231 3731 315d 0a77 6879 203d 2022  .[R1711].why = "
+00025d40: 4974 206c 6f6f 6b73 206c 696b 6520 7468  It looks like th
+00025d50: 6520 7369 6e67 6c65 205c 2272 6574 7572  e single \"retur
+00025d60: 6e5c 2220 6f72 205c 2272 6574 7572 6e20  n\" or \"return 
+00025d70: 4e6f 6e65 5c22 2073 7461 7465 6d65 6e74  None\" statement
+00025d80: 2069 7320 666f 756e 6420 6174 2074 6865   is found at the
+00025d90: 2065 6e64 206f 6620 6675 6e63 7469 6f6e   end of function
+00025da0: 206f 7220 6d65 7468 6f64 2064 6566 696e   or method defin
+00025db0: 6974 696f 6e2e 2054 6869 7320 7374 6174  ition. This stat
+00025dc0: 656d 656e 7420 6361 6e20 7361 6665 6c79  ement can safely
+00025dd0: 2062 6520 7265 6d6f 7665 6420 6265 6361   be removed beca
+00025de0: 7573 6520 5079 7468 6f6e 2077 696c 6c20  use Python will 
+00025df0: 696d 706c 6963 6974 6c79 2072 6574 7572  implicitly retur
+00025e00: 6e20 4e6f 6e65 220a 6578 616d 706c 6573  n None".examples
+00025e10: 203d 2022 2222 0a2a 2a50 726f 626c 656d   = """.**Problem
+00025e20: 6174 6963 2063 6f64 652a 2a0a 0a60 6060  atic code**..```
+00025e30: 7079 0a69 6d70 6f72 7420 7379 730a 0a0a  py.import sys...
+00025e40: 6465 6620 7072 696e 745f 7079 7468 6f6e  def print_python
+00025e50: 5f76 6572 7369 6f6e 2829 3a20 2023 205b  _version():  # [
+00025e60: 7573 656c 6573 732d 7265 7475 726e 5d0a  useless-return].
+00025e70: 2020 2020 7072 696e 7428 7379 732e 7665      print(sys.ve
+00025e80: 7273 696f 6e29 0a20 2020 2072 6574 7572  rsion).    retur
+00025e90: 6e20 4e6f 6e65 0a0a 6060 600a 0a2a 2a48  n None..```..**H
+00025ea0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00025eb0: 6060 6070 790a 696d 706f 7274 2073 7973  ```py.import sys
+00025ec0: 0a0a 0a64 6566 2070 7269 6e74 5f70 7974  ...def print_pyt
+00025ed0: 686f 6e5f 7665 7273 696f 6e28 293a 0a20  hon_version():. 
+00025ee0: 2020 2070 7269 6e74 2873 7973 2e76 6572     print(sys.ver
+00025ef0: 7369 6f6e 290a 0a60 6060 0a22 2222 0a0a  sion)..```."""..
+00025f00: 5b52 3137 3132 5d0a 7768 7920 3d20 2259  [R1712].why = "Y
+00025f10: 6f75 2064 6f20 6e6f 7420 6861 7665 2074  ou do not have t
+00025f20: 6f20 7573 6520 6120 7465 6d70 6f72 6172  o use a temporar
+00025f30: 7920 7661 7269 6162 6c65 2069 6e20 6f72  y variable in or
+00025f40: 6465 7220 746f 2073 7761 7020 7661 7269  der to swap vari
+00025f50: 6162 6c65 732e 2055 7369 6e67 205c 2274  ables. Using \"t
+00025f60: 7570 6c65 2075 6e70 6163 6b69 6e67 5c22  uple unpacking\"
+00025f70: 2074 6f20 6469 7265 6374 6c79 2073 7761   to directly swa
+00025f80: 7020 7661 7269 6162 6c65 7320 6d61 6b65  p variables make
+00025f90: 7320 7468 6520 696e 7465 6e74 696f 6e20  s the intention 
+00025fa0: 6d6f 7265 2063 6c65 6172 2e20 4578 616d  more clear. Exam
+00025fb0: 706c 653a 205c 2261 2c20 6220 3d20 622c  ple: \"a, b = b,
+00025fc0: 2061 5c22 2e22 0a65 7861 6d70 6c65 7320   a\".".examples 
+00025fd0: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
+00025fe0: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
+00025ff0: 790a 6120 3d20 310a 6220 3d20 320a 0a74  y.a = 1.b = 2..t
+00026000: 656d 7020 3d20 6120 2023 205b 636f 6e73  emp = a  # [cons
+00026010: 6964 6572 2d73 7761 702d 7661 7269 6162  ider-swap-variab
+00026020: 6c65 735d 0a61 203d 2062 0a62 203d 2074  les].a = b.b = t
+00026030: 656d 700a 0a60 6060 0a0a 2a2a 486f 7720  emp..```..**How 
+00026040: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
+00026050: 7079 0a61 203d 2031 0a62 203d 2032 0a0a  py.a = 1.b = 2..
+00026060: 612c 2062 203d 2062 2c20 610a 0a60 6060  a, b = b, a..```
+00026070: 0a22 2222 0a0a 5b52 3137 3133 5d0a 7768  ."""..[R1713].wh
+00026080: 7920 3d20 2255 7369 6e67 2073 7472 2e6a  y = "Using str.j
+00026090: 6f69 6e28 7365 7175 656e 6365 2920 6973  oin(sequence) is
+000260a0: 2066 6173 7465 722c 2075 7365 7320 6c65   faster, uses le
+000260b0: 7373 206d 656d 6f72 7920 616e 6420 696e  ss memory and in
+000260c0: 6372 6561 7365 7320 7265 6164 6162 696c  creases readabil
+000260d0: 6974 7920 636f 6d70 6172 6564 2074 6f20  ity compared to 
+000260e0: 666f 722d 6c6f 6f70 2069 7465 7261 7469  for-loop iterati
+000260f0: 6f6e 2e22 0a65 7861 6d70 6c65 7320 3d20  on.".examples = 
+00026100: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
+00026110: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
+00026120: 6465 6620 6672 7569 7473 5f74 6f5f 7374  def fruits_to_st
+00026130: 7269 6e67 2866 7275 6974 7329 3a0a 2020  ring(fruits):.  
+00026140: 2020 666f 726d 6174 7465 645f 6672 7569    formatted_frui
+00026150: 7420 3d20 5c22 5c22 0a20 2020 2066 6f72  t = \"\".    for
+00026160: 2066 7275 6974 2069 6e20 6672 7569 7473   fruit in fruits
+00026170: 3a0a 2020 2020 2020 2020 666f 726d 6174  :.        format
+00026180: 7465 645f 6672 7569 7420 2b3d 2066 7275  ted_fruit += fru
+00026190: 6974 2020 2320 5b63 6f6e 7369 6465 722d  it  # [consider-
+000261a0: 7573 696e 672d 6a6f 696e 5d0a 2020 2020  using-join].    
+000261b0: 7265 7475 726e 2066 6f72 6d61 7474 6564  return formatted
+000261c0: 5f66 7275 6974 0a0a 7072 696e 7428 6672  _fruit..print(fr
+000261d0: 7569 7473 5f74 6f5f 7374 7269 6e67 285b  uits_to_string([
+000261e0: 5c22 6170 706c 655c 222c 205c 2270 6561  \"apple\", \"pea
+000261f0: 725c 222c 205c 2270 6561 6368 5c22 5d29  r\", \"peach\"])
+00026200: 290a 0a60 6060 0a0a 2a2a 486f 7720 746f  )..```..**How to
+00026210: 2066 6978 2069 742a 2a0a 0a60 6060 7079   fix it**..```py
+00026220: 0a70 7269 6e74 285c 225c 222e 6a6f 696e  .print(\"\".join
+00026230: 285b 5c22 6170 706c 655c 222c 205c 2270  ([\"apple\", \"p
+00026240: 6561 725c 222c 205c 2270 6561 6368 5c22  ear\", \"peach\"
+00026250: 5d29 290a 0a60 6060 0a22 2222 0a0a 5b52  ]))..```."""..[R
+00026260: 3137 3134 5d0a 7768 7920 3d20 2253 686f  1714].why = "Sho
+00026270: 7274 6572 2063 6f6e 6469 7469 6f6e 7320  rter conditions 
+00026280: 6172 6520 7573 7561 6c6c 7920 6561 7369  are usually easi
+00026290: 6572 2074 6f20 7265 6164 2e22 0a65 7861  er to read.".exa
+000262a0: 6d70 6c65 7320 3d20 2222 220a 436f 6d70  mples = """.Comp
+000262b0: 6172 6973 6f6e 206f 6620 6120 7661 7269  arison of a vari
+000262c0: 6162 6c65 2074 6f20 7477 6f20 7661 6c75  able to two valu
+000262d0: 6573 2063 616e 2062 6520 7369 6d70 6c69  es can be simpli
+000262e0: 6669 6564 2075 7369 6e67 2074 6865 2060  fied using the `
+000262f0: 696e 6020 6f70 6572 6174 6f72 2e0a 5468  in` operator..Th
+00026300: 6973 2069 7320 6d6f 7265 2072 6561 6461  is is more reada
+00026310: 626c 6520 616e 6420 616c 736f 2073 6166  ble and also saf
+00026320: 6572 2061 6761 696e 7374 2063 6f70 792d  er against copy-
+00026330: 7061 7374 6520 6572 726f 7273 2e0a 0a60  paste errors...`
+00026340: 6060 7079 0a64 6566 2070 726f 626c 656d  ``py.def problem
+00026350: 6174 6963 2874 6578 743a 2073 7472 293a  atic(text: str):
+00026360: 0a20 2020 2069 6620 7465 7874 203d 3d20  .    if text == 
+00026370: 2761 2720 6f72 2074 6578 7420 3d3d 2027  'a' or text == '
+00026380: 6227 3a0a 2020 2020 2020 2020 7265 7475  b':.        retu
+00026390: 726e 0a60 6060 0a0a 6060 6070 790a 6465  rn.```..```py.de
+000263a0: 6620 676f 6f64 2874 6578 743a 2073 7472  f good(text: str
+000263b0: 293a 0a20 2020 2069 6620 7465 7874 2069  ):.    if text i
+000263c0: 6e20 2827 6127 2c20 2762 2729 3a0a 2020  n ('a', 'b'):.  
+000263d0: 2020 2020 2020 7265 7475 726e 0a60 6060        return.```
+000263e0: 0a0a 4966 2079 6f75 2061 7265 2063 6f6d  ..If you are com
+000263f0: 7061 7269 6e67 2061 2073 696e 676c 6520  paring a single 
+00026400: 6368 6172 6163 7465 722c 2079 6f75 2063  character, you c
+00026410: 616e 2061 6c73 6f20 646f 2074 6869 733a  an also do this:
+00026420: 0a0a 6060 6070 790a 6465 6620 676f 6f64  ..```py.def good
+00026430: 2863 6861 723a 2073 7472 293a 0a20 2020  (char: str):.   
+00026440: 2069 6620 6368 6172 2069 6e20 2761 6227   if char in 'ab'
+00026450: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00026460: 0a60 6060 0a22 2222 0a0a 5b52 3137 3135  .```."""..[R1715
+00026470: 5d0a 7768 7920 3d20 2255 7369 6e67 2074  ].why = "Using t
+00026480: 6865 2062 7569 6c74 696e 2064 6963 742e  he builtin dict.
+00026490: 6765 7420 666f 7220 6765 7474 696e 6720  get for getting 
+000264a0: 6120 7661 6c75 6520 6672 6f6d 2061 2064  a value from a d
+000264b0: 6963 7469 6f6e 6172 7920 6966 2061 206b  ictionary if a k
+000264c0: 6579 2069 7320 7072 6573 656e 7420 6f72  ey is present or
+000264d0: 2061 2064 6566 6175 6c74 2069 6620 6e6f   a default if no
+000264e0: 742c 2069 7320 7369 6d70 6c65 7220 616e  t, is simpler an
+000264f0: 6420 636f 6e73 6964 6572 6564 206d 6f72  d considered mor
+00026500: 6520 6964 696f 6d61 7469 632c 2061 6c74  e idiomatic, alt
+00026510: 686f 7567 6820 736f 6d65 7469 6d65 7320  hough sometimes 
+00026520: 6120 6269 7420 736c 6f77 6572 220a 6578  a bit slower".ex
+00026530: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
+00026540: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
+00026550: 2a0a 0a60 6060 7079 0a6b 6e69 6768 7473  *..```py.knights
+00026560: 203d 207b 5c22 4761 6c6c 6168 6164 5c22   = {\"Gallahad\"
+00026570: 3a20 5c22 7468 6520 7075 7265 5c22 2c20  : \"the pure\", 
+00026580: 5c22 526f 6269 6e5c 223a 205c 2274 6865  \"Robin\": \"the
+00026590: 2062 7261 7665 5c22 7d0a 0a69 6620 5c22   brave\"}..if \"
+000265a0: 4761 6c6c 6168 6164 5c22 2069 6e20 6b6e  Gallahad\" in kn
+000265b0: 6967 6874 733a 2020 2320 5b63 6f6e 7369  ights:  # [consi
+000265c0: 6465 722d 7573 696e 672d 6765 745d 0a20  der-using-get]. 
+000265d0: 2020 2044 4553 4352 4950 5449 4f4e 203d     DESCRIPTION =
+000265e0: 206b 6e69 6768 7473 5b5c 2247 616c 6c61   knights[\"Galla
+000265f0: 6861 645c 225d 0a65 6c73 653a 0a20 2020  had\"].else:.   
+00026600: 2044 4553 4352 4950 5449 4f4e 203d 205c   DESCRIPTION = \
+00026610: 225c 220a 0a60 6060 0a0a 2a2a 486f 7720  "\"..```..**How 
+00026620: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
+00026630: 7079 0a6b 6e69 6768 7473 203d 207b 5c22  py.knights = {\"
+00026640: 4761 6c6c 6168 6164 5c22 3a20 5c22 7468  Gallahad\": \"th
+00026650: 6520 7075 7265 5c22 2c20 5c22 526f 6269  e pure\", \"Robi
+00026660: 6e5c 223a 205c 2274 6865 2062 7261 7665  n\": \"the brave
+00026670: 5c22 7d0a 0a64 6573 6372 6970 7469 6f6e  \"}..description
+00026680: 203d 206b 6e69 6768 7473 2e67 6574 285c   = knights.get(\
+00026690: 2247 616c 6c61 6861 645c 222c 205c 225c  "Gallahad\", \"\
+000266a0: 2229 0a0a 6060 600a 2222 220a 0a5b 5231  ")..```."""..[R1
+000266b0: 3731 365d 0a77 6879 203d 2022 5468 6973  716].why = "This
+000266c0: 206d 6573 7361 6765 2069 7320 656d 6974   message is emit
+000266d0: 7465 6420 7768 656e 2070 796c 696e 7420  ted when pylint 
+000266e0: 656e 636f 756e 7465 7273 2062 6f6f 6c65  encounters boole
+000266f0: 616e 206f 7065 7261 7469 6f6e 206c 696b  an operation lik
+00026700: 655c 2261 203c 2062 2061 6e64 2062 203c  e\"a < b and b <
+00026710: 2063 5c22 2c20 7375 6767 6573 7469 6e67   c\", suggesting
+00026720: 2069 6e73 7465 6164 2074 6f20 7265 6661   instead to refa
+00026730: 6374 6f72 2069 7420 746f 205c 2261 203c  ctor it to \"a <
+00026740: 2062 203c 2063 5c22 220a 6578 616d 706c   b < c\"".exampl
+00026750: 6573 203d 2022 2222 0a2a 2a50 726f 626c  es = """.**Probl
+00026760: 656d 6174 6963 2063 6f64 652a 2a0a 0a60  ematic code**..`
+00026770: 6060 7079 0a61 203d 2069 6e74 2869 6e70  ``py.a = int(inp
+00026780: 7574 2829 290a 6220 3d20 696e 7428 696e  ut()).b = int(in
+00026790: 7075 7428 2929 0a63 203d 2069 6e74 2869  put()).c = int(i
+000267a0: 6e70 7574 2829 290a 6966 2061 203c 2062  nput()).if a < b
+000267b0: 2061 6e64 2062 203c 2063 3a20 2023 205b   and b < c:  # [
+000267c0: 6368 6169 6e65 642d 636f 6d70 6172 6973  chained-comparis
+000267d0: 6f6e 5d0a 2020 2020 7061 7373 0a0a 6060  on].    pass..``
+000267e0: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
+000267f0: 6974 2a2a 0a0a 6060 6070 790a 6120 3d20  it**..```py.a = 
+00026800: 696e 7428 696e 7075 7428 2929 0a62 203d  int(input()).b =
+00026810: 2069 6e74 2869 6e70 7574 2829 290a 6320   int(input()).c 
+00026820: 3d20 696e 7428 696e 7075 7428 2929 0a69  = int(input()).i
+00026830: 6620 6120 3c20 6220 3c20 633a 0a20 2020  f a < b < c:.   
+00026840: 2070 6173 730a 0a60 6060 0a22 2222 0a0a   pass..```."""..
+00026850: 5b52 3137 3137 5d0a 7768 7920 3d20 2249  [R1717].why = "I
+00026860: 7420 6c6f 6f6b 7320 6c69 6b65 2077 6520  t looks like we 
+00026870: 6465 7465 6374 2074 6865 2063 7265 6174  detect the creat
+00026880: 696f 6e20 6f66 2061 2064 6963 7469 6f6e  ion of a diction
+00026890: 6172 7920 7573 696e 6720 7468 6520 6469  ary using the di
+000268a0: 6374 2829 2063 616c 6c61 626c 6520 616e  ct() callable an
+000268b0: 6420 6120 7472 616e 7369 656e 7420 6c69  d a transient li
+000268c0: 7374 2e20 416c 7468 6f75 6768 2074 6865  st. Although the
+000268d0: 7265 2069 7320 6e6f 7468 696e 6720 7379  re is nothing sy
+000268e0: 6e74 6163 7469 6361 6c6c 7920 7772 6f6e  ntactically wron
+000268f0: 6720 7769 7468 2074 6869 7320 636f 6465  g with this code
+00026900: 2c20 6974 2069 7320 6861 7264 2074 6f20  , it is hard to 
+00026910: 7265 6164 2061 6e64 2063 616e 2062 6520  read and can be 
+00026920: 7369 6d70 6c69 6669 6564 2074 6f20 6120  simplified to a 
+00026930: 6469 6374 2063 6f6d 7072 6568 656e 7369  dict comprehensi
+00026940: 6f6e 2e41 6c73 6f20 6974 2069 7320 6661  on.Also it is fa
+00026950: 7374 6572 2073 696e 6365 2079 6f75 2064  ster since you d
+00026960: 6f6e 2774 206e 6565 6420 746f 2063 7265  on't need to cre
+00026970: 6174 6520 616e 6f74 6865 7220 7472 616e  ate another tran
+00026980: 7369 656e 7420 6c69 7374 220a 6578 616d  sient list".exam
+00026990: 706c 6573 203d 2022 2222 0a2a 2a50 726f  ples = """.**Pro
+000269a0: 626c 656d 6174 6963 2063 6f64 652a 2a0a  blematic code**.
+000269b0: 0a60 6060 7079 0a4e 554d 4245 5253 203d  .```py.NUMBERS =
+000269c0: 205b 312c 2032 2c20 335d 0a0a 2320 2b31   [1, 2, 3]..# +1
+000269d0: 3a20 5b63 6f6e 7369 6465 722d 7573 696e  : [consider-usin
+000269e0: 672d 6469 6374 2d63 6f6d 7072 6568 656e  g-dict-comprehen
+000269f0: 7369 6f6e 5d0a 444f 5542 4c45 445f 4e55  sion].DOUBLED_NU
+00026a00: 4d42 4552 5320 3d20 6469 6374 285b 286e  MBERS = dict([(n
+00026a10: 756d 6265 722c 206e 756d 6265 7220 2a20  umber, number * 
+00026a20: 3229 2066 6f72 206e 756d 6265 7220 696e  2) for number in
+00026a30: 204e 554d 4245 5253 5d29 0a0a 6060 600a   NUMBERS])..```.
+00026a40: 0a2a 2a48 6f77 2074 6f20 6669 7820 6974  .**How to fix it
+00026a50: 2a2a 0a0a 6060 6070 790a 4e55 4d42 4552  **..```py.NUMBER
+00026a60: 5320 3d20 5b31 2c20 322c 2033 5d0a 0a44  S = [1, 2, 3]..D
+00026a70: 4f55 424c 4544 5f4e 554d 4245 5253 203d  OUBLED_NUMBERS =
+00026a80: 207b 6e75 6d62 6572 3a20 6e75 6d62 6572   {number: number
+00026a90: 202a 2032 2066 6f72 206e 756d 6265 7220   * 2 for number 
+00026aa0: 696e 204e 554d 4245 5253 7d0a 0a60 6060  in NUMBERS}..```
+00026ab0: 0a0a 3c61 2068 7265 663d 5c22 6874 7470  ..<a href=\"http
+00026ac0: 733a 2f2f 7079 6c69 6e74 2e70 7963 7161  s://pylint.pycqa
+00026ad0: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f75  .org/en/latest/u
+00026ae0: 7365 725f 6775 6964 652f 6d65 7373 6167  ser_guide/messag
+00026af0: 6573 2f72 6566 6163 746f 722f 636f 6e73  es/refactor/cons
+00026b00: 6964 6572 2d75 7369 6e67 2d64 6963 742d  ider-using-dict-
+00026b10: 636f 6d70 7265 6865 6e73 696f 6e2e 6874  comprehension.ht
+00026b20: 6d6c 5c22 3e41 6464 6974 696f 6e61 6c20  ml\">Additional 
+00026b30: 696e 666f 726d 6174 696f 6e3c 2f61 3e22  information</a>"
+00026b40: 2222 0a0a 5b52 3137 3138 5d0a 7768 7920  ""..[R1718].why 
+00026b50: 3d20 2241 6c74 686f 7567 6820 7468 6572  = "Although ther
+00026b60: 6520 6973 206e 6f74 6869 6e67 2073 796e  e is nothing syn
+00026b70: 7461 6374 6963 616c 6c79 2077 726f 6e67  tactically wrong
+00026b80: 2077 6974 6820 7468 6973 2063 6f64 652c   with this code,
+00026b90: 2069 7420 6973 2068 6172 6420 746f 2072   it is hard to r
+00026ba0: 6561 6420 616e 6420 6361 6e20 6265 2073  ead and can be s
+00026bb0: 696d 706c 6966 6965 6420 746f 2061 2073  implified to a s
+00026bc0: 6574 2063 6f6d 7072 6568 656e 7369 6f6e  et comprehension
+00026bd0: 2e41 6c73 6f20 6974 2069 7320 6661 7374  .Also it is fast
+00026be0: 6572 2073 696e 6365 2079 6f75 2064 6f6e  er since you don
+00026bf0: 2774 206e 6565 6420 746f 2063 7265 6174  't need to creat
+00026c00: 6520 616e 6f74 6865 7220 7472 616e 7369  e another transi
+00026c10: 656e 7420 6c69 7374 220a 6578 616d 706c  ent list".exampl
+00026c20: 6573 203d 2022 2222 0a2a 2a50 726f 626c  es = """.**Probl
+00026c30: 656d 6174 6963 2063 6f64 652a 2a0a 0a60  ematic code**..`
+00026c40: 6060 7079 0a4e 554d 4245 5253 203d 205b  ``py.NUMBERS = [
+00026c50: 312c 2032 2c20 322c 2033 2c20 342c 2034  1, 2, 2, 3, 4, 4
+00026c60: 5d0a 0a23 202b 313a 205b 636f 6e73 6964  ]..# +1: [consid
+00026c70: 6572 2d75 7369 6e67 2d73 6574 2d63 6f6d  er-using-set-com
+00026c80: 7072 6568 656e 7369 6f6e 5d0a 554e 4951  prehension].UNIQ
+00026c90: 5545 5f45 5645 4e5f 4e55 4d42 4552 5320  UE_EVEN_NUMBERS 
+00026ca0: 3d20 7365 7428 5b6e 756d 6265 7220 666f  = set([number fo
+00026cb0: 7220 6e75 6d62 6572 2069 6e20 4e55 4d42  r number in NUMB
+00026cc0: 4552 5320 6966 206e 756d 6265 7220 2520  ERS if number % 
+00026cd0: 3220 3d3d 2030 5d29 0a0a 6060 600a 0a2a  2 == 0])..```..*
+00026ce0: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
+00026cf0: 0a0a 6060 6070 790a 4e55 4d42 4552 5320  ..```py.NUMBERS 
+00026d00: 3d20 5b31 2c20 322c 2032 2c20 332c 2034  = [1, 2, 2, 3, 4
+00026d10: 2c20 345d 0a0a 554e 4951 5545 5f45 5645  , 4]..UNIQUE_EVE
+00026d20: 4e5f 4e55 4d42 4552 5320 3d20 7b6e 756d  N_NUMBERS = {num
+00026d30: 6265 7220 666f 7220 6e75 6d62 6572 2069  ber for number i
+00026d40: 6e20 4e55 4d42 4552 5320 6966 206e 756d  n NUMBERS if num
+00026d50: 6265 7220 2520 3220 3d3d 2030 7d0a 0a60  ber % 2 == 0}..`
+00026d60: 6060 0a0a 3c61 2068 7265 663d 5c22 6874  ``..<a href=\"ht
+00026d70: 7470 733a 2f2f 7079 6c69 6e74 2e70 7963  tps://pylint.pyc
+00026d80: 7161 2e6f 7267 2f65 6e2f 6c61 7465 7374  qa.org/en/latest
+00026d90: 2f75 7365 725f 6775 6964 652f 6d65 7373  /user_guide/mess
+00026da0: 6167 6573 2f72 6566 6163 746f 722f 636f  ages/refactor/co
+00026db0: 6e73 6964 6572 2d75 7369 6e67 2d73 6574  nsider-using-set
+00026dc0: 2d63 6f6d 7072 6568 656e 7369 6f6e 2e68  -comprehension.h
+00026dd0: 746d 6c5c 223e 4164 6469 7469 6f6e 616c  tml\">Additional
+00026de0: 2069 6e66 6f72 6d61 7469 6f6e 3c2f 613e   information</a>
+00026df0: 2222 220a 0a5b 5231 3731 395d 0a77 6879  """..[R1719].why
+00026e00: 203d 2022 4974 206c 6f6f 6b73 206c 696b   = "It looks lik
+00026e10: 6520 7468 6520 6966 2065 7870 7265 7373  e the if express
+00026e20: 696f 6e20 6361 6e20 6265 2072 6570 6c61  ion can be repla
+00026e30: 6365 6420 7769 7468 2027 626f 6f6c 2874  ced with 'bool(t
+00026e40: 6573 7429 2720 6f72 2073 696d 706c 7920  est)' or simply 
+00026e50: 2774 6573 7427 2069 6620 7468 6520 626f  'test' if the bo
+00026e60: 6f6c 6561 6e20 6361 7374 2069 7320 696d  olean cast is im
+00026e70: 706c 6963 6974 2e22 0a65 7861 6d70 6c65  plicit.".example
+00026e80: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
+00026e90: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
+00026ea0: 6070 790a 464c 5949 4e47 5f54 4849 4e47  `py.FLYING_THING
+00026eb0: 5320 3d20 5b5c 2262 6972 645c 222c 205c  S = [\"bird\", \
+00026ec0: 2270 6c61 6e65 5c22 2c20 5c22 7375 7065  "plane\", \"supe
+00026ed0: 726d 616e 5c22 2c20 5c22 7468 6973 2065  rman\", \"this e
+00026ee0: 7861 6d70 6c65 5c22 5d0a 0a0a 6465 6620  xample\"]...def 
+00026ef0: 6973 5f66 6c79 696e 675f 7468 696e 6728  is_flying_thing(
+00026f00: 616e 5f6f 626a 6563 7429 3a0a 2020 2020  an_object):.    
+00026f10: 7265 7475 726e 2054 7275 6520 6966 2061  return True if a
+00026f20: 6e5f 6f62 6a65 6374 2069 6e20 464c 5949  n_object in FLYI
+00026f30: 4e47 5f54 4849 4e47 5320 656c 7365 2046  NG_THINGS else F
+00026f40: 616c 7365 2020 2320 5b73 696d 706c 6966  alse  # [simplif
+00026f50: 6961 626c 652d 6966 2d65 7870 7265 7373  iable-if-express
+00026f60: 696f 6e5d 0a0a 0a64 6566 2069 735f 6e6f  ion]...def is_no
+00026f70: 745f 666c 7969 6e67 5f74 6869 6e67 2861  t_flying_thing(a
+00026f80: 6e5f 6f62 6a65 6374 293a 0a20 2020 2072  n_object):.    r
+00026f90: 6574 7572 6e20 4661 6c73 6520 6966 2061  eturn False if a
+00026fa0: 6e5f 6f62 6a65 6374 2069 6e20 464c 5949  n_object in FLYI
+00026fb0: 4e47 5f54 4849 4e47 5320 656c 7365 2054  NG_THINGS else T
+00026fc0: 7275 6520 2023 205b 7369 6d70 6c69 6669  rue  # [simplifi
+00026fd0: 6162 6c65 2d69 662d 6578 7072 6573 7369  able-if-expressi
+00026fe0: 6f6e 5d0a 0a60 6060 0a0a 2a2a 486f 7720  on]..```..**How 
+00026ff0: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
+00027000: 7079 0a46 4c59 494e 475f 5448 494e 4753  py.FLYING_THINGS
+00027010: 203d 205b 5c22 6269 7264 5c22 2c20 5c22   = [\"bird\", \"
+00027020: 706c 616e 655c 222c 205c 2273 7570 6572  plane\", \"super
+00027030: 6d61 6e5c 222c 205c 2274 6869 7320 6578  man\", \"this ex
+00027040: 616d 706c 655c 225d 0a0a 0a64 6566 2069  ample\"]...def i
+00027050: 735f 666c 7969 6e67 5f74 6869 6e67 2861  s_flying_thing(a
+00027060: 6e5f 6f62 6a65 6374 293a 0a20 2020 2072  n_object):.    r
+00027070: 6574 7572 6e20 616e 5f6f 626a 6563 7420  eturn an_object 
+00027080: 696e 2046 4c59 494e 475f 5448 494e 4753  in FLYING_THINGS
+00027090: 0a0a 0a64 6566 2069 735f 6e6f 745f 666c  ...def is_not_fl
+000270a0: 7969 6e67 5f74 6869 6e67 2861 6e5f 6f62  ying_thing(an_ob
+000270b0: 6a65 6374 293a 0a20 2020 2072 6574 7572  ject):.    retur
+000270c0: 6e20 616e 5f6f 626a 6563 7420 6e6f 7420  n an_object not 
+000270d0: 696e 2046 4c59 494e 475f 5448 494e 4753  in FLYING_THINGS
+000270e0: 0a0a 6060 600a 2222 220a 0a5b 5231 3732  ..```."""..[R172
+000270f0: 305d 0a77 6879 203d 2022 5573 6564 2069  0].why = "Used i
+00027100: 6e20 6f72 6465 7220 746f 2068 6967 686c  n order to highl
+00027110: 6967 6874 2061 6e20 756e 6e65 6365 7373  ight an unnecess
+00027120: 6172 7920 626c 6f63 6b20 6f66 2063 6f64  ary block of cod
+00027130: 6520 666f 6c6c 6f77 696e 6720 616e 2069  e following an i
+00027140: 6620 636f 6e74 6169 6e69 6e67 2061 2072  f containing a r
+00027150: 6169 7365 2073 7461 7465 6d65 6e74 2e20  aise statement. 
+00027160: 4173 2073 7563 682c 2069 7420 7769 6c6c  As such, it will
+00027170: 2077 6172 6e20 7768 656e 2069 7420 656e   warn when it en
+00027180: 636f 756e 7465 7273 2061 6e20 656c 7365  counters an else
+00027190: 2066 6f6c 6c6f 7769 6e67 2061 2063 6861   following a cha
+000271a0: 696e 206f 6620 6966 732c 2061 6c6c 206f  in of ifs, all o
+000271b0: 6620 7468 656d 2063 6f6e 7461 696e 696e  f them containin
+000271c0: 6720 6120 7261 6973 6520 7374 6174 656d  g a raise statem
+000271d0: 656e 742e 220a 6578 616d 706c 6573 203d  ent.".examples =
+000271e0: 2022 2222 0a2a 2a50 726f 626c 656d 6174   """.**Problemat
+000271f0: 6963 2063 6f64 652a 2a0a 0a60 6060 7079  ic code**..```py
+00027200: 0a64 6566 2069 6e74 6567 6572 5f73 756d  .def integer_sum
+00027210: 2861 3a20 696e 742c 2062 3a20 696e 7429  (a: int, b: int)
+00027220: 202d 3e20 696e 743a 0a20 2020 2069 6620   -> int:.    if 
+00027230: 6e6f 7420 2869 7369 6e73 7461 6e63 6528  not (isinstance(
+00027240: 612c 2069 6e74 2920 616e 6420 6973 696e  a, int) and isin
+00027250: 7374 616e 6365 2862 2c20 696e 7429 293a  stance(b, int)):
+00027260: 2020 2020 2320 5b6e 6f2d 656c 7365 2d72      # [no-else-r
+00027270: 6169 7365 5d0a 2020 2020 2020 2020 7261  aise].        ra
+00027280: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00027290: 4675 6e63 7469 6f6e 2073 7570 706f 7274  Function support
+000272a0: 7320 6f6e 6c79 2069 6e74 6567 6572 2070  s only integer p
+000272b0: 6172 616d 6574 6572 732e 2729 0a20 2020  arameters.').   
+000272c0: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+000272d0: 6574 7572 6e20 6120 2b20 620a 0a60 6060  eturn a + b..```
+000272e0: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
+000272f0: 742a 2a0a 0a60 6060 7079 0a64 6566 2069  t**..```py.def i
+00027300: 6e74 6567 6572 5f73 756d 2861 3a20 696e  nteger_sum(a: in
+00027310: 742c 2062 3a20 696e 7429 202d 3e20 696e  t, b: int) -> in
+00027320: 743a 0a20 2020 2069 6620 6e6f 7420 2869  t:.    if not (i
+00027330: 7369 6e73 7461 6e63 6528 612c 2069 6e74  sinstance(a, int
+00027340: 2920 616e 6420 6973 696e 7374 616e 6365  ) and isinstance
+00027350: 2862 2c20 696e 7429 293a 0a20 2020 2020  (b, int)):.     
+00027360: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00027370: 726f 7228 2746 756e 6374 696f 6e20 7375  ror('Function su
+00027380: 7070 6f72 7473 206f 6e6c 7920 696e 7465  pports only inte
+00027390: 6765 7220 7061 7261 6d65 7465 7273 2e27  ger parameters.'
+000273a0: 290a 2020 2020 7265 7475 726e 2061 202b  ).    return a +
+000273b0: 2062 0a0a 6060 600a 2222 220a 0a5b 5231   b..```."""..[R1
+000273c0: 3732 315d 0a77 6879 203d 2022 496e 7374  721].why = "Inst
+000273d0: 6561 6420 6f66 2075 7369 6e67 2061 6e20  ead of using an 
+000273e0: 6964 656e 7469 7479 2063 6f6d 7072 6568  identity compreh
+000273f0: 656e 7369 6f6e 2c20 636f 6e73 6964 6572  ension, consider
+00027400: 2075 7369 6e67 2074 6865 206c 6973 742c   using the list,
+00027410: 2064 6963 7420 6f72 2073 6574 2063 6f6e   dict or set con
+00027420: 7374 7275 6374 6f72 2e20 4974 2069 7320  structor. It is 
+00027430: 6661 7374 6572 2061 6e64 2073 696d 706c  faster and simpl
+00027440: 6572 2e22 0a65 7861 6d70 6c65 7320 3d20  er.".examples = 
+00027450: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
+00027460: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
+00027470: 4e55 4d42 4552 5320 3d20 5b31 2c20 312c  NUMBERS = [1, 1,
+00027480: 2032 2c20 322c 2033 2c20 335d 0a0a 554e   2, 2, 3, 3]..UN
+00027490: 4951 5545 5f4e 554d 4245 5253 203d 207b  IQUE_NUMBERS = {
+000274a0: 6e75 6d62 6572 2066 6f72 206e 756d 6265  number for numbe
+000274b0: 7220 696e 204e 554d 4245 5253 7d20 2023  r in NUMBERS}  #
+000274c0: 205b 756e 6e65 6365 7373 6172 792d 636f   [unnecessary-co
+000274d0: 6d70 7265 6865 6e73 696f 6e5d 0a0a 6060  mprehension]..``
+000274e0: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
+000274f0: 6974 2a2a 0a0a 6060 6070 790a 4e55 4d42  it**..```py.NUMB
+00027500: 4552 5320 3d20 5b31 2c20 312c 2032 2c20  ERS = [1, 1, 2, 
+00027510: 322c 2033 2c20 335d 0a0a 554e 4951 5545  2, 3, 3]..UNIQUE
+00027520: 5f4e 554d 4245 5253 203d 2073 6574 284e  _NUMBERS = set(N
+00027530: 554d 4245 5253 290a 0a60 6060 0a22 2222  UMBERS)..```."""
+00027540: 0a0a 5b52 3137 3232 5d0a 7768 7920 3d20  ..[R1722].why = 
+00027550: 2249 6e73 7465 6164 206f 6620 7573 696e  "Instead of usin
+00027560: 6720 6578 6974 2829 206f 7220 7175 6974  g exit() or quit
+00027570: 2829 2c20 636f 6e73 6964 6572 2075 7369  (), consider usi
+00027580: 6e67 2074 6865 2073 7973 2e65 7869 7428  ng the sys.exit(
+00027590: 292e 220a 6578 616d 706c 6573 203d 2022  ).".examples = "
+000275a0: 2222 0a2a 2a50 726f 626c 656d 6174 6963  "".**Problematic
+000275b0: 2063 6f64 652a 2a0a 0a60 6060 7079 0a69   code**..```py.i
+000275c0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 5c22  f __name__ == \"
+000275d0: 5f5f 6d61 696e 5f5f 5c22 3a0a 2020 2020  __main__\":.    
+000275e0: 7573 6572 203d 2069 6e70 7574 285c 2245  user = input(\"E
+000275f0: 6e74 6572 2075 7365 7220 6e61 6d65 3a20  nter user name: 
+00027600: 5c22 290a 2020 2020 7072 696e 7428 665c  \").    print(f\
+00027610: 2248 656c 6c6f 2c20 7b75 7365 727d 5c22  "Hello, {user}\"
+00027620: 290a 2020 2020 6578 6974 2830 2920 2023  ).    exit(0)  #
+00027630: 205b 636f 6e73 6964 6572 2d75 7369 6e67   [consider-using
+00027640: 2d73 7973 2d65 7869 745d 0a0a 6060 600a  -sys-exit]..```.
+00027650: 0a2a 2a48 6f77 2074 6f20 6669 7820 6974  .**How to fix it
+00027660: 2a2a 0a0a 6060 6070 790a 696d 706f 7274  **..```py.import
+00027670: 2073 7973 0a0a 6966 205f 5f6e 616d 655f   sys..if __name_
+00027680: 5f20 3d3d 205c 225f 5f6d 6169 6e5f 5f5c  _ == \"__main__\
+00027690: 223a 0a20 2020 2075 7365 7220 3d20 696e  ":.    user = in
+000276a0: 7075 7428 5c22 456e 7465 7220 7573 6572  put(\"Enter user
+000276b0: 206e 616d 653a 205c 2229 0a20 2020 2070   name: \").    p
+000276c0: 7269 6e74 2866 5c22 4865 6c6c 6f2c 207b  rint(f\"Hello, {
+000276d0: 7573 6572 7d5c 2229 0a20 2020 2073 7973  user}\").    sys
+000276e0: 2e65 7869 7428 3029 0a0a 6060 600a 2222  .exit(0)..```.""
+000276f0: 220a 0a5b 5231 3732 335d 0a77 6879 203d  "..[R1723].why =
+00027700: 2022 5573 6564 2069 6e20 6f72 6465 7220   "Used in order 
+00027710: 746f 2068 6967 686c 6967 6874 2061 6e20  to highlight an 
+00027720: 756e 6e65 6365 7373 6172 7920 626c 6f63  unnecessary bloc
+00027730: 6b20 6f66 2063 6f64 6520 666f 6c6c 6f77  k of code follow
+00027740: 696e 6720 616e 2069 6620 636f 6e74 6169  ing an if contai
+00027750: 6e69 6e67 2061 2062 7265 616b 2073 7461  ning a break sta
+00027760: 7465 6d65 6e74 2e20 4173 2073 7563 682c  tement. As such,
+00027770: 2069 7420 7769 6c6c 2077 6172 6e20 7768   it will warn wh
+00027780: 656e 2069 7420 656e 636f 756e 7465 7273  en it encounters
+00027790: 2061 6e20 656c 7365 2066 6f6c 6c6f 7769   an else followi
+000277a0: 6e67 2061 2063 6861 696e 206f 6620 6966  ng a chain of if
+000277b0: 732c 2061 6c6c 206f 6620 7468 656d 2063  s, all of them c
+000277c0: 6f6e 7461 696e 696e 6720 6120 6272 6561  ontaining a brea
+000277d0: 6b20 7374 6174 656d 656e 742e 220a 6578  k statement.".ex
+000277e0: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
+000277f0: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
+00027800: 2a0a 0a60 6060 7079 0a64 6566 206e 6578  *..```py.def nex
+00027810: 745f 7365 7665 6e5f 656c 656d 656e 7473  t_seven_elements
+00027820: 2869 7465 7261 746f 7229 3a0a 2020 2020  (iterator):.    
+00027830: 666f 7220 692c 2069 7465 6d20 696e 2065  for i, item in e
+00027840: 6e75 6d65 7261 7465 2869 7465 7261 746f  numerate(iterato
+00027850: 7229 3a0a 2020 2020 2020 2020 6966 2069  r):.        if i
+00027860: 203d 3d20 373a 2020 2320 5b6e 6f2d 656c   == 7:  # [no-el
+00027870: 7365 2d62 7265 616b 5d0a 2020 2020 2020  se-break].      
+00027880: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00027890: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000278a0: 2020 2020 2020 7969 656c 6420 6974 656d        yield item
+000278b0: 0a0a 6060 600a 0a2a 2a48 6f77 2074 6f20  ..```..**How to 
+000278c0: 6669 7820 6974 2a2a 0a0a 6060 6070 790a  fix it**..```py.
+000278d0: 6465 6620 6e65 7874 5f73 6576 656e 5f65  def next_seven_e
+000278e0: 6c65 6d65 6e74 7328 6974 6572 6174 6f72  lements(iterator
+000278f0: 293a 0a20 2020 2066 6f72 2069 2c20 6974  ):.    for i, it
+00027900: 656d 2069 6e20 656e 756d 6572 6174 6528  em in enumerate(
+00027910: 6974 6572 6174 6f72 293a 0a20 2020 2020  iterator):.     
+00027920: 2020 2069 6620 6920 3d3d 2037 3a0a 2020     if i == 7:.  
+00027930: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00027940: 2020 2020 2020 2020 7969 656c 6420 6974          yield it
+00027950: 656d 0a0a 6060 600a 2222 220a 0a5b 5231  em..```."""..[R1
+00027960: 3732 345d 0a77 6879 203d 2022 5573 6564  724].why = "Used
+00027970: 2069 6e20 6f72 6465 7220 746f 2068 6967   in order to hig
+00027980: 686c 6967 6874 2061 6e20 756e 6e65 6365  hlight an unnece
+00027990: 7373 6172 7920 626c 6f63 6b20 6f66 2063  ssary block of c
+000279a0: 6f64 6520 666f 6c6c 6f77 696e 6720 616e  ode following an
+000279b0: 2069 6620 636f 6e74 6169 6e69 6e67 2061   if containing a
+000279c0: 2063 6f6e 7469 6e75 6520 7374 6174 656d   continue statem
+000279d0: 656e 742e 2041 7320 7375 6368 2c20 6974  ent. As such, it
+000279e0: 2077 696c 6c20 7761 726e 2077 6865 6e20   will warn when 
+000279f0: 6974 2065 6e63 6f75 6e74 6572 7320 616e  it encounters an
+00027a00: 2065 6c73 6520 666f 6c6c 6f77 696e 6720   else following 
+00027a10: 6120 6368 6169 6e20 6f66 2069 6673 2c20  a chain of ifs, 
+00027a20: 616c 6c20 6f66 2074 6865 6d20 636f 6e74  all of them cont
+00027a30: 6169 6e69 6e67 2061 2063 6f6e 7469 6e75  aining a continu
+00027a40: 6520 7374 6174 656d 656e 742e 220a 6578  e statement.".ex
+00027a50: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
+00027a60: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
+00027a70: 2a0a 0a60 6060 7079 0a64 6566 2065 7665  *..```py.def eve
+00027a80: 6e5f 6e75 6d62 6572 5f75 6e64 6572 286e  n_number_under(n
+00027a90: 3a20 696e 7429 3a0a 2020 2020 666f 7220  : int):.    for 
+00027aa0: 6920 696e 2072 616e 6765 286e 293a 0a20  i in range(n):. 
+00027ab0: 2020 2020 2020 2069 6620 6925 3220 3d3d         if i%2 ==
+00027ac0: 2031 3a20 2023 205b 6e6f 2d65 6c73 652d   1:  # [no-else-
+00027ad0: 636f 6e74 696e 7565 5d0a 2020 2020 2020  continue].      
+00027ae0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00027af0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00027b00: 2020 2020 2020 2020 2079 6965 6c64 2069           yield i
+00027b10: 0a0a 6060 600a 0a2a 2a48 6f77 2074 6f20  ..```..**How to 
+00027b20: 6669 7820 6974 2a2a 0a0a 6060 6070 790a  fix it**..```py.
+00027b30: 6465 6620 6576 656e 5f6e 756d 6265 725f  def even_number_
+00027b40: 756e 6465 7228 6e3a 2069 6e74 293a 0a20  under(n: int):. 
+00027b50: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00027b60: 6528 6e29 3a0a 2020 2020 2020 2020 6966  e(n):.        if
+00027b70: 2069 2532 203d 3d20 313a 0a20 2020 2020   i%2 == 1:.     
+00027b80: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00027b90: 2020 2020 2020 2020 7969 656c 6420 690a          yield i.
+00027ba0: 0a60 6060 0a22 2222 0a0a 5b52 3137 3235  .```."""..[R1725
+00027bb0: 5d0a 7768 7920 3d20 2249 7420 6c6f 6f6b  ].why = "It look
+00027bc0: 7320 6c69 6b65 2063 616c 6c69 6e67 2074  s like calling t
+00027bd0: 6865 2073 7570 6572 2829 2062 7569 6c74  he super() built
+00027be0: 696e 2077 6974 6820 7468 6520 6375 7272  in with the curr
+00027bf0: 656e 7420 636c 6173 7320 616e 6420 696e  ent class and in
+00027c00: 7374 616e 6365 2e20 4f6e 2050 7974 686f  stance. On Pytho
+00027c10: 6e20 3320 7468 6573 6520 6172 6775 6d65  n 3 these argume
+00027c20: 6e74 7320 6172 6520 7468 6520 6465 6661  nts are the defa
+00027c30: 756c 7420 616e 6420 7468 6579 2063 616e  ult and they can
+00027c40: 2062 6520 6f6d 6974 7465 642e 220a 6578   be omitted.".ex
+00027c50: 616d 706c 6573 203d 2022 2222 0a2a 2a50  amples = """.**P
+00027c60: 726f 626c 656d 6174 6963 2063 6f64 652a  roblematic code*
+00027c70: 2a0a 0a60 6060 7079 0a63 6c61 7373 2046  *..```py.class F
+00027c80: 7275 6974 3a0a 2020 2020 7061 7373 0a0a  ruit:.    pass..
+00027c90: 0a63 6c61 7373 204f 7261 6e67 6528 4672  .class Orange(Fr
+00027ca0: 7569 7429 3a0a 2020 2020 6465 6620 5f5f  uit):.    def __
+00027cb0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00027cc0: 2020 2020 2020 7375 7065 7228 4f72 616e        super(Oran
+00027cd0: 6765 2c20 7365 6c66 292e 5f5f 696e 6974  ge, self).__init
+00027ce0: 5f5f 2829 2020 2320 5b73 7570 6572 2d77  __()  # [super-w
+00027cf0: 6974 682d 6172 6775 6d65 6e74 735d 0a0a  ith-arguments]..
+00027d00: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
+00027d10: 7820 6974 2a2a 0a0a 6060 6070 790a 636c  x it**..```py.cl
+00027d20: 6173 7320 4672 7569 743a 0a20 2020 2070  ass Fruit:.    p
+00027d30: 6173 730a 0a0a 636c 6173 7320 4f72 616e  ass...class Oran
+00027d40: 6765 2846 7275 6974 293a 0a20 2020 2064  ge(Fruit):.    d
+00027d50: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00027d60: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+00027d70: 2829 2e5f 5f69 6e69 745f 5f28 290a 0a60  ().__init__()..`
+00027d80: 6060 0a22 2222 0a0a 5b52 3137 3236 5d0a  ``."""..[R1726].
+00027d90: 7768 7920 3d20 2249 7420 6c6f 6f6b 7320  why = "It looks 
+00027da0: 6c69 6b65 2074 6865 2062 6f6f 6c65 616e  like the boolean
+00027db0: 2063 6f6e 6469 7469 6f6e 2069 7320 6162   condition is ab
+00027dc0: 6c65 2074 6f20 6265 2073 696d 706c 6966  le to be simplif
+00027dd0: 6965 642e 220a 6578 616d 706c 6573 203d  ied.".examples =
+00027de0: 2022 2222 0a2a 2a50 726f 626c 656d 6174   """.**Problemat
+00027df0: 6963 2063 6f64 652a 2a0a 0a60 6060 7079  ic code**..```py
+00027e00: 0a64 6566 2068 6173 5f61 7070 6c65 7328  .def has_apples(
+00027e10: 6170 706c 6573 2920 2d3e 2062 6f6f 6c3a  apples) -> bool:
+00027e20: 0a20 2020 2072 6574 7572 6e20 626f 6f6c  .    return bool
+00027e30: 2861 7070 6c65 7320 6f72 2046 616c 7365  (apples or False
+00027e40: 2920 2023 205b 7369 6d70 6c69 6669 6162  )  # [simplifiab
+00027e50: 6c65 2d63 6f6e 6469 7469 6f6e 5d0a 0a60  le-condition]..`
+00027e60: 6060 0a0a 2a2a 486f 7720 746f 2066 6978  ``..**How to fix
+00027e70: 2069 742a 2a0a 0a60 6060 7079 0a64 6566   it**..```py.def
+00027e80: 2068 6173 5f61 7070 6c65 7328 6170 706c   has_apples(appl
+00027e90: 6573 2920 2d3e 2062 6f6f 6c3a 0a20 2020  es) -> bool:.   
+00027ea0: 2072 6574 7572 6e20 626f 6f6c 2861 7070   return bool(app
+00027eb0: 6c65 7329 0a0a 6060 600a 2222 220a 0a5b  les)..```."""..[
+00027ec0: 5231 3732 375d 0a77 6879 203d 2022 4974  R1727].why = "It
+00027ed0: 206c 6f6f 6b73 206c 696b 6520 7468 6520   looks like the 
+00027ee0: 626f 6f6c 6561 6e20 636f 6e64 6974 696f  boolean conditio
+00027ef0: 6e20 6361 6e20 6265 2073 696d 706c 6966  n can be simplif
+00027f00: 6965 6420 746f 2061 2063 6f6e 7374 616e  ied to a constan
+00027f10: 7420 7661 6c75 652e 220a 6578 616d 706c  t value.".exampl
+00027f20: 6573 203d 2022 2222 0a2a 2a50 726f 626c  es = """.**Probl
+00027f30: 656d 6174 6963 2063 6f64 652a 2a0a 0a60  ematic code**..`
+00027f40: 6060 7079 0a64 6566 2069 735f 615f 6672  ``py.def is_a_fr
+00027f50: 7569 7428 6672 7569 7429 3a0a 2020 2020  uit(fruit):.    
+00027f60: 7265 7475 726e 2062 6f6f 6c28 6672 7569  return bool(frui
+00027f70: 7420 696e 207b 5c22 6170 706c 655c 222c  t in {\"apple\",
+00027f80: 205c 226f 7261 6e67 655c 227d 206f 7220   \"orange\"} or 
+00027f90: 5472 7565 2920 2023 205b 636f 6e64 6974  True)  # [condit
+00027fa0: 696f 6e2d 6576 616c 732d 746f 2d63 6f6e  ion-evals-to-con
+00027fb0: 7374 616e 745d 0a0a 6060 600a 0a2a 2a48  stant]..```..**H
+00027fc0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00027fd0: 6060 6070 790a 6465 6620 6973 5f61 5f66  ```py.def is_a_f
+00027fe0: 7275 6974 2866 7275 6974 293a 0a20 2020  ruit(fruit):.   
+00027ff0: 2072 6574 7572 6e20 6672 7569 7420 696e   return fruit in
+00028000: 207b 5c22 6170 706c 655c 222c 205c 226f   {\"apple\", \"o
+00028010: 7261 6e67 655c 227d 0a0a 6060 600a 2222  range\"}..```.""
+00028020: 220a 0a5b 5231 3732 385d 0a77 6879 203d  "..[R1728].why =
+00028030: 2022 4966 2079 6f75 7220 636f 6e74 6169   "If your contai
+00028040: 6e65 7220 6361 6e20 6265 206c 6172 6765  ner can be large
+00028050: 2075 7369 6e67 2061 2067 656e 6572 6174   using a generat
+00028060: 6f72 2077 696c 6c20 6272 696e 6720 6265  or will bring be
+00028070: 7474 6572 2070 6572 666f 726d 616e 6365  tter performance
+00028080: 2e22 0a65 7861 6d70 6c65 7320 3d20 2222  .".examples = ""
+00028090: 220a 2a2a 5072 6f62 6c65 6d61 7469 6320  ".**Problematic 
+000280a0: 636f 6465 2a2a 0a0a 6060 6070 790a 6c69  code**..```py.li
+000280b0: 7374 285b 3020 666f 7220 7920 696e 206c  st([0 for y in l
+000280c0: 6973 7428 7261 6e67 6528 3130 2929 5d29  ist(range(10))])
+000280d0: 2020 2320 5b63 6f6e 7369 6465 722d 7573    # [consider-us
+000280e0: 696e 672d 6765 6e65 7261 746f 725d 0a74  ing-generator].t
+000280f0: 7570 6c65 285b 3020 666f 7220 7920 696e  uple([0 for y in
+00028100: 206c 6973 7428 7261 6e67 6528 3130 2929   list(range(10))
+00028110: 5d29 2020 2320 5b63 6f6e 7369 6465 722d  ])  # [consider-
+00028120: 7573 696e 672d 6765 6e65 7261 746f 725d  using-generator]
+00028130: 0a73 756d 285b 792a 2a32 2066 6f72 2079  .sum([y**2 for y
+00028140: 2069 6e20 6c69 7374 2872 616e 6765 2831   in list(range(1
+00028150: 3029 295d 2920 2023 205b 636f 6e73 6964  0))])  # [consid
+00028160: 6572 2d75 7369 6e67 2d67 656e 6572 6174  er-using-generat
+00028170: 6f72 5d0a 6d61 7828 5b79 2a2a 3220 666f  or].max([y**2 fo
+00028180: 7220 7920 696e 206c 6973 7428 7261 6e67  r y in list(rang
+00028190: 6528 3130 2929 5d29 2020 2320 5b63 6f6e  e(10))])  # [con
+000281a0: 7369 6465 722d 7573 696e 672d 6765 6e65  sider-using-gene
+000281b0: 7261 746f 725d 0a6d 696e 285b 792a 2a32  rator].min([y**2
+000281c0: 2066 6f72 2079 2069 6e20 6c69 7374 2872   for y in list(r
+000281d0: 616e 6765 2831 3029 295d 2920 2023 205b  ange(10))])  # [
+000281e0: 636f 6e73 6964 6572 2d75 7369 6e67 2d67  consider-using-g
+000281f0: 656e 6572 6174 6f72 5d0a 0a60 6060 0a0a  enerator]..```..
+00028200: 2a2a 486f 7720 746f 2066 6978 2069 742a  **How to fix it*
+00028210: 2a0a 0a60 6060 7079 0a6c 6973 7428 3020  *..```py.list(0 
+00028220: 666f 7220 7920 696e 206c 6973 7428 7261  for y in list(ra
+00028230: 6e67 6528 3130 2929 290a 7475 706c 6528  nge(10))).tuple(
+00028240: 3020 666f 7220 7920 696e 206c 6973 7428  0 for y in list(
+00028250: 7261 6e67 6528 3130 2929 290a 7375 6d28  range(10))).sum(
+00028260: 792a 2a32 2066 6f72 2079 2069 6e20 6c69  y**2 for y in li
+00028270: 7374 2872 616e 6765 2831 3029 2929 0a6d  st(range(10))).m
+00028280: 6178 2879 2a2a 3220 666f 7220 7920 696e  ax(y**2 for y in
+00028290: 206c 6973 7428 7261 6e67 6528 3130 2929   list(range(10))
+000282a0: 290a 6d69 6e28 792a 2a32 2066 6f72 2079  ).min(y**2 for y
+000282b0: 2069 6e20 6c69 7374 2872 616e 6765 2831   in list(range(1
+000282c0: 3029 2929 0a0a 6060 600a 0a3c 6120 6872  0)))..```..<a hr
+000282d0: 6566 3d5c 2268 7474 7073 3a2f 2f70 796c  ef=\"https://pyl
+000282e0: 696e 742e 7079 6371 612e 6f72 672f 656e  int.pycqa.org/en
+000282f0: 2f6c 6174 6573 742f 7573 6572 5f67 7569  /latest/user_gui
+00028300: 6465 2f6d 6573 7361 6765 732f 7265 6661  de/messages/refa
+00028310: 6374 6f72 2f63 6f6e 7369 6465 722d 7573  ctor/consider-us
+00028320: 696e 672d 6765 6e65 7261 746f 722e 6874  ing-generator.ht
+00028330: 6d6c 5c22 3e41 6464 6974 696f 6e61 6c20  ml\">Additional 
+00028340: 696e 666f 726d 6174 696f 6e3c 2f61 3e22  information</a>"
+00028350: 2222 0a0a 5b52 3137 3239 5d0a 7768 7920  ""..[R1729].why 
+00028360: 3d20 2243 6f6d 7072 6568 656e 7369 6f6e  = "Comprehension
+00028370: 2069 6e73 6964 6520 6f66 2027 616e 7927   inside of 'any'
+00028380: 2c20 2761 6c6c 272c 2027 6d61 7827 2c20  , 'all', 'max', 
+00028390: 276d 696e 2720 6f72 2027 7375 6d27 2069  'min' or 'sum' i
+000283a0: 7320 756e 6e65 6365 7373 6172 792e 2041  s unnecessary. A
+000283b0: 2067 656e 6572 6174 6f72 2077 6f75 6c64   generator would
+000283c0: 2062 6520 7375 6666 6963 6965 6e74 2061   be sufficient a
+000283d0: 6e64 2066 6173 7465 722e 220a 6578 616d  nd faster.".exam
+000283e0: 706c 6573 203d 2022 2222 0a2a 2a50 726f  ples = """.**Pro
+000283f0: 626c 656d 6174 6963 2063 6f64 652a 2a0a  blematic code**.
+00028400: 0a60 6060 7079 0a66 726f 6d20 7261 6e64  .```py.from rand
+00028410: 6f6d 2069 6d70 6f72 7420 7261 6e64 696e  om import randin
+00028420: 740a 0a61 6c6c 285b 7261 6e64 696e 7428  t..all([randint(
+00028430: 2d35 2c20 3529 203e 2030 2066 6f72 205f  -5, 5) > 0 for _
+00028440: 2069 6e20 7261 6e67 6528 3130 295d 2920   in range(10)]) 
+00028450: 2023 205b 7573 652d 612d 6765 6e65 7261   # [use-a-genera
+00028460: 746f 725d 0a61 6e79 285b 7261 6e64 696e  tor].any([randin
+00028470: 7428 2d35 2c20 3529 203e 2030 2066 6f72  t(-5, 5) > 0 for
+00028480: 205f 2069 6e20 7261 6e67 6528 3130 295d   _ in range(10)]
+00028490: 2920 2023 205b 7573 652d 612d 6765 6e65  )  # [use-a-gene
+000284a0: 7261 746f 725d 0a0a 6060 600a 0a2a 2a48  rator]..```..**H
+000284b0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+000284c0: 6060 6070 790a 6672 6f6d 2072 616e 646f  ```py.from rando
+000284d0: 6d20 696d 706f 7274 2072 616e 6469 6e74  m import randint
+000284e0: 0a0a 616c 6c28 7261 6e64 696e 7428 2d35  ..all(randint(-5
+000284f0: 2c20 3529 203e 2030 2066 6f72 205f 2069  , 5) > 0 for _ i
+00028500: 6e20 7261 6e67 6528 3130 2929 0a61 6e79  n range(10)).any
+00028510: 2872 616e 6469 6e74 282d 352c 2035 2920  (randint(-5, 5) 
+00028520: 3e20 3020 666f 7220 5f20 696e 2072 616e  > 0 for _ in ran
+00028530: 6765 2831 3029 290a 0a60 6060 0a0a 3c61  ge(10))..```..<a
+00028540: 2068 7265 663d 5c22 6874 7470 733a 2f2f   href=\"https://
+00028550: 7079 6c69 6e74 2e70 7963 7161 2e6f 7267  pylint.pycqa.org
+00028560: 2f65 6e2f 6c61 7465 7374 2f75 7365 725f  /en/latest/user_
+00028570: 6775 6964 652f 6d65 7373 6167 6573 2f72  guide/messages/r
+00028580: 6566 6163 746f 722f 7573 652d 612d 6765  efactor/use-a-ge
+00028590: 6e65 7261 746f 722e 6874 6d6c 5c22 3e41  nerator.html\">A
+000285a0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
+000285b0: 6174 696f 6e3c 2f61 3e22 2222 0a0a 5b52  ation</a>"""..[R
+000285c0: 3137 3330 5d0a 7768 7920 3d20 2255 7369  1730].why = "Usi
+000285d0: 6e67 2074 6865 206d 696e 2062 7569 6c74  ng the min built
+000285e0: 696e 2069 6e73 7465 6164 206f 6620 6120  in instead of a 
+000285f0: 636f 6e64 6974 696f 6e61 6c20 696d 7072  conditional impr
+00028600: 6f76 6573 2072 6561 6461 6269 6c69 7479  oves readability
+00028610: 2061 6e64 2063 6f6e 6369 7365 6e65 7373   and conciseness
+00028620: 2e22 0a65 7861 6d70 6c65 7320 3d20 2222  .".examples = ""
+00028630: 220a 2a2a 5072 6f62 6c65 6d61 7469 6320  ".**Problematic 
+00028640: 636f 6465 2a2a 0a0a 6060 6070 790a 6465  code**..```py.de
+00028650: 6620 6765 745f 6d69 6e28 7661 6c75 6531  f get_min(value1
+00028660: 2c20 7661 6c75 6532 293a 0a20 2020 2069  , value2):.    i
+00028670: 6620 7661 6c75 6531 203e 2076 616c 7565  f value1 > value
+00028680: 323a 2020 2320 5b63 6f6e 7369 6465 722d  2:  # [consider-
+00028690: 7573 696e 672d 6d69 6e2d 6275 696c 7469  using-min-builti
+000286a0: 6e5d 0a20 2020 2020 2020 2076 616c 7565  n].        value
+000286b0: 3120 3d20 7661 6c75 6532 0a20 2020 2072  1 = value2.    r
+000286c0: 6574 7572 6e20 7661 6c75 6531 0a0a 0a70  eturn value1...p
+000286d0: 7269 6e74 2867 6574 5f6d 696e 2831 2c20  rint(get_min(1, 
+000286e0: 3229 290a 0a60 6060 0a0a 2a2a 486f 7720  2))..```..**How 
+000286f0: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
+00028700: 7079 0a70 7269 6e74 286d 696e 2831 2c20  py.print(min(1, 
+00028710: 3229 290a 0a60 6060 0a22 2222 0a0a 5b52  2))..```."""..[R
+00028720: 3137 3331 5d0a 7768 7920 3d20 2255 7369  1731].why = "Usi
+00028730: 6e67 2074 6865 206d 6178 2062 7569 6c74  ng the max built
+00028740: 696e 2069 6e73 7465 6164 206f 6620 6120  in instead of a 
+00028750: 636f 6e64 6974 696f 6e61 6c20 696d 7072  conditional impr
+00028760: 6f76 6573 2072 6561 6461 6269 6c69 7479  oves readability
+00028770: 2061 6e64 2063 6f6e 6369 7365 6e65 7373   and conciseness
+00028780: 2e22 0a65 7861 6d70 6c65 7320 3d20 2222  .".examples = ""
+00028790: 220a 2a2a 5072 6f62 6c65 6d61 7469 6320  ".**Problematic 
+000287a0: 636f 6465 2a2a 0a0a 6060 6070 790a 6465  code**..```py.de
+000287b0: 6620 6765 745f 6d61 7828 7661 6c75 6531  f get_max(value1
+000287c0: 2c20 7661 6c75 6532 293a 0a20 2020 2069  , value2):.    i
+000287d0: 6620 7661 6c75 6531 203c 2076 616c 7565  f value1 < value
+000287e0: 323a 2020 2320 5b63 6f6e 7369 6465 722d  2:  # [consider-
+000287f0: 7573 696e 672d 6d61 782d 6275 696c 7469  using-max-builti
+00028800: 6e5d 0a20 2020 2020 2020 2076 616c 7565  n].        value
+00028810: 3120 3d20 7661 6c75 6532 0a20 2020 2072  1 = value2.    r
+00028820: 6574 7572 6e20 7661 6c75 6531 0a0a 0a70  eturn value1...p
+00028830: 7269 6e74 2867 6574 5f6d 6178 2831 2c20  rint(get_max(1, 
+00028840: 3229 290a 0a60 6060 0a0a 2a2a 486f 7720  2))..```..**How 
+00028850: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
+00028860: 7079 0a70 7269 6e74 286d 6178 2831 2c20  py.print(max(1, 
+00028870: 3229 290a 0a60 6060 0a22 2222 0a0a 5b52  2))..```."""..[R
+00028880: 3137 3332 5d0a 7768 7920 3d20 2245 6d69  1732].why = "Emi
+00028890: 7474 6564 2069 6620 6120 7265 736f 7572  tted if a resour
+000288a0: 6365 2d61 6c6c 6f63 6174 696e 6720 6173  ce-allocating as
+000288b0: 7369 676e 6d65 6e74 206f 7220 6361 6c6c  signment or call
+000288c0: 206d 6179 2062 6520 7265 706c 6163 6564   may be replaced
+000288d0: 2062 7920 6120 2777 6974 6827 2062 6c6f   by a 'with' blo
+000288e0: 636b 2e20 4279 2075 7369 6e67 2027 7769  ck. By using 'wi
+000288f0: 7468 2720 7468 6520 7265 6c65 6173 6520  th' the release 
+00028900: 6f66 2074 6865 2061 6c6c 6f63 6174 6564  of the allocated
+00028910: 2072 6573 6f75 7263 6573 2069 7320 656e   resources is en
+00028920: 7375 7265 6420 6576 656e 2069 6e20 7468  sured even in th
+00028930: 6520 6361 7365 206f 6620 616e 2065 7863  e case of an exc
+00028940: 6570 7469 6f6e 2e22 0a65 7861 6d70 6c65  eption.".example
+00028950: 7320 3d20 2222 220a 2a2a 5072 6f62 6c65  s = """.**Proble
+00028960: 6d61 7469 6320 636f 6465 2a2a 0a0a 6060  matic code**..``
+00028970: 6070 790a 6669 6c65 203d 206f 7065 6e28  `py.file = open(
+00028980: 5c22 6170 706c 652e 7478 745c 222c 205c  \"apple.txt\", \
+00028990: 2272 5c22 2c20 656e 636f 6469 6e67 3d5c  "r\", encoding=\
+000289a0: 2275 7466 385c 2229 2020 2320 5b63 6f6e  "utf8\")  # [con
+000289b0: 7369 6465 722d 7573 696e 672d 7769 7468  sider-using-with
+000289c0: 5d0a 636f 6e74 656e 7473 203d 2066 696c  ].contents = fil
+000289d0: 652e 7265 6164 2829 0a66 696c 652e 636c  e.read().file.cl
+000289e0: 6f73 6528 290a 0a77 6f72 7374 203d 206f  ose()..worst = o
+000289f0: 7065 6e28 5c22 6261 6e61 6e61 2e74 7874  pen(\"banana.txt
+00028a00: 5c22 2c20 5c22 725c 222c 2065 6e63 6f64  \", \"r\", encod
+00028a10: 696e 673d 5c22 7574 6638 5c22 292e 7265  ing=\"utf8\").re
+00028a20: 6164 2829 2020 2320 5b63 6f6e 7369 6465  ad()  # [conside
+00028a30: 722d 7573 696e 672d 7769 7468 5d0a 0a60  r-using-with]..`
+00028a40: 6060 0a0a 2a2a 486f 7720 746f 2066 6978  ``..**How to fix
+00028a50: 2069 742a 2a0a 0a60 6060 7079 0a77 6974   it**..```py.wit
+00028a60: 6820 6f70 656e 285c 2261 7070 6c65 2e74  h open(\"apple.t
+00028a70: 7874 5c22 2c20 5c22 725c 222c 2065 6e63  xt\", \"r\", enc
+00028a80: 6f64 696e 673d 5c22 7574 6638 5c22 2920  oding=\"utf8\") 
+00028a90: 6173 2066 696c 653a 0a20 2020 2063 6f6e  as file:.    con
+00028aa0: 7465 6e74 7320 3d20 6669 6c65 2e72 6561  tents = file.rea
+00028ab0: 6428 290a 0a77 6974 6820 6f70 656e 285c  d()..with open(\
 00028ac0: 2262 616e 616e 612e 7478 745c 222c 205c  "banana.txt\", \
 00028ad0: 2272 5c22 2c20 656e 636f 6469 6e67 3d5c  "r\", encoding=\
-00028ae0: 2275 7466 385c 2229 2e72 6561 6428 2920  "utf8\").read() 
-00028af0: 2023 205b 636f 6e73 6964 6572 2d75 7369   # [consider-usi
-00028b00: 6e67 2d77 6974 685d 0a0a 6060 600a 0a2a  ng-with]..```..*
-00028b10: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
-00028b20: 0a0a 6060 6070 790a 7769 7468 206f 7065  ..```py.with ope
-00028b30: 6e28 5c22 6170 706c 652e 7478 745c 222c  n(\"apple.txt\",
-00028b40: 205c 2272 5c22 2c20 656e 636f 6469 6e67   \"r\", encoding
-00028b50: 3d5c 2275 7466 385c 2229 2061 7320 6669  =\"utf8\") as fi
-00028b60: 6c65 3a0a 2020 2020 636f 6e74 656e 7473  le:.    contents
-00028b70: 203d 2066 696c 652e 7265 6164 2829 0a0a   = file.read()..
-00028b80: 7769 7468 206f 7065 6e28 5c22 6261 6e61  with open(\"bana
-00028b90: 6e61 2e74 7874 5c22 2c20 5c22 725c 222c  na.txt\", \"r\",
-00028ba0: 2065 6e63 6f64 696e 673d 5c22 7574 6638   encoding=\"utf8
-00028bb0: 5c22 2920 6173 2066 3a0a 2020 2020 6265  \") as f:.    be
-00028bc0: 7374 203d 2066 2e72 6561 6428 290a 0a60  st = f.read()..`
-00028bd0: 6060 0a0a 3c61 2068 7265 663d 5c22 6874  ``..<a href=\"ht
-00028be0: 7470 733a 2f2f 7079 6c69 6e74 2e70 7963  tps://pylint.pyc
-00028bf0: 7161 2e6f 7267 2f65 6e2f 6c61 7465 7374  qa.org/en/latest
-00028c00: 2f75 7365 725f 6775 6964 652f 6d65 7373  /user_guide/mess
-00028c10: 6167 6573 2f72 6566 6163 746f 722f 636f  ages/refactor/co
-00028c20: 6e73 6964 6572 2d75 7369 6e67 2d77 6974  nsider-using-wit
-00028c30: 682e 6874 6d6c 5c22 3e41 6464 6974 696f  h.html\">Additio
-00028c40: 6e61 6c20 696e 666f 726d 6174 696f 6e3c  nal information<
-00028c50: 2f61 3e22 2222 0a0a 5b52 3137 3333 5d0a  /a>"""..[R1733].
-00028c60: 7768 7920 3d20 2249 7420 6c6f 6f6b 7320  why = "It looks 
-00028c70: 6c69 6b65 2069 7465 7261 7469 6e67 206f  like iterating o
-00028c80: 7665 7220 7468 6520 6469 6374 696f 6e61  ver the dictiona
-00028c90: 7279 2069 7465 6d73 2028 6b65 792d 6974  ry items (key-it
-00028ca0: 656d 2070 6169 7273 2920 616e 6420 6163  em pairs) and ac
-00028cb0: 6365 7373 696e 6720 7468 6520 7661 6c75  cessing the valu
-00028cc0: 6520 6279 2069 6e64 6578 206c 6f6f 6b75  e by index looku
-00028cd0: 702e 2054 6865 2076 616c 7565 2063 616e  p. The value can
-00028ce0: 2062 6520 6163 6365 7373 6564 2064 6972   be accessed dir
-00028cf0: 6563 746c 7920 696e 7374 6561 642e 220a  ectly instead.".
-00028d00: 6578 616d 706c 6573 203d 2022 2222 0a2a  examples = """.*
-00028d10: 2a50 726f 626c 656d 6174 6963 2063 6f64  *Problematic cod
-00028d20: 652a 2a0a 0a60 6060 7079 0a46 5255 4954  e**..```py.FRUIT
-00028d30: 5320 3d20 7b5c 2261 7070 6c65 5c22 3a20  S = {\"apple\": 
-00028d40: 312c 205c 226f 7261 6e67 655c 223a 2031  1, \"orange\": 1
-00028d50: 302c 205c 2262 6572 7279 5c22 3a20 3232  0, \"berry\": 22
-00028d60: 7d0a 0a66 6f72 2066 7275 6974 5f6e 616d  }..for fruit_nam
-00028d70: 652c 2066 7275 6974 5f63 6f75 6e74 2069  e, fruit_count i
-00028d80: 6e20 4652 5549 5453 2e69 7465 6d73 2829  n FRUITS.items()
-00028d90: 3a0a 2020 2020 7072 696e 7428 4652 5549  :.    print(FRUI
-00028da0: 5453 5b66 7275 6974 5f6e 616d 655d 2920  TS[fruit_name]) 
-00028db0: 2023 205b 756e 6e65 6365 7373 6172 792d   # [unnecessary-
-00028dc0: 6469 6374 2d69 6e64 6578 2d6c 6f6f 6b75  dict-index-looku
-00028dd0: 705d 0a0a 6060 600a 0a2a 2a48 6f77 2074  p]..```..**How t
-00028de0: 6f20 6669 7820 6974 2a2a 0a0a 6060 6070  o fix it**..```p
-00028df0: 790a 4652 5549 5453 203d 207b 5c22 6170  y.FRUITS = {\"ap
-00028e00: 706c 655c 223a 2031 2c20 5c22 6f72 616e  ple\": 1, \"oran
-00028e10: 6765 5c22 3a20 3130 2c20 5c22 6265 7272  ge\": 10, \"berr
-00028e20: 795c 223a 2032 327d 0a0a 666f 7220 6672  y\": 22}..for fr
-00028e30: 7569 745f 6e61 6d65 2c20 6672 7569 745f  uit_name, fruit_
-00028e40: 636f 756e 7420 696e 2046 5255 4954 532e  count in FRUITS.
-00028e50: 6974 656d 7328 293a 0a20 2020 2070 7269  items():.    pri
-00028e60: 6e74 2866 7275 6974 5f63 6f75 6e74 290a  nt(fruit_count).
-00028e70: 0a60 6060 0a22 2222 0a0a 5b52 3137 3334  .```."""..[R1734
-00028e80: 5d0a 7768 7920 3d20 2249 7420 6c6f 6f6b  ].why = "It look
-00028e90: 7320 6c69 6b65 2075 7369 6e67 206c 6973  s like using lis
-00028ea0: 7428 2920 746f 2063 7265 6174 6520 616e  t() to create an
-00028eb0: 2065 6d70 7479 206c 6973 7420 696e 7374   empty list inst
-00028ec0: 6561 6420 6f66 2074 6865 206c 6974 6572  ead of the liter
-00028ed0: 616c 205b 5d2e 2054 6865 206c 6974 6572  al []. The liter
-00028ee0: 616c 2069 7320 6661 7374 6572 2061 7320  al is faster as 
-00028ef0: 6974 2061 766f 6964 7320 616e 2061 6464  it avoids an add
-00028f00: 6974 696f 6e61 6c20 6675 6e63 7469 6f6e  itional function
-00028f10: 2063 616c 6c2e 220a 6578 616d 706c 6573   call.".examples
-00028f20: 203d 2022 2222 0a2a 2a50 726f 626c 656d   = """.**Problem
-00028f30: 6174 6963 2063 6f64 652a 2a0a 0a60 6060  atic code**..```
-00028f40: 7079 0a65 6d70 7479 5f6c 6973 7420 3d20  py.empty_list = 
-00028f50: 6c69 7374 2829 2020 2320 5b75 7365 2d6c  list()  # [use-l
-00028f60: 6973 742d 6c69 7465 7261 6c5d 0a0a 6060  ist-literal]..``
-00028f70: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
-00028f80: 6974 2a2a 0a0a 6060 6070 790a 656d 7074  it**..```py.empt
-00028f90: 795f 6c69 7374 203d 205b 5d0a 0a60 6060  y_list = []..```
-00028fa0: 0a22 2222 0a0a 5b52 3137 3335 5d0a 7768  ."""..[R1735].wh
-00028fb0: 7920 3d20 2249 7420 6c6f 6f6b 7320 6c69  y = "It looks li
-00028fc0: 6b65 2075 7369 6e67 2064 6963 7428 2920  ke using dict() 
-00028fd0: 746f 2063 7265 6174 6520 616e 2065 6d70  to create an emp
-00028fe0: 7479 2064 6963 7469 6f6e 6172 7920 696e  ty dictionary in
-00028ff0: 7374 6561 6420 6f66 2074 6865 206c 6974  stead of the lit
-00029000: 6572 616c 207b 7d2e 2054 6865 206c 6974  eral {}. The lit
-00029010: 6572 616c 2069 7320 6661 7374 6572 2061  eral is faster a
-00029020: 7320 6974 2061 766f 6964 7320 616e 2061  s it avoids an a
-00029030: 6464 6974 696f 6e61 6c20 6675 6e63 7469  dditional functi
-00029040: 6f6e 2063 616c 6c2e 220a 6578 616d 706c  on call.".exampl
-00029050: 6573 203d 2022 2222 0a2a 2a50 726f 626c  es = """.**Probl
-00029060: 656d 6174 6963 2063 6f64 652a 2a0a 0a60  ematic code**..`
-00029070: 6060 7079 0a65 6d70 7479 5f64 6963 7420  ``py.empty_dict 
-00029080: 3d20 6469 6374 2829 2020 2320 5b75 7365  = dict()  # [use
-00029090: 2d64 6963 742d 6c69 7465 7261 6c5d 0a6e  -dict-literal].n
-000290a0: 6577 5f64 6963 7420 3d20 6469 6374 2866  ew_dict = dict(f
-000290b0: 6f6f 3d5c 2262 6172 5c22 2920 2023 205b  oo=\"bar\")  # [
-000290c0: 7573 652d 6469 6374 2d6c 6974 6572 616c  use-dict-literal
-000290d0: 5d0a 6e65 775f 6469 6374 203d 2064 6963  ].new_dict = dic
-000290e0: 7428 2a2a 616e 6f74 6865 725f 6469 6374  t(**another_dict
-000290f0: 2920 2023 205b 7573 652d 6469 6374 2d6c  )  # [use-dict-l
-00029100: 6974 6572 616c 5d0a 0a60 6060 0a0a 2a2a  iteral]..```..**
-00029110: 486f 7720 746f 2066 6978 2069 742a 2a0a  How to fix it**.
-00029120: 0a60 6060 7079 0a65 6d70 7479 5f64 6963  .```py.empty_dic
-00029130: 7420 3d20 7b7d 0a0a 2320 6372 6561 7465  t = {}..# create
-00029140: 2075 7369 6e67 2061 206c 6974 6572 616c   using a literal
-00029150: 2064 6963 740a 6e65 775f 6469 6374 203d   dict.new_dict =
-00029160: 207b 5c22 666f 6f5c 223a 205c 2262 6172   {\"foo\": \"bar
-00029170: 5c22 7d0a 0a23 2073 6861 6c6c 6f77 2063  \"}..# shallow c
-00029180: 6f70 7920 6120 6469 6374 0a6e 6577 5f64  opy a dict.new_d
-00029190: 6963 7420 3d20 7b2a 2a61 6e6f 7468 6572  ict = {**another
-000291a0: 5f64 6963 747d 0a0a 6060 600a 0a3c 6120  _dict}..```..<a 
-000291b0: 6872 6566 3d5c 2268 7474 7073 3a2f 2f70  href=\"https://p
-000291c0: 796c 696e 742e 7079 6371 612e 6f72 672f  ylint.pycqa.org/
-000291d0: 656e 2f6c 6174 6573 742f 7573 6572 5f67  en/latest/user_g
-000291e0: 7569 6465 2f6d 6573 7361 6765 732f 7265  uide/messages/re
-000291f0: 6661 6374 6f72 2f75 7365 2d64 6963 742d  factor/use-dict-
-00029200: 6c69 7465 7261 6c2e 6874 6d6c 5c22 3e41  literal.html\">A
-00029210: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00029220: 6174 696f 6e3c 2f61 3e22 2222 0a0a 5b52  ation</a>"""..[R
-00029230: 3137 3336 5d0a 7768 7920 3d20 2249 7420  1736].why = "It 
-00029240: 6c6f 6f6b 7320 6c69 6b65 2069 7465 7261  looks like itera
-00029250: 7469 6e67 206f 7665 7220 616e 2065 6e75  ting over an enu
-00029260: 6d65 7261 7469 6f6e 2061 6e64 2061 6363  meration and acc
-00029270: 6573 7369 6e67 2074 6865 2076 616c 7565  essing the value
-00029280: 2062 7920 696e 6465 7820 6c6f 6f6b 7570   by index lookup
-00029290: 2e20 5468 6520 7661 6c75 6520 6361 6e20  . The value can 
-000292a0: 6265 2061 6363 6573 7365 6420 6469 7265  be accessed dire
-000292b0: 6374 6c79 2069 6e73 7465 6164 2e22 0a65  ctly instead.".e
-000292c0: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
-000292d0: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
-000292e0: 2a2a 0a0a 6060 6070 790a 6c65 7474 6572  **..```py.letter
-000292f0: 7320 3d20 5b27 6127 2c20 2762 272c 2027  s = ['a', 'b', '
-00029300: 6327 5d0a 0a66 6f72 2069 6e64 6578 2c20  c']..for index, 
-00029310: 6c65 7474 6572 2069 6e20 656e 756d 6572  letter in enumer
-00029320: 6174 6528 6c65 7474 6572 7329 3a0a 2020  ate(letters):.  
-00029330: 2020 7072 696e 7428 6c65 7474 6572 735b    print(letters[
-00029340: 696e 6465 785d 2920 2023 205b 756e 6e65  index])  # [unne
-00029350: 6365 7373 6172 792d 6c69 7374 2d69 6e64  cessary-list-ind
-00029360: 6578 2d6c 6f6f 6b75 705d 0a0a 6060 600a  ex-lookup]..```.
-00029370: 0a2a 2a48 6f77 2074 6f20 6669 7820 6974  .**How to fix it
-00029380: 2a2a 0a0a 6060 6070 790a 6c65 7474 6572  **..```py.letter
-00029390: 7320 3d20 5b27 6127 2c20 2762 272c 2027  s = ['a', 'b', '
-000293a0: 6327 5d0a 0a66 6f72 2069 6e64 6578 2c20  c']..for index, 
-000293b0: 6c65 7474 6572 2069 6e20 656e 756d 6572  letter in enumer
-000293c0: 6174 6528 6c65 7474 6572 7329 3a0a 2020  ate(letters):.  
-000293d0: 2020 7072 696e 7428 6c65 7474 6572 290a    print(letter).
-000293e0: 0a60 6060 0a22 2222 0a0a 5b52 3132 3630  .```."""..[R1260
-000293f0: 5d0a 7768 7920 3d20 2249 7420 6c6f 6f6b  ].why = "It look
-00029400: 7320 6c69 6b65 2074 6865 206d 6574 686f  s like the metho
-00029410: 6420 6f72 2066 756e 6374 696f 6e20 6973  d or function is
-00029420: 2074 6f6f 2063 6f6d 706c 6578 2062 6173   too complex bas
-00029430: 6564 206f 6e20 4d63 4361 6265 2043 6f6d  ed on McCabe Com
-00029440: 706c 6578 6974 7920 4379 636c 6f6d 6174  plexity Cyclomat
-00029450: 6963 220a 6578 616d 706c 6573 203d 2022  ic".examples = "
-00029460: 3c61 2068 7265 663d 5c22 6874 7470 733a  <a href=\"https:
-00029470: 2f2f 7079 6c69 6e74 2e70 7963 7161 2e6f  //pylint.pycqa.o
-00029480: 7267 2f65 6e2f 6c61 7465 7374 2f75 7365  rg/en/latest/use
-00029490: 725f 6775 6964 652f 6d65 7373 6167 6573  r_guide/messages
-000294a0: 2f72 6566 6163 746f 722f 746f 6f2d 636f  /refactor/too-co
-000294b0: 6d70 6c65 782e 6874 6d6c 5c22 3e41 6464  mplex.html\">Add
-000294c0: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-000294d0: 696f 6e3c 2f61 3e22 0a0a 5b52 3039 3031  ion</a>"..[R0901
-000294e0: 5d0a 7768 7920 3d20 2249 7420 6c6f 6f6b  ].why = "It look
-000294f0: 7320 6c69 6b65 2063 6c61 7373 2068 6173  s like class has
-00029500: 2074 6f6f 206d 616e 7920 7061 7265 6e74   too many parent
-00029510: 2063 6c61 7373 6573 2c20 7472 7920 746f   classes, try to
-00029520: 2072 6564 7563 6520 7468 6973 2074 6f20   reduce this to 
-00029530: 6765 7420 6120 7369 6d70 6c65 7220 2861  get a simpler (a
-00029540: 6e64 2073 6f20 6561 7369 6572 2074 6f20  nd so easier to 
-00029550: 7573 6529 2063 6c61 7373 2e22 0a65 7861  use) class.".exa
-00029560: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
-00029570: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
-00029580: 0a0a 6060 6070 790a 636c 6173 7320 416e  ..```py.class An
-00029590: 696d 616c 3a20 2e2e 2e0a 636c 6173 7320  imal: ....class 
-000295a0: 4265 616b 7941 6e69 6d61 6c28 416e 696d  BeakyAnimal(Anim
-000295b0: 616c 293a 202e 2e2e 0a63 6c61 7373 2046  al): ....class F
-000295c0: 7572 7279 416e 696d 616c 2841 6e69 6d61  urryAnimal(Anima
-000295d0: 6c29 3a20 2e2e 2e0a 636c 6173 7320 5377  l): ....class Sw
-000295e0: 696d 6d65 7228 416e 696d 616c 293a 202e  immer(Animal): .
-000295f0: 2e2e 0a63 6c61 7373 2045 6767 4c61 7965  ...class EggLaye
-00029600: 7228 416e 696d 616c 293a 202e 2e2e 0a63  r(Animal): ....c
-00029610: 6c61 7373 2056 656e 6f6d 6f75 7341 6e69  lass VenomousAni
-00029620: 6d61 6c28 416e 696d 616c 293a 202e 2e2e  mal(Animal): ...
-00029630: 0a63 6c61 7373 2050 726f 7465 6374 6564  .class Protected
-00029640: 5370 6563 6965 2841 6e69 6d61 6c29 3a20  Specie(Animal): 
-00029650: 2e2e 2e0a 636c 6173 7320 4265 6176 6572  ....class Beaver
-00029660: 5461 696c 6564 416e 696d 616c 2841 6e69  TailedAnimal(Ani
-00029670: 6d61 6c29 3a20 2e2e 2e0a 636c 6173 7320  mal): ....class 
-00029680: 5665 7274 6562 7261 7465 2841 6e69 6d61  Vertebrate(Anima
-00029690: 6c29 3a20 2e2e 2e0a 0a0a 2320 6d61 7820  l): ......# max 
-000296a0: 6f66 2037 2062 7920 6465 6661 756c 742c  of 7 by default,
-000296b0: 2063 616e 2062 6520 636f 6e66 6967 7572   can be configur
-000296c0: 6564 0a23 2065 6163 6820 6564 6765 206f  ed.# each edge o
-000296d0: 6620 6120 6469 616d 6f6e 6420 696e 6865  f a diamond inhe
-000296e0: 7269 7461 6e63 6520 636f 756e 7473 0a63  ritance counts.c
-000296f0: 6c61 7373 2050 6c61 7974 7970 7573 2820  lass Playtypus( 
-00029700: 2023 205b 746f 6f2d 6d61 6e79 2d61 6e63   # [too-many-anc
-00029710: 6573 746f 7273 5d0a 2020 2020 4265 616b  estors].    Beak
-00029720: 7941 6e69 6d61 6c2c 0a20 2020 2046 7572  yAnimal,.    Fur
-00029730: 7279 416e 696d 616c 2c0a 2020 2020 5377  ryAnimal,.    Sw
-00029740: 696d 6d65 722c 0a20 2020 2045 6767 4c61  immer,.    EggLa
-00029750: 7965 722c 0a20 2020 2056 656e 6f6d 6f75  yer,.    Venomou
-00029760: 7341 6e69 6d61 6c2c 0a20 2020 2050 726f  sAnimal,.    Pro
-00029770: 7465 6374 6564 5370 6563 6965 2c0a 2020  tectedSpecie,.  
-00029780: 2020 4265 6176 6572 5461 696c 6564 416e    BeaverTailedAn
-00029790: 696d 616c 2c0a 2020 2020 5665 7274 6562  imal,.    Verteb
-000297a0: 7261 7465 2c0a 293a 0a20 2020 2070 6173  rate,.):.    pas
-000297b0: 730a 0a60 6060 0a0a 2a2a 486f 7720 746f  s..```..**How to
-000297c0: 2066 6978 2069 742a 2a0a 0a60 6060 7079   fix it**..```py
-000297d0: 0a63 6c61 7373 2041 6e69 6d61 6c3a 0a20  .class Animal:. 
-000297e0: 2020 2062 6561 7665 725f 7461 696c 6564     beaver_tailed
-000297f0: 3a20 626f 6f6c 0a20 2020 2063 616e 5f73  : bool.    can_s
-00029800: 7769 6d3a 2062 6f6f 6c0a 2020 2020 6861  wim: bool.    ha
-00029810: 735f 6265 616b 3a20 626f 6f6c 0a20 2020  s_beak: bool.   
-00029820: 2068 6173 5f66 7572 3a20 626f 6f6c 0a20   has_fur: bool. 
-00029830: 2020 2068 6173 5f76 6572 7465 6272 6165     has_vertebrae
-00029840: 3a20 626f 6f6c 0a20 2020 206c 6179 735f  : bool.    lays_
-00029850: 6567 673a 2062 6f6f 6c0a 2020 2020 7072  egg: bool.    pr
-00029860: 6f74 6563 7465 645f 7370 6563 6965 3a20  otected_specie: 
-00029870: 626f 6f6c 0a20 2020 2076 656e 6f6d 6f75  bool.    venomou
-00029880: 733a 2062 6f6f 6c0a 0a0a 636c 6173 7320  s: bool...class 
-00029890: 496e 7665 7274 6562 7261 7465 2841 6e69  Invertebrate(Ani
-000298a0: 6d61 6c29 3a0a 2020 2020 6861 735f 7665  mal):.    has_ve
-000298b0: 7274 6562 7261 6520 3d20 4661 6c73 650a  rtebrae = False.
-000298c0: 0a0a 636c 6173 7320 5665 7274 6562 7261  ..class Vertebra
-000298d0: 7465 2841 6e69 6d61 6c29 3a0a 2020 2020  te(Animal):.    
-000298e0: 6861 735f 7665 7274 6562 7261 6520 3d20  has_vertebrae = 
-000298f0: 5472 7565 0a0a 0a63 6c61 7373 204d 616d  True...class Mam
-00029900: 6d61 6c28 5665 7274 6562 7261 7465 293a  mal(Vertebrate):
-00029910: 0a20 2020 2068 6173 5f62 6561 6b20 3d20  .    has_beak = 
-00029920: 4661 6c73 650a 2020 2020 6861 735f 6675  False.    has_fu
-00029930: 7220 3d20 5472 7565 0a20 2020 206c 6179  r = True.    lay
-00029940: 735f 6567 6720 3d20 4661 6c73 650a 2020  s_egg = False.  
-00029950: 2020 7665 6e6f 6d6f 7573 203d 2046 616c    venomous = Fal
-00029960: 7365 0a0a 0a63 6c61 7373 2050 6c61 7974  se...class Playt
-00029970: 7970 7573 284d 616d 6d61 6c29 3a0a 2020  ypus(Mammal):.  
-00029980: 2020 6265 6176 6572 5f74 6169 6c65 6420    beaver_tailed 
-00029990: 3d20 5472 7565 0a20 2020 2063 616e 5f73  = True.    can_s
-000299a0: 7769 6d20 3d20 5472 7565 0a20 2020 2068  wim = True.    h
-000299b0: 6173 5f62 6561 6b20 3d20 5472 7565 0a20  as_beak = True. 
-000299c0: 2020 206c 6179 735f 6567 6720 3d20 4661     lays_egg = Fa
-000299d0: 6c73 650a 2020 2020 7072 6f74 6563 7465  lse.    protecte
-000299e0: 645f 7370 6563 6965 203d 2054 7275 650a  d_specie = True.
-000299f0: 2020 2020 7665 6e6f 6d6f 7573 203d 2054      venomous = T
-00029a00: 7275 650a 0a60 6060 0a22 2222 0a0a 5b52  rue..```."""..[R
-00029a10: 3039 3032 5d0a 7768 7920 3d20 2249 7420  0902].why = "It 
-00029a20: 6c6f 6f6b 7320 6c69 6b65 2063 6c61 7373  looks like class
-00029a30: 2068 6173 2074 6f6f 206d 616e 7920 696e   has too many in
-00029a40: 7374 616e 6365 2061 7474 7269 6275 7465  stance attribute
-00029a50: 732c 2074 7279 2074 6f20 7265 6475 6365  s, try to reduce
-00029a60: 2074 6869 7320 746f 2067 6574 2061 2073   this to get a s
-00029a70: 696d 706c 6572 2028 616e 6420 736f 2065  impler (and so e
-00029a80: 6173 6965 7220 746f 2075 7365 2920 636c  asier to use) cl
-00029a90: 6173 732e 220a 6578 616d 706c 6573 203d  ass.".examples =
-00029aa0: 2022 2222 0a2a 2a50 726f 626c 656d 6174   """.**Problemat
-00029ab0: 6963 2063 6f64 652a 2a0a 0a60 6060 7079  ic code**..```py
-00029ac0: 0a63 6c61 7373 2046 7275 6974 3a20 2023  .class Fruit:  #
-00029ad0: 205b 746f 6f2d 6d61 6e79 2d69 6e73 7461   [too-many-insta
-00029ae0: 6e63 652d 6174 7472 6962 7574 6573 5d0a  nce-attributes].
-00029af0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00029b00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00029b10: 2320 6d61 7820 6f66 2037 2061 7474 7269  # max of 7 attri
-00029b20: 6275 7465 7320 6279 2064 6566 6175 6c74  butes by default
-00029b30: 2c20 6361 6e20 6265 2063 6f6e 6669 6775  , can be configu
-00029b40: 7265 640a 2020 2020 2020 2020 7365 6c66  red.        self
-00029b50: 2e77 6f72 6d5f 6e61 6d65 203d 205c 224a  .worm_name = \"J
-00029b60: 696d 6d79 5c22 0a20 2020 2020 2020 2073  immy\".        s
-00029b70: 656c 662e 776f 726d 5f74 7970 6520 3d20  elf.worm_type = 
-00029b80: 5c22 436f 646c 696e 6720 4d6f 7468 735c  \"Codling Moths\
-00029b90: 220a 2020 2020 2020 2020 7365 6c66 2e77  ".        self.w
-00029ba0: 6f72 6d5f 636f 6c6f 7220 3d20 5c22 6c69  orm_color = \"li
-00029bb0: 6768 7420 6272 6f77 6e5c 220a 2020 2020  ght brown\".    
-00029bc0: 2020 2020 7365 6c66 2e66 7275 6974 5f6e      self.fruit_n
-00029bd0: 616d 6520 3d20 5c22 4c69 7474 6c65 2041  ame = \"Little A
-00029be0: 7070 6c65 5c22 0a20 2020 2020 2020 2073  pple\".        s
-00029bf0: 656c 662e 6672 7569 745f 636f 6c6f 7220  elf.fruit_color 
-00029c00: 3d20 5c22 4272 6967 6874 2072 6564 5c22  = \"Bright red\"
-00029c10: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
-00029c20: 7569 745f 7669 7461 6d69 6e73 203d 205b  uit_vitamins = [
-00029c30: 5c22 415c 222c 205c 2242 315c 225d 0a20  \"A\", \"B1\"]. 
-00029c40: 2020 2020 2020 2073 656c 662e 6672 7569         self.frui
-00029c50: 745f 616e 7469 6f78 6964 616e 7473 203d  t_antioxidants =
-00029c60: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00029c70: 6c66 2e73 6563 6f6e 6461 7279 5f77 6f72  lf.secondary_wor
-00029c80: 6d5f 6e61 6d65 203d 205c 224b 696d 5c22  m_name = \"Kim\"
-00029c90: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00029ca0: 636f 6e64 6172 795f 776f 726d 5f74 7970  condary_worm_typ
-00029cb0: 6520 3d20 5c22 4170 706c 6520 6d61 6767  e = \"Apple magg
-00029cc0: 6f74 5c22 0a20 2020 2020 2020 2073 656c  ot\".        sel
-00029cd0: 662e 7365 636f 6e64 6172 795f 776f 726d  f.secondary_worm
-00029ce0: 5f63 6f6c 6f72 203d 205c 2257 6869 7469  _color = \"Whiti
-00029cf0: 7368 5c22 0a0a 6060 600a 0a2a 2a48 6f77  sh\"..```..**How
-00029d00: 2074 6f20 6669 7820 6974 2a2a 0a0a 6060   to fix it**..``
-00029d10: 6070 790a 696d 706f 7274 2064 6174 6163  `py.import datac
-00029d20: 6c61 7373 6573 0a0a 0a40 6461 7461 636c  lasses...@datacl
-00029d30: 6173 7365 732e 6461 7461 636c 6173 730a  asses.dataclass.
-00029d40: 636c 6173 7320 576f 726d 3a0a 2020 2020  class Worm:.    
-00029d50: 6e61 6d65 3a20 7374 720a 2020 2020 7479  name: str.    ty
-00029d60: 7065 3a20 7374 720a 2020 2020 636f 6c6f  pe: str.    colo
-00029d70: 723a 2073 7472 0a0a 0a63 6c61 7373 2046  r: str...class F
-00029d80: 7275 6974 3a0a 2020 2020 6465 6620 5f5f  ruit:.    def __
-00029d90: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-00029da0: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00029db0: 3d20 5c22 4c69 7474 6c65 2041 7070 6c65  = \"Little Apple
-00029dc0: 5c22 0a20 2020 2020 2020 2073 656c 662e  \".        self.
-00029dd0: 636f 6c6f 7220 3d20 5c22 4272 6967 6874  color = \"Bright
-00029de0: 2072 6564 5c22 0a20 2020 2020 2020 2073   red\".        s
-00029df0: 656c 662e 7669 7461 6d69 6e73 203d 205b  elf.vitamins = [
-00029e00: 5c22 415c 222c 205c 2242 315c 225d 0a20  \"A\", \"B1\"]. 
-00029e10: 2020 2020 2020 2073 656c 662e 616e 7469         self.anti
-00029e20: 6f78 6964 616e 7473 203d 204e 6f6e 650a  oxidants = None.
-00029e30: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-00029e40: 6d73 203d 205b 0a20 2020 2020 2020 2020  ms = [.         
-00029e50: 2020 2057 6f72 6d28 6e61 6d65 3d5c 224a     Worm(name=\"J
-00029e60: 696d 6d79 5c22 2c20 7479 7065 3d5c 2243  immy\", type=\"C
-00029e70: 6f64 6c69 6e67 204d 6f74 6873 5c22 2c20  odling Moths\", 
-00029e80: 636f 6c6f 723d 5c22 6c69 6768 7420 6272  color=\"light br
-00029e90: 6f77 6e5c 2229 2c0a 2020 2020 2020 2020  own\"),.        
-00029ea0: 2020 2020 576f 726d 286e 616d 653d 5c22      Worm(name=\"
-00029eb0: 4b69 6d5c 222c 2074 7970 653d 5c22 4170  Kim\", type=\"Ap
-00029ec0: 706c 6520 6d61 6767 6f74 5c22 2c20 636f  ple maggot\", co
-00029ed0: 6c6f 723d 5c22 5768 6974 6973 685c 2229  lor=\"Whitish\")
-00029ee0: 2c0a 2020 2020 2020 2020 5d0a 0a60 6060  ,.        ]..```
-00029ef0: 0a22 2222 0a0a 5b52 3039 3033 5d0a 7768  ."""..[R0903].wh
-00029f00: 7920 3d20 2249 7420 6c6f 6f6b 7320 6c69  y = "It looks li
-00029f10: 6b65 2063 6c61 7373 2068 6173 2074 6f6f  ke class has too
-00029f20: 2066 6577 2070 7562 6c69 6320 6d65 7468   few public meth
-00029f30: 6f64 732c 2073 6f20 6265 2073 7572 6520  ods, so be sure 
-00029f40: 6974 2773 2072 6561 6c6c 7920 776f 7274  it's really wort
-00029f50: 6820 6974 2e22 0a65 7861 6d70 6c65 7320  h it.".examples 
-00029f60: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-00029f70: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-00029f80: 790a 636c 6173 7320 576f 726d 3a20 2023  y.class Worm:  #
-00029f90: 205b 746f 6f2d 6665 772d 7075 626c 6963   [too-few-public
-00029fa0: 2d6d 6574 686f 6473 5d0a 2020 2020 6465  -methods].    de
-00029fb0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00029fc0: 206e 616d 653a 2073 7472 2c20 6672 7569   name: str, frui
-00029fd0: 745f 6f66 5f72 6573 6964 656e 6365 3a20  t_of_residence: 
-00029fe0: 4672 7569 7429 3a0a 2020 2020 2020 2020  Fruit):.        
-00029ff0: 7365 6c66 2e6e 616d 6520 3d20 6e61 6d65  self.name = name
-0002a000: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
-0002a010: 7569 745f 6f66 5f72 6573 6964 656e 6365  uit_of_residence
-0002a020: 203d 2066 7275 6974 5f6f 665f 7265 7369   = fruit_of_resi
-0002a030: 6465 6e63 650a 0a20 2020 2064 6566 2062  dence..    def b
-0002a040: 6f72 6528 7365 6c66 293a 0a20 2020 2020  ore(self):.     
-0002a050: 2020 2070 7269 6e74 2866 5c22 7b73 656c     print(f\"{sel
-0002a060: 662e 6e61 6d65 7d20 6973 2062 6f72 696e  f.name} is borin
-0002a070: 6720 696e 746f 207b 7365 6c66 2e66 7275  g into {self.fru
-0002a080: 6974 5f6f 665f 7265 7369 6465 6e63 657d  it_of_residence}
-0002a090: 5c22 290a 0a60 6060 0a0a 2a2a 486f 7720  \")..```..**How 
-0002a0a0: 746f 2066 6978 2069 742a 2a0a 0a60 6060  to fix it**..```
-0002a0b0: 7079 0a69 6d70 6f72 7420 6461 7461 636c  py.import datacl
-0002a0c0: 6173 7365 730a 0a0a 636c 6173 7320 576f  asses...class Wo
-0002a0d0: 726d 3a0a 2020 2020 6465 6620 5f5f 696e  rm:.    def __in
-0002a0e0: 6974 5f5f 2873 656c 662c 206e 616d 653a  it__(self, name:
-0002a0f0: 2073 7472 2c20 6672 7569 745f 6f66 5f72   str, fruit_of_r
-0002a100: 6573 6964 656e 6365 3a20 4672 7569 7429  esidence: Fruit)
-0002a110: 3a0a 2020 2020 2020 2020 7365 6c66 2e6e  :.        self.n
-0002a120: 616d 6520 3d20 6e61 6d65 0a20 2020 2020  ame = name.     
-0002a130: 2020 2073 656c 662e 6672 7569 745f 6f66     self.fruit_of
-0002a140: 5f72 6573 6964 656e 6365 203d 2066 7275  _residence = fru
-0002a150: 6974 5f6f 665f 7265 7369 6465 6e63 650a  it_of_residence.
-0002a160: 0a20 2020 2064 6566 2062 6f72 6528 7365  .    def bore(se
-0002a170: 6c66 293a 0a20 2020 2020 2020 2070 7269  lf):.        pri
-0002a180: 6e74 2866 5c22 7b73 656c 662e 6e61 6d65  nt(f\"{self.name
-0002a190: 7d20 6973 2062 6f72 696e 6720 696e 746f  } is boring into
-0002a1a0: 207b 7365 6c66 2e66 7275 6974 5f6f 665f   {self.fruit_of_
-0002a1b0: 7265 7369 6465 6e63 657d 5c22 290a 0a20  residence}\").. 
-0002a1c0: 2020 2064 6566 2077 6967 676c 6528 7365     def wiggle(se
-0002a1d0: 6c66 293a 0a20 2020 2020 2020 2070 7269  lf):.        pri
-0002a1e0: 6e74 2866 5c22 7b73 656c 662e 6e61 6d65  nt(f\"{self.name
-0002a1f0: 7d20 7769 6767 6c65 2061 726f 756e 6420  } wiggle around 
-0002a200: 776f 726d 696c 792e 5c22 290a 0a23 206f  wormily.\")..# o
-0002a210: 720a 0a40 6461 7461 636c 6173 7365 732e  r..@dataclasses.
-0002a220: 6461 7461 636c 6173 730a 636c 6173 7320  dataclass.class 
-0002a230: 576f 726d 3a0a 2020 2020 6e61 6d65 3a73  Worm:.    name:s
-0002a240: 7472 0a20 2020 2066 7275 6974 5f6f 665f  tr.    fruit_of_
-0002a250: 7265 7369 6465 6e63 653a 2046 7275 6974  residence: Fruit
-0002a260: 0a0a 6465 6620 626f 7265 2877 6f72 6d3a  ..def bore(worm:
-0002a270: 2057 6f72 6d29 3a0a 2020 2020 7072 696e   Worm):.    prin
-0002a280: 7428 665c 227b 776f 726d 2e6e 616d 657d  t(f\"{worm.name}
-0002a290: 2069 7320 626f 7269 6e67 2069 6e74 6f20   is boring into 
-0002a2a0: 7b77 6f72 6d2e 6672 7569 745f 6f66 5f72  {worm.fruit_of_r
-0002a2b0: 6573 6964 656e 6365 7d5c 2229 0a0a 2320  esidence}\")..# 
-0002a2c0: 6f72 0a0a 6465 6620 626f 7265 2866 7275  or..def bore(fru
-0002a2d0: 6974 3a20 4672 7569 742c 2077 6f72 6d5f  it: Fruit, worm_
-0002a2e0: 6e61 6d65 3a20 7374 7229 3a0a 2020 2020  name: str):.    
-0002a2f0: 7072 696e 7428 665c 227b 776f 726d 5f6e  print(f\"{worm_n
-0002a300: 616d 657d 2069 7320 626f 7269 6e67 2069  ame} is boring i
-0002a310: 6e74 6f20 7b66 7275 6974 7d5c 2229 0a0a  nto {fruit}\")..
-0002a320: 6060 600a 2222 220a 0a5b 5230 3930 345d  ```."""..[R0904]
-0002a330: 0a77 6879 203d 2022 4974 206c 6f6f 6b73  .why = "It looks
-0002a340: 206c 696b 6520 636c 6173 7320 6861 7320   like class has 
-0002a350: 746f 6f20 6d61 6e79 2070 7562 6c69 6320  too many public 
-0002a360: 6d65 7468 6f64 732c 2074 7279 2074 6f20  methods, try to 
-0002a370: 7265 6475 6365 2074 6869 7320 746f 2067  reduce this to g
-0002a380: 6574 2061 2073 696d 706c 6572 2028 616e  et a simpler (an
-0002a390: 6420 736f 2065 6173 6965 7220 746f 2075  d so easier to u
-0002a3a0: 7365 2920 636c 6173 732e 220a 6578 616d  se) class.".exam
-0002a3b0: 706c 6573 203d 2022 3c61 2068 7265 663d  ples = "<a href=
-0002a3c0: 5c22 6874 7470 733a 2f2f 7079 6c69 6e74  \"https://pylint
-0002a3d0: 2e70 7963 7161 2e6f 7267 2f65 6e2f 6c61  .pycqa.org/en/la
-0002a3e0: 7465 7374 2f75 7365 725f 6775 6964 652f  test/user_guide/
-0002a3f0: 6d65 7373 6167 6573 2f72 6566 6163 746f  messages/refacto
-0002a400: 722f 746f 6f2d 6d61 6e79 2d70 7562 6c69  r/too-many-publi
-0002a410: 632d 6d65 7468 6f64 732e 6874 6d6c 5c22  c-methods.html\"
-0002a420: 3e41 6464 6974 696f 6e61 6c20 696e 666f  >Additional info
-0002a430: 726d 6174 696f 6e3c 2f61 3e22 0a0a 5b52  rmation</a>"..[R
-0002a440: 3039 3131 5d0a 7768 7920 3d20 2249 7420  0911].why = "It 
-0002a450: 6c6f 6f6b 7320 6c69 6b65 2074 6865 2066  looks like the f
-0002a460: 756e 6374 696f 6e20 6f72 206d 6574 686f  unction or metho
-0002a470: 6420 6861 7320 746f 6f20 6d61 6e79 2072  d has too many r
-0002a480: 6574 7572 6e20 7374 6174 656d 656e 742c  eturn statement,
-0002a490: 206d 616b 696e 6720 6974 2068 6172 6420   making it hard 
-0002a4a0: 746f 2066 6f6c 6c6f 772e 220a 6578 616d  to follow.".exam
-0002a4b0: 706c 6573 203d 2022 2222 0a2a 2a50 726f  ples = """.**Pro
-0002a4c0: 626c 656d 6174 6963 2063 6f64 652a 2a0a  blematic code**.
-0002a4d0: 0a60 6060 7079 0a64 6566 2074 6f5f 7374  .```py.def to_st
-0002a4e0: 7269 6e67 2878 293a 2020 2320 5b74 6f6f  ring(x):  # [too
-0002a4f0: 2d6d 616e 792d 7265 7475 726e 2d73 7461  -many-return-sta
-0002a500: 7465 6d65 6e74 735d 0a20 2020 2023 206d  tements].    # m
-0002a510: 6178 206f 6620 3620 6279 2064 6566 6175  ax of 6 by defau
-0002a520: 6c74 2c20 6361 6e20 6265 2063 6f6e 6669  lt, can be confi
-0002a530: 6775 7265 640a 2020 2020 6966 2078 203d  gured.    if x =
-0002a540: 3d20 313a 0a20 2020 2020 2020 2072 6574  = 1:.        ret
-0002a550: 7572 6e20 2754 6869 7320 6973 206f 6e65  urn 'This is one
-0002a560: 2e27 0a20 2020 2069 6620 7820 3d3d 2032  .'.    if x == 2
-0002a570: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0002a580: 2027 5468 6973 2069 7320 7477 6f2e 270a   'This is two.'.
-0002a590: 2020 2020 6966 2078 203d 3d20 333a 0a20      if x == 3:. 
-0002a5a0: 2020 2020 2020 2072 6574 7572 6e20 2754         return 'T
-0002a5b0: 6869 7320 6973 2074 6872 6565 2e27 0a20  his is three.'. 
-0002a5c0: 2020 2069 6620 7820 3d3d 2034 3a0a 2020     if x == 4:.  
-0002a5d0: 2020 2020 2020 7265 7475 726e 2027 5468        return 'Th
-0002a5e0: 6973 2069 7320 666f 7572 2e27 0a20 2020  is is four.'.   
-0002a5f0: 2069 6620 7820 3d3d 2035 3a0a 2020 2020   if x == 5:.    
-0002a600: 2020 2020 7265 7475 726e 2027 5468 6973      return 'This
-0002a610: 2069 7320 6669 7665 2e27 0a20 2020 2069   is five.'.    i
-0002a620: 6620 7820 3d3d 2036 3a0a 2020 2020 2020  f x == 6:.      
-0002a630: 2020 7265 7475 726e 2027 5468 6973 2069    return 'This i
-0002a640: 7320 7369 782e 270a 2020 2020 6966 2078  s six.'.    if x
-0002a650: 203d 3d20 373a 0a20 2020 2020 2020 2072   == 7:.        r
-0002a660: 6574 7572 6e20 2754 6869 7320 6973 2073  eturn 'This is s
-0002a670: 6576 656e 2e27 0a0a 6060 600a 0a2a 2a48  even.'..```..**H
-0002a680: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
-0002a690: 6060 6070 790a 4e55 4d42 4552 535f 544f  ```py.NUMBERS_TO
-0002a6a0: 5f53 5452 494e 4753 203d 207b 0a20 2020  _STRINGS = {.   
-0002a6b0: 2031 3a20 276f 6e65 272c 0a20 2020 2032   1: 'one',.    2
-0002a6c0: 3a20 2774 776f 272c 0a20 2020 2033 3a20  : 'two',.    3: 
-0002a6d0: 2774 6872 6565 272c 0a20 2020 2034 3a20  'three',.    4: 
-0002a6e0: 2766 6f75 7227 2c0a 2020 2020 353a 2027  'four',.    5: '
-0002a6f0: 6669 7665 272c 0a20 2020 2036 3a20 2773  five',.    6: 's
-0002a700: 6978 272c 0a20 2020 2037 3a20 2773 6576  ix',.    7: 'sev
-0002a710: 656e 270a 7d0a 0a0a 6465 6620 746f 5f73  en'.}...def to_s
-0002a720: 7472 696e 6728 7829 3a0a 2020 2020 7265  tring(x):.    re
-0002a730: 7475 726e 2066 2754 6869 7320 6973 207b  turn f'This is {
-0002a740: 4e55 4d42 4552 535f 544f 5f53 5452 494e  NUMBERS_TO_STRIN
-0002a750: 4753 2e67 6574 2878 297d 2e27 0a0a 6060  GS.get(x)}.'..``
-0002a760: 600a 2222 220a 0a5b 5230 3931 325d 0a77  `."""..[R0912].w
-0002a770: 6879 203d 2022 4974 206c 6f6f 6b73 206c  hy = "It looks l
-0002a780: 696b 6520 7468 6520 6675 6e63 7469 6f6e  ike the function
-0002a790: 206f 7220 6d65 7468 6f64 2068 6173 2074   or method has t
-0002a7a0: 6f6f 206d 616e 7920 6272 616e 6368 6573  oo many branches
-0002a7b0: 2c20 6d61 6b69 6e67 2069 7420 6861 7264  , making it hard
-0002a7c0: 2074 6f20 666f 6c6c 6f77 2e22 0a65 7861   to follow.".exa
-0002a7d0: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
-0002a7e0: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
-0002a7f0: 0a0a 6060 6070 790a 6465 6620 6e75 6d5f  ..```py.def num_
-0002a800: 746f 5f77 6f72 6428 7829 3a20 2023 205b  to_word(x):  # [
-0002a810: 746f 6f2d 6d61 6e79 2d62 7261 6e63 6865  too-many-branche
-0002a820: 735d 0a20 2020 2069 6620 7820 3d3d 2030  s].    if x == 0
-0002a830: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0002a840: 205c 227a 6572 6f5c 220a 2020 2020 656c   \"zero\".    el
-0002a850: 6966 2078 203d 3d20 313a 0a20 2020 2020  if x == 1:.     
-0002a860: 2020 2072 6574 7572 6e20 5c22 6f6e 655c     return \"one\
-0002a870: 220a 2020 2020 656c 6966 2078 203d 3d20  ".    elif x == 
-0002a880: 323a 0a20 2020 2020 2020 2072 6574 7572  2:.        retur
-0002a890: 6e20 5c22 7477 6f5c 220a 2020 2020 656c  n \"two\".    el
-0002a8a0: 6966 2078 203d 3d20 333a 0a20 2020 2020  if x == 3:.     
-0002a8b0: 2020 2072 6574 7572 6e20 5c22 7468 7265     return \"thre
-0002a8c0: 655c 220a 2020 2020 656c 6966 2078 203d  e\".    elif x =
-0002a8d0: 3d20 343a 0a20 2020 2020 2020 2072 6574  = 4:.        ret
-0002a8e0: 7572 6e20 5c22 666f 7572 5c22 0a20 2020  urn \"four\".   
-0002a8f0: 2065 6c69 6620 7820 3d3d 2035 3a0a 2020   elif x == 5:.  
-0002a900: 2020 2020 2020 7265 7475 726e 205c 2266        return \"f
-0002a910: 6976 655c 220a 2020 2020 656c 6966 2078  ive\".    elif x
-0002a920: 203d 3d20 363a 0a20 2020 2020 2020 2072   == 6:.        r
-0002a930: 6574 7572 6e20 5c22 7369 785c 220a 2020  eturn \"six\".  
-0002a940: 2020 656c 6966 2078 203d 3d20 373a 0a20    elif x == 7:. 
-0002a950: 2020 2020 2020 2072 6574 7572 6e20 5c22         return \"
-0002a960: 7365 7665 6e5c 220a 2020 2020 656c 6966  seven\".    elif
-0002a970: 2078 203d 3d20 383a 0a20 2020 2020 2020   x == 8:.       
-0002a980: 2072 6574 7572 6e20 5c22 6569 6768 745c   return \"eight\
-0002a990: 220a 2020 2020 656c 6966 2078 203d 3d20  ".    elif x == 
-0002a9a0: 393a 0a20 2020 2020 2020 2072 6574 7572  9:.        retur
-0002a9b0: 6e20 5c22 6e69 6e65 5c22 0a20 2020 2065  n \"nine\".    e
-0002a9c0: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
-0002a9d0: 7572 6e20 4e6f 6e65 0a0a 6060 600a 0a2a  urn None..```..*
-0002a9e0: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
-0002a9f0: 0a0a 6060 6070 790a 6465 6620 6e75 6d5f  ..```py.def num_
-0002aa00: 746f 5f77 6f72 6428 7829 3a0a 2020 2020  to_word(x):.    
-0002aa10: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-0002aa20: 2030 3a20 5c22 7a65 726f 5c22 2c0a 2020   0: \"zero\",.  
-0002aa30: 2020 2020 2020 313a 205c 226f 6e65 5c22        1: \"one\"
-0002aa40: 2c0a 2020 2020 2020 2020 323a 205c 2274  ,.        2: \"t
-0002aa50: 776f 5c22 2c0a 2020 2020 2020 2020 333a  wo\",.        3:
-0002aa60: 205c 2274 6872 6565 5c22 2c0a 2020 2020   \"three\",.    
-0002aa70: 2020 2020 343a 205c 2266 6f72 5c22 2c0a      4: \"for\",.
-0002aa80: 2020 2020 2020 2020 353a 205c 2266 6965          5: \"fie
-0002aa90: 5c22 2c0a 2020 2020 2020 2020 363a 205c  \",.        6: \
-0002aaa0: 2273 6978 5c22 2c0a 2020 2020 2020 2020  "six\",.        
-0002aab0: 373a 205c 2273 6576 656e 5c22 2c0a 2020  7: \"seven\",.  
-0002aac0: 2020 2020 2020 383a 205c 2265 6967 6874        8: \"eight
-0002aad0: 5c22 2c0a 2020 2020 2020 2020 393a 205c  \",.        9: \
-0002aae0: 226e 696e 655c 222c 0a20 2020 207d 2e67  "nine\",.    }.g
-0002aaf0: 6574 2878 290a 0a60 6060 0a22 2222 0a0a  et(x)..```."""..
-0002ab00: 5b52 3039 3133 5d0a 7768 7920 3d20 2249  [R0913].why = "I
-0002ab10: 7420 6c6f 6f6b 7320 6c69 6b65 2074 6865  t looks like the
-0002ab20: 2066 756e 6374 696f 6e20 6f72 206d 6574   function or met
-0002ab30: 686f 6420 7461 6b65 7320 746f 6f20 6d61  hod takes too ma
-0002ab40: 6e79 2061 7267 756d 656e 7473 2e22 0a65  ny arguments.".e
-0002ab50: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
-0002ab60: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
-0002ab70: 2a2a 0a0a 6060 6070 790a 6465 6620 7468  **..```py.def th
-0002ab80: 7265 655f 645f 6368 6573 735f 6d6f 7665  ree_d_chess_move
-0002ab90: 2820 2023 205b 746f 6f2d 6d61 6e79 2d61  (  # [too-many-a
-0002aba0: 7267 756d 656e 7473 5d0a 2020 2020 785f  rguments].    x_
-0002abb0: 7768 6974 652c 0a20 2020 2079 5f77 6869  white,.    y_whi
-0002abc0: 7465 2c0a 2020 2020 7a5f 7768 6974 652c  te,.    z_white,
-0002abd0: 0a20 2020 2070 6965 6365 5f77 6869 7465  .    piece_white
-0002abe0: 2c0a 2020 2020 785f 626c 6163 6b2c 0a20  ,.    x_black,. 
-0002abf0: 2020 2079 5f62 6c61 636b 2c0a 2020 2020     y_black,.    
-0002ac00: 7a5f 626c 6163 6b2c 0a20 2020 2070 6965  z_black,.    pie
-0002ac10: 6365 5f62 6c61 636b 2c0a 2020 2020 785f  ce_black,.    x_
-0002ac20: 626c 7565 2c0a 2020 2020 795f 626c 7565  blue,.    y_blue
-0002ac30: 2c0a 2020 2020 7a5f 626c 7565 2c0a 2020  ,.    z_blue,.  
-0002ac40: 2020 7069 6563 655f 626c 7565 2c0a 2020    piece_blue,.  
-0002ac50: 2020 6375 7272 656e 745f 706c 6179 6572    current_player
-0002ac60: 2c0a 293a 0a20 2020 2070 6173 730a 0a60  ,.):.    pass..`
-0002ac70: 6060 0a0a 2a2a 486f 7720 746f 2066 6978  ``..**How to fix
-0002ac80: 2069 742a 2a0a 0a60 6060 7079 0a66 726f   it**..```py.fro
-0002ac90: 6d20 6461 7461 636c 6173 7365 7320 696d  m dataclasses im
-0002aca0: 706f 7274 2064 6174 6163 6c61 7373 0a0a  port dataclass..
-0002acb0: 0a40 6461 7461 636c 6173 730a 636c 6173  .@dataclass.clas
-0002acc0: 7320 5468 7265 6544 4368 6573 7350 6965  s ThreeDChessPie
-0002acd0: 6365 3a0a 2020 2020 783a 2069 6e74 0a20  ce:.    x: int. 
-0002ace0: 2020 2079 3a20 696e 740a 2020 2020 7a3a     y: int.    z:
-0002acf0: 2069 6e74 0a20 2020 2074 7970 653a 2073   int.    type: s
-0002ad00: 7472 0a0a 0a64 6566 2074 6872 6565 5f64  tr...def three_d
-0002ad10: 5f63 6865 7373 5f6d 6f76 6528 0a20 2020  _chess_move(.   
-0002ad20: 2077 6869 7465 3a20 5468 7265 6544 4368   white: ThreeDCh
-0002ad30: 6573 7350 6965 6365 2c0a 2020 2020 626c  essPiece,.    bl
-0002ad40: 6163 6b3a 2054 6872 6565 4443 6865 7373  ack: ThreeDChess
-0002ad50: 5069 6563 652c 0a20 2020 2062 6c75 653a  Piece,.    blue:
-0002ad60: 2054 6872 6565 4443 6865 7373 5069 6563   ThreeDChessPiec
-0002ad70: 652c 0a20 2020 2063 7572 7265 6e74 5f70  e,.    current_p
-0002ad80: 6c61 7965 722c 0a29 3a0a 2020 2020 7061  layer,.):.    pa
-0002ad90: 7373 0a0a 6060 600a 2222 220a 0a5b 5230  ss..```."""..[R0
-0002ada0: 3931 345d 0a77 6879 203d 2022 4974 206c  914].why = "It l
-0002adb0: 6f6f 6b73 206c 696b 6520 7468 6520 6675  ooks like the fu
-0002adc0: 6e63 7469 6f6e 206f 7220 6d65 7468 6f64  nction or method
-0002add0: 2068 6173 2074 6f6f 206d 616e 7920 6c6f   has too many lo
-0002ade0: 6361 6c20 7661 7269 6162 6c65 732e 220a  cal variables.".
-0002adf0: 6578 616d 706c 6573 203d 2022 3c61 2068  examples = "<a h
-0002ae00: 7265 663d 5c22 6874 7470 733a 2f2f 7079  ref=\"https://py
-0002ae10: 6c69 6e74 2e70 7963 7161 2e6f 7267 2f65  lint.pycqa.org/e
-0002ae20: 6e2f 6c61 7465 7374 2f75 7365 725f 6775  n/latest/user_gu
-0002ae30: 6964 652f 6d65 7373 6167 6573 2f72 6566  ide/messages/ref
-0002ae40: 6163 746f 722f 746f 6f2d 6d61 6e79 2d6c  actor/too-many-l
-0002ae50: 6f63 616c 732e 6874 6d6c 5c22 3e41 6464  ocals.html\">Add
-0002ae60: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-0002ae70: 696f 6e3c 2f61 3e22 0a0a 5b52 3039 3135  ion</a>"..[R0915
-0002ae80: 5d0a 7768 7920 3d20 2249 7420 6c6f 6f6b  ].why = "It look
-0002ae90: 7320 6c69 6b65 2074 6865 2066 756e 6374  s like the funct
-0002aea0: 696f 6e20 6f72 206d 6574 686f 6420 6861  ion or method ha
-0002aeb0: 7320 746f 6f20 6d61 6e79 2073 7461 7465  s too many state
-0002aec0: 6d65 6e74 732e 2059 6f75 2073 686f 756c  ments. You shoul
-0002aed0: 6420 7468 656e 2073 706c 6974 2069 7420  d then split it 
-0002aee0: 696e 2073 6d61 6c6c 6572 2066 756e 6374  in smaller funct
-0002aef0: 696f 6e73 202f 206d 6574 686f 6473 2e22  ions / methods."
-0002af00: 0a65 7861 6d70 6c65 7320 3d20 223c 6120  .examples = "<a 
-0002af10: 6872 6566 3d5c 2268 7474 7073 3a2f 2f70  href=\"https://p
-0002af20: 796c 696e 742e 7079 6371 612e 6f72 672f  ylint.pycqa.org/
-0002af30: 656e 2f6c 6174 6573 742f 7573 6572 5f67  en/latest/user_g
-0002af40: 7569 6465 2f6d 6573 7361 6765 732f 7265  uide/messages/re
-0002af50: 6661 6374 6f72 2f74 6f6f 2d6d 616e 792d  factor/too-many-
-0002af60: 7374 6174 656d 656e 7473 2e68 746d 6c5c  statements.html\
-0002af70: 223e 4164 6469 7469 6f6e 616c 2069 6e66  ">Additional inf
-0002af80: 6f72 6d61 7469 6f6e 3c2f 613e 220a 0a5b  ormation</a>"..[
-0002af90: 5230 3931 365d 0a77 6879 203d 2022 436f  R0916].why = "Co
-0002afa0: 6e73 6964 6572 2073 696d 706c 6966 7969  nsider simplifyi
-0002afb0: 6e67 2074 6865 2065 7870 7265 7373 696f  ng the expressio
-0002afc0: 6e20 7769 7468 2068 656c 7065 7220 7661  n with helper va
-0002afd0: 7269 6162 6c65 7320 6f72 2066 756e 6374  riables or funct
-0002afe0: 696f 6e73 2e22 0a65 7861 6d70 6c65 7320  ions.".examples 
-0002aff0: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-0002b000: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-0002b010: 790a 6465 6620 6361 6e5f 6265 5f64 6976  y.def can_be_div
-0002b020: 6964 6564 5f62 795f 7477 6f5f 616e 645f  ided_by_two_and_
-0002b030: 6172 655f 6e6f 745f 7a65 726f 2878 2c20  are_not_zero(x, 
-0002b040: 792c 207a 293a 0a20 2020 2023 204d 6178  y, z):.    # Max
-0002b050: 696d 756d 206e 756d 6265 7220 6f66 2062  imum number of b
-0002b060: 6f6f 6c65 616e 2065 7870 7265 7373 696f  oolean expressio
-0002b070: 6e73 2069 6e20 616e 2069 6620 7374 6174  ns in an if stat
-0002b080: 656d 656e 7420 2862 7920 6465 6661 756c  ement (by defaul
-0002b090: 7420 3529 0a20 2020 2023 202b 313a 205b  t 5).    # +1: [
-0002b0a0: 746f 6f2d 6d61 6e79 2d62 6f6f 6c65 616e  too-many-boolean
-0002b0b0: 2d65 7870 7265 7373 696f 6e73 5d0a 2020  -expressions].  
-0002b0c0: 2020 6966 2028 7820 616e 6420 7920 616e    if (x and y an
-0002b0d0: 6420 7a29 2061 6e64 2028 7820 2520 3220  d z) and (x % 2 
-0002b0e0: 3d3d 2030 2061 6e64 2079 2025 2032 203d  == 0 and y % 2 =
-0002b0f0: 3d20 3020 616e 6420 7a20 2520 3220 3d3d  = 0 and z % 2 ==
-0002b100: 2030 293a 0a20 2020 2020 2020 2070 6173   0):.        pas
-0002b110: 730a 0a60 6060 0a0a 2a2a 486f 7720 746f  s..```..**How to
-0002b120: 2066 6978 2069 742a 2a0a 0a60 6060 7079   fix it**..```py
-0002b130: 0a64 6566 2063 616e 5f62 655f 6469 7669  .def can_be_divi
-0002b140: 6465 645f 6279 5f74 776f 5f61 6e64 5f61  ded_by_two_and_a
-0002b150: 7265 5f6e 6f74 5f7a 6572 6f28 782c 2079  re_not_zero(x, y
-0002b160: 2c20 7a29 3a0a 2020 2020 6966 2061 6c6c  , z):.    if all
-0002b170: 2869 2061 6e64 2069 2532 3d3d 3020 666f  (i and i%2==0 fo
-0002b180: 7220 6920 696e 205b 782c 2079 2c20 7a5d  r i in [x, y, z]
-0002b190: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0002b1a0: 0a60 6060 0a22 2222 0a0a 5b52 3038 3031  .```."""..[R0801
-0002b1b0: 5d0a 7768 7920 3d20 2249 6e64 6963 6174  ].why = "Indicat
-0002b1c0: 6573 2074 6861 7420 6120 7365 7420 6f66  es that a set of
-0002b1d0: 2073 696d 696c 6172 206c 696e 6573 2068   similar lines h
-0002b1e0: 6173 2062 6565 6e20 6465 7465 6374 6564  as been detected
-0002b1f0: 2061 6d6f 6e67 206d 756c 7469 706c 6520   among multiple 
-0002b200: 6669 6c65 2e20 5468 6973 2075 7375 616c  file. This usual
-0002b210: 6c79 206d 6561 6e73 2074 6861 7420 7468  ly means that th
-0002b220: 6520 636f 6465 2073 686f 756c 6420 6265  e code should be
-0002b230: 2072 6566 6163 746f 7265 6420 746f 2061   refactored to a
-0002b240: 766f 6964 2074 6869 7320 6475 706c 6963  void this duplic
-0002b250: 6174 696f 6e2e 220a 6578 616d 706c 6573  ation.".examples
-0002b260: 203d 2022 3c61 2068 7265 663d 5c22 6874   = "<a href=\"ht
-0002b270: 7470 733a 2f2f 7079 6c69 6e74 2e70 7963  tps://pylint.pyc
-0002b280: 7161 2e6f 7267 2f65 6e2f 6c61 7465 7374  qa.org/en/latest
-0002b290: 2f75 7365 725f 6775 6964 652f 6d65 7373  /user_guide/mess
-0002b2a0: 6167 6573 2f72 6566 6163 746f 722f 6475  ages/refactor/du
-0002b2b0: 706c 6963 6174 652d 636f 6465 2e68 746d  plicate-code.htm
-0002b2c0: 6c5c 223e 4164 6469 7469 6f6e 616c 2069  l\">Additional i
-0002b2d0: 6e66 6f72 6d61 7469 6f6e 3c2f 613e 220a  nformation</a>".
-0002b2e0: 0a5b 5236 3030 325d 0a77 6879 203d 2022  .[R6002].why = "
-0002b2f0: 4f6e 6c79 2065 6d69 7474 6564 2069 6620  Only emitted if 
-0002b300: 2772 756e 7469 6d65 2d74 7970 696e 673d  'runtime-typing=
-0002b310: 6e6f 2720 616e 6420 6120 6465 7072 6563  no' and a deprec
-0002b320: 6174 6564 2074 7970 696e 6720 616c 6961  ated typing alia
-0002b330: 7320 6973 2075 7365 6420 696e 2061 2074  s is used in a t
-0002b340: 7970 6520 616e 6e6f 7461 7469 6f6e 2063  ype annotation c
-0002b350: 6f6e 7465 7874 2069 6e20 5079 7468 6f6e  ontext in Python
-0002b360: 2033 2e37 206f 7220 332e 382e 220a 6578   3.7 or 3.8.".ex
-0002b370: 616d 706c 6573 203d 2022 3c61 2068 7265  amples = "<a hre
-0002b380: 663d 5c22 6874 7470 733a 2f2f 7079 6c69  f=\"https://pyli
-0002b390: 6e74 2e70 7963 7161 2e6f 7267 2f65 6e2f  nt.pycqa.org/en/
-0002b3a0: 6c61 7465 7374 2f75 7365 725f 6775 6964  latest/user_guid
-0002b3b0: 652f 6d65 7373 6167 6573 2f72 6566 6163  e/messages/refac
-0002b3c0: 746f 722f 636f 6e73 6964 6572 2d75 7369  tor/consider-usi
-0002b3d0: 6e67 2d61 6c69 6173 2e68 746d 6c5c 223e  ng-alias.html\">
-0002b3e0: 4164 6469 7469 6f6e 616c 2069 6e66 6f72  Additional infor
-0002b3f0: 6d61 7469 6f6e 3c2f 613e 220a 0a5b 5236  mation</a>"..[R6
-0002b400: 3030 335d 0a77 6879 203d 2022 4974 206c  003].why = "It l
-0002b410: 6f6f 6b73 206c 696b 6520 2774 7970 696e  ooks like 'typin
-0002b420: 672e 556e 696f 6e27 206f 7220 2774 7970  g.Union' or 'typ
-0002b430: 696e 672e 4f70 7469 6f6e 616c 2720 6973  ing.Optional' is
-0002b440: 2075 7365 6420 696e 7374 6561 6420 6f66   used instead of
-0002b450: 2074 6865 2061 6c74 6572 6e61 7469 7665   the alternative
-0002b460: 2055 6e69 6f6e 2073 796e 7461 7820 2769   Union syntax 'i
-0002b470: 6e74 207c 204e 6f6e 6527 2e22 0a65 7861  nt | None'.".exa
-0002b480: 6d70 6c65 7320 3d20 223c 6120 6872 6566  mples = "<a href
-0002b490: 3d5c 2268 7474 7073 3a2f 2f70 796c 696e  =\"https://pylin
-0002b4a0: 742e 7079 6371 612e 6f72 672f 656e 2f6c  t.pycqa.org/en/l
-0002b4b0: 6174 6573 742f 7573 6572 5f67 7569 6465  atest/user_guide
-0002b4c0: 2f6d 6573 7361 6765 732f 7265 6661 6374  /messages/refact
-0002b4d0: 6f72 2f63 6f6e 7369 6465 722d 616c 7465  or/consider-alte
-0002b4e0: 726e 6174 6976 652d 756e 696f 6e2d 7379  rnative-union-sy
-0002b4f0: 6e74 6178 2e68 746d 6c5c 223e 4164 6469  ntax.html\">Addi
-0002b500: 7469 6f6e 616c 2069 6e66 6f72 6d61 7469  tional informati
-0002b510: 6f6e 3c2f 613e 220a 0a5b 4930 3030 315d  on</a>"..[I0001]
-0002b520: 0a77 6879 203d 2022 5573 6564 2074 6f20  .why = "Used to 
-0002b530: 696e 666f 726d 2074 6861 7420 6120 6275  inform that a bu
-0002b540: 696c 742d 696e 206d 6f64 756c 6520 6861  ilt-in module ha
-0002b550: 7320 6e6f 7420 6265 656e 2063 6865 636b  s not been check
-0002b560: 6564 2075 7369 6e67 2074 6865 2072 6177  ed using the raw
-0002b570: 2063 6865 636b 6572 732e 220a 6578 616d   checkers.".exam
-0002b580: 706c 6573 203d 2022 3c61 2068 7265 663d  ples = "<a href=
-0002b590: 5c22 6874 7470 733a 2f2f 7079 6c69 6e74  \"https://pylint
-0002b5a0: 2e70 7963 7161 2e6f 7267 2f65 6e2f 6c61  .pycqa.org/en/la
-0002b5b0: 7465 7374 2f75 7365 725f 6775 6964 652f  test/user_guide/
-0002b5c0: 6d65 7373 6167 6573 2f69 6e66 6f72 6d61  messages/informa
-0002b5d0: 7469 6f6e 2f72 6177 2d63 6865 636b 6572  tion/raw-checker
-0002b5e0: 2d66 6169 6c65 642e 6874 6d6c 5c22 3e41  -failed.html\">A
-0002b5f0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-0002b600: 6174 696f 6e3c 2f61 3e22 0a0a 5b49 3030  ation</a>"..[I00
-0002b610: 3130 5d0a 7768 7920 3d20 2249 7420 6c6f  10].why = "It lo
-0002b620: 6f6b 7320 6c69 6b65 2074 6865 2069 6e6c  oks like the inl
-0002b630: 696e 6520 6f70 7469 6f6e 2069 7320 6569  ine option is ei
-0002b640: 7468 6572 2062 6164 6c79 2066 6f72 6d61  ther badly forma
-0002b650: 7474 6564 206f 7220 6361 6e27 7420 6265  tted or can't be
-0002b660: 2075 7365 6420 696e 7369 6465 206d 6f64   used inside mod
-0002b670: 756c 6573 2e22 0a65 7861 6d70 6c65 7320  ules.".examples 
-0002b680: 3d20 2222 220a 2a2a 5072 6f62 6c65 6d61  = """.**Problema
-0002b690: 7469 6320 636f 6465 2a2a 0a0a 6060 6070  tic code**..```p
-0002b6a0: 790a 2320 323a 5b62 6164 2d69 6e6c 696e  y.# 2:[bad-inlin
-0002b6b0: 652d 6f70 7469 6f6e 5d0a 2320 7079 6c69  e-option].# pyli
-0002b6c0: 6e74 3a20 6469 7361 626c 6520 6c69 6e65  nt: disable line
-0002b6d0: 2d74 6f6f 2d6c 6f6e 670a 0a60 6060 0a0a  -too-long..```..
-0002b6e0: 2a2a 486f 7720 746f 2066 6978 2069 742a  **How to fix it*
-0002b6f0: 2a0a 0a60 6060 7079 0a23 2070 796c 696e  *..```py.# pylin
-0002b700: 743a 2064 6973 6162 6c65 3d6c 696e 652d  t: disable=line-
-0002b710: 746f 6f2d 6c6f 6e67 0a0a 6060 600a 2222  too-long..```.""
-0002b720: 220a 0a5b 4930 3031 315d 0a77 6879 203d  "..[I0011].why =
-0002b730: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
-0002b740: 7468 6520 696e 6c69 6e65 206f 7074 696f  the inline optio
-0002b750: 6e20 6469 7361 626c 6573 2061 206d 6573  n disables a mes
-0002b760: 7361 6765 206f 7220 6120 6d65 7373 6167  sage or a messag
-0002b770: 6573 2063 6174 6567 6f72 792e 220a 6578  es category.".ex
-0002b780: 616d 706c 6573 203d 2022 3c61 2068 7265  amples = "<a hre
-0002b790: 663d 5c22 6874 7470 733a 2f2f 7079 6c69  f=\"https://pyli
-0002b7a0: 6e74 2e70 7963 7161 2e6f 7267 2f65 6e2f  nt.pycqa.org/en/
-0002b7b0: 6c61 7465 7374 2f75 7365 725f 6775 6964  latest/user_guid
-0002b7c0: 652f 6d65 7373 6167 6573 2f69 6e66 6f72  e/messages/infor
-0002b7d0: 6d61 7469 6f6e 2f6c 6f63 616c 6c79 2d64  mation/locally-d
-0002b7e0: 6973 6162 6c65 642e 6874 6d6c 5c22 3e41  isabled.html\">A
+00028ae0: 2275 7466 385c 2229 2061 7320 663a 0a20  "utf8\") as f:. 
+00028af0: 2020 2062 6573 7420 3d20 662e 7265 6164     best = f.read
+00028b00: 2829 0a0a 6060 600a 0a3c 6120 6872 6566  ()..```..<a href
+00028b10: 3d5c 2268 7474 7073 3a2f 2f70 796c 696e  =\"https://pylin
+00028b20: 742e 7079 6371 612e 6f72 672f 656e 2f6c  t.pycqa.org/en/l
+00028b30: 6174 6573 742f 7573 6572 5f67 7569 6465  atest/user_guide
+00028b40: 2f6d 6573 7361 6765 732f 7265 6661 6374  /messages/refact
+00028b50: 6f72 2f63 6f6e 7369 6465 722d 7573 696e  or/consider-usin
+00028b60: 672d 7769 7468 2e68 746d 6c5c 223e 4164  g-with.html\">Ad
+00028b70: 6469 7469 6f6e 616c 2069 6e66 6f72 6d61  ditional informa
+00028b80: 7469 6f6e 3c2f 613e 2222 220a 0a5b 5231  tion</a>"""..[R1
+00028b90: 3733 335d 0a77 6879 203d 2022 4974 206c  733].why = "It l
+00028ba0: 6f6f 6b73 206c 696b 6520 6974 6572 6174  ooks like iterat
+00028bb0: 696e 6720 6f76 6572 2074 6865 2064 6963  ing over the dic
+00028bc0: 7469 6f6e 6172 7920 6974 656d 7320 286b  tionary items (k
+00028bd0: 6579 2d69 7465 6d20 7061 6972 7329 2061  ey-item pairs) a
+00028be0: 6e64 2061 6363 6573 7369 6e67 2074 6865  nd accessing the
+00028bf0: 2076 616c 7565 2062 7920 696e 6465 7820   value by index 
+00028c00: 6c6f 6f6b 7570 2e20 5468 6520 7661 6c75  lookup. The valu
+00028c10: 6520 6361 6e20 6265 2061 6363 6573 7365  e can be accesse
+00028c20: 6420 6469 7265 6374 6c79 2069 6e73 7465  d directly inste
+00028c30: 6164 2e22 0a65 7861 6d70 6c65 7320 3d20  ad.".examples = 
+00028c40: 2222 220a 2a2a 5072 6f62 6c65 6d61 7469  """.**Problemati
+00028c50: 6320 636f 6465 2a2a 0a0a 6060 6070 790a  c code**..```py.
+00028c60: 4652 5549 5453 203d 207b 5c22 6170 706c  FRUITS = {\"appl
+00028c70: 655c 223a 2031 2c20 5c22 6f72 616e 6765  e\": 1, \"orange
+00028c80: 5c22 3a20 3130 2c20 5c22 6265 7272 795c  \": 10, \"berry\
+00028c90: 223a 2032 327d 0a0a 666f 7220 6672 7569  ": 22}..for frui
+00028ca0: 745f 6e61 6d65 2c20 6672 7569 745f 636f  t_name, fruit_co
+00028cb0: 756e 7420 696e 2046 5255 4954 532e 6974  unt in FRUITS.it
+00028cc0: 656d 7328 293a 0a20 2020 2070 7269 6e74  ems():.    print
+00028cd0: 2846 5255 4954 535b 6672 7569 745f 6e61  (FRUITS[fruit_na
+00028ce0: 6d65 5d29 2020 2320 5b75 6e6e 6563 6573  me])  # [unneces
+00028cf0: 7361 7279 2d64 6963 742d 696e 6465 782d  sary-dict-index-
+00028d00: 6c6f 6f6b 7570 5d0a 0a60 6060 0a0a 2a2a  lookup]..```..**
+00028d10: 486f 7720 746f 2066 6978 2069 742a 2a0a  How to fix it**.
+00028d20: 0a60 6060 7079 0a46 5255 4954 5320 3d20  .```py.FRUITS = 
+00028d30: 7b5c 2261 7070 6c65 5c22 3a20 312c 205c  {\"apple\": 1, \
+00028d40: 226f 7261 6e67 655c 223a 2031 302c 205c  "orange\": 10, \
+00028d50: 2262 6572 7279 5c22 3a20 3232 7d0a 0a66  "berry\": 22}..f
+00028d60: 6f72 2066 7275 6974 5f6e 616d 652c 2066  or fruit_name, f
+00028d70: 7275 6974 5f63 6f75 6e74 2069 6e20 4652  ruit_count in FR
+00028d80: 5549 5453 2e69 7465 6d73 2829 3a0a 2020  UITS.items():.  
+00028d90: 2020 7072 696e 7428 6672 7569 745f 636f    print(fruit_co
+00028da0: 756e 7429 0a0a 6060 600a 2222 220a 0a5b  unt)..```."""..[
+00028db0: 5231 3733 345d 0a77 6879 203d 2022 4974  R1734].why = "It
+00028dc0: 206c 6f6f 6b73 206c 696b 6520 7573 696e   looks like usin
+00028dd0: 6720 6c69 7374 2829 2074 6f20 6372 6561  g list() to crea
+00028de0: 7465 2061 6e20 656d 7074 7920 6c69 7374  te an empty list
+00028df0: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
+00028e00: 6c69 7465 7261 6c20 5b5d 2e20 5468 6520  literal []. The 
+00028e10: 6c69 7465 7261 6c20 6973 2066 6173 7465  literal is faste
+00028e20: 7220 6173 2069 7420 6176 6f69 6473 2061  r as it avoids a
+00028e30: 6e20 6164 6469 7469 6f6e 616c 2066 756e  n additional fun
+00028e40: 6374 696f 6e20 6361 6c6c 2e22 0a65 7861  ction call.".exa
+00028e50: 6d70 6c65 7320 3d20 2222 220a 2a2a 5072  mples = """.**Pr
+00028e60: 6f62 6c65 6d61 7469 6320 636f 6465 2a2a  oblematic code**
+00028e70: 0a0a 6060 6070 790a 656d 7074 795f 6c69  ..```py.empty_li
+00028e80: 7374 203d 206c 6973 7428 2920 2023 205b  st = list()  # [
+00028e90: 7573 652d 6c69 7374 2d6c 6974 6572 616c  use-list-literal
+00028ea0: 5d0a 0a60 6060 0a0a 2a2a 486f 7720 746f  ]..```..**How to
+00028eb0: 2066 6978 2069 742a 2a0a 0a60 6060 7079   fix it**..```py
+00028ec0: 0a65 6d70 7479 5f6c 6973 7420 3d20 5b5d  .empty_list = []
+00028ed0: 0a0a 6060 600a 2222 220a 0a5b 5231 3733  ..```."""..[R173
+00028ee0: 355d 0a77 6879 203d 2022 4974 206c 6f6f  5].why = "It loo
+00028ef0: 6b73 206c 696b 6520 7573 696e 6720 6469  ks like using di
+00028f00: 6374 2829 2074 6f20 6372 6561 7465 2061  ct() to create a
+00028f10: 6e20 656d 7074 7920 6469 6374 696f 6e61  n empty dictiona
+00028f20: 7279 2069 6e73 7465 6164 206f 6620 7468  ry instead of th
+00028f30: 6520 6c69 7465 7261 6c20 7b7d 2e20 5468  e literal {}. Th
+00028f40: 6520 6c69 7465 7261 6c20 6973 2066 6173  e literal is fas
+00028f50: 7465 7220 6173 2069 7420 6176 6f69 6473  ter as it avoids
+00028f60: 2061 6e20 6164 6469 7469 6f6e 616c 2066   an additional f
+00028f70: 756e 6374 696f 6e20 6361 6c6c 2e22 0a65  unction call.".e
+00028f80: 7861 6d70 6c65 7320 3d20 2222 220a 2a2a  xamples = """.**
+00028f90: 5072 6f62 6c65 6d61 7469 6320 636f 6465  Problematic code
+00028fa0: 2a2a 0a0a 6060 6070 790a 656d 7074 795f  **..```py.empty_
+00028fb0: 6469 6374 203d 2064 6963 7428 2920 2023  dict = dict()  #
+00028fc0: 205b 7573 652d 6469 6374 2d6c 6974 6572   [use-dict-liter
+00028fd0: 616c 5d0a 6e65 775f 6469 6374 203d 2064  al].new_dict = d
+00028fe0: 6963 7428 666f 6f3d 5c22 6261 725c 2229  ict(foo=\"bar\")
+00028ff0: 2020 2320 5b75 7365 2d64 6963 742d 6c69    # [use-dict-li
+00029000: 7465 7261 6c5d 0a6e 6577 5f64 6963 7420  teral].new_dict 
+00029010: 3d20 6469 6374 282a 2a61 6e6f 7468 6572  = dict(**another
+00029020: 5f64 6963 7429 2020 2320 5b75 7365 2d64  _dict)  # [use-d
+00029030: 6963 742d 6c69 7465 7261 6c5d 0a0a 6060  ict-literal]..``
+00029040: 600a 0a2a 2a48 6f77 2074 6f20 6669 7820  `..**How to fix 
+00029050: 6974 2a2a 0a0a 6060 6070 790a 656d 7074  it**..```py.empt
+00029060: 795f 6469 6374 203d 207b 7d0a 0a23 2063  y_dict = {}..# c
+00029070: 7265 6174 6520 7573 696e 6720 6120 6c69  reate using a li
+00029080: 7465 7261 6c20 6469 6374 0a6e 6577 5f64  teral dict.new_d
+00029090: 6963 7420 3d20 7b5c 2266 6f6f 5c22 3a20  ict = {\"foo\": 
+000290a0: 5c22 6261 725c 227d 0a0a 2320 7368 616c  \"bar\"}..# shal
+000290b0: 6c6f 7720 636f 7079 2061 2064 6963 740a  low copy a dict.
+000290c0: 6e65 775f 6469 6374 203d 207b 2a2a 616e  new_dict = {**an
+000290d0: 6f74 6865 725f 6469 6374 7d0a 0a60 6060  other_dict}..```
+000290e0: 0a0a 3c61 2068 7265 663d 5c22 6874 7470  ..<a href=\"http
+000290f0: 733a 2f2f 7079 6c69 6e74 2e70 7963 7161  s://pylint.pycqa
+00029100: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f75  .org/en/latest/u
+00029110: 7365 725f 6775 6964 652f 6d65 7373 6167  ser_guide/messag
+00029120: 6573 2f72 6566 6163 746f 722f 7573 652d  es/refactor/use-
+00029130: 6469 6374 2d6c 6974 6572 616c 2e68 746d  dict-literal.htm
+00029140: 6c5c 223e 4164 6469 7469 6f6e 616c 2069  l\">Additional i
+00029150: 6e66 6f72 6d61 7469 6f6e 3c2f 613e 2222  nformation</a>""
+00029160: 220a 0a5b 5231 3733 365d 0a77 6879 203d  "..[R1736].why =
+00029170: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
+00029180: 6974 6572 6174 696e 6720 6f76 6572 2061  iterating over a
+00029190: 6e20 656e 756d 6572 6174 696f 6e20 616e  n enumeration an
+000291a0: 6420 6163 6365 7373 696e 6720 7468 6520  d accessing the 
+000291b0: 7661 6c75 6520 6279 2069 6e64 6578 206c  value by index l
+000291c0: 6f6f 6b75 702e 2054 6865 2076 616c 7565  ookup. The value
+000291d0: 2063 616e 2062 6520 6163 6365 7373 6564   can be accessed
+000291e0: 2064 6972 6563 746c 7920 696e 7374 6561   directly instea
+000291f0: 642e 220a 6578 616d 706c 6573 203d 2022  d.".examples = "
+00029200: 2222 0a2a 2a50 726f 626c 656d 6174 6963  "".**Problematic
+00029210: 2063 6f64 652a 2a0a 0a60 6060 7079 0a6c   code**..```py.l
+00029220: 6574 7465 7273 203d 205b 2761 272c 2027  etters = ['a', '
+00029230: 6227 2c20 2763 275d 0a0a 666f 7220 696e  b', 'c']..for in
+00029240: 6465 782c 206c 6574 7465 7220 696e 2065  dex, letter in e
+00029250: 6e75 6d65 7261 7465 286c 6574 7465 7273  numerate(letters
+00029260: 293a 0a20 2020 2070 7269 6e74 286c 6574  ):.    print(let
+00029270: 7465 7273 5b69 6e64 6578 5d29 2020 2320  ters[index])  # 
+00029280: 5b75 6e6e 6563 6573 7361 7279 2d6c 6973  [unnecessary-lis
+00029290: 742d 696e 6465 782d 6c6f 6f6b 7570 5d0a  t-index-lookup].
+000292a0: 0a60 6060 0a0a 2a2a 486f 7720 746f 2066  .```..**How to f
+000292b0: 6978 2069 742a 2a0a 0a60 6060 7079 0a6c  ix it**..```py.l
+000292c0: 6574 7465 7273 203d 205b 2761 272c 2027  etters = ['a', '
+000292d0: 6227 2c20 2763 275d 0a0a 666f 7220 696e  b', 'c']..for in
+000292e0: 6465 782c 206c 6574 7465 7220 696e 2065  dex, letter in e
+000292f0: 6e75 6d65 7261 7465 286c 6574 7465 7273  numerate(letters
+00029300: 293a 0a20 2020 2070 7269 6e74 286c 6574  ):.    print(let
+00029310: 7465 7229 0a0a 6060 600a 2222 220a 0a5b  ter)..```."""..[
+00029320: 5231 3236 305d 0a77 6879 203d 2022 4974  R1260].why = "It
+00029330: 206c 6f6f 6b73 206c 696b 6520 7468 6520   looks like the 
+00029340: 6d65 7468 6f64 206f 7220 6675 6e63 7469  method or functi
+00029350: 6f6e 2069 7320 746f 6f20 636f 6d70 6c65  on is too comple
+00029360: 7820 6261 7365 6420 6f6e 204d 6343 6162  x based on McCab
+00029370: 6520 436f 6d70 6c65 7869 7479 2043 7963  e Complexity Cyc
+00029380: 6c6f 6d61 7469 6322 0a65 7861 6d70 6c65  lomatic".example
+00029390: 7320 3d20 223c 6120 6872 6566 3d5c 2268  s = "<a href=\"h
+000293a0: 7474 7073 3a2f 2f70 796c 696e 742e 7079  ttps://pylint.py
+000293b0: 6371 612e 6f72 672f 656e 2f6c 6174 6573  cqa.org/en/lates
+000293c0: 742f 7573 6572 5f67 7569 6465 2f6d 6573  t/user_guide/mes
+000293d0: 7361 6765 732f 7265 6661 6374 6f72 2f74  sages/refactor/t
+000293e0: 6f6f 2d63 6f6d 706c 6578 2e68 746d 6c5c  oo-complex.html\
+000293f0: 223e 4164 6469 7469 6f6e 616c 2069 6e66  ">Additional inf
+00029400: 6f72 6d61 7469 6f6e 3c2f 613e 220a 0a5b  ormation</a>"..[
+00029410: 5230 3930 315d 0a77 6879 203d 2022 4974  R0901].why = "It
+00029420: 206c 6f6f 6b73 206c 696b 6520 636c 6173   looks like clas
+00029430: 7320 6861 7320 746f 6f20 6d61 6e79 2070  s has too many p
+00029440: 6172 656e 7420 636c 6173 7365 732c 2074  arent classes, t
+00029450: 7279 2074 6f20 7265 6475 6365 2074 6869  ry to reduce thi
+00029460: 7320 746f 2067 6574 2061 2073 696d 706c  s to get a simpl
+00029470: 6572 2028 616e 6420 736f 2065 6173 6965  er (and so easie
+00029480: 7220 746f 2075 7365 2920 636c 6173 732e  r to use) class.
+00029490: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
+000294a0: 0a2a 2a50 726f 626c 656d 6174 6963 2063  .**Problematic c
+000294b0: 6f64 652a 2a0a 0a60 6060 7079 0a63 6c61  ode**..```py.cla
+000294c0: 7373 2041 6e69 6d61 6c3a 202e 2e2e 0a63  ss Animal: ....c
+000294d0: 6c61 7373 2042 6561 6b79 416e 696d 616c  lass BeakyAnimal
+000294e0: 2841 6e69 6d61 6c29 3a20 2e2e 2e0a 636c  (Animal): ....cl
+000294f0: 6173 7320 4675 7272 7941 6e69 6d61 6c28  ass FurryAnimal(
+00029500: 416e 696d 616c 293a 202e 2e2e 0a63 6c61  Animal): ....cla
+00029510: 7373 2053 7769 6d6d 6572 2841 6e69 6d61  ss Swimmer(Anima
+00029520: 6c29 3a20 2e2e 2e0a 636c 6173 7320 4567  l): ....class Eg
+00029530: 674c 6179 6572 2841 6e69 6d61 6c29 3a20  gLayer(Animal): 
+00029540: 2e2e 2e0a 636c 6173 7320 5665 6e6f 6d6f  ....class Venomo
+00029550: 7573 416e 696d 616c 2841 6e69 6d61 6c29  usAnimal(Animal)
+00029560: 3a20 2e2e 2e0a 636c 6173 7320 5072 6f74  : ....class Prot
+00029570: 6563 7465 6453 7065 6369 6528 416e 696d  ectedSpecie(Anim
+00029580: 616c 293a 202e 2e2e 0a63 6c61 7373 2042  al): ....class B
+00029590: 6561 7665 7254 6169 6c65 6441 6e69 6d61  eaverTailedAnima
+000295a0: 6c28 416e 696d 616c 293a 202e 2e2e 0a63  l(Animal): ....c
+000295b0: 6c61 7373 2056 6572 7465 6272 6174 6528  lass Vertebrate(
+000295c0: 416e 696d 616c 293a 202e 2e2e 0a0a 0a23  Animal): ......#
+000295d0: 206d 6178 206f 6620 3720 6279 2064 6566   max of 7 by def
+000295e0: 6175 6c74 2c20 6361 6e20 6265 2063 6f6e  ault, can be con
+000295f0: 6669 6775 7265 640a 2320 6561 6368 2065  figured.# each e
+00029600: 6467 6520 6f66 2061 2064 6961 6d6f 6e64  dge of a diamond
+00029610: 2069 6e68 6572 6974 616e 6365 2063 6f75   inheritance cou
+00029620: 6e74 730a 636c 6173 7320 506c 6179 7479  nts.class Playty
+00029630: 7075 7328 2020 2320 5b74 6f6f 2d6d 616e  pus(  # [too-man
+00029640: 792d 616e 6365 7374 6f72 735d 0a20 2020  y-ancestors].   
+00029650: 2042 6561 6b79 416e 696d 616c 2c0a 2020   BeakyAnimal,.  
+00029660: 2020 4675 7272 7941 6e69 6d61 6c2c 0a20    FurryAnimal,. 
+00029670: 2020 2053 7769 6d6d 6572 2c0a 2020 2020     Swimmer,.    
+00029680: 4567 674c 6179 6572 2c0a 2020 2020 5665  EggLayer,.    Ve
+00029690: 6e6f 6d6f 7573 416e 696d 616c 2c0a 2020  nomousAnimal,.  
+000296a0: 2020 5072 6f74 6563 7465 6453 7065 6369    ProtectedSpeci
+000296b0: 652c 0a20 2020 2042 6561 7665 7254 6169  e,.    BeaverTai
+000296c0: 6c65 6441 6e69 6d61 6c2c 0a20 2020 2056  ledAnimal,.    V
+000296d0: 6572 7465 6272 6174 652c 0a29 3a0a 2020  ertebrate,.):.  
+000296e0: 2020 7061 7373 0a0a 6060 600a 0a2a 2a48    pass..```..**H
+000296f0: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+00029700: 6060 6070 790a 636c 6173 7320 416e 696d  ```py.class Anim
+00029710: 616c 3a0a 2020 2020 6265 6176 6572 5f74  al:.    beaver_t
+00029720: 6169 6c65 643a 2062 6f6f 6c0a 2020 2020  ailed: bool.    
+00029730: 6361 6e5f 7377 696d 3a20 626f 6f6c 0a20  can_swim: bool. 
+00029740: 2020 2068 6173 5f62 6561 6b3a 2062 6f6f     has_beak: boo
+00029750: 6c0a 2020 2020 6861 735f 6675 723a 2062  l.    has_fur: b
+00029760: 6f6f 6c0a 2020 2020 6861 735f 7665 7274  ool.    has_vert
+00029770: 6562 7261 653a 2062 6f6f 6c0a 2020 2020  ebrae: bool.    
+00029780: 6c61 7973 5f65 6767 3a20 626f 6f6c 0a20  lays_egg: bool. 
+00029790: 2020 2070 726f 7465 6374 6564 5f73 7065     protected_spe
+000297a0: 6369 653a 2062 6f6f 6c0a 2020 2020 7665  cie: bool.    ve
+000297b0: 6e6f 6d6f 7573 3a20 626f 6f6c 0a0a 0a63  nomous: bool...c
+000297c0: 6c61 7373 2049 6e76 6572 7465 6272 6174  lass Invertebrat
+000297d0: 6528 416e 696d 616c 293a 0a20 2020 2068  e(Animal):.    h
+000297e0: 6173 5f76 6572 7465 6272 6165 203d 2046  as_vertebrae = F
+000297f0: 616c 7365 0a0a 0a63 6c61 7373 2056 6572  alse...class Ver
+00029800: 7465 6272 6174 6528 416e 696d 616c 293a  tebrate(Animal):
+00029810: 0a20 2020 2068 6173 5f76 6572 7465 6272  .    has_vertebr
+00029820: 6165 203d 2054 7275 650a 0a0a 636c 6173  ae = True...clas
+00029830: 7320 4d61 6d6d 616c 2856 6572 7465 6272  s Mammal(Vertebr
+00029840: 6174 6529 3a0a 2020 2020 6861 735f 6265  ate):.    has_be
+00029850: 616b 203d 2046 616c 7365 0a20 2020 2068  ak = False.    h
+00029860: 6173 5f66 7572 203d 2054 7275 650a 2020  as_fur = True.  
+00029870: 2020 6c61 7973 5f65 6767 203d 2046 616c    lays_egg = Fal
+00029880: 7365 0a20 2020 2076 656e 6f6d 6f75 7320  se.    venomous 
+00029890: 3d20 4661 6c73 650a 0a0a 636c 6173 7320  = False...class 
+000298a0: 506c 6179 7479 7075 7328 4d61 6d6d 616c  Playtypus(Mammal
+000298b0: 293a 0a20 2020 2062 6561 7665 725f 7461  ):.    beaver_ta
+000298c0: 696c 6564 203d 2054 7275 650a 2020 2020  iled = True.    
+000298d0: 6361 6e5f 7377 696d 203d 2054 7275 650a  can_swim = True.
+000298e0: 2020 2020 6861 735f 6265 616b 203d 2054      has_beak = T
+000298f0: 7275 650a 2020 2020 6c61 7973 5f65 6767  rue.    lays_egg
+00029900: 203d 2046 616c 7365 0a20 2020 2070 726f   = False.    pro
+00029910: 7465 6374 6564 5f73 7065 6369 6520 3d20  tected_specie = 
+00029920: 5472 7565 0a20 2020 2076 656e 6f6d 6f75  True.    venomou
+00029930: 7320 3d20 5472 7565 0a0a 6060 600a 2222  s = True..```.""
+00029940: 220a 0a5b 5230 3930 325d 0a77 6879 203d  "..[R0902].why =
+00029950: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
+00029960: 636c 6173 7320 6861 7320 746f 6f20 6d61  class has too ma
+00029970: 6e79 2069 6e73 7461 6e63 6520 6174 7472  ny instance attr
+00029980: 6962 7574 6573 2c20 7472 7920 746f 2072  ibutes, try to r
+00029990: 6564 7563 6520 7468 6973 2074 6f20 6765  educe this to ge
+000299a0: 7420 6120 7369 6d70 6c65 7220 2861 6e64  t a simpler (and
+000299b0: 2073 6f20 6561 7369 6572 2074 6f20 7573   so easier to us
+000299c0: 6529 2063 6c61 7373 2e22 0a65 7861 6d70  e) class.".examp
+000299d0: 6c65 7320 3d20 2222 220a 2a2a 5072 6f62  les = """.**Prob
+000299e0: 6c65 6d61 7469 6320 636f 6465 2a2a 0a0a  lematic code**..
+000299f0: 6060 6070 790a 636c 6173 7320 4672 7569  ```py.class Frui
+00029a00: 743a 2020 2320 5b74 6f6f 2d6d 616e 792d  t:  # [too-many-
+00029a10: 696e 7374 616e 6365 2d61 7474 7269 6275  instance-attribu
+00029a20: 7465 735d 0a20 2020 2064 6566 205f 5f69  tes].    def __i
+00029a30: 6e69 745f 5f28 7365 6c66 293a 0a20 2020  nit__(self):.   
+00029a40: 2020 2020 2023 206d 6178 206f 6620 3720       # max of 7 
+00029a50: 6174 7472 6962 7574 6573 2062 7920 6465  attributes by de
+00029a60: 6661 756c 742c 2063 616e 2062 6520 636f  fault, can be co
+00029a70: 6e66 6967 7572 6564 0a20 2020 2020 2020  nfigured.       
+00029a80: 2073 656c 662e 776f 726d 5f6e 616d 6520   self.worm_name 
+00029a90: 3d20 5c22 4a69 6d6d 795c 220a 2020 2020  = \"Jimmy\".    
+00029aa0: 2020 2020 7365 6c66 2e77 6f72 6d5f 7479      self.worm_ty
+00029ab0: 7065 203d 205c 2243 6f64 6c69 6e67 204d  pe = \"Codling M
+00029ac0: 6f74 6873 5c22 0a20 2020 2020 2020 2073  oths\".        s
+00029ad0: 656c 662e 776f 726d 5f63 6f6c 6f72 203d  elf.worm_color =
+00029ae0: 205c 226c 6967 6874 2062 726f 776e 5c22   \"light brown\"
+00029af0: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
+00029b00: 7569 745f 6e61 6d65 203d 205c 224c 6974  uit_name = \"Lit
+00029b10: 746c 6520 4170 706c 655c 220a 2020 2020  tle Apple\".    
+00029b20: 2020 2020 7365 6c66 2e66 7275 6974 5f63      self.fruit_c
+00029b30: 6f6c 6f72 203d 205c 2242 7269 6768 7420  olor = \"Bright 
+00029b40: 7265 645c 220a 2020 2020 2020 2020 7365  red\".        se
+00029b50: 6c66 2e66 7275 6974 5f76 6974 616d 696e  lf.fruit_vitamin
+00029b60: 7320 3d20 5b5c 2241 5c22 2c20 5c22 4231  s = [\"A\", \"B1
+00029b70: 5c22 5d0a 2020 2020 2020 2020 7365 6c66  \"].        self
+00029b80: 2e66 7275 6974 5f61 6e74 696f 7869 6461  .fruit_antioxida
+00029b90: 6e74 7320 3d20 4e6f 6e65 0a20 2020 2020  nts = None.     
+00029ba0: 2020 2073 656c 662e 7365 636f 6e64 6172     self.secondar
+00029bb0: 795f 776f 726d 5f6e 616d 6520 3d20 5c22  y_worm_name = \"
+00029bc0: 4b69 6d5c 220a 2020 2020 2020 2020 7365  Kim\".        se
+00029bd0: 6c66 2e73 6563 6f6e 6461 7279 5f77 6f72  lf.secondary_wor
+00029be0: 6d5f 7479 7065 203d 205c 2241 7070 6c65  m_type = \"Apple
+00029bf0: 206d 6167 676f 745c 220a 2020 2020 2020   maggot\".      
+00029c00: 2020 7365 6c66 2e73 6563 6f6e 6461 7279    self.secondary
+00029c10: 5f77 6f72 6d5f 636f 6c6f 7220 3d20 5c22  _worm_color = \"
+00029c20: 5768 6974 6973 685c 220a 0a60 6060 0a0a  Whitish\"..```..
+00029c30: 2a2a 486f 7720 746f 2066 6978 2069 742a  **How to fix it*
+00029c40: 2a0a 0a60 6060 7079 0a69 6d70 6f72 7420  *..```py.import 
+00029c50: 6461 7461 636c 6173 7365 730a 0a0a 4064  dataclasses...@d
+00029c60: 6174 6163 6c61 7373 6573 2e64 6174 6163  ataclasses.datac
+00029c70: 6c61 7373 0a63 6c61 7373 2057 6f72 6d3a  lass.class Worm:
+00029c80: 0a20 2020 206e 616d 653a 2073 7472 0a20  .    name: str. 
+00029c90: 2020 2074 7970 653a 2073 7472 0a20 2020     type: str.   
+00029ca0: 2063 6f6c 6f72 3a20 7374 720a 0a0a 636c   color: str...cl
+00029cb0: 6173 7320 4672 7569 743a 0a20 2020 2064  ass Fruit:.    d
+00029cc0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00029cd0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00029ce0: 6e61 6d65 203d 205c 224c 6974 746c 6520  name = \"Little 
+00029cf0: 4170 706c 655c 220a 2020 2020 2020 2020  Apple\".        
+00029d00: 7365 6c66 2e63 6f6c 6f72 203d 205c 2242  self.color = \"B
+00029d10: 7269 6768 7420 7265 645c 220a 2020 2020  right red\".    
+00029d20: 2020 2020 7365 6c66 2e76 6974 616d 696e      self.vitamin
+00029d30: 7320 3d20 5b5c 2241 5c22 2c20 5c22 4231  s = [\"A\", \"B1
+00029d40: 5c22 5d0a 2020 2020 2020 2020 7365 6c66  \"].        self
+00029d50: 2e61 6e74 696f 7869 6461 6e74 7320 3d20  .antioxidants = 
+00029d60: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00029d70: 662e 776f 726d 7320 3d20 5b0a 2020 2020  f.worms = [.    
+00029d80: 2020 2020 2020 2020 576f 726d 286e 616d          Worm(nam
+00029d90: 653d 5c22 4a69 6d6d 795c 222c 2074 7970  e=\"Jimmy\", typ
+00029da0: 653d 5c22 436f 646c 696e 6720 4d6f 7468  e=\"Codling Moth
+00029db0: 735c 222c 2063 6f6c 6f72 3d5c 226c 6967  s\", color=\"lig
+00029dc0: 6874 2062 726f 776e 5c22 292c 0a20 2020  ht brown\"),.   
+00029dd0: 2020 2020 2020 2020 2057 6f72 6d28 6e61           Worm(na
+00029de0: 6d65 3d5c 224b 696d 5c22 2c20 7479 7065  me=\"Kim\", type
+00029df0: 3d5c 2241 7070 6c65 206d 6167 676f 745c  =\"Apple maggot\
+00029e00: 222c 2063 6f6c 6f72 3d5c 2257 6869 7469  ", color=\"Whiti
+00029e10: 7368 5c22 292c 0a20 2020 2020 2020 205d  sh\"),.        ]
+00029e20: 0a0a 6060 600a 2222 220a 0a5b 5230 3930  ..```."""..[R090
+00029e30: 335d 0a77 6879 203d 2022 4974 206c 6f6f  3].why = "It loo
+00029e40: 6b73 206c 696b 6520 636c 6173 7320 6861  ks like class ha
+00029e50: 7320 746f 6f20 6665 7720 7075 626c 6963  s too few public
+00029e60: 206d 6574 686f 6473 2c20 736f 2062 6520   methods, so be 
+00029e70: 7375 7265 2069 7427 7320 7265 616c 6c79  sure it's really
+00029e80: 2077 6f72 7468 2069 742e 220a 6578 616d   worth it.".exam
+00029e90: 706c 6573 203d 2022 2222 0a2a 2a50 726f  ples = """.**Pro
+00029ea0: 626c 656d 6174 6963 2063 6f64 652a 2a0a  blematic code**.
+00029eb0: 0a60 6060 7079 0a63 6c61 7373 2057 6f72  .```py.class Wor
+00029ec0: 6d3a 2020 2320 5b74 6f6f 2d66 6577 2d70  m:  # [too-few-p
+00029ed0: 7562 6c69 632d 6d65 7468 6f64 735d 0a20  ublic-methods]. 
+00029ee0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00029ef0: 7365 6c66 2c20 6e61 6d65 3a20 7374 722c  self, name: str,
+00029f00: 2066 7275 6974 5f6f 665f 7265 7369 6465   fruit_of_reside
+00029f10: 6e63 653a 2046 7275 6974 293a 0a20 2020  nce: Fruit):.   
+00029f20: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
+00029f30: 206e 616d 650a 2020 2020 2020 2020 7365   name.        se
+00029f40: 6c66 2e66 7275 6974 5f6f 665f 7265 7369  lf.fruit_of_resi
+00029f50: 6465 6e63 6520 3d20 6672 7569 745f 6f66  dence = fruit_of
+00029f60: 5f72 6573 6964 656e 6365 0a0a 2020 2020  _residence..    
+00029f70: 6465 6620 626f 7265 2873 656c 6629 3a0a  def bore(self):.
+00029f80: 2020 2020 2020 2020 7072 696e 7428 665c          print(f\
+00029f90: 227b 7365 6c66 2e6e 616d 657d 2069 7320  "{self.name} is 
+00029fa0: 626f 7269 6e67 2069 6e74 6f20 7b73 656c  boring into {sel
+00029fb0: 662e 6672 7569 745f 6f66 5f72 6573 6964  f.fruit_of_resid
+00029fc0: 656e 6365 7d5c 2229 0a0a 6060 600a 0a2a  ence}\")..```..*
+00029fd0: 2a48 6f77 2074 6f20 6669 7820 6974 2a2a  *How to fix it**
+00029fe0: 0a0a 6060 6070 790a 696d 706f 7274 2064  ..```py.import d
+00029ff0: 6174 6163 6c61 7373 6573 0a0a 0a63 6c61  ataclasses...cla
+0002a000: 7373 2057 6f72 6d3a 0a20 2020 2064 6566  ss Worm:.    def
+0002a010: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0002a020: 6e61 6d65 3a20 7374 722c 2066 7275 6974  name: str, fruit
+0002a030: 5f6f 665f 7265 7369 6465 6e63 653a 2046  _of_residence: F
+0002a040: 7275 6974 293a 0a20 2020 2020 2020 2073  ruit):.        s
+0002a050: 656c 662e 6e61 6d65 203d 206e 616d 650a  elf.name = name.
+0002a060: 2020 2020 2020 2020 7365 6c66 2e66 7275          self.fru
+0002a070: 6974 5f6f 665f 7265 7369 6465 6e63 6520  it_of_residence 
+0002a080: 3d20 6672 7569 745f 6f66 5f72 6573 6964  = fruit_of_resid
+0002a090: 656e 6365 0a0a 2020 2020 6465 6620 626f  ence..    def bo
+0002a0a0: 7265 2873 656c 6629 3a0a 2020 2020 2020  re(self):.      
+0002a0b0: 2020 7072 696e 7428 665c 227b 7365 6c66    print(f\"{self
+0002a0c0: 2e6e 616d 657d 2069 7320 626f 7269 6e67  .name} is boring
+0002a0d0: 2069 6e74 6f20 7b73 656c 662e 6672 7569   into {self.frui
+0002a0e0: 745f 6f66 5f72 6573 6964 656e 6365 7d5c  t_of_residence}\
+0002a0f0: 2229 0a0a 2020 2020 6465 6620 7769 6767  ")..    def wigg
+0002a100: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+0002a110: 2020 7072 696e 7428 665c 227b 7365 6c66    print(f\"{self
+0002a120: 2e6e 616d 657d 2077 6967 676c 6520 6172  .name} wiggle ar
+0002a130: 6f75 6e64 2077 6f72 6d69 6c79 2e5c 2229  ound wormily.\")
+0002a140: 0a0a 2320 6f72 0a0a 4064 6174 6163 6c61  ..# or..@datacla
+0002a150: 7373 6573 2e64 6174 6163 6c61 7373 0a63  sses.dataclass.c
+0002a160: 6c61 7373 2057 6f72 6d3a 0a20 2020 206e  lass Worm:.    n
+0002a170: 616d 653a 7374 720a 2020 2020 6672 7569  ame:str.    frui
+0002a180: 745f 6f66 5f72 6573 6964 656e 6365 3a20  t_of_residence: 
+0002a190: 4672 7569 740a 0a64 6566 2062 6f72 6528  Fruit..def bore(
+0002a1a0: 776f 726d 3a20 576f 726d 293a 0a20 2020  worm: Worm):.   
+0002a1b0: 2070 7269 6e74 2866 5c22 7b77 6f72 6d2e   print(f\"{worm.
+0002a1c0: 6e61 6d65 7d20 6973 2062 6f72 696e 6720  name} is boring 
+0002a1d0: 696e 746f 207b 776f 726d 2e66 7275 6974  into {worm.fruit
+0002a1e0: 5f6f 665f 7265 7369 6465 6e63 657d 5c22  _of_residence}\"
+0002a1f0: 290a 0a23 206f 720a 0a64 6566 2062 6f72  )..# or..def bor
+0002a200: 6528 6672 7569 743a 2046 7275 6974 2c20  e(fruit: Fruit, 
+0002a210: 776f 726d 5f6e 616d 653a 2073 7472 293a  worm_name: str):
+0002a220: 0a20 2020 2070 7269 6e74 2866 5c22 7b77  .    print(f\"{w
+0002a230: 6f72 6d5f 6e61 6d65 7d20 6973 2062 6f72  orm_name} is bor
+0002a240: 696e 6720 696e 746f 207b 6672 7569 747d  ing into {fruit}
+0002a250: 5c22 290a 0a60 6060 0a22 2222 0a0a 5b52  \")..```."""..[R
+0002a260: 3039 3034 5d0a 7768 7920 3d20 2249 7420  0904].why = "It 
+0002a270: 6c6f 6f6b 7320 6c69 6b65 2063 6c61 7373  looks like class
+0002a280: 2068 6173 2074 6f6f 206d 616e 7920 7075   has too many pu
+0002a290: 626c 6963 206d 6574 686f 6473 2c20 7472  blic methods, tr
+0002a2a0: 7920 746f 2072 6564 7563 6520 7468 6973  y to reduce this
+0002a2b0: 2074 6f20 6765 7420 6120 7369 6d70 6c65   to get a simple
+0002a2c0: 7220 2861 6e64 2073 6f20 6561 7369 6572  r (and so easier
+0002a2d0: 2074 6f20 7573 6529 2063 6c61 7373 2e22   to use) class."
+0002a2e0: 0a65 7861 6d70 6c65 7320 3d20 223c 6120  .examples = "<a 
+0002a2f0: 6872 6566 3d5c 2268 7474 7073 3a2f 2f70  href=\"https://p
+0002a300: 796c 696e 742e 7079 6371 612e 6f72 672f  ylint.pycqa.org/
+0002a310: 656e 2f6c 6174 6573 742f 7573 6572 5f67  en/latest/user_g
+0002a320: 7569 6465 2f6d 6573 7361 6765 732f 7265  uide/messages/re
+0002a330: 6661 6374 6f72 2f74 6f6f 2d6d 616e 792d  factor/too-many-
+0002a340: 7075 626c 6963 2d6d 6574 686f 6473 2e68  public-methods.h
+0002a350: 746d 6c5c 223e 4164 6469 7469 6f6e 616c  tml\">Additional
+0002a360: 2069 6e66 6f72 6d61 7469 6f6e 3c2f 613e   information</a>
+0002a370: 220a 0a5b 5230 3931 315d 0a77 6879 203d  "..[R0911].why =
+0002a380: 2022 4974 206c 6f6f 6b73 206c 696b 6520   "It looks like 
+0002a390: 7468 6520 6675 6e63 7469 6f6e 206f 7220  the function or 
+0002a3a0: 6d65 7468 6f64 2068 6173 2074 6f6f 206d  method has too m
+0002a3b0: 616e 7920 7265 7475 726e 2073 7461 7465  any return state
+0002a3c0: 6d65 6e74 2c20 6d61 6b69 6e67 2069 7420  ment, making it 
+0002a3d0: 6861 7264 2074 6f20 666f 6c6c 6f77 2e22  hard to follow."
+0002a3e0: 0a65 7861 6d70 6c65 7320 3d20 2222 220a  .examples = """.
+0002a3f0: 2a2a 5072 6f62 6c65 6d61 7469 6320 636f  **Problematic co
+0002a400: 6465 2a2a 0a0a 6060 6070 790a 6465 6620  de**..```py.def 
+0002a410: 746f 5f73 7472 696e 6728 7829 3a20 2023  to_string(x):  #
+0002a420: 205b 746f 6f2d 6d61 6e79 2d72 6574 7572   [too-many-retur
+0002a430: 6e2d 7374 6174 656d 656e 7473 5d0a 2020  n-statements].  
+0002a440: 2020 2320 6d61 7820 6f66 2036 2062 7920    # max of 6 by 
+0002a450: 6465 6661 756c 742c 2063 616e 2062 6520  default, can be 
+0002a460: 636f 6e66 6967 7572 6564 0a20 2020 2069  configured.    i
+0002a470: 6620 7820 3d3d 2031 3a0a 2020 2020 2020  f x == 1:.      
+0002a480: 2020 7265 7475 726e 2027 5468 6973 2069    return 'This i
+0002a490: 7320 6f6e 652e 270a 2020 2020 6966 2078  s one.'.    if x
+0002a4a0: 203d 3d20 323a 0a20 2020 2020 2020 2072   == 2:.        r
+0002a4b0: 6574 7572 6e20 2754 6869 7320 6973 2074  eturn 'This is t
+0002a4c0: 776f 2e27 0a20 2020 2069 6620 7820 3d3d  wo.'.    if x ==
+0002a4d0: 2033 3a0a 2020 2020 2020 2020 7265 7475   3:.        retu
+0002a4e0: 726e 2027 5468 6973 2069 7320 7468 7265  rn 'This is thre
+0002a4f0: 652e 270a 2020 2020 6966 2078 203d 3d20  e.'.    if x == 
+0002a500: 343a 0a20 2020 2020 2020 2072 6574 7572  4:.        retur
+0002a510: 6e20 2754 6869 7320 6973 2066 6f75 722e  n 'This is four.
+0002a520: 270a 2020 2020 6966 2078 203d 3d20 353a  '.    if x == 5:
+0002a530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002a540: 2754 6869 7320 6973 2066 6976 652e 270a  'This is five.'.
+0002a550: 2020 2020 6966 2078 203d 3d20 363a 0a20      if x == 6:. 
+0002a560: 2020 2020 2020 2072 6574 7572 6e20 2754         return 'T
+0002a570: 6869 7320 6973 2073 6978 2e27 0a20 2020  his is six.'.   
+0002a580: 2069 6620 7820 3d3d 2037 3a0a 2020 2020   if x == 7:.    
+0002a590: 2020 2020 7265 7475 726e 2027 5468 6973      return 'This
+0002a5a0: 2069 7320 7365 7665 6e2e 270a 0a60 6060   is seven.'..```
+0002a5b0: 0a0a 2a2a 486f 7720 746f 2066 6978 2069  ..**How to fix i
+0002a5c0: 742a 2a0a 0a60 6060 7079 0a4e 554d 4245  t**..```py.NUMBE
+0002a5d0: 5253 5f54 4f5f 5354 5249 4e47 5320 3d20  RS_TO_STRINGS = 
+0002a5e0: 7b0a 2020 2020 313a 2027 6f6e 6527 2c0a  {.    1: 'one',.
+0002a5f0: 2020 2020 323a 2027 7477 6f27 2c0a 2020      2: 'two',.  
+0002a600: 2020 333a 2027 7468 7265 6527 2c0a 2020    3: 'three',.  
+0002a610: 2020 343a 2027 666f 7572 272c 0a20 2020    4: 'four',.   
+0002a620: 2035 3a20 2766 6976 6527 2c0a 2020 2020   5: 'five',.    
+0002a630: 363a 2027 7369 7827 2c0a 2020 2020 373a  6: 'six',.    7:
+0002a640: 2027 7365 7665 6e27 0a7d 0a0a 0a64 6566   'seven'.}...def
+0002a650: 2074 6f5f 7374 7269 6e67 2878 293a 0a20   to_string(x):. 
+0002a660: 2020 2072 6574 7572 6e20 6627 5468 6973     return f'This
+0002a670: 2069 7320 7b4e 554d 4245 5253 5f54 4f5f   is {NUMBERS_TO_
+0002a680: 5354 5249 4e47 532e 6765 7428 7829 7d2e  STRINGS.get(x)}.
+0002a690: 270a 0a60 6060 0a22 2222 0a0a 5b52 3039  '..```."""..[R09
+0002a6a0: 3132 5d0a 7768 7920 3d20 2249 7420 6c6f  12].why = "It lo
+0002a6b0: 6f6b 7320 6c69 6b65 2074 6865 2066 756e  oks like the fun
+0002a6c0: 6374 696f 6e20 6f72 206d 6574 686f 6420  ction or method 
+0002a6d0: 6861 7320 746f 6f20 6d61 6e79 2062 7261  has too many bra
+0002a6e0: 6e63 6865 732c 206d 616b 696e 6720 6974  nches, making it
+0002a6f0: 2068 6172 6420 746f 2066 6f6c 6c6f 772e   hard to follow.
+0002a700: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
+0002a710: 0a2a 2a50 726f 626c 656d 6174 6963 2063  .**Problematic c
+0002a720: 6f64 652a 2a0a 0a60 6060 7079 0a64 6566  ode**..```py.def
+0002a730: 206e 756d 5f74 6f5f 776f 7264 2878 293a   num_to_word(x):
+0002a740: 2020 2320 5b74 6f6f 2d6d 616e 792d 6272    # [too-many-br
+0002a750: 616e 6368 6573 5d0a 2020 2020 6966 2078  anches].    if x
+0002a760: 203d 3d20 303a 0a20 2020 2020 2020 2072   == 0:.        r
+0002a770: 6574 7572 6e20 5c22 7a65 726f 5c22 0a20  eturn \"zero\". 
+0002a780: 2020 2065 6c69 6620 7820 3d3d 2031 3a0a     elif x == 1:.
+0002a790: 2020 2020 2020 2020 7265 7475 726e 205c          return \
+0002a7a0: 226f 6e65 5c22 0a20 2020 2065 6c69 6620  "one\".    elif 
+0002a7b0: 7820 3d3d 2032 3a0a 2020 2020 2020 2020  x == 2:.        
+0002a7c0: 7265 7475 726e 205c 2274 776f 5c22 0a20  return \"two\". 
+0002a7d0: 2020 2065 6c69 6620 7820 3d3d 2033 3a0a     elif x == 3:.
+0002a7e0: 2020 2020 2020 2020 7265 7475 726e 205c          return \
+0002a7f0: 2274 6872 6565 5c22 0a20 2020 2065 6c69  "three\".    eli
+0002a800: 6620 7820 3d3d 2034 3a0a 2020 2020 2020  f x == 4:.      
+0002a810: 2020 7265 7475 726e 205c 2266 6f75 725c    return \"four\
+0002a820: 220a 2020 2020 656c 6966 2078 203d 3d20  ".    elif x == 
+0002a830: 353a 0a20 2020 2020 2020 2072 6574 7572  5:.        retur
+0002a840: 6e20 5c22 6669 7665 5c22 0a20 2020 2065  n \"five\".    e
+0002a850: 6c69 6620 7820 3d3d 2036 3a0a 2020 2020  lif x == 6:.    
+0002a860: 2020 2020 7265 7475 726e 205c 2273 6978      return \"six
+0002a870: 5c22 0a20 2020 2065 6c69 6620 7820 3d3d  \".    elif x ==
+0002a880: 2037 3a0a 2020 2020 2020 2020 7265 7475   7:.        retu
+0002a890: 726e 205c 2273 6576 656e 5c22 0a20 2020  rn \"seven\".   
+0002a8a0: 2065 6c69 6620 7820 3d3d 2038 3a0a 2020   elif x == 8:.  
+0002a8b0: 2020 2020 2020 7265 7475 726e 205c 2265        return \"e
+0002a8c0: 6967 6874 5c22 0a20 2020 2065 6c69 6620  ight\".    elif 
+0002a8d0: 7820 3d3d 2039 3a0a 2020 2020 2020 2020  x == 9:.        
+0002a8e0: 7265 7475 726e 205c 226e 696e 655c 220a  return \"nine\".
+0002a8f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0002a900: 2020 7265 7475 726e 204e 6f6e 650a 0a60    return None..`
+0002a910: 6060 0a0a 2a2a 486f 7720 746f 2066 6978  ``..**How to fix
+0002a920: 2069 742a 2a0a 0a60 6060 7079 0a64 6566   it**..```py.def
+0002a930: 206e 756d 5f74 6f5f 776f 7264 2878 293a   num_to_word(x):
+0002a940: 0a20 2020 2072 6574 7572 6e20 7b0a 2020  .    return {.  
+0002a950: 2020 2020 2020 303a 205c 227a 6572 6f5c        0: \"zero\
+0002a960: 222c 0a20 2020 2020 2020 2031 3a20 5c22  ",.        1: \"
+0002a970: 6f6e 655c 222c 0a20 2020 2020 2020 2032  one\",.        2
+0002a980: 3a20 5c22 7477 6f5c 222c 0a20 2020 2020  : \"two\",.     
+0002a990: 2020 2033 3a20 5c22 7468 7265 655c 222c     3: \"three\",
+0002a9a0: 0a20 2020 2020 2020 2034 3a20 5c22 666f  .        4: \"fo
+0002a9b0: 725c 222c 0a20 2020 2020 2020 2035 3a20  r\",.        5: 
+0002a9c0: 5c22 6669 655c 222c 0a20 2020 2020 2020  \"fie\",.       
+0002a9d0: 2036 3a20 5c22 7369 785c 222c 0a20 2020   6: \"six\",.   
+0002a9e0: 2020 2020 2037 3a20 5c22 7365 7665 6e5c       7: \"seven\
+0002a9f0: 222c 0a20 2020 2020 2020 2038 3a20 5c22  ",.        8: \"
+0002aa00: 6569 6768 745c 222c 0a20 2020 2020 2020  eight\",.       
+0002aa10: 2039 3a20 5c22 6e69 6e65 5c22 2c0a 2020   9: \"nine\",.  
+0002aa20: 2020 7d2e 6765 7428 7829 0a0a 6060 600a    }.get(x)..```.
+0002aa30: 2222 220a 0a5b 5230 3931 335d 0a77 6879  """..[R0913].why
+0002aa40: 203d 2022 4974 206c 6f6f 6b73 206c 696b   = "It looks lik
+0002aa50: 6520 7468 6520 6675 6e63 7469 6f6e 206f  e the function o
+0002aa60: 7220 6d65 7468 6f64 2074 616b 6573 2074  r method takes t
+0002aa70: 6f6f 206d 616e 7920 6172 6775 6d65 6e74  oo many argument
+0002aa80: 732e 220a 6578 616d 706c 6573 203d 2022  s.".examples = "
+0002aa90: 2222 0a2a 2a50 726f 626c 656d 6174 6963  "".**Problematic
+0002aaa0: 2063 6f64 652a 2a0a 0a60 6060 7079 0a64   code**..```py.d
+0002aab0: 6566 2074 6872 6565 5f64 5f63 6865 7373  ef three_d_chess
+0002aac0: 5f6d 6f76 6528 2020 2320 5b74 6f6f 2d6d  _move(  # [too-m
+0002aad0: 616e 792d 6172 6775 6d65 6e74 735d 0a20  any-arguments]. 
+0002aae0: 2020 2078 5f77 6869 7465 2c0a 2020 2020     x_white,.    
+0002aaf0: 795f 7768 6974 652c 0a20 2020 207a 5f77  y_white,.    z_w
+0002ab00: 6869 7465 2c0a 2020 2020 7069 6563 655f  hite,.    piece_
+0002ab10: 7768 6974 652c 0a20 2020 2078 5f62 6c61  white,.    x_bla
+0002ab20: 636b 2c0a 2020 2020 795f 626c 6163 6b2c  ck,.    y_black,
+0002ab30: 0a20 2020 207a 5f62 6c61 636b 2c0a 2020  .    z_black,.  
+0002ab40: 2020 7069 6563 655f 626c 6163 6b2c 0a20    piece_black,. 
+0002ab50: 2020 2078 5f62 6c75 652c 0a20 2020 2079     x_blue,.    y
+0002ab60: 5f62 6c75 652c 0a20 2020 207a 5f62 6c75  _blue,.    z_blu
+0002ab70: 652c 0a20 2020 2070 6965 6365 5f62 6c75  e,.    piece_blu
+0002ab80: 652c 0a20 2020 2063 7572 7265 6e74 5f70  e,.    current_p
+0002ab90: 6c61 7965 722c 0a29 3a0a 2020 2020 7061  layer,.):.    pa
+0002aba0: 7373 0a0a 6060 600a 0a2a 2a48 6f77 2074  ss..```..**How t
+0002abb0: 6f20 6669 7820 6974 2a2a 0a0a 6060 6070  o fix it**..```p
+0002abc0: 790a 6672 6f6d 2064 6174 6163 6c61 7373  y.from dataclass
+0002abd0: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+0002abe0: 6173 730a 0a0a 4064 6174 6163 6c61 7373  ass...@dataclass
+0002abf0: 0a63 6c61 7373 2054 6872 6565 4443 6865  .class ThreeDChe
+0002ac00: 7373 5069 6563 653a 0a20 2020 2078 3a20  ssPiece:.    x: 
+0002ac10: 696e 740a 2020 2020 793a 2069 6e74 0a20  int.    y: int. 
+0002ac20: 2020 207a 3a20 696e 740a 2020 2020 7479     z: int.    ty
+0002ac30: 7065 3a20 7374 720a 0a0a 6465 6620 7468  pe: str...def th
+0002ac40: 7265 655f 645f 6368 6573 735f 6d6f 7665  ree_d_chess_move
+0002ac50: 280a 2020 2020 7768 6974 653a 2054 6872  (.    white: Thr
+0002ac60: 6565 4443 6865 7373 5069 6563 652c 0a20  eeDChessPiece,. 
+0002ac70: 2020 2062 6c61 636b 3a20 5468 7265 6544     black: ThreeD
+0002ac80: 4368 6573 7350 6965 6365 2c0a 2020 2020  ChessPiece,.    
+0002ac90: 626c 7565 3a20 5468 7265 6544 4368 6573  blue: ThreeDChes
+0002aca0: 7350 6965 6365 2c0a 2020 2020 6375 7272  sPiece,.    curr
+0002acb0: 656e 745f 706c 6179 6572 2c0a 293a 0a20  ent_player,.):. 
+0002acc0: 2020 2070 6173 730a 0a60 6060 0a22 2222     pass..```."""
+0002acd0: 0a0a 5b52 3039 3134 5d0a 7768 7920 3d20  ..[R0914].why = 
+0002ace0: 2249 7420 6c6f 6f6b 7320 6c69 6b65 2074  "It looks like t
+0002acf0: 6865 2066 756e 6374 696f 6e20 6f72 206d  he function or m
+0002ad00: 6574 686f 6420 6861 7320 746f 6f20 6d61  ethod has too ma
+0002ad10: 6e79 206c 6f63 616c 2076 6172 6961 626c  ny local variabl
+0002ad20: 6573 2e22 0a65 7861 6d70 6c65 7320 3d20  es.".examples = 
+0002ad30: 223c 6120 6872 6566 3d5c 2268 7474 7073  "<a href=\"https
+0002ad40: 3a2f 2f70 796c 696e 742e 7079 6371 612e  ://pylint.pycqa.
+0002ad50: 6f72 672f 656e 2f6c 6174 6573 742f 7573  org/en/latest/us
+0002ad60: 6572 5f67 7569 6465 2f6d 6573 7361 6765  er_guide/message
+0002ad70: 732f 7265 6661 6374 6f72 2f74 6f6f 2d6d  s/refactor/too-m
+0002ad80: 616e 792d 6c6f 6361 6c73 2e68 746d 6c5c  any-locals.html\
+0002ad90: 223e 4164 6469 7469 6f6e 616c 2069 6e66  ">Additional inf
+0002ada0: 6f72 6d61 7469 6f6e 3c2f 613e 220a 0a5b  ormation</a>"..[
+0002adb0: 5230 3931 355d 0a77 6879 203d 2022 4974  R0915].why = "It
+0002adc0: 206c 6f6f 6b73 206c 696b 6520 7468 6520   looks like the 
+0002add0: 6675 6e63 7469 6f6e 206f 7220 6d65 7468  function or meth
+0002ade0: 6f64 2068 6173 2074 6f6f 206d 616e 7920  od has too many 
+0002adf0: 7374 6174 656d 656e 7473 2e20 596f 7520  statements. You 
+0002ae00: 7368 6f75 6c64 2074 6865 6e20 7370 6c69  should then spli
+0002ae10: 7420 6974 2069 6e20 736d 616c 6c65 7220  t it in smaller 
+0002ae20: 6675 6e63 7469 6f6e 7320 2f20 6d65 7468  functions / meth
+0002ae30: 6f64 732e 220a 6578 616d 706c 6573 203d  ods.".examples =
+0002ae40: 2022 3c61 2068 7265 663d 5c22 6874 7470   "<a href=\"http
+0002ae50: 733a 2f2f 7079 6c69 6e74 2e70 7963 7161  s://pylint.pycqa
+0002ae60: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f75  .org/en/latest/u
+0002ae70: 7365 725f 6775 6964 652f 6d65 7373 6167  ser_guide/messag
+0002ae80: 6573 2f72 6566 6163 746f 722f 746f 6f2d  es/refactor/too-
+0002ae90: 6d61 6e79 2d73 7461 7465 6d65 6e74 732e  many-statements.
+0002aea0: 6874 6d6c 5c22 3e41 6464 6974 696f 6e61  html\">Additiona
+0002aeb0: 6c20 696e 666f 726d 6174 696f 6e3c 2f61  l information</a
+0002aec0: 3e22 0a0a 5b52 3039 3136 5d0a 7768 7920  >"..[R0916].why 
+0002aed0: 3d20 2243 6f6e 7369 6465 7220 7369 6d70  = "Consider simp
+0002aee0: 6c69 6679 696e 6720 7468 6520 6578 7072  lifying the expr
+0002aef0: 6573 7369 6f6e 2077 6974 6820 6865 6c70  ession with help
+0002af00: 6572 2076 6172 6961 626c 6573 206f 7220  er variables or 
+0002af10: 6675 6e63 7469 6f6e 732e 220a 6578 616d  functions.".exam
+0002af20: 706c 6573 203d 2022 2222 0a2a 2a50 726f  ples = """.**Pro
+0002af30: 626c 656d 6174 6963 2063 6f64 652a 2a0a  blematic code**.
+0002af40: 0a60 6060 7079 0a64 6566 2063 616e 5f62  .```py.def can_b
+0002af50: 655f 6469 7669 6465 645f 6279 5f74 776f  e_divided_by_two
+0002af60: 5f61 6e64 5f61 7265 5f6e 6f74 5f7a 6572  _and_are_not_zer
+0002af70: 6f28 782c 2079 2c20 7a29 3a0a 2020 2020  o(x, y, z):.    
+0002af80: 2320 4d61 7869 6d75 6d20 6e75 6d62 6572  # Maximum number
+0002af90: 206f 6620 626f 6f6c 6561 6e20 6578 7072   of boolean expr
+0002afa0: 6573 7369 6f6e 7320 696e 2061 6e20 6966  essions in an if
+0002afb0: 2073 7461 7465 6d65 6e74 2028 6279 2064   statement (by d
+0002afc0: 6566 6175 6c74 2035 290a 2020 2020 2320  efault 5).    # 
+0002afd0: 2b31 3a20 5b74 6f6f 2d6d 616e 792d 626f  +1: [too-many-bo
+0002afe0: 6f6c 6561 6e2d 6578 7072 6573 7369 6f6e  olean-expression
+0002aff0: 735d 0a20 2020 2069 6620 2878 2061 6e64  s].    if (x and
+0002b000: 2079 2061 6e64 207a 2920 616e 6420 2878   y and z) and (x
+0002b010: 2025 2032 203d 3d20 3020 616e 6420 7920   % 2 == 0 and y 
+0002b020: 2520 3220 3d3d 2030 2061 6e64 207a 2025  % 2 == 0 and z %
+0002b030: 2032 203d 3d20 3029 3a0a 2020 2020 2020   2 == 0):.      
+0002b040: 2020 7061 7373 0a0a 6060 600a 0a2a 2a48    pass..```..**H
+0002b050: 6f77 2074 6f20 6669 7820 6974 2a2a 0a0a  ow to fix it**..
+0002b060: 6060 6070 790a 6465 6620 6361 6e5f 6265  ```py.def can_be
+0002b070: 5f64 6976 6964 6564 5f62 795f 7477 6f5f  _divided_by_two_
+0002b080: 616e 645f 6172 655f 6e6f 745f 7a65 726f  and_are_not_zero
+0002b090: 2878 2c20 792c 207a 293a 0a20 2020 2069  (x, y, z):.    i
+0002b0a0: 6620 616c 6c28 6920 616e 6420 6925 323d  f all(i and i%2=
+0002b0b0: 3d30 2066 6f72 2069 2069 6e20 5b78 2c20  =0 for i in [x, 
+0002b0c0: 792c 207a 5d29 3a0a 2020 2020 2020 2020  y, z]):.        
+0002b0d0: 7061 7373 0a0a 6060 600a 2222 220a 0a5b  pass..```."""..[
+0002b0e0: 5230 3830 315d 0a77 6879 203d 2022 496e  R0801].why = "In
+0002b0f0: 6469 6361 7465 7320 7468 6174 2061 2073  dicates that a s
+0002b100: 6574 206f 6620 7369 6d69 6c61 7220 6c69  et of similar li
+0002b110: 6e65 7320 6861 7320 6265 656e 2064 6574  nes has been det
+0002b120: 6563 7465 6420 616d 6f6e 6720 6d75 6c74  ected among mult
+0002b130: 6970 6c65 2066 696c 652e 2054 6869 7320  iple file. This 
+0002b140: 7573 7561 6c6c 7920 6d65 616e 7320 7468  usually means th
+0002b150: 6174 2074 6865 2063 6f64 6520 7368 6f75  at the code shou
+0002b160: 6c64 2062 6520 7265 6661 6374 6f72 6564  ld be refactored
+0002b170: 2074 6f20 6176 6f69 6420 7468 6973 2064   to avoid this d
+0002b180: 7570 6c69 6361 7469 6f6e 2e22 0a65 7861  uplication.".exa
+0002b190: 6d70 6c65 7320 3d20 223c 6120 6872 6566  mples = "<a href
+0002b1a0: 3d5c 2268 7474 7073 3a2f 2f70 796c 696e  =\"https://pylin
+0002b1b0: 742e 7079 6371 612e 6f72 672f 656e 2f6c  t.pycqa.org/en/l
+0002b1c0: 6174 6573 742f 7573 6572 5f67 7569 6465  atest/user_guide
+0002b1d0: 2f6d 6573 7361 6765 732f 7265 6661 6374  /messages/refact
+0002b1e0: 6f72 2f64 7570 6c69 6361 7465 2d63 6f64  or/duplicate-cod
+0002b1f0: 652e 6874 6d6c 5c22 3e41 6464 6974 696f  e.html\">Additio
+0002b200: 6e61 6c20 696e 666f 726d 6174 696f 6e3c  nal information<
+0002b210: 2f61 3e22 0a0a 5b52 3630 3032 5d0a 7768  /a>"..[R6002].wh
+0002b220: 7920 3d20 224f 6e6c 7920 656d 6974 7465  y = "Only emitte
+0002b230: 6420 6966 2027 7275 6e74 696d 652d 7479  d if 'runtime-ty
+0002b240: 7069 6e67 3d6e 6f27 2061 6e64 2061 2064  ping=no' and a d
+0002b250: 6570 7265 6361 7465 6420 7479 7069 6e67  eprecated typing
+0002b260: 2061 6c69 6173 2069 7320 7573 6564 2069   alias is used i
+0002b270: 6e20 6120 7479 7065 2061 6e6e 6f74 6174  n a type annotat
+0002b280: 696f 6e20 636f 6e74 6578 7420 696e 2050  ion context in P
+0002b290: 7974 686f 6e20 332e 3720 6f72 2033 2e38  ython 3.7 or 3.8
+0002b2a0: 2e22 0a65 7861 6d70 6c65 7320 3d20 223c  .".examples = "<
+0002b2b0: 6120 6872 6566 3d5c 2268 7474 7073 3a2f  a href=\"https:/
+0002b2c0: 2f70 796c 696e 742e 7079 6371 612e 6f72  /pylint.pycqa.or
+0002b2d0: 672f 656e 2f6c 6174 6573 742f 7573 6572  g/en/latest/user
+0002b2e0: 5f67 7569 6465 2f6d 6573 7361 6765 732f  _guide/messages/
+0002b2f0: 7265 6661 6374 6f72 2f63 6f6e 7369 6465  refactor/conside
+0002b300: 722d 7573 696e 672d 616c 6961 732e 6874  r-using-alias.ht
+0002b310: 6d6c 5c22 3e41 6464 6974 696f 6e61 6c20  ml\">Additional 
+0002b320: 696e 666f 726d 6174 696f 6e3c 2f61 3e22  information</a>"
+0002b330: 0a0a 5b52 3630 3033 5d0a 7768 7920 3d20  ..[R6003].why = 
+0002b340: 2249 7420 6c6f 6f6b 7320 6c69 6b65 2027  "It looks like '
+0002b350: 7479 7069 6e67 2e55 6e69 6f6e 2720 6f72  typing.Union' or
+0002b360: 2027 7479 7069 6e67 2e4f 7074 696f 6e61   'typing.Optiona
+0002b370: 6c27 2069 7320 7573 6564 2069 6e73 7465  l' is used inste
+0002b380: 6164 206f 6620 7468 6520 616c 7465 726e  ad of the altern
+0002b390: 6174 6976 6520 556e 696f 6e20 7379 6e74  ative Union synt
+0002b3a0: 6178 2027 696e 7420 7c20 4e6f 6e65 272e  ax 'int | None'.
+0002b3b0: 220a 6578 616d 706c 6573 203d 2022 3c61  ".examples = "<a
+0002b3c0: 2068 7265 663d 5c22 6874 7470 733a 2f2f   href=\"https://
+0002b3d0: 7079 6c69 6e74 2e70 7963 7161 2e6f 7267  pylint.pycqa.org
+0002b3e0: 2f65 6e2f 6c61 7465 7374 2f75 7365 725f  /en/latest/user_
+0002b3f0: 6775 6964 652f 6d65 7373 6167 6573 2f72  guide/messages/r
+0002b400: 6566 6163 746f 722f 636f 6e73 6964 6572  efactor/consider
+0002b410: 2d61 6c74 6572 6e61 7469 7665 2d75 6e69  -alternative-uni
+0002b420: 6f6e 2d73 796e 7461 782e 6874 6d6c 5c22  on-syntax.html\"
+0002b430: 3e41 6464 6974 696f 6e61 6c20 696e 666f  >Additional info
+0002b440: 726d 6174 696f 6e3c 2f61 3e22 0a0a 5b49  rmation</a>"..[I
+0002b450: 3030 3031 5d0a 7768 7920 3d20 2255 7365  0001].why = "Use
+0002b460: 6420 746f 2069 6e66 6f72 6d20 7468 6174  d to inform that
+0002b470: 2061 2062 7569 6c74 2d69 6e20 6d6f 6475   a built-in modu
+0002b480: 6c65 2068 6173 206e 6f74 2062 6565 6e20  le has not been 
+0002b490: 6368 6563 6b65 6420 7573 696e 6720 7468  checked using th
+0002b4a0: 6520 7261 7720 6368 6563 6b65 7273 2e22  e raw checkers."
+0002b4b0: 0a65 7861 6d70 6c65 7320 3d20 223c 6120  .examples = "<a 
+0002b4c0: 6872 6566 3d5c 2268 7474 7073 3a2f 2f70  href=\"https://p
+0002b4d0: 796c 696e 742e 7079 6371 612e 6f72 672f  ylint.pycqa.org/
+0002b4e0: 656e 2f6c 6174 6573 742f 7573 6572 5f67  en/latest/user_g
+0002b4f0: 7569 6465 2f6d 6573 7361 6765 732f 696e  uide/messages/in
+0002b500: 666f 726d 6174 696f 6e2f 7261 772d 6368  formation/raw-ch
+0002b510: 6563 6b65 722d 6661 696c 6564 2e68 746d  ecker-failed.htm
+0002b520: 6c5c 223e 4164 6469 7469 6f6e 616c 2069  l\">Additional i
+0002b530: 6e66 6f72 6d61 7469 6f6e 3c2f 613e 220a  nformation</a>".
+0002b540: 0a5b 4930 3031 305d 0a77 6879 203d 2022  .[I0010].why = "
+0002b550: 4974 206c 6f6f 6b73 206c 696b 6520 7468  It looks like th
+0002b560: 6520 696e 6c69 6e65 206f 7074 696f 6e20  e inline option 
+0002b570: 6973 2065 6974 6865 7220 6261 646c 7920  is either badly 
+0002b580: 666f 726d 6174 7465 6420 6f72 2063 616e  formatted or can
+0002b590: 2774 2062 6520 7573 6564 2069 6e73 6964  't be used insid
+0002b5a0: 6520 6d6f 6475 6c65 732e 220a 6578 616d  e modules.".exam
+0002b5b0: 706c 6573 203d 2022 2222 0a2a 2a50 726f  ples = """.**Pro
+0002b5c0: 626c 656d 6174 6963 2063 6f64 652a 2a0a  blematic code**.
+0002b5d0: 0a60 6060 7079 0a23 2032 3a5b 6261 642d  .```py.# 2:[bad-
+0002b5e0: 696e 6c69 6e65 2d6f 7074 696f 6e5d 0a23  inline-option].#
+0002b5f0: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+0002b600: 206c 696e 652d 746f 6f2d 6c6f 6e67 0a0a   line-too-long..
+0002b610: 6060 600a 0a2a 2a48 6f77 2074 6f20 6669  ```..**How to fi
+0002b620: 7820 6974 2a2a 0a0a 6060 6070 790a 2320  x it**..```py.# 
+0002b630: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+0002b640: 6c69 6e65 2d74 6f6f 2d6c 6f6e 670a 0a60  line-too-long..`
+0002b650: 6060 0a22 2222 0a0a 5b49 3030 3131 5d0a  ``."""..[I0011].
+0002b660: 7768 7920 3d20 2249 7420 6c6f 6f6b 7320  why = "It looks 
+0002b670: 6c69 6b65 2074 6865 2069 6e6c 696e 6520  like the inline 
+0002b680: 6f70 7469 6f6e 2064 6973 6162 6c65 7320  option disables 
+0002b690: 6120 6d65 7373 6167 6520 6f72 2061 206d  a message or a m
+0002b6a0: 6573 7361 6765 7320 6361 7465 676f 7279  essages category
+0002b6b0: 2e22 0a65 7861 6d70 6c65 7320 3d20 223c  .".examples = "<
+0002b6c0: 6120 6872 6566 3d5c 2268 7474 7073 3a2f  a href=\"https:/
+0002b6d0: 2f70 796c 696e 742e 7079 6371 612e 6f72  /pylint.pycqa.or
+0002b6e0: 672f 656e 2f6c 6174 6573 742f 7573 6572  g/en/latest/user
+0002b6f0: 5f67 7569 6465 2f6d 6573 7361 6765 732f  _guide/messages/
+0002b700: 696e 666f 726d 6174 696f 6e2f 6c6f 6361  information/loca
+0002b710: 6c6c 792d 6469 7361 626c 6564 2e68 746d  lly-disabled.htm
+0002b720: 6c5c 223e 4164 6469 7469 6f6e 616c 2069  l\">Additional i
+0002b730: 6e66 6f72 6d61 7469 6f6e 3c2f 613e 220a  nformation</a>".
+0002b740: 0a5b 4930 3031 335d 0a77 6879 203d 2022  .[I0013].why = "
+0002b750: 5573 6564 2074 6f20 696e 666f 726d 2074  Used to inform t
+0002b760: 6861 7420 7468 6520 6669 6c65 2077 696c  hat the file wil
+0002b770: 6c20 6e6f 7420 6265 2063 6865 636b 6564  l not be checked
+0002b780: 220a 6578 616d 706c 6573 203d 2022 3c61  ".examples = "<a
+0002b790: 2068 7265 663d 5c22 6874 7470 733a 2f2f   href=\"https://
+0002b7a0: 7079 6c69 6e74 2e70 7963 7161 2e6f 7267  pylint.pycqa.org
+0002b7b0: 2f65 6e2f 6c61 7465 7374 2f75 7365 725f  /en/latest/user_
+0002b7c0: 6775 6964 652f 6d65 7373 6167 6573 2f69  guide/messages/i
+0002b7d0: 6e66 6f72 6d61 7469 6f6e 2f66 696c 652d  nformation/file-
+0002b7e0: 6967 6e6f 7265 642e 6874 6d6c 5c22 3e41  ignored.html\">A
 0002b7f0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
 0002b800: 6174 696f 6e3c 2f61 3e22 0a0a 5b49 3030  ation</a>"..[I00
-0002b810: 3133 5d0a 7768 7920 3d20 2255 7365 6420  13].why = "Used 
-0002b820: 746f 2069 6e66 6f72 6d20 7468 6174 2074  to inform that t
-0002b830: 6865 2066 696c 6520 7769 6c6c 206e 6f74  he file will not
-0002b840: 2062 6520 6368 6563 6b65 6422 0a65 7861   be checked".exa
-0002b850: 6d70 6c65 7320 3d20 223c 6120 6872 6566  mples = "<a href
-0002b860: 3d5c 2268 7474 7073 3a2f 2f70 796c 696e  =\"https://pylin
-0002b870: 742e 7079 6371 612e 6f72 672f 656e 2f6c  t.pycqa.org/en/l
-0002b880: 6174 6573 742f 7573 6572 5f67 7569 6465  atest/user_guide
-0002b890: 2f6d 6573 7361 6765 732f 696e 666f 726d  /messages/inform
-0002b8a0: 6174 696f 6e2f 6669 6c65 2d69 676e 6f72  ation/file-ignor
-0002b8b0: 6564 2e68 746d 6c5c 223e 4164 6469 7469  ed.html\">Additi
-0002b8c0: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
-0002b8d0: 3c2f 613e 220a 0a5b 4930 3032 305d 0a77  </a>"..[I0020].w
-0002b8e0: 6879 203d 2022 4120 6d65 7373 6167 6520  hy = "A message 
-0002b8f0: 7761 7320 7472 6967 6765 7265 6420 6f6e  was triggered on
-0002b900: 2061 206c 696e 652c 2062 7574 2073 7570   a line, but sup
-0002b910: 7072 6573 7365 6420 6578 706c 6963 6974  pressed explicit
-0002b920: 6c79 2062 7920 6120 6469 7361 626c 653d  ly by a disable=
-0002b930: 2063 6f6d 6d65 6e74 2069 6e20 7468 6520   comment in the 
-0002b940: 6669 6c65 2e20 5468 6973 206d 6573 7361  file. This messa
-0002b950: 6765 2069 7320 6e6f 7420 6765 6e65 7261  ge is not genera
-0002b960: 7465 6420 666f 7220 6d65 7373 6167 6573  ted for messages
-0002b970: 2074 6861 7420 6172 6520 6967 6e6f 7265   that are ignore
-0002b980: 6420 6475 6520 746f 2063 6f6e 6669 6775  d due to configu
-0002b990: 7261 7469 6f6e 2073 6574 7469 6e67 732e  ration settings.
-0002b9a0: 220a 6578 616d 706c 6573 203d 2022 3c61  ".examples = "<a
-0002b9b0: 2068 7265 663d 5c22 6874 7470 733a 2f2f   href=\"https://
-0002b9c0: 7079 6c69 6e74 2e70 7963 7161 2e6f 7267  pylint.pycqa.org
-0002b9d0: 2f65 6e2f 6c61 7465 7374 2f75 7365 725f  /en/latest/user_
-0002b9e0: 6775 6964 652f 6d65 7373 6167 6573 2f69  guide/messages/i
-0002b9f0: 6e66 6f72 6d61 7469 6f6e 2f73 7570 7072  nformation/suppr
-0002ba00: 6573 7365 642d 6d65 7373 6167 652e 6874  essed-message.ht
-0002ba10: 6d6c 5c22 3e41 6464 6974 696f 6e61 6c20  ml\">Additional 
-0002ba20: 696e 666f 726d 6174 696f 6e3c 2f61 3e22  information</a>"
-0002ba30: 0a0a 5b49 3030 3231 5d0a 7768 7920 3d20  ..[I0021].why = 
-0002ba40: 2252 6570 6f72 7465 6420 7768 656e 2061  "Reported when a
-0002ba50: 206d 6573 7361 6765 2069 7320 6578 706c   message is expl
-0002ba60: 6963 6974 6c79 2064 6973 6162 6c65 6420  icitly disabled 
-0002ba70: 666f 7220 6120 6c69 6e65 206f 7220 6120  for a line or a 
-0002ba80: 626c 6f63 6b20 6f66 2063 6f64 652c 2062  block of code, b
-0002ba90: 7574 206e 6576 6572 2074 7269 6767 6572  ut never trigger
-0002baa0: 6564 2e22 0a65 7861 6d70 6c65 7320 3d20  ed.".examples = 
-0002bab0: 223c 6120 6872 6566 3d5c 2268 7474 7073  "<a href=\"https
-0002bac0: 3a2f 2f70 796c 696e 742e 7079 6371 612e  ://pylint.pycqa.
-0002bad0: 6f72 672f 656e 2f6c 6174 6573 742f 7573  org/en/latest/us
-0002bae0: 6572 5f67 7569 6465 2f6d 6573 7361 6765  er_guide/message
-0002baf0: 732f 696e 666f 726d 6174 696f 6e2f 7573  s/information/us
-0002bb00: 656c 6573 732d 7375 7070 7265 7373 696f  eless-suppressio
-0002bb10: 6e2e 6874 6d6c 5c22 3e41 6464 6974 696f  n.html\">Additio
-0002bb20: 6e61 6c20 696e 666f 726d 6174 696f 6e3c  nal information<
-0002bb30: 2f61 3e22 0a0a 5b49 3030 3232 5d0a 7768  /a>"..[I0022].wh
-0002bb40: 7920 3d20 2253 6f6d 6520 696e 6c69 6e65  y = "Some inline
-0002bb50: 2070 796c 696e 7420 6f70 7469 6f6e 7320   pylint options 
-0002bb60: 6861 7665 2062 6565 6e20 7265 6e61 6d65  have been rename
-0002bb70: 6420 6f72 2072 6577 6f72 6b65 642c 206f  d or reworked, o
-0002bb80: 6e6c 7920 7468 6520 6d6f 7374 2072 6563  nly the most rec
-0002bb90: 656e 7420 666f 726d 2073 686f 756c 6420  ent form should 
-0002bba0: 6265 2075 7365 642e 204e 4f54 453a 736b  be used. NOTE:sk
-0002bbb0: 6970 2d61 6c6c 2069 7320 6f6e 6c79 2061  ip-all is only a
-0002bbc0: 7661 696c 6162 6c65 2077 6974 6820 7079  vailable with py
-0002bbd0: 6c69 6e74 203e 3d20 302e 3236 220a 6578  lint >= 0.26".ex
-0002bbe0: 616d 706c 6573 203d 2022 3c61 2068 7265  amples = "<a hre
-0002bbf0: 663d 5c22 6874 7470 733a 2f2f 7079 6c69  f=\"https://pyli
-0002bc00: 6e74 2e70 7963 7161 2e6f 7267 2f65 6e2f  nt.pycqa.org/en/
-0002bc10: 6c61 7465 7374 2f75 7365 725f 6775 6964  latest/user_guid
-0002bc20: 652f 6d65 7373 6167 6573 2f69 6e66 6f72  e/messages/infor
-0002bc30: 6d61 7469 6f6e 2f64 6570 7265 6361 7465  mation/deprecate
-0002bc40: 642d 7072 6167 6d61 2e68 746d 6c5c 223e  d-pragma.html\">
-0002bc50: 4164 6469 7469 6f6e 616c 2069 6e66 6f72  Additional infor
-0002bc60: 6d61 7469 6f6e 3c2f 613e 220a 0a5b 4930  mation</a>"..[I0
-0002bc70: 3032 335d 0a77 6879 203d 2022 4974 206c  023].why = "It l
-0002bc80: 6f6f 6b73 206c 696b 6520 7468 6520 6d65  ooks like the me
-0002bc90: 7373 6167 6520 6973 2065 6e61 626c 6564  ssage is enabled
-0002bca0: 206f 7220 6469 7361 626c 6564 2062 7920   or disabled by 
-0002bcb0: 6964 2e22 0a65 7861 6d70 6c65 7320 3d20  id.".examples = 
-0002bcc0: 223c 6120 6872 6566 3d5c 2268 7474 7073  "<a href=\"https
-0002bcd0: 3a2f 2f70 796c 696e 742e 7079 6371 612e  ://pylint.pycqa.
-0002bce0: 6f72 672f 656e 2f6c 6174 6573 742f 7573  org/en/latest/us
-0002bcf0: 6572 5f67 7569 6465 2f6d 6573 7361 6765  er_guide/message
-0002bd00: 732f 696e 666f 726d 6174 696f 6e2f 7573  s/information/us
-0002bd10: 652d 7379 6d62 6f6c 6963 2d6d 6573 7361  e-symbolic-messa
-0002bd20: 6765 2d69 6e73 7465 6164 2e68 746d 6c5c  ge-instead.html\
-0002bd30: 223e 4164 6469 7469 6f6e 616c 2069 6e66  ">Additional inf
-0002bd40: 6f72 6d61 7469 6f6e 3c2f 613e 220a 0a5b  ormation</a>"..[
-0002bd50: 4931 3130 315d 0a77 6879 203d 2022 4974  I1101].why = "It
-0002bd60: 206c 6f6f 6b73 206c 696b 6520 7468 6520   looks like the 
-0002bd70: 7661 7269 6162 6c65 2069 7320 6163 6365  variable is acce
-0002bd80: 7373 6564 2066 6f72 206e 6f6e 2d65 7869  ssed for non-exi
-0002bd90: 7374 656e 7420 6d65 6d62 6572 206f 6620  stent member of 
-0002bda0: 4320 6578 7465 6e73 696f 6e2e 2044 7565  C extension. Due
-0002bdb0: 2074 6f20 756e 6176 6169 6c61 6269 6c69   to unavailabili
-0002bdc0: 7479 206f 6620 736f 7572 6365 2073 7461  ty of source sta
-0002bdd0: 7469 6320 616e 616c 7973 6973 2069 7320  tic analysis is 
-0002bde0: 696d 706f 7373 6962 6c65 2c20 6275 7420  impossible, but 
-0002bdf0: 6974 206d 6179 2062 6520 7065 7266 6f72  it may be perfor
-0002be00: 6d65 6420 6279 2069 6e74 726f 7370 6563  med by introspec
-0002be10: 7469 6e67 206c 6976 696e 6720 6f62 6a65  ting living obje
-0002be20: 6374 7320 696e 2072 756e 2d74 696d 652e  cts in run-time.
-0002be30: 220a 6578 616d 706c 6573 203d 2022 3c61  ".examples = "<a
-0002be40: 2068 7265 663d 5c22 6874 7470 733a 2f2f   href=\"https://
-0002be50: 7079 6c69 6e74 2e70 7963 7161 2e6f 7267  pylint.pycqa.org
-0002be60: 2f65 6e2f 6c61 7465 7374 2f75 7365 725f  /en/latest/user_
-0002be70: 6775 6964 652f 6d65 7373 6167 6573 2f69  guide/messages/i
-0002be80: 6e66 6f72 6d61 7469 6f6e 2f63 2d65 7874  nformation/c-ext
-0002be90: 656e 7369 6f6e 2d6e 6f2d 6d65 6d62 6572  ension-no-member
-0002bea0: 2e68 746d 6c5c 223e 4164 6469 7469 6f6e  .html\">Addition
-0002beb0: 616c 2069 6e66 6f72 6d61 7469 6f6e 3c2f  al information</
-0002bec0: 613e 220a 0a5b 5731 3631 335d 0a77 6879  a>"..[W1613].why
-0002bed0: 203d 2022 5573 6564 2077 6865 6e20 7468   = "Used when th
-0002bee0: 6520 7872 616e 6765 2062 7569 6c74 2d69  e xrange built-i
-0002bef0: 6e20 6675 6e63 7469 6f6e 2069 7320 7265  n function is re
-0002bf00: 6665 7265 6e63 6564 2028 6d69 7373 696e  ferenced (missin
-0002bf10: 6720 6672 6f6d 2050 7974 686f 6e20 3329  g from Python 3)
-0002bf20: 2e20 5573 6520 7261 6e67 6520 696e 7374  . Use range inst
-0002bf30: 6561 642e 220a 0a5b 5731 3632 305d 0a77  ead."..[W1620].w
-0002bf40: 6879 203d 2022 5573 6564 2066 6f72 2063  hy = "Used for c
-0002bf50: 616c 6c73 2074 6f20 6469 6374 2e69 7465  alls to dict.ite
-0002bf60: 726b 6579 7328 292c 2069 7465 7276 616c  rkeys(), iterval
-0002bf70: 7565 7328 2920 6f72 2069 7465 7269 7465  ues() or iterite
-0002bf80: 6d73 2829 2e20 5079 7468 6f6e 2033 206c  ms(). Python 3 l
-0002bf90: 6163 6b73 2074 6865 7365 206d 6574 686f  acks these metho
-0002bfa0: 6473 2c20 7573 6520 6469 6374 2e6b 6579  ds, use dict.key
-0002bfb0: 7328 292c 2076 616c 7565 7328 2920 6f72  s(), values() or
-0002bfc0: 2069 7465 6d73 2829 2e22 0a0a 5b57 3136   items()."..[W16
-0002bfd0: 3231 5d0a 7768 7920 3d20 2255 7365 6420  21].why = "Used 
-0002bfe0: 666f 7220 6361 6c6c 7320 746f 2064 6963  for calls to dic
-0002bff0: 742e 7669 6577 6b65 7973 2829 2c20 7669  t.viewkeys(), vi
-0002c000: 6577 7661 6c75 6573 2829 206f 7220 7669  ewvalues() or vi
-0002c010: 6577 6974 656d 7328 292e 2050 7974 686f  ewitems(). Pytho
-0002c020: 6e20 3320 6c61 636b 7320 7468 6573 6520  n 3 lacks these 
-0002c030: 6d65 7468 6f64 732c 2020 7573 6520 6469  methods,  use di
-0002c040: 6374 2e6b 6579 7328 292c 2076 616c 7565  ct.keys(), value
-0002c050: 7328 2920 6f72 2069 7465 6d73 2829 2e22  s() or items()."
-0002c060: 0a                                       .
+0002b810: 3230 5d0a 7768 7920 3d20 2241 206d 6573  20].why = "A mes
+0002b820: 7361 6765 2077 6173 2074 7269 6767 6572  sage was trigger
+0002b830: 6564 206f 6e20 6120 6c69 6e65 2c20 6275  ed on a line, bu
+0002b840: 7420 7375 7070 7265 7373 6564 2065 7870  t suppressed exp
+0002b850: 6c69 6369 746c 7920 6279 2061 2064 6973  licitly by a dis
+0002b860: 6162 6c65 3d20 636f 6d6d 656e 7420 696e  able= comment in
+0002b870: 2074 6865 2066 696c 652e 2054 6869 7320   the file. This 
+0002b880: 6d65 7373 6167 6520 6973 206e 6f74 2067  message is not g
+0002b890: 656e 6572 6174 6564 2066 6f72 206d 6573  enerated for mes
+0002b8a0: 7361 6765 7320 7468 6174 2061 7265 2069  sages that are i
+0002b8b0: 676e 6f72 6564 2064 7565 2074 6f20 636f  gnored due to co
+0002b8c0: 6e66 6967 7572 6174 696f 6e20 7365 7474  nfiguration sett
+0002b8d0: 696e 6773 2e22 0a65 7861 6d70 6c65 7320  ings.".examples 
+0002b8e0: 3d20 223c 6120 6872 6566 3d5c 2268 7474  = "<a href=\"htt
+0002b8f0: 7073 3a2f 2f70 796c 696e 742e 7079 6371  ps://pylint.pycq
+0002b900: 612e 6f72 672f 656e 2f6c 6174 6573 742f  a.org/en/latest/
+0002b910: 7573 6572 5f67 7569 6465 2f6d 6573 7361  user_guide/messa
+0002b920: 6765 732f 696e 666f 726d 6174 696f 6e2f  ges/information/
+0002b930: 7375 7070 7265 7373 6564 2d6d 6573 7361  suppressed-messa
+0002b940: 6765 2e68 746d 6c5c 223e 4164 6469 7469  ge.html\">Additi
+0002b950: 6f6e 616c 2069 6e66 6f72 6d61 7469 6f6e  onal information
+0002b960: 3c2f 613e 220a 0a5b 4930 3032 315d 0a77  </a>"..[I0021].w
+0002b970: 6879 203d 2022 5265 706f 7274 6564 2077  hy = "Reported w
+0002b980: 6865 6e20 6120 6d65 7373 6167 6520 6973  hen a message is
+0002b990: 2065 7870 6c69 6369 746c 7920 6469 7361   explicitly disa
+0002b9a0: 626c 6564 2066 6f72 2061 206c 696e 6520  bled for a line 
+0002b9b0: 6f72 2061 2062 6c6f 636b 206f 6620 636f  or a block of co
+0002b9c0: 6465 2c20 6275 7420 6e65 7665 7220 7472  de, but never tr
+0002b9d0: 6967 6765 7265 642e 220a 6578 616d 706c  iggered.".exampl
+0002b9e0: 6573 203d 2022 3c61 2068 7265 663d 5c22  es = "<a href=\"
+0002b9f0: 6874 7470 733a 2f2f 7079 6c69 6e74 2e70  https://pylint.p
+0002ba00: 7963 7161 2e6f 7267 2f65 6e2f 6c61 7465  ycqa.org/en/late
+0002ba10: 7374 2f75 7365 725f 6775 6964 652f 6d65  st/user_guide/me
+0002ba20: 7373 6167 6573 2f69 6e66 6f72 6d61 7469  ssages/informati
+0002ba30: 6f6e 2f75 7365 6c65 7373 2d73 7570 7072  on/useless-suppr
+0002ba40: 6573 7369 6f6e 2e68 746d 6c5c 223e 4164  ession.html\">Ad
+0002ba50: 6469 7469 6f6e 616c 2069 6e66 6f72 6d61  ditional informa
+0002ba60: 7469 6f6e 3c2f 613e 220a 0a5b 4930 3032  tion</a>"..[I002
+0002ba70: 325d 0a77 6879 203d 2022 536f 6d65 2069  2].why = "Some i
+0002ba80: 6e6c 696e 6520 7079 6c69 6e74 206f 7074  nline pylint opt
+0002ba90: 696f 6e73 2068 6176 6520 6265 656e 2072  ions have been r
+0002baa0: 656e 616d 6564 206f 7220 7265 776f 726b  enamed or rework
+0002bab0: 6564 2c20 6f6e 6c79 2074 6865 206d 6f73  ed, only the mos
+0002bac0: 7420 7265 6365 6e74 2066 6f72 6d20 7368  t recent form sh
+0002bad0: 6f75 6c64 2062 6520 7573 6564 2e20 4e4f  ould be used. NO
+0002bae0: 5445 3a73 6b69 702d 616c 6c20 6973 206f  TE:skip-all is o
+0002baf0: 6e6c 7920 6176 6169 6c61 626c 6520 7769  nly available wi
+0002bb00: 7468 2070 796c 696e 7420 3e3d 2030 2e32  th pylint >= 0.2
+0002bb10: 3622 0a65 7861 6d70 6c65 7320 3d20 223c  6".examples = "<
+0002bb20: 6120 6872 6566 3d5c 2268 7474 7073 3a2f  a href=\"https:/
+0002bb30: 2f70 796c 696e 742e 7079 6371 612e 6f72  /pylint.pycqa.or
+0002bb40: 672f 656e 2f6c 6174 6573 742f 7573 6572  g/en/latest/user
+0002bb50: 5f67 7569 6465 2f6d 6573 7361 6765 732f  _guide/messages/
+0002bb60: 696e 666f 726d 6174 696f 6e2f 6465 7072  information/depr
+0002bb70: 6563 6174 6564 2d70 7261 676d 612e 6874  ecated-pragma.ht
+0002bb80: 6d6c 5c22 3e41 6464 6974 696f 6e61 6c20  ml\">Additional 
+0002bb90: 696e 666f 726d 6174 696f 6e3c 2f61 3e22  information</a>"
+0002bba0: 0a0a 5b49 3030 3233 5d0a 7768 7920 3d20  ..[I0023].why = 
+0002bbb0: 2249 7420 6c6f 6f6b 7320 6c69 6b65 2074  "It looks like t
+0002bbc0: 6865 206d 6573 7361 6765 2069 7320 656e  he message is en
+0002bbd0: 6162 6c65 6420 6f72 2064 6973 6162 6c65  abled or disable
+0002bbe0: 6420 6279 2069 642e 220a 6578 616d 706c  d by id.".exampl
+0002bbf0: 6573 203d 2022 3c61 2068 7265 663d 5c22  es = "<a href=\"
+0002bc00: 6874 7470 733a 2f2f 7079 6c69 6e74 2e70  https://pylint.p
+0002bc10: 7963 7161 2e6f 7267 2f65 6e2f 6c61 7465  ycqa.org/en/late
+0002bc20: 7374 2f75 7365 725f 6775 6964 652f 6d65  st/user_guide/me
+0002bc30: 7373 6167 6573 2f69 6e66 6f72 6d61 7469  ssages/informati
+0002bc40: 6f6e 2f75 7365 2d73 796d 626f 6c69 632d  on/use-symbolic-
+0002bc50: 6d65 7373 6167 652d 696e 7374 6561 642e  message-instead.
+0002bc60: 6874 6d6c 5c22 3e41 6464 6974 696f 6e61  html\">Additiona
+0002bc70: 6c20 696e 666f 726d 6174 696f 6e3c 2f61  l information</a
+0002bc80: 3e22 0a0a 5b49 3131 3031 5d0a 7768 7920  >"..[I1101].why 
+0002bc90: 3d20 2249 7420 6c6f 6f6b 7320 6c69 6b65  = "It looks like
+0002bca0: 2074 6865 2076 6172 6961 626c 6520 6973   the variable is
+0002bcb0: 2061 6363 6573 7365 6420 666f 7220 6e6f   accessed for no
+0002bcc0: 6e2d 6578 6973 7465 6e74 206d 656d 6265  n-existent membe
+0002bcd0: 7220 6f66 2043 2065 7874 656e 7369 6f6e  r of C extension
+0002bce0: 2e20 4475 6520 746f 2075 6e61 7661 696c  . Due to unavail
+0002bcf0: 6162 696c 6974 7920 6f66 2073 6f75 7263  ability of sourc
+0002bd00: 6520 7374 6174 6963 2061 6e61 6c79 7369  e static analysi
+0002bd10: 7320 6973 2069 6d70 6f73 7369 626c 652c  s is impossible,
+0002bd20: 2062 7574 2069 7420 6d61 7920 6265 2070   but it may be p
+0002bd30: 6572 666f 726d 6564 2062 7920 696e 7472  erformed by intr
+0002bd40: 6f73 7065 6374 696e 6720 6c69 7669 6e67  ospecting living
+0002bd50: 206f 626a 6563 7473 2069 6e20 7275 6e2d   objects in run-
+0002bd60: 7469 6d65 2e22 0a65 7861 6d70 6c65 7320  time.".examples 
+0002bd70: 3d20 223c 6120 6872 6566 3d5c 2268 7474  = "<a href=\"htt
+0002bd80: 7073 3a2f 2f70 796c 696e 742e 7079 6371  ps://pylint.pycq
+0002bd90: 612e 6f72 672f 656e 2f6c 6174 6573 742f  a.org/en/latest/
+0002bda0: 7573 6572 5f67 7569 6465 2f6d 6573 7361  user_guide/messa
+0002bdb0: 6765 732f 696e 666f 726d 6174 696f 6e2f  ges/information/
+0002bdc0: 632d 6578 7465 6e73 696f 6e2d 6e6f 2d6d  c-extension-no-m
+0002bdd0: 656d 6265 722e 6874 6d6c 5c22 3e41 6464  ember.html\">Add
+0002bde0: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
+0002bdf0: 696f 6e3c 2f61 3e22 0a0a 5b57 3136 3133  ion</a>"..[W1613
+0002be00: 5d0a 7768 7920 3d20 2255 7365 6420 7768  ].why = "Used wh
+0002be10: 656e 2074 6865 2078 7261 6e67 6520 6275  en the xrange bu
+0002be20: 696c 742d 696e 2066 756e 6374 696f 6e20  ilt-in function 
+0002be30: 6973 2072 6566 6572 656e 6365 6420 286d  is referenced (m
+0002be40: 6973 7369 6e67 2066 726f 6d20 5079 7468  issing from Pyth
+0002be50: 6f6e 2033 292e 2055 7365 2072 616e 6765  on 3). Use range
+0002be60: 2069 6e73 7465 6164 2e22 0a0a 5b57 3136   instead."..[W16
+0002be70: 3230 5d0a 7768 7920 3d20 2255 7365 6420  20].why = "Used 
+0002be80: 666f 7220 6361 6c6c 7320 746f 2064 6963  for calls to dic
+0002be90: 742e 6974 6572 6b65 7973 2829 2c20 6974  t.iterkeys(), it
+0002bea0: 6572 7661 6c75 6573 2829 206f 7220 6974  ervalues() or it
+0002beb0: 6572 6974 656d 7328 292e 2050 7974 686f  eritems(). Pytho
+0002bec0: 6e20 3320 6c61 636b 7320 7468 6573 6520  n 3 lacks these 
+0002bed0: 6d65 7468 6f64 732c 2075 7365 2064 6963  methods, use dic
+0002bee0: 742e 6b65 7973 2829 2c20 7661 6c75 6573  t.keys(), values
+0002bef0: 2829 206f 7220 6974 656d 7328 292e 220a  () or items().".
+0002bf00: 0a5b 5731 3632 315d 0a77 6879 203d 2022  .[W1621].why = "
+0002bf10: 5573 6564 2066 6f72 2063 616c 6c73 2074  Used for calls t
+0002bf20: 6f20 6469 6374 2e76 6965 776b 6579 7328  o dict.viewkeys(
+0002bf30: 292c 2076 6965 7776 616c 7565 7328 2920  ), viewvalues() 
+0002bf40: 6f72 2076 6965 7769 7465 6d73 2829 2e20  or viewitems(). 
+0002bf50: 5079 7468 6f6e 2033 206c 6163 6b73 2074  Python 3 lacks t
+0002bf60: 6865 7365 206d 6574 686f 6473 2c20 2075  hese methods,  u
+0002bf70: 7365 2064 6963 742e 6b65 7973 2829 2c20  se dict.keys(), 
+0002bf80: 7661 6c75 6573 2829 206f 7220 6974 656d  values() or item
+0002bf90: 7328 292e 220a 0a5b 5236 3630 395d 0a77  s()."..[R6609].w
+0002bfa0: 6879 203d 2022 5573 696e 6720 6175 676d  hy = "Using augm
+0002bfb0: 656e 7465 6420 6173 7369 676e 2069 7320  ented assign is 
+0002bfc0: 6e6f 7420 6f6e 6c79 2073 686f 7274 6572  not only shorter
+0002bfd0: 2c20 6275 7420 616c 736f 2063 6c65 6172  , but also clear
+0002bfe0: 6572 2061 6e64 206c 6573 7320 7072 6f6e  er and less pron
+0002bff0: 6520 746f 2065 7272 6f72 732e 220a 6578  e to errors.".ex
+0002c000: 616d 706c 6573 203d 2022 466f 7220 6578  amples = "For ex
+0002c010: 616d 706c 652c 2069 6e73 7465 6164 206f  ample, instead o
+0002c020: 6620 7772 6974 696e 6720 6078 203d 2078  f writing `x = x
+0002c030: 202b 2031 602c 2079 6f75 2063 616e 2077   + 1`, you can w
+0002c040: 7269 7465 2060 7820 2b3d 2031 602e 2057  rite `x += 1`. W
+0002c050: 6f72 6b73 2066 6f72 2061 6c6d 6f73 7420  orks for almost 
+0002c060: 616e 7920 6f70 6572 6174 6f72 2e22 0a0a  any operator."..
+0002c070: 5b52 3632 3037 5d0a 7768 7920 3d20 2259  [R6207].why = "Y
+0002c080: 6f75 2073 686f 756c 6420 7573 6520 7369  ou should use si
+0002c090: 6e67 6c65 2060 6966 6020 7374 6174 656d  ngle `if` statem
+0002c0a0: 656e 7420 7769 7468 2063 6f6e 6469 7469  ent with conditi
+0002c0b0: 6f6e 7320 6a6f 696e 6564 2062 7920 6061  ons joined by `a
+0002c0c0: 6e64 6020 696e 7374 6561 6420 6f66 206e  nd` instead of n
+0002c0d0: 6573 7465 6420 6069 6660 2073 7461 7465  ested `if` state
+0002c0e0: 6d65 6e74 7320 6265 6361 7573 6520 636f  ments because co
+0002c0f0: 6465 2077 6974 6820 6e65 7374 6564 2060  de with nested `
+0002c100: 6966 6073 2069 7320 6861 7264 6572 2074  if`s is harder t
+0002c110: 6f20 7472 6163 653a 2074 6865 2072 6561  o trace: the rea
+0002c120: 6465 7220 6861 7320 746f 2063 6865 636b  der has to check
+0002c130: 2074 6865 7265 2069 7320 6e6f 2060 656c   there is no `el
+0002c140: 7365 6020 6f72 206f 7468 6572 2063 6f64  se` or other cod
+0002c150: 6520 6166 7465 7220 7468 6520 696e 6e65  e after the inne
+0002c160: 7220 6069 6660 2e22 0a65 7861 6d70 6c65  r `if`.".example
+0002c170: 7320 3d20 2222 220a 6060 6070 790a 6465  s = """.```py.de
+0002c180: 6620 7072 6f62 6c65 6d61 7469 6328 782c  f problematic(x,
+0002c190: 2079 293a 0a20 2020 2069 6620 7820 3e20   y):.    if x > 
+0002c1a0: 303a 0a20 2020 2020 2020 2069 6620 7920  0:.        if y 
+0002c1b0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+0002c1c0: 2070 7269 6e74 285c 2262 6f74 6820 7661   print(\"both va
+0002c1d0: 6c75 6573 2061 7265 2070 6f73 6974 6976  lues are positiv
+0002c1e0: 655c 2229 0a0a 6465 6620 676f 6f64 2878  e\")..def good(x
+0002c1f0: 2c20 7929 3a0a 2020 2020 6966 2078 203e  , y):.    if x >
+0002c200: 2030 2061 6e64 2079 203e 2030 3a0a 2020   0 and y > 0:.  
+0002c210: 2020 2020 2020 7072 696e 7428 5c22 626f        print(\"bo
+0002c220: 7468 2076 616c 7565 7320 6172 6520 706f  th values are po
+0002c230: 7369 7469 7665 5c22 290a 6060 600a 2222  sitive\").```.""
+0002c240: 220a 0a5b 5236 3630 355d 0a77 6879 203d  "..[R6605].why =
+0002c250: 2022 596f 7520 7368 6f75 6c64 2075 7365   "You should use
+0002c260: 2060 656c 6966 6020 6f76 6572 2060 656c   `elif` over `el
+0002c270: 7365 3a20 6966 602e 204f 7468 6572 7769  se: if`. Otherwi
+0002c280: 7365 2069 7420 6973 2068 6172 6465 7220  se it is harder 
+0002c290: 746f 2073 6565 2077 6861 7420 7468 6520  to see what the 
+0002c2a0: 706f 7373 6962 6c65 2062 7261 6e63 6865  possible branche
+0002c2b0: 7320 646f 2c20 6173 2074 6865 7920 6172  s do, as they ar
+0002c2c0: 6520 6e6f 7420 6f6e 2074 6865 2073 616d  e not on the sam
+0002c2d0: 6520 696e 6465 6e74 6174 696f 6e20 6c65  e indentation le
+0002c2e0: 7665 6c2e 220a 6578 616d 706c 6573 203d  vel.".examples =
+0002c2f0: 2022 2222 0a60 6060 7079 0a64 6566 2070   """.```py.def p
+0002c300: 726f 626c 656d 6174 6963 2878 293a 0a20  roblematic(x):. 
+0002c310: 2020 2069 6620 7820 3c20 303a 0a20 2020     if x < 0:.   
+0002c320: 2020 2020 2070 7269 6e74 285c 2278 2069       print(\"x i
+0002c330: 7320 6e65 6761 7469 7665 5c22 290a 2020  s negative\").  
+0002c340: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002c350: 6966 2078 203d 3d20 303a 0a20 2020 2020  if x == 0:.     
+0002c360: 2020 2020 2020 2070 7269 6e74 285c 2278         print(\"x
+0002c370: 2069 7320 7a65 726f 5c22 290a 2020 2020   is zero\").    
+0002c380: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0002c390: 2020 2020 2020 7072 696e 7428 5c22 7820        print(\"x 
+0002c3a0: 6973 2070 6f73 6974 6976 655c 2229 0a0a  is positive\")..
+0002c3b0: 6465 6620 676f 6f64 2878 293a 0a20 2020  def good(x):.   
+0002c3c0: 2069 6620 7820 3c20 303a 0a20 2020 2020   if x < 0:.     
+0002c3d0: 2020 2070 7269 6e74 285c 2278 2069 7320     print(\"x is 
+0002c3e0: 6e65 6761 7469 7665 5c22 290a 2020 2020  negative\").    
+0002c3f0: 656c 6966 2078 203d 3d20 303a 0a20 2020  elif x == 0:.   
+0002c400: 2020 2020 2070 7269 6e74 285c 2278 2069       print(\"x i
+0002c410: 7320 7a65 726f 5c22 290a 2020 2020 656c  s zero\").    el
+0002c420: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
+0002c430: 7428 5c22 7820 6973 2070 6f73 6974 6976  t(\"x is positiv
+0002c440: 655c 2229 0a60 6060 0a22 2222 0a0a 5b52  e\").```."""..[R
+0002c450: 3633 3035 5d0a 7768 7920 3d20 2255 7365  6305].why = "Use
+0002c460: 2060 666f 7260 206c 6f6f 7020 7768 656e   `for` loop when
+0002c470: 2079 6f75 206b 6e6f 7720 7468 6520 6e75   you know the nu
+0002c480: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+0002c490: 6e73 2069 6e20 6164 7661 6e63 6520 2865  ns in advance (e
+0002c4a0: 2e67 2e20 7468 6520 6e75 6d62 6572 206f  .g. the number o
+0002c4b0: 6620 6974 6572 6174 696f 6e73 2069 7320  f iterations is 
+0002c4c0: 636f 6e73 7461 6e74 206f 7220 7374 6f72  constant or stor
+0002c4d0: 6564 2069 6e20 6120 7661 7269 6162 6c65  ed in a variable
+0002c4e0: 292e 2055 7369 6e67 2061 2060 7768 696c  ). Using a `whil
+0002c4f0: 6560 206c 6f6f 7020 6973 206d 6f72 6520  e` loop is more 
+0002c500: 7665 7262 6f73 6520 616e 6420 6361 6e20  verbose and can 
+0002c510: 6c65 6164 2074 6f20 6572 726f 7273 2069  lead to errors i
+0002c520: 6620 796f 7520 666f 7267 6574 2074 6f20  f you forget to 
+0002c530: 696e 6372 656d 656e 7420 7468 6520 6974  increment the it
+0002c540: 6572 6174 696f 6e20 636f 756e 7465 722e  eration counter.
+0002c550: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
+0002c560: 0a60 6060 7079 0a64 6566 2070 726f 626c  .```py.def probl
+0002c570: 656d 6174 6963 286e 293a 0a20 2020 2069  ematic(n):.    i
+0002c580: 203d 2030 0a20 2020 2077 6869 6c65 2069   = 0.    while i
+0002c590: 203c 206e 3a0a 2020 2020 2020 2020 7072   < n:.        pr
+0002c5a0: 696e 7428 6929 0a20 2020 2020 2020 2069  int(i).        i
+0002c5b0: 202b 3d20 310a 0a64 6566 2067 6f6f 6428   += 1..def good(
+0002c5c0: 6e29 3a0a 2020 2020 666f 7220 6920 696e  n):.    for i in
+0002c5d0: 2072 616e 6765 286e 293a 0a20 2020 2020   range(n):.     
+0002c5e0: 2020 2070 7269 6e74 2869 290a 6060 600a     print(i).```.
+0002c5f0: 2222 220a 0a5b 5236 3230 385d 0a77 6879  """..[R6208].why
+0002c600: 203d 2022 596f 7520 7368 6f75 6c64 2075   = "You should u
+0002c610: 7365 2073 696e 676c 6520 6069 6660 2073  se single `if` s
+0002c620: 7461 7465 6d65 6e74 2077 6974 6820 636f  tatement with co
+0002c630: 6e64 6974 696f 6e73 206a 6f69 6e65 6420  nditions joined 
+0002c640: 6279 2060 6f72 6020 696e 7374 6561 6420  by `or` instead 
+0002c650: 6f66 2063 6f6e 7365 6375 7469 7665 2060  of consecutive `
+0002c660: 6966 6020 7374 6174 656d 656e 7473 2072  if` statements r
+0002c670: 6574 7572 6e69 6e67 2074 6865 2073 616d  eturning the sam
+0002c680: 6520 7661 6c75 652e 204f 7468 6572 7769  e value. Otherwi
+0002c690: 7365 2074 6865 2063 6f64 6520 6973 2075  se the code is u
+0002c6a0: 6e6e 6563 6573 7361 7269 6c79 206c 6f6e  nnecessarily lon
+0002c6b0: 672e 220a 6578 616d 706c 6573 203d 2022  g.".examples = "
+0002c6c0: 2222 0a66 726f 6d20 6d61 7468 2069 6d70  "".from math imp
+0002c6d0: 6f72 7420 7371 7274 0a0a 6465 6620 7072  ort sqrt..def pr
+0002c6e0: 6f62 6c65 6d61 7469 6328 782c 2079 293a  oblematic(x, y):
+0002c6f0: 0a20 2020 2069 6620 7820 3c20 303a 0a20  .    if x < 0:. 
+0002c700: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0002c710: 6e65 0a20 2020 2069 6620 7920 3c20 303a  ne.    if y < 0:
+0002c720: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002c730: 4e6f 6e65 0a20 2020 2072 6574 7572 6e20  None.    return 
+0002c740: 7371 7274 2878 202a 2079 290a 0a64 6566  sqrt(x * y)..def
+0002c750: 2067 6f6f 6428 782c 2079 293a 0a20 2020   good(x, y):.   
+0002c760: 2069 6620 7820 3c20 3020 6f72 2079 203c   if x < 0 or y <
+0002c770: 2030 3a0a 2020 2020 2020 2020 7265 7475   0:.        retu
+0002c780: 726e 204e 6f6e 650a 2020 2020 7265 7475  rn None.    retu
+0002c790: 726e 2073 7172 7428 7820 2a20 7929 0a22  rn sqrt(x * y)."
+0002c7a0: 2222 0a0a 5b52 3632 3032 5d0a 7768 7920  ""..[R6202].why 
+0002c7b0: 3d20 2249 6e20 736f 6d65 2063 6173 6573  = "In some cases
+0002c7c0: 2c20 7573 696e 6720 6c6f 6769 6361 6c20  , using logical 
+0002c7d0: 6f70 6572 6174 6f72 2063 616e 2073 696d  operator can sim
+0002c7e0: 706c 6966 7920 616e 2060 6966 6020 7374  plify an `if` st
+0002c7f0: 6174 656d 656e 7420 6576 656e 2069 6620  atement even if 
+0002c800: 6f6e 6520 6f66 2074 6865 2062 7261 6e63  one of the branc
+0002c810: 6865 7320 646f 6573 206e 6f74 2072 6574  hes does not ret
+0002c820: 7572 6e20 6120 626f 6f6c 2076 616c 7565  urn a bool value
+0002c830: 2e20 5573 696e 6720 6061 6e64 602c 2060  . Using `and`, `
+0002c840: 6f72 6020 616e 6420 6e65 6761 7469 6f6e  or` and negation
+0002c850: 2063 616e 206d 616b 6520 7468 6520 636f   can make the co
+0002c860: 6465 206d 6f72 6520 636f 6e63 6973 652e  de more concise.
+0002c870: 220a 6578 616d 706c 6573 203d 2022 2222  ".examples = """
+0002c880: 0a60 6060 7079 0a23 2061 2066 756e 6374  .```py.# a funct
+0002c890: 696f 6e20 6368 6563 6b69 6e67 2069 6620  ion checking if 
+0002c8a0: 6120 776f 7264 2073 7461 7274 7320 7769  a word starts wi
+0002c8b0: 7468 2041 0a0a 6465 6620 7072 6f62 6c65  th A..def proble
+0002c8c0: 6d61 7469 6328 776f 7264 293a 0a20 2020  matic(word):.   
+0002c8d0: 2069 6620 776f 7264 203d 3d20 5c22 5c22   if word == \"\"
+0002c8e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0002c8f0: 2046 616c 7365 0a20 2020 2072 6574 7572   False.    retur
+0002c900: 6e20 776f 7264 5b30 5d20 3d3d 205c 2241  n word[0] == \"A
+0002c910: 5c22 0a0a 6465 6620 676f 6f64 2877 6f72  \"..def good(wor
+0002c920: 6429 3a0a 2020 2020 7265 7475 726e 2077  d):.    return w
+0002c930: 6f72 6420 213d 205c 225c 2220 616e 6420  ord != \"\" and 
+0002c940: 776f 7264 5b30 5d20 3d3d 205c 2241 5c22  word[0] == \"A\"
+0002c950: 0a60 6060 0a22 2222 0a0a 5b52 3636 3033  .```."""..[R6603
+0002c960: 5d0a 7768 7920 3d20 2222 220a 5573 6520  ].why = """.Use 
+0002c970: 6069 7364 6563 696d 616c 602c 2062 6563  `isdecimal`, bec
+0002c980: 6175 7365 2069 7420 6973 206d 6f72 6520  ause it is more 
+0002c990: 7374 7269 6374 2061 6e64 206f 6e6c 7920  strict and only 
+0002c9a0: 616c 6c6f 7773 2072 6561 6c20 6465 6369  allows real deci
+0002c9b0: 6d61 6c20 6469 6769 7473 2074 6861 7420  mal digits that 
+0002c9c0: 6361 6e20 6265 2063 6f6e 7665 7274 6564  can be converted
+0002c9d0: 2074 6f20 6e75 6d62 6572 2075 7369 6e67   to number using
+0002c9e0: 2060 696e 7460 2e20 6069 736e 756d 6572   `int`. `isnumer
+0002c9f0: 6963 6020 616e 6420 6069 7364 6967 6974  ic` and `isdigit
+0002ca00: 6020 616c 736f 2072 6574 7572 6e20 6054  ` also return `T
+0002ca10: 7275 6560 2066 6f72 206f 7468 6572 206e  rue` for other n
+0002ca20: 756d 6572 6963 2063 6861 7261 6374 6572  umeric character
+0002ca30: 7320 6c69 6b65 2074 6865 7365 205c 22c2  s like these \".
+0002ca40: b9e2 8282 e291 a2c2 bce2 85a4 5c22 2e20  ............\". 
+0002ca50: 486f 7765 7665 722c 2069 6620 6120 7374  However, if a st
+0002ca60: 7269 6e67 2063 6f6e 7461 696e 7320 7468  ring contains th
+0002ca70: 6573 6520 6368 6172 6163 7465 7273 2c20  ese characters, 
+0002ca80: 6974 2063 616e 2070 6173 7320 7468 726f  it can pass thro
+0002ca90: 7567 6820 6069 736e 756d 6572 6963 6020  ugh `isnumeric` 
+0002caa0: 6f72 2060 6973 6469 6769 7460 2c20 6275  or `isdigit`, bu
+0002cab0: 7420 636f 6e76 6572 7469 6e67 2074 6865  t converting the
+0002cac0: 206e 756d 6265 7220 7573 696e 6720 6069   number using `i
+0002cad0: 6e74 6020 6661 696c 732e 0a0a 446f 206e  nt` fails...Do n
+0002cae0: 6f74 2072 656c 7920 6f6e 2066 756e 6374  ot rely on funct
+0002caf0: 696f 6e27 7320 6e61 6d65 2c20 6368 6563  ion's name, chec
+0002cb00: 6b20 6974 7320 646f 6375 6d65 6e74 6174  k its documentat
+0002cb10: 696f 6e20 3a29 2222 220a 0a5b 5236 3631  ion :)"""..[R661
+0002cb20: 335d 0a77 6879 203d 2022 2222 0a44 6f20  3].why = """.Do 
+0002cb30: 6e6f 7420 7573 6520 6069 7360 2077 6974  not use `is` wit
+0002cb40: 6820 626f 6f6c 2e20 4974 2069 7320 756e  h bool. It is un
+0002cb50: 6e65 6365 7373 6172 792c 2079 6f75 2063  necessary, you c
+0002cb60: 616e 2075 7365 2074 6865 2076 616c 7565  an use the value
+0002cb70: 2064 6972 6563 746c 792e 0a0a 4164 7661   directly...Adva
+0002cb80: 6e63 6564 206e 6f74 653a 2049 6620 796f  nced note: If yo
+0002cb90: 7520 6172 6520 676f 696e 6720 666f 7220  u are going for 
+0002cba0: 7468 7265 652d 7661 6c75 6564 206c 6f67  three-valued log
+0002cbb0: 6963 2028 6054 7275 6560 2c20 6046 616c  ic (`True`, `Fal
+0002cbc0: 7365 602c 2060 4e6f 6e65 6029 2c20 7472  se`, `None`), tr
+0002cbd0: 7920 7265 7374 7275 6374 7572 696e 6720  y restructuring 
+0002cbe0: 796f 7572 2063 6f64 6520 746f 2066 6972  your code to fir
+0002cbf0: 7374 2063 6f6d 7061 7265 2074 6f20 4e6f  st compare to No
+0002cc00: 6e65 2e20 5468 6973 2069 7320 6e6f 7420  ne. This is not 
+0002cc10: 7468 6520 6265 7374 2070 7261 6374 6963  the best practic
+0002cc20: 6520 6275 7420 7468 6572 6520 6973 206e  e but there is n
+0002cc30: 6f20 7761 7920 746f 2064 6966 6665 7265  o way to differe
+0002cc40: 6e74 6961 7465 206c 6567 6974 696d 6174  ntiate legitimat
+0002cc50: 6520 7573 6520 6f66 2060 6973 2062 6f6f  e use of `is boo
+0002cc60: 6c60 2066 726f 6d20 696c 6c65 6769 7469  l` from illegiti
+0002cc70: 6d61 7465 2e22 2222 0a65 7861 6d70 6c65  mate.""".example
+0002cc80: 7320 3d20 2255 7365 2060 636f 6e64 6020  s = "Use `cond` 
+0002cc90: 696e 7374 6561 6420 6f66 2060 636f 6e64  instead of `cond
+0002cca0: 2069 7320 5472 7565 6020 616e 6420 606e   is True` and `n
+0002ccb0: 6f74 2063 6f6e 6460 2069 6e73 7465 6164  ot cond` instead
+0002ccc0: 206f 6620 6063 6f6e 6420 6973 2046 616c   of `cond is Fal
+0002ccd0: 7365 602e 220a 0a5b 5236 3631 315d 0a77  se`."..[R6611].w
+0002cce0: 6879 203d 2022 4861 7669 6e67 2061 2064  hy = "Having a d
+0002ccf0: 7570 6c69 6361 7465 2063 6f6e 6469 7469  uplicate conditi
+0002cd00: 6f6e 2069 6e20 796f 7572 2063 6f64 6520  on in your code 
+0002cd10: 6361 6e20 6561 7369 6c79 2069 6e74 726f  can easily intro
+0002cd20: 6475 6365 2061 2062 7567 2e20 5573 6520  duce a bug. Use 
+0002cd30: 6065 6c73 6560 2069 6e73 7465 6164 206f  `else` instead o
+0002cd40: 6620 6065 6c69 6660 2077 6974 6820 6e65  f `elif` with ne
+0002cd50: 6761 7465 6420 636f 6e64 6974 696f 6e2c  gated condition,
+0002cd60: 206f 7220 6368 616e 6765 2074 6865 2063   or change the c
+0002cd70: 6f6e 6469 7469 6f6e 7320 6966 2074 6865  onditions if the
+0002cd80: 7920 6172 6520 6e6f 7420 7375 7070 6f73  y are not suppos
+0002cd90: 6564 2074 6f20 6265 206e 6567 6174 696f  ed to be negatio
+0002cda0: 6e73 206f 6620 6561 6368 206f 7468 6572  ns of each other
+0002cdb0: 2e22 0a65 7861 6d70 6c65 7320 3d20 2222  .".examples = ""
+0002cdc0: 220a 6060 6070 790a 6465 6620 7072 6f62  ".```py.def prob
+0002cdd0: 6c65 6d61 7469 6328 7829 3a0a 2020 2020  lematic(x):.    
+0002cde0: 6966 2078 203e 2030 3a0a 2020 2020 2020  if x > 0:.      
+0002cdf0: 2020 7072 696e 7428 5c22 6772 6561 7465    print(\"greate
+0002ce00: 7220 7468 616e 207a 6572 6f5c 2229 0a20  r than zero\"). 
+0002ce10: 2020 2065 6c69 6620 7820 3c3d 2030 3a0a     elif x <= 0:.
+0002ce20: 2020 2020 2020 2020 7072 696e 7428 5c22          print(\"
+0002ce30: 6c65 7373 6572 2074 6861 6e20 7a65 726f  lesser than zero
+0002ce40: 206f 7220 6571 7561 6c20 746f 2069 745c   or equal to it\
+0002ce50: 2229 0a0a 6465 6620 676f 6f64 3128 7829  ")..def good1(x)
+0002ce60: 3a0a 2020 2020 6966 2078 203e 2030 3a0a  :.    if x > 0:.
+0002ce70: 2020 2020 2020 2020 7072 696e 7428 5c22          print(\"
+0002ce80: 6772 6561 7465 7220 7468 616e 207a 6572  greater than zer
+0002ce90: 6f5c 2229 0a20 2020 2065 6c73 653a 0a20  o\").    else:. 
+0002cea0: 2020 2020 2020 2070 7269 6e74 285c 226c         print(\"l
+0002ceb0: 6573 7365 7220 7468 616e 207a 6572 6f20  esser than zero 
+0002cec0: 6f72 2065 7175 616c 2074 6f20 6974 5c22  or equal to it\"
+0002ced0: 290a 0a64 6566 2067 6f6f 6432 2878 293a  )..def good2(x):
+0002cee0: 0a20 2020 2069 6620 7820 3e20 303a 0a20  .    if x > 0:. 
+0002cef0: 2020 2020 2020 2070 7269 6e74 285c 2267         print(\"g
+0002cf00: 7265 6174 6572 2074 6861 6e20 7a65 726f  reater than zero
+0002cf10: 5c22 290a 2020 2020 656c 6966 2078 203c  \").    elif x <
+0002cf20: 2030 3a0a 2020 2020 2020 2020 7072 696e   0:.        prin
+0002cf30: 7428 5c22 6c65 7373 6572 2074 6861 6e20  t(\"lesser than 
+0002cf40: 7a65 726f 5c22 290a 6060 600a 2222 220a  zero\").```.""".
+0002cf50: 0a5b 5236 3630 385d 0a77 6879 203d 2022  .[R6608].why = "
+0002cf60: 5265 706c 6163 6520 6f70 6572 6174 696f  Replace operatio
+0002cf70: 6e73 2077 686f 7365 2072 6573 756c 7420  ns whose result 
+0002cf80: 646f 6573 206e 6f74 2064 6570 656e 6420  does not depend 
+0002cf90: 6f6e 2074 6865 2076 6172 6961 626c 6573  on the variables
+0002cfa0: 2077 6974 6820 7468 6569 7220 7265 7375   with their resu
+0002cfb0: 6c74 2e20 556e 6e65 6365 7373 6172 7920  lt. Unnecessary 
+0002cfc0: 6f70 6572 6174 696f 6e73 2069 6e20 636f  operations in co
+0002cfd0: 6465 2061 7265 2075 6e6e 6563 6573 7361  de are unnecessa
+0002cfe0: 7279 203a 2920 4275 7420 6d61 7962 6520  ry :) But maybe 
+0002cff0: 796f 7520 6d61 6465 2061 206d 6973 7461  you made a mista
+0002d000: 6b65 2069 6e20 7468 6520 7072 696f 7269  ke in the priori
+0002d010: 7479 206f 6620 616e 206f 7065 7261 746f  ty of an operato
+0002d020: 723f 220a 6578 616d 706c 6573 203d 2022  r?".examples = "
+0002d030: 2222 0a55 7365 2060 7860 2069 6e73 7465  "".Use `x` inste
+0002d040: 6164 206f 6620 6078 202b 2030 602c 2060  ad of `x + 0`, `
+0002d050: 7820 2a20 3160 2c20 6078 202b 205c 225c  x * 1`, `x + \"\
+0002d060: 2260 2c20 6f72 2060 7820 2b20 5b5d 602c  "`, or `x + []`,
+0002d070: 2060 3160 2069 6e73 7465 6164 206f 6620   `1` instead of 
+0002d080: 6078 202f 2078 6020 616e 6420 736f 206f  `x / x` and so o
+0002d090: 6e2e 0a0a 4966 2079 6f75 2077 616e 7420  n...If you want 
+0002d0a0: 746f 206d 616b 6520 6120 636f 7079 206f  to make a copy o
+0002d0b0: 6620 6120 6c69 7374 2c20 7573 6520 6974  f a list, use it
+0002d0c0: 7320 6063 6f70 7960 206d 6574 686f 642e  s `copy` method.
+0002d0d0: 0a0a 496e 2050 7974 686f 6e2c 2073 7472  ..In Python, str
+0002d0e0: 696e 6773 2061 7265 2069 6d6d 7574 6162  ings are immutab
+0002d0f0: 6c65 2c20 736f 2061 6464 696e 6720 616e  le, so adding an
+0002d100: 2065 6d70 7479 2073 7472 696e 6720 746f   empty string to
+0002d110: 205c 2263 7265 6174 6520 6120 636f 7079   \"create a copy
+0002d120: 5c22 2069 7320 756e 6e65 6365 7361 7279  \" is unnecesary
+0002d130: 2e20 416e 7920 6d6f 6469 6669 6361 7469  . Any modificati
+0002d140: 6f6e 2074 6f20 6120 6c69 7374 2063 7265  on to a list cre
+0002d150: 6174 6573 2061 2063 6f70 792e 0a22 2222  ates a copy.."""
+0002d160: 0a0a 5b52 3636 3037 5d0a 7768 7920 3d20  ..[R6607].why = 
+0002d170: 2259 6f75 2073 686f 756c 6420 7072 6566  "You should pref
+0002d180: 6572 206d 756c 7469 706c 6963 6174 696f  er multiplicatio
+0002d190: 6e2f 6578 706f 6e65 6e69 6174 696f 6e20  n/exponeniation 
+0002d1a0: 6f76 6572 2072 6570 6561 7469 6e67 2061  over repeating a
+0002d1b0: 6464 6974 696f 6e2f 6d75 6c74 6970 6c69  ddition/multipli
+0002d1c0: 6361 7469 6f6e 2e20 5573 696e 6720 7468  cation. Using th
+0002d1d0: 6520 6170 7072 6f70 7269 6174 6520 6f70  e appropriate op
+0002d1e0: 6572 6174 6f72 206d 616b 6573 2074 6865  erator makes the
+0002d1f0: 2063 6f64 6520 6d6f 7265 2072 6561 6461   code more reada
+0002d200: 626c 652c 2061 7320 796f 7520 6d61 6b65  ble, as you make
+0002d210: 2079 6f75 7220 696e 7465 6e74 696f 6e20   your intention 
+0002d220: 6d6f 7265 2065 7870 6c69 6369 742e 220a  more explicit.".
+0002d230: 6578 616d 706c 6573 203d 2022 5573 6520  examples = "Use 
+0002d240: 6078 202a 2032 6020 696e 7374 6561 6420  `x * 2` instead 
+0002d250: 6f66 2060 7820 2b20 7860 2061 6e64 2060  of `x + x` and `
+0002d260: 7820 2a2a 2032 6020 696e 7374 6561 6420  x ** 2` instead 
+0002d270: 6f66 2060 7820 2a20 7860 2e22 0a0a 5b52  of `x * x`."..[R
+0002d280: 3636 3031 5d0a 7768 7920 3d20 2241 766f  6601].why = "Avo
+0002d290: 6964 2063 7265 6174 696e 6720 7465 6d70  id creating temp
+0002d2a0: 6f72 6172 7920 7374 7275 6374 7572 652e  orary structure.
+0002d2b0: 2049 7420 6973 2069 6e65 6666 6963 6965   It is inefficie
+0002d2c0: 6e74 2061 6e64 2063 6f64 6520 7468 6174  nt and code that
+0002d2d0: 2075 7365 7320 7468 6520 636f 7272 6563   uses the correc
+0002d2e0: 7420 746f 6f6c 7320 6973 206d 6f72 6520  t tools is more 
+0002d2f0: 7265 6164 6162 6c65 2e22 0a65 7861 6d70  readable.".examp
+0002d300: 6c65 7320 3d20 2255 7365 2060 6c73 742e  les = "Use `lst.
+0002d310: 6170 7065 6e64 2876 616c 2960 2069 6e73  append(val)` ins
+0002d320: 7465 6164 206f 6620 606c 7374 202b 3d20  tead of `lst += 
+0002d330: 5b76 616c 5d60 2061 6e64 2060 6c73 742e  [val]` and `lst.
+0002d340: 6578 7465 6e64 2876 616c 2960 2e22 0a0a  extend(val)`."..
+0002d350: 5b52 3636 3032 5d0a 7768 7920 3d20 2244  [R6602].why = "D
+0002d360: 6563 696d 616c 206e 756d 6265 7273 2063  ecimal numbers c
+0002d370: 616e 6e6f 7420 6265 2072 6570 7265 7365  annot be represe
+0002d380: 6e74 6564 2070 7265 6369 7365 6c79 206f  nted precisely o
+0002d390: 6e20 6120 636f 6d70 7574 6572 2c20 636f  n a computer, co
+0002d3a0: 6e74 7261 7279 2074 6f20 696e 7465 6765  ntrary to intege
+0002d3b0: 7273 2e20 4279 2069 6e74 726f 6475 6369  rs. By introduci
+0002d3c0: 6e67 2066 6c6f 6174 2064 6976 6973 696f  ng float divisio
+0002d3d0: 6e2c 2079 6f75 7220 636f 6465 2073 7461  n, your code sta
+0002d3e0: 7274 7320 746f 2062 6568 6176 6520 696e  rts to behave in
+0002d3f0: 636f 7272 6563 746c 7920 7768 656e 206f  correctly when o
+0002d400: 7065 7261 7469 6e67 2077 6974 6820 7665  perating with ve
+0002d410: 7279 206c 6172 6765 206e 756d 6265 7273  ry large numbers
+0002d420: 2e22 0a65 7861 6d70 6c65 7320 3d20 2255  .".examples = "U
+0002d430: 7365 2069 6e74 6567 6572 2064 6976 6973  se integer divis
+0002d440: 696f 6e3a 2060 7820 2f2f 2079 6020 696e  ion: `x // y` in
+0002d450: 7374 6561 6420 6f66 2060 696e 7428 7820  stead of `int(x 
+0002d460: 2f20 7929 2e22 0a0a 5b52 3634 3031 5d0a  / y)."..[R6401].
+0002d470: 7768 7920 3d20 2255 7365 206f 6620 676c  why = "Use of gl
+0002d480: 6f62 616c 2076 6172 6961 626c 6573 206d  obal variables m
+0002d490: 616b 6573 2074 6865 2063 6f64 6520 6d75  akes the code mu
+0002d4a0: 6368 206c 6573 7320 7265 6164 6162 6c65  ch less readable
+0002d4b0: 2061 6e64 2074 7261 6365 6162 6c65 2c20   and traceable, 
+0002d4c0: 6173 2069 7420 6973 2068 6172 6420 746f  as it is hard to
+0002d4d0: 2061 6e74 6963 6970 6174 6520 616c 6c20   anticipate all 
+0002d4e0: 706f 7373 6962 6c65 2065 7865 6375 7469  possible executi
+0002d4f0: 6f6e 2070 6174 6873 2077 6865 6e20 7468  on paths when th
+0002d500: 6572 6520 6973 2067 6c6f 6261 6c20 7374  ere is global st
+0002d510: 6174 6520 696e 766f 6c76 6564 2e22 0a65  ate involved.".e
+0002d520: 7861 6d70 6c65 7320 3d20 2252 6573 7472  xamples = "Restr
+0002d530: 7563 7475 7265 2079 6f75 7220 636f 6465  ucture your code
+0002d540: 206e 6f74 2074 6f20 6e65 6564 2074 6865   not to need the
+0002d550: 2067 6c6f 6261 6c20 7661 7269 6162 6c65   global variable
+0002d560: 2e20 596f 7520 6361 6e20 646f 2074 6869  . You can do thi
+0002d570: 7320 6279 2070 6173 7369 6e67 2074 6865  s by passing the
+0002d580: 2076 616c 7565 2061 7320 6120 6675 6e63   value as a func
+0002d590: 7469 6f6e 2070 6172 616d 6574 6572 2061  tion parameter a
+0002d5a0: 6e64 2072 6574 7572 6e69 6e67 2074 6865  nd returning the
+0002d5b0: 2061 6c74 6572 6564 2076 6172 6961 7469   altered variati
+0002d5c0: 6f6e 2069 6e73 7465 6164 2e22 0a0a 5b52  on instead."..[R
+0002d5d0: 3636 3134 5d0a 7768 7920 3d20 2259 6f75  6614].why = "You
+0002d5e0: 7220 636f 6465 2075 7365 7320 6120 6d61  r code uses a ma
+0002d5f0: 6769 6320 6e75 6d62 6572 2e20 4120 6d61  gic number. A ma
+0002d600: 6769 6320 6e75 6d62 6572 2069 7320 6120  gic number is a 
+0002d610: 6e75 6d62 6572 2074 6861 7420 636f 6d65  number that come
+0002d620: 7320 6f75 7420 6f66 206e 6f77 6865 7265  s out of nowhere
+0002d630: 2061 6e64 2061 7420 6669 7273 7420 676c   and at first gl
+0002d640: 616e 6365 2c20 7468 6520 7265 6164 6572  ance, the reader
+0002d650: 2068 6173 206e 6f20 6964 6561 2077 6861   has no idea wha
+0002d660: 7420 6974 206d 6561 6e73 2e20 5573 696e  t it means. Usin
+0002d670: 6720 6d61 6769 6320 6e75 6d62 6572 7320  g magic numbers 
+0002d680: 6d61 6b65 7320 7468 6520 636f 6465 2075  makes the code u
+0002d690: 6e72 6561 6461 626c 6520 616e 6420 6361  nreadable and ca
+0002d6a0: 6e20 616c 736f 2072 6561 6420 746f 2062  n also read to b
+0002d6b0: 7567 732c 2061 7320 736f 6f6e 2061 7320  ugs, as soon as 
+0002d6c0: 7468 6520 636f 6465 2773 2077 7269 7465  the code's write
+0002d6d0: 7220 616c 736f 2066 6f72 6765 7473 2077  r also forgets w
+0002d6e0: 6861 7420 7468 6520 6d61 6769 6320 7661  hat the magic va
+0002d6f0: 6c75 6520 6d65 616e 732e 220a 6578 616d  lue means.".exam
+0002d700: 706c 6573 203d 2022 596f 7520 6361 6e20  ples = "You can 
+0002d710: 7573 6520 606f 7264 6020 746f 2063 6f6e  use `ord` to con
+0002d720: 7665 7274 2061 2063 6861 7261 6374 6572  vert a character
+0002d730: 2074 6f20 6974 7320 6e75 6d65 7269 6320   to its numeric 
+0002d740: 7661 6c75 652c 2075 7369 6e67 2074 6861  value, using tha
+0002d750: 7420 696e 7374 6561 6420 6f66 2074 6865  t instead of the
+0002d760: 206e 756d 6265 7220 6974 7365 6c66 2e20   number itself. 
+0002d770: 5468 6174 206d 6561 6e73 2c20 7573 6520  That means, use 
+0002d780: 606f 7264 2827 4127 2960 2069 6e73 7465  `ord('A')` inste
+0002d790: 6164 206f 6620 6036 3560 2e22 0a0a 5b52  ad of `65`."..[R
+0002d7a0: 3632 3035 5d0a 7768 7920 3d20 2245 6d70  6205].why = "Emp
+0002d7b0: 7479 2069 6620 636f 6e64 6974 696f 6e20  ty if condition 
+0002d7c0: 6d61 6b65 7320 7468 6520 636f 6465 2063  makes the code c
+0002d7d0: 6c75 7474 6572 6564 2061 6e64 2061 6c73  luttered and als
+0002d7e0: 6f20 6861 7264 6572 2074 6f20 7265 6164  o harder to read
+0002d7f0: 2028 7468 6520 7265 6164 6572 206d 7573   (the reader mus
+0002d800: 7420 6e65 6761 7465 2074 6865 2063 6f6e  t negate the con
+0002d810: 6469 7469 6f6e 2074 6865 6d73 656c 6620  dition themself 
+0002d820: 746f 2073 6565 2077 6865 6e20 7468 6520  to see when the 
+0002d830: 6065 6c73 6560 2062 7261 6e63 6820 6578  `else` branch ex
+0002d840: 6563 7574 6573 292e 220a 6578 616d 706c  ecutes).".exampl
+0002d850: 6573 203d 2022 2222 0a60 6060 7079 0a64  es = """.```py.d
+0002d860: 6566 2070 726f 626c 656d 6174 6963 2878  ef problematic(x
+0002d870: 293a 0a20 2020 2069 6620 7820 3c3d 2030  ):.    if x <= 0
+0002d880: 3a0a 2020 2020 2020 2020 7061 7373 0a20  :.        pass. 
+0002d890: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002d8a0: 2070 7269 6e74 285c 2267 7265 6174 6572   print(\"greater
+0002d8b0: 2074 6861 6e20 7a65 726f 5c22 290a 0a64   than zero\")..d
+0002d8c0: 6566 2067 6f6f 6428 7829 3a0a 2020 2020  ef good(x):.    
+0002d8d0: 6966 2078 203e 2030 3a0a 2020 2020 2020  if x > 0:.      
+0002d8e0: 2020 7072 696e 7428 5c22 6772 6561 7465    print(\"greate
+0002d8f0: 7220 7468 616e 207a 6572 6f5c 2229 0a60  r than zero\").`
+0002d900: 6060 0a22 2222 0a0a 5b52 3636 3135 5d0a  ``."""..[R6615].
+0002d910: 7768 7920 3d20 2259 6f75 7220 636f 6465  why = "Your code
+0002d920: 2075 7365 7320 6120 6d61 6769 6320 6e75   uses a magic nu
+0002d930: 6d62 6572 2e20 4120 6d61 6769 6320 6e75  mber. A magic nu
+0002d940: 6d62 6572 2069 7320 6120 6e75 6d62 6572  mber is a number
+0002d950: 2074 6861 7420 636f 6d65 7320 6f75 7420   that comes out 
+0002d960: 6f66 206e 6f77 6865 7265 2061 6e64 2061  of nowhere and a
+0002d970: 7420 6669 7273 7420 676c 616e 6365 2c20  t first glance, 
+0002d980: 7468 6520 7265 6164 6572 2068 6173 206e  the reader has n
+0002d990: 6f20 6964 6561 2077 6861 7420 6974 206d  o idea what it m
+0002d9a0: 6561 6e73 2e20 5573 696e 6720 6d61 6769  eans. Using magi
+0002d9b0: 6320 6e75 6d62 6572 7320 6d61 6b65 7320  c numbers makes 
+0002d9c0: 7468 6520 636f 6465 2075 6e72 6561 6461  the code unreada
+0002d9d0: 626c 6520 616e 6420 6361 6e20 616c 736f  ble and can also
+0002d9e0: 2072 6561 6420 746f 2062 7567 732c 2061   read to bugs, a
+0002d9f0: 7320 736f 6f6e 2061 7320 7468 6520 636f  s soon as the co
+0002da00: 6465 2773 2077 7269 7465 7220 616c 736f  de's writer also
+0002da10: 2066 6f72 6765 7473 2077 6861 7420 7468   forgets what th
+0002da20: 6520 6d61 6769 6320 7661 6c75 6520 6d65  e magic value me
+0002da30: 616e 732e 220a 6578 616d 706c 6573 203d  ans.".examples =
+0002da40: 2022 2222 0a49 6e20 5079 7468 6f6e 2c20   """.In Python, 
+0002da50: 796f 7520 6361 6e20 636f 6d70 6172 6520  you can compare 
+0002da60: 6368 6172 6163 7465 7273 2064 6972 6563  characters direc
+0002da70: 746c 792e 2054 6865 7265 666f 7265 2c20  tly. Therefore, 
+0002da80: 796f 7520 6361 6e20 6472 6f70 2074 6865  you can drop the
+0002da90: 2063 616c 6c20 746f 2060 6f72 6460 2061   call to `ord` a
+0002daa0: 6e64 2063 6f6d 7061 7265 2074 6865 206c  nd compare the l
+0002dab0: 6574 7465 7273 2064 6972 6563 746c 793a  etters directly:
+0002dac0: 2075 7365 2060 6c65 7474 6572 203e 2027   use `letter > '
+0002dad0: 4127 6020 696e 7374 6561 6420 6f66 2060  A'` instead of `
+0002dae0: 6f72 6428 6c65 7474 6572 2920 3e20 3635  ord(letter) > 65
+0002daf0: 602e 0a0a 4966 2079 6f75 2064 6f20 6e6f  `...If you do no
+0002db00: 7420 6c69 6b65 2074 6865 2069 6465 6120  t like the idea 
+0002db10: 6f66 2063 6f6d 7061 7269 6e67 206c 6574  of comparing let
+0002db20: 7465 7273 2c20 796f 7520 6361 6e20 7573  ters, you can us
+0002db30: 6520 606f 7264 286c 6574 7465 7229 203e  e `ord(letter) >
+0002db40: 206f 7264 2827 4127 2960 2e20 426f 7468   ord('A')`. Both
+0002db50: 2061 7265 2062 6574 7465 7220 7468 616e   are better than
+0002db60: 2075 7369 6e67 206d 6167 6963 206e 756d   using magic num
+0002db70: 6265 7273 2e0a 2222 220a 0a5b 5236 3230  bers.."""..[R620
+0002db80: 345d 0a77 6879 203d 2022 4861 7669 6e67  4].why = "Having
+0002db90: 2075 6e6e 6563 6573 7361 7279 2063 6f6e   unnecessary con
+0002dba0: 6469 7469 6f6e 7320 696e 2063 6f64 6520  ditions in code 
+0002dbb0: 6d61 6b65 7320 7468 6520 636f 6465 206d  makes the code m
+0002dbc0: 6f72 6520 636c 7574 7465 7265 6420 616e  ore cluttered an
+0002dbd0: 6420 7468 6572 6566 6f72 6520 6861 7264  d therefore hard
+0002dbe0: 6572 2074 6f20 756e 6465 7273 7461 6e64  er to understand
+0002dbf0: 2e22 0a65 7861 6d70 6c65 7320 3d20 2255  .".examples = "U
+0002dc00: 7365 2060 7820 3e20 3060 2069 6e73 7465  se `x > 0` inste
+0002dc10: 6164 206f 6620 6054 7275 6520 6966 2078  ad of `True if x
+0002dc20: 203e 2030 2065 6c73 6520 4661 6c73 6560   > 0 else False`
+0002dc30: 2e22 0a0a 5b52 3636 3034 5d0a 7768 7920  ."..[R6604].why 
+0002dc40: 3d20 224c 6f6f 7073 2077 6974 6820 6065  = "Loops with `e
+0002dc50: 6c73 6560 2062 7261 6e63 6820 6172 6520  lse` branch are 
+0002dc60: 6861 7264 6572 2074 6f20 7472 6163 652c  harder to trace,
+0002dc70: 2073 6f20 7573 696e 6720 7468 656d 2069   so using them i
+0002dc80: 7320 7072 6f6e 6520 746f 2061 6e20 6572  s prone to an er
+0002dc90: 726f 722e 204f 7220 6d61 7962 6520 796f  ror. Or maybe yo
+0002dca0: 7520 6469 6420 6e6f 7420 7265 616c 697a  u did not realiz
+0002dcb0: 6520 7468 6174 2061 206c 6f6f 7020 646f  e that a loop do
+0002dcc0: 6573 206e 6f74 2068 6176 6520 746f 2068  es not have to h
+0002dcd0: 6176 6520 616e 2060 656c 7365 6020 6272  ave an `else` br
+0002dce0: 616e 6368 3f22 0a65 7861 6d70 6c65 7320  anch?".examples 
+0002dcf0: 3d20 2222 220a 446f 6573 2079 6f75 7220  = """.Does your 
+0002dd00: 636f 6465 206d 616b 6520 7573 6520 6f66  code make use of
+0002dd10: 2074 6865 2060 656c 7365 6020 6272 616e   the `else` bran
+0002dd20: 6368 3f20 4d61 7962 6520 796f 7520 6361  ch? Maybe you ca
+0002dd30: 6e20 6a75 7374 2064 726f 7020 6974 2061  n just drop it a
+0002dd40: 6e64 2063 6f6e 7469 6e75 6520 7468 6520  nd continue the 
+0002dd50: 636f 6465 2061 6674 6572 2075 6e69 6e64  code after unind
+0002dd60: 656e 7465 643f 0a0a 6060 6070 790a 6465  ented?..```py.de
+0002dd70: 6620 7072 6f62 6c65 6d61 7469 6328 6e75  f problematic(nu
+0002dd80: 6d62 6572 7329 3a0a 2020 2020 666f 7220  mbers):.    for 
+0002dd90: 6e75 6d20 696e 206e 756d 6265 7273 3a0a  num in numbers:.
+0002dda0: 2020 2020 2020 2020 6966 206e 756d 203e          if num >
+0002ddb0: 2031 3030 3a0a 2020 2020 2020 2020 2020   100:.          
+0002ddc0: 2020 7072 696e 7428 5c22 466f 756e 6420    print(\"Found 
+0002ddd0: 6e75 6d62 6572 2067 7265 6174 6572 2074  number greater t
+0002dde0: 6861 6e20 3130 302e 5c22 290a 2020 2020  han 100.\").    
+0002ddf0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+0002de00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002de10: 7072 696e 7428 5c22 416c 6c20 6e75 6d62  print(\"All numb
+0002de20: 6572 7320 6172 6520 6c65 7373 6572 206f  ers are lesser o
+0002de30: 7220 6571 7561 6c20 746f 2031 3030 2e5c  r equal to 100.\
+0002de40: 2229 0a0a 0a64 6566 2063 6f6e 7461 696e  ")...def contain
+0002de50: 735f 6162 6f76 6528 6e75 6d62 6572 732c  s_above(numbers,
+0002de60: 206c 696d 6974 293a 0a20 2020 2066 6f72   limit):.    for
+0002de70: 206e 756d 2069 6e20 6e75 6d62 6572 733a   num in numbers:
+0002de80: 0a20 2020 2020 2020 2069 6620 6e75 6d20  .        if num 
+0002de90: 3e20 6c69 6d69 743a 0a20 2020 2020 2020  > limit:.       
+0002dea0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0002deb0: 0a20 2020 2072 6574 7572 6e20 4661 6c73  .    return Fals
+0002dec0: 650a 0a64 6566 2067 6f6f 6428 6e75 6d62  e..def good(numb
+0002ded0: 6572 7329 3a0a 2020 2020 6966 2063 6f6e  ers):.    if con
+0002dee0: 7461 696e 735f 6162 6f76 6528 6e75 6d62  tains_above(numb
+0002def0: 6572 732c 2031 3030 293a 0a20 2020 2020  ers, 100):.     
+0002df00: 2020 2070 7269 6e74 285c 2246 6f75 6e64     print(\"Found
+0002df10: 206e 756d 6265 7220 6772 6561 7465 7220   number greater 
+0002df20: 7468 616e 2031 3030 2e5c 2229 0a20 2020  than 100.\").   
+0002df30: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
+0002df40: 7269 6e74 285c 2241 6c6c 206e 756d 6265  rint(\"All numbe
+0002df50: 7273 2061 7265 206c 6573 7365 7220 6f72  rs are lesser or
+0002df60: 2065 7175 616c 2074 6f20 3130 302e 5c22   equal to 100.\"
+0002df70: 290a 6060 600a 2222 220a 0a5b 5236 3330  ).```."""..[R630
+0002df80: 335d 0a77 6879 203d 2022 4164 6469 6e67  3].why = "Adding
+0002df90: 2065 6c65 6d65 6e74 7320 746f 2061 2073   elements to a s
+0002dfa0: 7472 7563 7475 7265 2079 6f75 2069 7465  tructure you ite
+0002dfb0: 7261 7465 206f 7665 7220 6f72 2072 656d  rate over or rem
+0002dfc0: 6f76 696e 6720 656c 656d 656e 7473 2066  oving elements f
+0002dfd0: 726f 6d20 6974 2063 616e 206c 6561 6420  rom it can lead 
+0002dfe0: 746f 2075 6e65 7870 6563 7465 6420 6265  to unexpected be
+0002dff0: 6861 7669 6f72 2061 6e64 2074 6f20 6275  havior and to bu
+0002e000: 6773 2e22 0a65 7861 6d70 6c65 7320 3d20  gs.".examples = 
+0002e010: 2222 220a 6060 6070 790a 2320 6675 6e63  """.```py.# func
+0002e020: 7469 6f6e 2077 6869 6368 2072 656d 6f76  tion which remov
+0002e030: 6573 2065 7665 6e20 6e75 6d62 6572 7320  es even numbers 
+0002e040: 6672 6f6d 2061 206c 6973 740a 0a64 6566  from a list..def
+0002e050: 2070 726f 626c 656d 6174 6963 286e 756d   problematic(num
+0002e060: 6265 7273 293a 0a20 2020 2066 6f72 206e  bers):.    for n
+0002e070: 756d 2069 6e20 6e75 6d62 6572 733a 0a20  um in numbers:. 
+0002e080: 2020 2020 2020 2069 6620 6e75 6d20 2520         if num % 
+0002e090: 3220 3d3d 2030 3a0a 2020 2020 2020 2020  2 == 0:.        
+0002e0a0: 2020 2020 6e75 6d62 6572 732e 7265 6d6f      numbers.remo
+0002e0b0: 7665 286e 756d 290a 2020 2020 7265 7475  ve(num).    retu
+0002e0c0: 726e 206e 756d 6265 7273 0a0a 6465 6620  rn numbers..def 
+0002e0d0: 676f 6f64 286e 756d 6265 7273 293a 0a20  good(numbers):. 
+0002e0e0: 2020 2023 206e 6f77 2074 6865 2063 6f64     # now the cod
+0002e0f0: 6520 6974 6572 6174 6573 206f 7665 7220  e iterates over 
+0002e100: 6120 636f 7079 2c20 6275 7420 6d6f 6469  a copy, but modi
+0002e110: 6669 6573 2074 6865 206f 7269 6769 6e61  fies the origina
+0002e120: 6c20 7661 6c75 650a 2020 2020 666f 7220  l value.    for 
+0002e130: 6e75 6d20 696e 206e 756d 6265 7273 2e63  num in numbers.c
+0002e140: 6f70 7928 293a 0a20 2020 2020 2020 2069  opy():.        i
+0002e150: 6620 6e75 6d20 2520 3220 3d3d 2030 3a0a  f num % 2 == 0:.
+0002e160: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+0002e170: 6572 732e 7265 6d6f 7665 286e 756d 290a  ers.remove(num).
+0002e180: 2020 2020 7265 7475 726e 206e 756d 6265      return numbe
+0002e190: 7273 0a0a 6465 6620 676f 6f64 5f61 6e64  rs..def good_and
+0002e1a0: 5f65 6666 6963 6965 6e74 286e 756d 6265  _efficient(numbe
+0002e1b0: 7273 293a 0a20 2020 206f 6464 5f6e 756d  rs):.    odd_num
+0002e1c0: 6265 7273 203d 205b 5d0a 2020 2020 666f  bers = [].    fo
+0002e1d0: 7220 6e75 6d20 696e 206e 756d 6265 7273  r num in numbers
+0002e1e0: 3a0a 2020 2020 2020 2020 6966 206e 756d  :.        if num
+0002e1f0: 2025 2032 203d 3d20 313a 0a20 2020 2020   % 2 == 1:.     
+0002e200: 2020 2020 2020 206f 6464 5f6e 756d 6265         odd_numbe
+0002e210: 7273 2e61 7070 656e 6428 6e75 6d29 0a20  rs.append(num). 
+0002e220: 2020 2072 6574 7572 6e20 6f64 645f 6e75     return odd_nu
+0002e230: 6d62 6572 730a 6060 600a 2222 220a 0a5b  mbers.```."""..[
+0002e240: 5236 3330 365d 0a77 6879 203d 2022 5368  R6306].why = "Sh
+0002e250: 6164 6f77 696e 6720 7661 7269 6162 6c65  adowing variable
+0002e260: 206e 616d 6573 2069 7320 6572 726f 722d   names is error-
+0002e270: 7072 6f6e 652e 220a 6578 616d 706c 6573  prone.".examples
+0002e280: 203d 2022 2222 0a60 6060 7079 0a23 2066   = """.```py.# f
+0002e290: 756e 6374 696f 6e20 7468 6174 2070 7269  unction that pri
+0002e2a0: 6e74 7320 6120 7265 6374 616e 676c 6520  nts a rectangle 
+0002e2b0: 6672 6f6d 2023 2074 6861 7420 6861 7320  from # that has 
+0002e2c0: 6e20 726f 7773 2061 6e64 206d 2063 6f6c  n rows and m col
+0002e2d0: 756d 6e73 0a0a 6465 6620 7072 6f62 6c65  umns..def proble
+0002e2e0: 6d61 7469 6328 6e2c 206d 293a 0a20 2020  matic(n, m):.   
+0002e2f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0002e300: 6e29 3a0a 2020 2020 2020 2020 666f 7220  n):.        for 
+0002e310: 6920 696e 2072 616e 6765 286d 293a 0a20  i in range(m):. 
+0002e320: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0002e330: 285c 2223 5c22 2c20 656e 643d 5c22 5c22  (\"#\", end=\"\"
+0002e340: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0002e350: 290a 0a64 6566 2067 6f6f 6428 6e2c 206d  )..def good(n, m
+0002e360: 293a 0a20 2020 2066 6f72 2069 2069 6e20  ):.    for i in 
+0002e370: 7261 6e67 6528 6e29 3a0a 2020 2020 2020  range(n):.      
+0002e380: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+0002e390: 286d 293a 0a20 2020 2020 2020 2020 2020  (m):.           
+0002e3a0: 2070 7269 6e74 285c 2223 5c22 2c20 656e   print(\"#\", en
+0002e3b0: 643d 5c22 5c22 290a 2020 2020 2020 2020  d=\"\").        
+0002e3c0: 7072 696e 7428 290a 6060 600a 496e 2074  print().```.In t
+0002e3d0: 6865 2070 726f 626c 656d 6174 6963 2063  he problematic c
+0002e3e0: 6f64 652c 2062 6f74 6820 6066 6f72 6020  ode, both `for` 
+0002e3f0: 6c6f 6f70 7320 6861 7665 2060 6960 2061  loops have `i` a
+0002e400: 7320 7468 6569 7220 7461 7267 6574 2e20  s their target. 
+0002e410: 4974 2069 7320 6265 7474 6572 2074 6f20  It is better to 
+0002e420: 6769 7665 206e 6573 7465 6420 6c6f 6f70  give nested loop
+0002e430: 7320 6469 6666 6572 656e 7420 7661 7269  s different vari
+0002e440: 6162 6c65 206e 616d 6573 2c20 6576 656e  able names, even
+0002e450: 2069 6620 796f 7520 646f 206e 6f74 2075   if you do not u
+0002e460: 7365 2074 6865 6d2e 0a22 2222 0a0a 5b52  se them.."""..[R
+0002e470: 3633 3034 5d0a 7768 7920 3d20 224d 6f64  6304].why = "Mod
+0002e480: 6966 7969 6e67 2074 6865 2063 6f6e 7472  ifying the contr
+0002e490: 6f6c 2076 6172 6961 626c 6520 6174 2074  ol variable at t
+0002e4a0: 6865 2065 6e64 206f 6620 6120 6066 6f72  he end of a `for
+0002e4b0: 6020 6c6f 6f70 2068 6173 206e 6f20 6566  ` loop has no ef
+0002e4c0: 6665 6374 2e20 496e 2050 7974 686f 6e2c  fect. In Python,
+0002e4d0: 2074 6865 2060 666f 7260 206c 6f6f 7020   the `for` loop 
+0002e4e0: 6974 7365 6c66 2074 616b 6573 2063 6172  itself takes car
+0002e4f0: 6520 6f66 2061 7373 6967 6e69 6e67 206e  e of assigning n
+0002e500: 6577 2076 616c 7565 2069 6e20 6561 6368  ew value in each
+0002e510: 2069 7465 7261 7469 6f6e 2e22 0a65 7861   iteration.".exa
+0002e520: 6d70 6c65 7320 3d20 2259 6f75 2063 616e  mples = "You can
+0002e530: 206a 7573 7420 7265 6d6f 7665 2074 6865   just remove the
+0002e540: 206c 696e 6520 7768 6963 6820 6d6f 6469   line which modi
+0002e550: 6669 6573 2074 6865 2076 6172 6961 626c  fies the variabl
+0002e560: 652e 220a 0a5b 5236 3330 325d 0a65 7861  e."..[R6302].exa
+0002e570: 6d70 6c65 7320 3d20 2222 220a 6060 6070  mples = """.```p
+0002e580: 790a 6465 6620 7072 6f62 6c65 6d61 7469  y.def problemati
+0002e590: 6328 6e29 3a0a 2020 2020 666f 7220 6920  c(n):.    for i 
+0002e5a0: 696e 2072 616e 6765 286e 293a 0a20 2020  in range(n):.   
+0002e5b0: 2020 2020 2069 6620 6920 3d3d 2030 3a0a       if i == 0:.
+0002e5c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0002e5d0: 696e 7565 0a20 2020 2020 2020 2023 2073  inue.        # s
+0002e5e0: 6f6d 6520 636f 6465 0a0a 6465 6620 676f  ome code..def go
+0002e5f0: 6f64 286e 293a 0a20 2020 2066 6f72 2069  od(n):.    for i
+0002e600: 2069 6e20 7261 6e67 6528 312c 206e 293a   in range(1, n):
+0002e610: 0a20 2020 2020 2020 2023 2073 6f6d 6520  .        # some 
+0002e620: 636f 6465 0a60 6060 0a22 2222 0a0a 5b52  code.```."""..[R
+0002e630: 3636 3130 5d0a 7768 7920 3d20 2222 220a  6610].why = """.
+0002e640: 496e 2050 7974 686f 6e2c 206d 756c 7469  In Python, multi
+0002e650: 706c 7969 6e67 2061 206c 6973 7420 6372  plying a list cr
+0002e660: 6561 7465 7320 6120 6c69 7374 206f 6620  eates a list of 
+0002e670: 7265 6665 7265 6e63 6573 205f 746f 2074  references _to t
+0002e680: 6865 2073 616d 6520 696e 7374 616e 6365  he same instance
+0002e690: 5f20 6f66 2074 6865 206f 626a 6563 7420  _ of the object 
+0002e6a0: 7468 6520 6c69 7374 2063 6f6e 7461 696e  the list contain
+0002e6b0: 732e 2053 6565 2074 6865 2066 6f6c 6c6f  s. See the follo
+0002e6c0: 7769 6e67 2063 6f64 653a 0a0a 6060 600a  wing code:..```.
+0002e6d0: 6c73 7420 3d20 5b5b 5d5d 202a 2033 0a6c  lst = [[]] * 3.l
+0002e6e0: 7374 5b30 5d2e 6170 7065 6e64 2834 3229  st[0].append(42)
+0002e6f0: 0a60 6060 0a0a 606c 7374 6020 6e6f 7720  .```..`lst` now 
+0002e700: 6571 7561 6c73 2060 5b5b 3432 5d2c 205b  equals `[[42], [
+0002e710: 3432 5d2c 205b 3432 5d5d 2028 7472 7920  42], [42]] (try 
+0002e720: 6974 2129 2e0a 2222 220a 6578 616d 706c  it!)..""".exampl
+0002e730: 6573 203d 2022 496e 7374 6561 6420 6f66  es = "Instead of
+0002e740: 2060 5b5b 5d5d 202a 2033 6020 7573 6520   `[[]] * 3` use 
+0002e750: 666f 7220 6578 616d 706c 6520 605b 5b5d  for example `[[]
+0002e760: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0002e770: 3329 5d60 2e22 0a                        3)]`.".
```

### Comparing `edulint-2.6.2/edulint/linters.py` & `edulint-2.6.3/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/.pylintrc` & `edulint-2.6.3/edulint/linting/.pylintrc`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/basic_checker.py` & `edulint-2.6.3/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/improper_loop.py` & `edulint-2.6.3/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/modified_listener.py` & `edulint-2.6.3/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.6.3/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/short_problems.py` & `edulint-2.6.3/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.6.3/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/checkers/utils.py` & `edulint-2.6.3/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/linting.py` & `edulint-2.6.3/edulint/linting/linting.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/overrides.py` & `edulint-2.6.3/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/problem.py` & `edulint-2.6.3/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/process_handler.py` & `edulint-2.6.3/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/linting/tweakers.py` & `edulint-2.6.3/edulint/linting/tweakers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/options.py` & `edulint-2.6.3/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/__init__.py` & `edulint-2.6.3/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.6.3/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.6.3/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.6.3/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.6.3/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.6.3/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.6.3/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/edulint.egg-info/PKG-INFO` & `edulint-2.6.3/edulint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.6.2
+Version: 2.6.3
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.6.2/edulint.egg-info/SOURCES.txt` & `edulint-2.6.3/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/setup.cfg` & `edulint-2.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/setup.py` & `edulint-2.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_config.py` & `edulint-2.6.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_improper_loop.py` & `edulint-2.6.3/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_lint.py` & `edulint-2.6.3/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_main.py` & `edulint-2.6.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_short_problems.py` & `edulint-2.6.3/tests/test_short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_simplifiable_if.py` & `edulint-2.6.3/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.2/tests/test_visitors.py` & `edulint-2.6.3/tests/test_visitors.py`

 * *Files identical despite different names*


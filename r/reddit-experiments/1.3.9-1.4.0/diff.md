# Comparing `tmp/reddit_experiments-1.3.9.tar.gz` & `tmp/reddit_experiments-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_experiments-1.3.9.tar", last modified: Mon Aug 22 18:52:58 2022, max compression
+gzip compressed data, was "reddit_experiments-1.4.0.tar", last modified: Thu May 11 21:52:14 2023, max compression
```

## Comparing `reddit_experiments-1.3.9.tar` & `reddit_experiments-1.4.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    53651 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/images/ddg-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/docs/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/legacy/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.464296 reddit_experiments-1.3.9/reddit_decider/
--rw-r--r--   0 runner    (1001) docker     (121)    47376 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_decider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/
--rw-r--r--   0 runner    (1001) docker     (121)    14628 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/providers/
--rw-r--r--   0 runner    (1001) docker     (121)     5508 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/forced_variant.py
--rw-r--r--   0 runner    (1001) docker     (121)    13980 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11799 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/providers/simple_experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/targeting/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/targeting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/targeting/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8285 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/targeting/tree_targeting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/multi_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/range_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/rollout_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/reddit_experiments/variant_sets/single_variant_set.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/reddit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:52:58.000000 reddit_experiments-1.3.9/reddit_experiments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    69905 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/decider_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    36949 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (121)    27412 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/feature_flag_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/forced_variant_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    29866 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/r2_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    18526 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/simple_experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/providers/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/multi_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/range_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3115 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/rollout_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/providers/variant_sets/single_variant_set_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.468296 reddit_experiments-1.3.9/tests/range_variant_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/tests/range_variant_tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   154451 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/data/original_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (121) 14213529 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/data/output.json
--rw-r--r--   0 runner    (1001) docker     (121)   163729 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/data/range_variant_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/range_variant_tests/range_variant_parity_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:52:58.484296 reddit_experiments-1.3.9/tests/targeting/
--rw-r--r--   0 runner    (1001) docker     (121)    19814 2022-08-22 18:52:47.000000 reddit_experiments-1.3.9/tests/targeting/tree_targeting_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.922507 reddit_experiments-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.898507 reddit_experiments-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-11 21:52:14.922507 reddit_experiments-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/images/ddg-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/docs/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/legacy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_decider/
+-rw-r--r--   0 runner    (1001) docker     (123)    45454 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_decider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_decider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/forced_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/simple_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/targeting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/targeting/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/targeting/tree_targeting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/multi_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/range_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/rollout_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/single_variant_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-11 21:52:14.922507 reddit_experiments-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    79965 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/decider_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38015 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.906507 reddit_experiments-1.4.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/feature_flag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/forced_variant_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/r2_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/simple_experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.906507 reddit_experiments-1.4.0/tests/providers/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/multi_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/range_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/rollout_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/single_variant_set_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.906507 reddit_experiments-1.4.0/tests/range_variant_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.918507 reddit_experiments-1.4.0/tests/range_variant_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/data/original_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/data/output.json
+-rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/data/range_variant_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/range_variant_parity_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.918507 reddit_experiments-1.4.0/tests/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/targeting/tree_targeting_tests.py
```

### Comparing `reddit_experiments-1.3.9/.github/workflows/python-package.yaml` & `reddit_experiments-1.4.0/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/.readthedocs.yaml` & `reddit_experiments-1.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/LICENSE` & `reddit_experiments-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/Makefile` & `reddit_experiments-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/PKG-INFO` & `reddit_experiments-1.4.0/reddit_experiments.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reddit_experiments
-Version: 1.3.9
+Name: reddit-experiments
+Version: 1.4.0
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
         
@@ -21,15 +21,15 @@
         $ pip install reddit-experiments
         ```
         
         Add the client to your application's Baseplate context:
         
         ```python
          from reddit_decider import decider_client_from_config
-         
+        
          decider = decider_client_from_config(
              app_config=app_config,
              event_logger=ExperimentLogger(),
              request_field_extractor=decider_field_extractor,
          )
          baseplate.add_to_context("decider", decider)
         ```
@@ -38,15 +38,16 @@
         
         ```python
         def my_method(request):
            if request.decider.get_variant("foo") == "bar":
                pass
         ```
         
-        See [the documentation] for more information.
+        See [the documentation] for more information (documentation builds can be found [here](https://readthedocs.org/projects/reddit-experiments/builds/))
+        .
         
         [the documentation]: https://reddit-experiments.readthedocs.io/
         
         ## Development
         
         A Dockerfile is provided to get a development environment running. To use it,
         build the base Docker image:
```

### Comparing `reddit_experiments-1.3.9/README.md` & `reddit_experiments-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 $ pip install reddit-experiments
 ```
 
 Add the client to your application's Baseplate context:
 
 ```python
  from reddit_decider import decider_client_from_config
- 
+
  decider = decider_client_from_config(
      app_config=app_config,
      event_logger=ExperimentLogger(),
      request_field_extractor=decider_field_extractor,
  )
  baseplate.add_to_context("decider", decider)
 ```
@@ -30,15 +30,16 @@
 
 ```python
 def my_method(request):
    if request.decider.get_variant("foo") == "bar":
        pass
 ```
 
-See [the documentation] for more information.
+See [the documentation] for more information (documentation builds can be found [here](https://readthedocs.org/projects/reddit-experiments/builds/))
+.
 
 [the documentation]: https://reddit-experiments.readthedocs.io/
 
 ## Development
 
 A Dockerfile is provided to get a development environment running. To use it,
 build the base Docker image:
```

### Comparing `reddit_experiments-1.3.9/docs/conf.py` & `reddit_experiments-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/docs/images/ddg-logo.png` & `reddit_experiments-1.4.0/docs/images/ddg-logo.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/docs/images/favicon.png` & `reddit_experiments-1.4.0/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/docs/index.rst` & `reddit_experiments-1.4.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,30 @@
 ---------------------
 .. code-block:: python
 
     baseplate>=2.0.0
 
     reddit-edgecontext>=1.0.0
 
-    # upgrade or integrate latest reddit-v2-events package
-    # or manually update thrift schemas
-    # to allow event fields to be populated in exposures
-    reddit-v2-events
+    reddit-v2-events>=2.8.2
 
 Prerequisite infrastructure
 ---------------------------
+**Zookeeper live-data sidecar**:
+
 Set up your service to pull down & synchronize experiment configurations from Zookeeper via the Baseplate `live-data watcher sidecar
-<https://baseplate.readthedocs.io/en/stable/api/baseplate/lib/live_data.html?highlight=sidecar#watcher-daemon>`_ (minimum v2.4.13).
+<https://baseplate.readthedocs.io/en/stable/api/baseplate/lib/live_data.html?highlight=sidecar#watcher-daemon>`_ (minimum v2.5.4).
 You'll have to make sure that your service is authorized to fetch the appropriate secret from Vault.
+See example setup `here
+<https://reddit.atlassian.net/wiki/spaces/EX/pages/343212125/Running+Experiments+at+Reddit#Live-Data-Sidecar>`__.
+
+**Event publisher sidecar**:
+
+Set up your service to be able to publish v2 exposure events via an `events sidecar <https://baseplate.readthedocs.io/en/stable/api/baseplate/lib/events.html?highlight=sidecar#publishing-events>`_
+. See example setup `here <https://reddit.atlassian.net/wiki/spaces/EX/pages/343212125/Running+Experiments+at+Reddit#Event-Publisher-Sidecar>`__.
 
 Prerequisite configuration
 ---------------------------
 Setup :code:`reddit-experiments` in your application's configuration file:
 
 .. code-block:: ini
 
@@ -55,26 +61,25 @@
 -----------------------------------------------------------
 
 Upgrade or integrate reddit-experiments package:
 
 .. code-block:: python
 
     # import latest reddit-experiments package in service requirements.txt
-    reddit-experiments>=1.3.9
+    reddit-experiments>=1.3.14
 
 Initialize :code:`decider` instance on Baseplate context
 --------------------------------------------------------
 
 In your service's initialization process, add a :code:`decider` instance to baseplate's context:
-(Note the use of the :code:`ExperimentLogger`, which is used to publish exposure V2 events,
-an example can be seen `here <https://github.snooguts.net/reddit/reddit-service-graphql/blob/3734b51732c29d07eef32aced86677cce5064dbb/graphql-py/graphql_api/events/utils.py#L205>`_)
 
 .. code-block:: python
 
     # application code
+    from event_utils.v2_event_utils import ExperimentLogger
     from reddit_decider import decider_client_from_config
     from reddit_decider import DeciderClient
 
     # optional
     from some_file import my_field_extractor
 
 
@@ -87,15 +92,15 @@
         baseplate.add_to_context("decider", decider_factory)
 
         # Or use `DeciderClient` with `configure_context()`,
         # which internally calls `decider_client_from_config()`
         baseplate.configure_context({
             "decider": DeciderClient(
                 prefix="experiments.",
-                event_logger=ExperimentLogger,
+                event_logger=ExperimentLogger()),
                 request_field_extractor=my_field_extractor  # optional
         })
 
 Make sure :code:`EdgeContext` is accessible on :code:`request` object like so:
 
 .. code-block:: python
 
@@ -113,15 +118,15 @@
     #   - logged_in
     #   - cookie_created_timestamp
     #   - oauth_client_id
     #   - country_code
     #   - locale
     #   - origin_service
     #   - is_employee
-    #   - loid_created_ms (>=1.3.9)
+    #   - loid_created_ms (>=1.3.11)
 
     # Customized fields can be defined below to be extracted from a baseplate request
     # and will override above edge_context fields.
     # These fields may be used for targeting.
 
     def my_field_extractor(request):
         # an example of customized baseplate request field extractor:
```

### Comparing `reddit_experiments-1.3.9/docs/legacy/index.rst` & `reddit_experiments-1.4.0/docs/legacy/index.rst`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_decider/__init__.py` & `reddit_experiments-1.4.0/reddit_decider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,35 +5,48 @@
 from enum import Enum
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import IO
 from typing import List
 from typing import Optional
+from typing import Type
+from typing import TypeVar
 from typing import Union
 
-import rust_decider  # type: ignore
-
 from baseplate import RequestContext
 from baseplate import Span
 from baseplate.clients import ContextFactory
 from baseplate.lib import config
 from baseplate.lib.events import DebugLogger
 from baseplate.lib.events import EventLogger
 from baseplate.lib.file_watcher import FileWatcher
 from baseplate.lib.file_watcher import T
 from baseplate.lib.file_watcher import WatchedFileNotAvailableError
 from reddit_edgecontext import ValidatedAuthenticationToken
+from rust_decider import Decider as RustDecider
+from rust_decider import DeciderException
+from rust_decider import Decision
+from rust_decider import FeatureNotFoundException
+from rust_decider import ValueTypeMismatchException
 from typing_extensions import Literal
 
 
 logger = logging.getLogger(__name__)
 
 EMPLOYEE_ROLES = ["employee", "contractor"]
-IDENTIFIERS = ["user_id", "device_id", "canonical_url"]
+IDENTIFIERS = [
+    "user_id",
+    "device_id",
+    "canonical_url",
+    "subreddit_id",
+    "ad_account_id",
+    "business_id",
+]
+TYPE_STR_LOOKUP = {bool: "boolean", int: "integer", float: "float", str: "string", dict: "map"}
 
 
 class EventType(Enum):
     EXPOSE = "expose"
 
 
 @dataclass
@@ -41,22 +54,25 @@
     id: int
     version: str
     name: str
     bucket_val: str
     start_ts: int
     stop_ts: int
     owner: str
+    emit_event: Optional[bool] = None
 
 
 class DeciderContext:
     """DeciderContext() is used to contain all fields necessary for
     bucketing, targeting, and overrides.
     :code:`DeciderContext()` is populated in :code:`make_object_for_context()`.
     """
 
+    T = TypeVar("T")
+
     def __init__(
         self,
         user_id: Optional[str] = None,
         country_code: Optional[str] = None,
         locale: Optional[str] = None,
         user_is_employee: Optional[bool] = None,
         logged_in: Optional[bool] = None,
@@ -144,94 +160,43 @@
             "request": request_fields,
             "platform": platform_fields,
             **ef,
         }
 
 
 def init_decider_parser(file: IO) -> Any:
-    return rust_decider.init(
-        "darkmode overrides targeting holdout mutex_group fractional_availability value", file.name
-    )
-
-
-def validate_decider(decider: Optional[Any]) -> None:
-    if decider is None:
-        logger.error("Rust decider is None--did not initialize.")
-
-    if decider:
-        decider_err = decider.err()
-        if decider_err:
-            logger.error(f"Rust decider has initialization error: {decider_err}")
+    return RustDecider(file.name)
 
 
 class Decider:
     """Access to experiments with automatic refresh when changed.
 
     This decider client allows access to the experiments cached on disk by
     the experiment configuration fetcher daemon.
     It will automatically reload the cache when changed.
     """
 
     def __init__(
         self,
         decider_context: DeciderContext,
-        config_watcher: FileWatcher,
+        internal: Optional[RustDecider],
         server_span: Span,
         context_name: str,
         event_logger: Optional[EventLogger] = None,
     ):
         self._decider_context = decider_context
-        self._config_watcher = config_watcher
+        self._internal: RustDecider = internal
         self._span = server_span
         self._context_name = context_name
         if event_logger:
             self._event_logger = event_logger
         else:
             self._event_logger = DebugLogger()
 
-    def _get_decider(self) -> Optional[T]:
-        try:
-            decider = self._config_watcher.get_data()
-            validate_decider(decider)
-            return decider
-        except WatchedFileNotAvailableError as exc:
-            logger.error("Experiment config file unavailable: %s", str(exc))
-        except TypeError as exc:
-            logger.error("Could not load experiment config: %s", str(exc))
-        return None
-
-    def _get_ctx(self) -> Any:
-        context_fields = self._decider_context.to_dict()
-        return rust_decider.make_ctx(context_fields)
-
-    def _get_ctx_with_set_identifier(
-        self, identifier: str, identifier_type: Literal["user_id", "device_id", "canonical_url"]
-    ) -> Dict[str, Any]:
-        context_fields = self._decider_context.to_dict()
-        context_fields[identifier_type] = identifier
-
-        return rust_decider.make_ctx(context_fields)
-
-    def _format_decision(self, decision_dict: Dict[str, str]) -> Dict[str, Any]:
-        out = {}
-        # cast id to int
-        for k, v in decision_dict.items():
-            if k == "id":
-                try:
-                    out[k] = int(v)
-                except ValueError:
-                    out[k] = v  # type: ignore
-            else:
-                out[k] = v  # type: ignore
-
-        return out
-
-    def _send_expose(
-        self, event: str, exposure_fields: dict, overwrite_identifier: bool = False
-    ) -> None:
+    def _send_expose(self, event: str, exposure_fields: dict) -> None:
         event_fields = deepcopy(exposure_fields)
         try:
             (
                 _event_type,
                 exp_id,
                 name,
                 version,
@@ -254,30 +219,27 @@
             version=version,
             bucket_val=bucket_val,
             start_ts=self._cast_to_int(start_ts),
             stop_ts=self._cast_to_int(stop_ts),
             owner=owner,
         )
 
-        if overwrite_identifier:
-            event_fields = {**event_fields, **{bucket_val: bucketing_value}}
+        event_fields = {**event_fields, **{bucket_val: bucketing_value}}
 
         self._event_logger.log(
             experiment=experiment,
             variant=event_variant,
             span=self._span,
             event_type=EventType.EXPOSE,
             inputs=event_fields,
             **event_fields,
         )
         return
 
-    def _send_expose_if_holdout(
-        self, event: str, exposure_fields: dict, overwrite_identifier: bool = False
-    ) -> None:
+    def _send_expose_if_holdout(self, event: str, exposure_fields: dict) -> None:
         event_fields = deepcopy(exposure_fields)
         try:
             (
                 event_type,
                 exp_id,
                 name,
                 version,
@@ -305,16 +267,15 @@
                 version=version,
                 bucket_val=bucket_val,
                 start_ts=self._cast_to_int(start_ts),
                 stop_ts=self._cast_to_int(stop_ts),
                 owner=owner,
             )
 
-            if overwrite_identifier:
-                event_fields = {**event_fields, **{bucket_val: bucketing_value}}
+            event_fields = {**event_fields, **{bucket_val: bucketing_value}}
 
             self._event_logger.log(
                 experiment=experiment,
                 variant=event_variant,
                 span=self._span,
                 event_type=EventType.EXPOSE,
                 inputs=event_fields,
@@ -348,40 +309,27 @@
 
         :param exposure_kwargs:  Additional arguments that will be passed
             to :code:`events_logger` (keys must be part of v2 event schema,
             use dicts for nested fields) under :code:`inputs` and as :code:`kwargs`
 
         :return: Variant name if a variant is assigned, :code:`None` otherwise.
         """
-        decider = self._get_decider()
-        if decider is None:
-            return None
-
-        ctx = self._get_ctx()
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return None
-
-        choice = decider.choose(experiment_name, ctx)
-        error = choice.err()
+        ctx = self._decider_context.to_dict()
+        decision = self._get_decision(experiment_name, ctx)
 
-        if error:
-            logger.info(f"Encountered error in decider.choose(): {error}")
+        if decision is None:
             return None
 
-        variant = choice.decision()
-
         event_context_fields = self._decider_context.to_event_dict()
         event_context_fields.update(exposure_kwargs or {})
 
-        for event in choice.events():
+        for event in decision.events:
             self._send_expose(event=event, exposure_fields=event_context_fields)
 
-        return variant
+        return decision.variant
 
     def get_variant_without_expose(self, experiment_name: str) -> Optional[str]:
         """Return a bucketing variant, if any, without emitting exposure event.
 
         The :code:`expose()` function is available to be manually called afterward.
 
         However, experiments in Holdout Groups will still send an exposure for
@@ -390,40 +338,26 @@
         returned :code:`None` or :code:`"control_1"` string
         came from the holdout group or its child experiment once this function exits).
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :return: Variant name if a variant is assigned, None otherwise.
         """
-        decider = self._get_decider()
-        if decider is None:
-            return None
-
-        ctx = self._get_ctx()
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return None
-
-        choice = decider.choose(experiment_name, ctx)
-        error = choice.err()
+        ctx = self._decider_context.to_dict()
+        decision = self._get_decision(experiment_name, ctx)
 
-        if error:
-            logger.info(f"Encountered error in decider.choose(): {error}")
+        if decision is None:
             return None
 
-        variant = choice.decision()
-
         event_context_fields = self._decider_context.to_event_dict()
 
-        # expose Holdout if the experiment is part of one
-        for event in choice.events():
+        for event in decision.events:
             self._send_expose_if_holdout(event=event, exposure_fields=event_context_fields)
 
-        return variant
+        return decision.variant
 
     def expose(
         self, experiment_name: str, variant_name: str, **exposure_kwargs: Optional[Dict[str, Any]]
     ) -> None:
         """Log an event to indicate that a user has been exposed to an experimental treatment.
 
         Meant to be used after calling :code:`get_variant_without_expose()`
@@ -433,38 +367,46 @@
 
         :param variant_name: Name of the variant that was exposed.
 
         :param exposure_kwargs: Additional arguments that will be passed
             to :code:`events_logger` (keys must be part of v2 event schema,
             use dicts for nested fields) under :code:`inputs` and as :code:`kwargs`
         """
-        decider = self._get_decider()
-        if decider is None:
+        if variant_name is None or variant_name == "":
             return
 
-        experiment = decider.get_experiment(experiment_name)
-        error = experiment.err()
-        if error:
-            logger.warning(f"Encountered error in decider.get_experiment(): {error}")
+        if self._internal is None:
+            logger.error("RustDecider is None--did not initialize.")
+            return
+
+        try:
+            feature = self._internal.get_feature(experiment_name)
+        except FeatureNotFoundException as exc:
+            logger.debug(str(exc))
+            return
+        except DeciderException as exc:
+            logger.info(str(exc))
+            return
+
+        # drop exposure for feature rollouts
+        if not feature.emit_event:
             return
 
         event_context_fields = self._decider_context.to_event_dict()
         event_context_fields.update(exposure_kwargs or {})
         event_fields = deepcopy(event_context_fields)
 
-        exp_dict = experiment.val()
-
         experiment = ExperimentConfig(
-            id=int(exp_dict.get("id", 0)),
-            name=exp_dict.get("name"),
-            version=str(exp_dict.get("version")),
-            bucket_val=exp_dict.get("variant_set", {}).get("bucket_val"),
-            start_ts=exp_dict.get("variant_set", {}).get("start_ts"),
-            stop_ts=exp_dict.get("variant_set", {}).get("stop_ts"),
-            owner=exp_dict.get("owner"),
+            id=feature.id,
+            name=feature.name,
+            version=str(feature.version),
+            bucket_val=feature.bucket_val,
+            start_ts=feature.start_ts,
+            stop_ts=feature.stop_ts,
+            owner=feature.owner,
         )
 
         self._event_logger.log(
             experiment=experiment,
             variant=variant_name,
             span=self._span,
             event_type=EventType.EXPOSE,
@@ -472,140 +414,133 @@
             **event_fields,
         )
 
     def get_variant_for_identifier(
         self,
         experiment_name: str,
         identifier: str,
-        identifier_type: Literal["user_id", "device_id", "canonical_url"],
+        identifier_type: Literal[
+            "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id"
+        ],
         **exposure_kwargs: Optional[Dict[str, Any]],
     ) -> Optional[str]:
         """Return a bucketing variant, if any, with auto-exposure for a given :code:`identifier`.
 
+        Note: If the experiment's :code:`bucket_val` (e.g. "user_id", "device_id", "canonical_url")
+            does not match the :code:`identifier_type` param,
+            the :code:`identifier` will be ignored and not used to bucket (:code:`{identifier_type: identifier}` is
+            added to internal :code:`DeciderContext` instance, but doesn't act like a bucketing override).
+
+            If the :code:`bucket_val` field exists on the :code:`DeciderContext` instance,
+            that field will be used to bucket, since it corresponds to the experiment's config.
+
         Since calling :code:`get_variant_for_identifier()` will fire an exposure event, it
         is best to call it when you are sure the user will be exposed to the experiment.
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :param identifier: an arbitary string used to bucket the experiment by
             being set on :code:`DeciderContext`'s :code:`identifier_type` field.
 
-        :param identifier_type: Sets :code:`{identifier_type: identifier}` on DeciderContext and
-            should match an experiment's :code:`bucket_val` to get a variant.
+        :param identifier_type: Sets :code:`{identifier_type: identifier}` on :code:`DeciderContext`.
+            The experiment's :code:`bucket_val` will be looked up in :code:`DeciderContext` and be used to bucket.
+            If the experiment's :code:`bucket_val` field does not match :code:`identifier_type` param,
+            :code:`identifier` will be ignored, and the field corresponding :code:`bucket_val` will be looked up
+            from :code:`DeciderContext` for bucketing.
 
         :param exposure_kwargs: Additional arguments that will be passed
             to :code:`events_logger` (keys must be part of v2 event schema,
             use dicts for nested fields) under :code:`inputs` and as :code:`kwargs`
 
 
         :return: Variant name if a variant is assigned, None otherwise.
         """
         if identifier_type not in IDENTIFIERS:
             logger.warning(
                 f'"{identifier_type}" is not one of supported "identifier_type": {IDENTIFIERS}.'
             )
             return None
 
-        decider = self._get_decider()
-        if decider is None:
-            return None
+        ctx = self._decider_context.to_dict()
+        ctx[identifier_type] = identifier
 
-        ctx = self._get_ctx_with_set_identifier(
-            identifier=identifier, identifier_type=identifier_type
-        )
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return None
-
-        choice = decider.choose(
-            feature_name=experiment_name, ctx=ctx, identifier_type=identifier_type
-        )
-        error = choice.err()
+        decision = self._get_decision(experiment_name, ctx)
 
-        if error:
-            logger.info(f"Encountered error in decider.choose(): {error}")
+        if decision is None:
             return None
 
-        variant = choice.decision()
-
         event_context_fields = self._decider_context.to_event_dict()
         event_context_fields.update(exposure_kwargs or {})
 
-        for event in choice.events():
-            self._send_expose(
-                event=event, exposure_fields=event_context_fields, overwrite_identifier=True
-            )
+        for event in decision.events:
+            self._send_expose(event=event, exposure_fields=event_context_fields)
 
-        return variant
+        return decision.variant
 
     def get_variant_for_identifier_without_expose(
         self,
         experiment_name: str,
         identifier: str,
-        identifier_type: Literal["user_id", "device_id", "canonical_url"],
+        identifier_type: Literal[
+            "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id"
+        ],
     ) -> Optional[str]:
         """Return a bucketing variant, if any, without emitting exposure event for a given :code:`identifier`.
 
+        Note: If the experiment's :code:`bucket_val` (e.g. "user_id", "device_id", "canonical_url")
+            does not match the :code:`identifier_type` param,
+            the :code:`identifier` will be ignored and not used to bucket (:code:`{identifier_type: identifier}` is
+            added to internal :code:`DeciderContext` instance, but doesn't act like a bucketing override).
+
+            If the :code:`bucket_val` field exists on the :code:`DeciderContext` instance,
+            that field will be used to bucket, since it corresponds to the experiment's config.
+
         The :code:`expose()` function is available to be manually called afterward to emit
         exposure event.
 
         However, experiments in Holdout Groups will still send an exposure for
         the holdout parent experiment, since it is not possible to
         manually expose the holdout later (because it's impossible to know if a
         returned :code:`None` or :code:`"control_1"` string
         came from the holdout group or its child experiment once this function exits).
 
         :param experiment_name: Name of the experiment you want a variant for.
 
         :param identifier: an arbitary string used to bucket the experiment by
             being set on :code:`DeciderContext`'s :code:`identifier_type` field.
 
-        :param identifier_type: Sets :code:`{identifier_type: identifier}` on DeciderContext and
-            should match an experiment's :code:`bucket_val` to get a variant.
+        :param identifier_type: Sets :code:`{identifier_type: identifier}` on :code:`DeciderContext`.
+            The experiment's :code:`bucket_val` will be looked up in :code:`DeciderContext` and be used to bucket.
+            If the experiment's :code:`bucket_val` field does not match :code:`identifier_type` param,
+            :code:`identifier` will be ignored and the field corresponding :code:`bucket_val` will be looked up
+            from :code:`DeciderContext` for bucketing.
 
         :return: Variant name if a variant is assigned, None otherwise.
         """
         if identifier_type not in IDENTIFIERS:
             logger.warning(
                 f'"{identifier_type}" is not one of supported "identifier_type": {IDENTIFIERS}.'
             )
             return None
 
-        decider = self._get_decider()
-        if decider is None:
-            return None
+        ctx = self._decider_context.to_dict()
+        ctx[identifier_type] = identifier
 
-        ctx = self._get_ctx_with_set_identifier(
-            identifier=identifier, identifier_type=identifier_type
-        )
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return None
+        decision = self._get_decision(experiment_name, ctx)
 
-        choice = decider.choose(
-            feature_name=experiment_name, ctx=ctx, identifier_type=identifier_type
-        )
-        error = choice.err()
-        if error:
-            logger.info(f"Encountered error in decider.choose(): {error}")
+        if decision is None:
             return None
 
-        variant = choice.decision()
-
         event_context_fields = self._decider_context.to_event_dict()
 
         # expose Holdout if the experiment is part of one
-        for event in choice.events():
-            self._send_expose_if_holdout(
-                event=event, exposure_fields=event_context_fields, overwrite_identifier=True
-            )
+        for event in decision.events:
+            self._send_expose_if_holdout(event=event, exposure_fields=event_context_fields)
 
-        return variant
+        return decision.variant
 
     def get_all_variants_without_expose(self) -> List[Dict[str, Union[str, int]]]:
         """Return a list of experiment dicts in this format:
 
             .. code-block:: json
 
                 [
@@ -629,59 +564,52 @@
         the holdout parent experiment, since it is not possible to
         manually expose the holdout later (because it's impossible to know if a
         returned :code:`None` or :code:`"control_1"` string
         came from the holdout group or its child experiment once this function exits).
 
         :return: list of experiment dicts with non-:code:`None` variants.
         """
-        decider = self._get_decider()
-        if decider is None:
-            return []
+        ctx = self._decider_context.to_dict()
 
-        ctx = self._get_ctx()
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return []
+        all_decisions = self._get_all_decisions(ctx)
 
-        all_decisions_result = decider.choose_all(ctx)
-
-        error = all_decisions_result.err()
-        if error:
-            logger.info(f"Encountered error in decider.choose_all(): {error}")
+        if all_decisions is None:
             return []
 
-        all_decisions = all_decisions_result.decisions()
         parsed_choices = []
 
         event_context_fields = self._decider_context.to_event_dict()
 
-        for exp_name, decision in all_decisions.items():
-            decision_error = decision.err()
-            if decision_error:
-                logger.info(
-                    f"Encountered error for experiment: {exp_name} in decider.choose_all(): {decision_error}"
-                )
-                continue
-
-            decision_dict = decision.decision_dict()
-
-            if decision_dict:
-                parsed_choices.append(self._format_decision(decision_dict))
+        for decision in all_decisions.values():
+            if decision.variant:
+                parsed_choices.append(self._decision_to_dict(decision))
 
             # expose Holdout if the experiment is part of one
-            for event in decision.events():
+            for event in decision.events:
                 self._send_expose_if_holdout(event=event, exposure_fields=event_context_fields)
 
         return parsed_choices
 
+    def _decision_to_dict(self, decision: Decision) -> Dict[str, Any]:
+        return {
+            "name": decision.variant,
+            "id": decision.feature_id,
+            "version": str(decision.feature_version),
+            "experimentName": decision.feature_name,
+        }
+
     def get_all_variants_for_identifier_without_expose(
-        self, identifier: str, identifier_type: Literal["user_id", "device_id", "canonical_url"]
+        self,
+        identifier: str,
+        identifier_type: Literal[
+            "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id"
+        ],
     ) -> List[Dict[str, Union[str, int]]]:
-        """Return a list of experiment dicts for a given :code:`identifier` in this format:
+        """Return a list of experiment dicts for experiments having :code:`bucket_val` match
+        :code:`identifier_type`, for a given :code:`identifier`, in this format:
 
                 .. code-block:: json
 
                     [
                         {
                             "id": 1,
                             "name": "variant_1",
@@ -700,165 +628,107 @@
         returned :code:`None` or :code:`"control_1"` string
         came from the holdout group or its child experiment once this function exits).
 
         :param identifier: an arbitary string used to bucket the experiment by
             being set on :code:`DeciderContext`'s :code:`identifier_type` field.
 
         :param identifier_type: Sets :code:`{identifier_type: identifier}` on DeciderContext and
-            should match an experiment's :code:`bucket_val` to get a variant.
+            buckets all experiment with matching :code:`bucket_val`.
 
         :return: list of experiment dicts with non-:code:`None` variants.
         """
         if identifier_type not in IDENTIFIERS:
             logger.warning(
                 f'"{identifier_type}" is not one of supported "identifier_type": {IDENTIFIERS}.'
             )
             return []
 
-        decider = self._get_decider()
-        if decider is None:
-            return []
+        ctx = self._decider_context.to_dict()
+        ctx[identifier_type] = identifier
 
-        ctx = self._get_ctx_with_set_identifier(
-            identifier=identifier, identifier_type=identifier_type
-        )
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return []
+        all_decisions = self._get_all_decisions(ctx=ctx, bucketing_field_filter=identifier_type)
 
-        all_decisions_result = decider.choose_all(ctx=ctx, identifier_type=identifier_type)
-
-        error = all_decisions_result.err()
-        if error:
-            logger.info(f"Encountered error in decider.choose_all(): {error}")
+        if all_decisions is None:
             return []
 
-        all_decisions = all_decisions_result.decisions()
         parsed_choices = []
 
         event_context_fields = self._decider_context.to_event_dict()
 
-        for exp_name, decision in all_decisions.items():
-            decision_error = decision.err()
-            if decision_error:
-                logger.info(
-                    f"Encountered error for experiment: {exp_name} in decider.choose_all(): {decision_error}"
-                )
-                continue
-
-            decision_dict = decision.decision_dict()
-
-            if decision_dict:
-                parsed_choices.append(self._format_decision(decision_dict))
+        for decision in all_decisions.values():
+            if decision.variant:
+                parsed_choices.append(self._decision_to_dict(decision))
 
             # expose Holdout if the experiment is part of one
-            for event in decision.events():
-                self._send_expose_if_holdout(
-                    event=event, exposure_fields=event_context_fields, overwrite_identifier=True
-                )
+            for event in decision.events:
+                self._send_expose_if_holdout(event=event, exposure_fields=event_context_fields)
 
         return parsed_choices
 
-    def _get_dynamic_config_value(
-        self,
-        feature_name: str,
-        decider_func: Callable[[str, DeciderContext], Any],
-        default: Any,
-    ) -> Optional[Any]:
-        ctx = self._get_ctx()
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
-            return None
-
-        res = decider_func(feature_name, ctx)
-        if res is None:
-            return default
-        error = res.err()
-        if error:
-            logger.warning(f"Encountered error {decider_func.__name__}: {error}")
-            return default
-
-        return res.val()
-
     def get_bool(self, feature_name: str, default: bool = False) -> bool:
         """Fetch a Dynamic Configuration of boolean type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`False` unless overriden).
 
         :return: the boolean value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
-        decider = self._get_decider()
-        if not decider:
-            return default
-        return self._get_dynamic_config_value(feature_name, decider.get_bool, default)
+        return self._get_dynamic_config_value(feature_name, default, bool, self._internal.get_bool)
 
     def get_int(self, feature_name: str, default: int = 0) -> int:
         """Fetch a Dynamic Configuration of int type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`0` unless overriden).
 
         :return: the int value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
-        decider = self._get_decider()
-        if not decider:
-            return default
-        return self._get_dynamic_config_value(feature_name, decider.get_int, default)
+        return self._get_dynamic_config_value(feature_name, default, int, self._internal.get_int)
 
     def get_float(self, feature_name: str, default: float = 0.0) -> float:
         """Fetch a Dynamic Configuration of float type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`0.0` unless overriden).
 
         :return: the float value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
-        decider = self._get_decider()
-        if not decider:
-            return default
-        return self._get_dynamic_config_value(feature_name, decider.get_float, default)
+        return self._get_dynamic_config_value(
+            feature_name, default, float, self._internal.get_float
+        )
 
     def get_string(self, feature_name: str, default: str = "") -> str:
         """Fetch a Dynamic Configuration of string type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`""` unless overriden).
 
         :return: the string value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
-        decider = self._get_decider()
-        if not decider:
-            return default
-        return self._get_dynamic_config_value(feature_name, decider.get_string, default)
+        return self._get_dynamic_config_value(feature_name, default, str, self._internal.get_string)
 
     def get_map(self, feature_name: str, default: Optional[dict] = None) -> Optional[dict]:
         """Fetch a Dynamic Configuration of map type.
 
         :param feature_name: Name of the dynamic config you want a value for.
 
         :param default: what is returned if dynamic config is not active
             (:code:`None` unless overriden).
 
         :return: the map value of the dyanimc config if it is active/exists, :code:`default` parameter otherwise.
         """
-        decider = self._get_decider()
-        if not decider:
-            return default
-        return self._get_dynamic_config_value(feature_name, decider.get_map, default)
+        return self._get_dynamic_config_value(feature_name, default, dict, self._internal.get_map)
 
     def get_all_dynamic_configs(self) -> List[Dict[str, Any]]:
         """Return a list of dynamic configuration dicts in this format:
 
             .. code-block:: json
 
                 [
@@ -885,82 +755,132 @@
             "integer" -> 0
             "float"   -> 0.0
             "string"  -> ""
             "map"     -> {}
 
         :return: list of all active dynamic config dicts.
         """
-        decider = self._get_decider()
-        if not decider:
-            return []
-
-        ctx = self._get_ctx()
-        ctx_err = ctx.err()
-        if ctx_err is not None:
-            logger.info(f"Encountered error in rust_decider.make_ctx(): {ctx_err}")
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
             return []
 
-        all_decisions_result = decider.get_all_values(ctx)
+        ctx = self._decider_context.to_dict()
 
-        error = all_decisions_result.err()
-        if error:
-            logger.info(f"Encountered error in decider.choose_all(): {error}")
+        try:
+            values = self._internal.all_values(ctx)
+        except DeciderException as exc:
+            logger.info(str(exc))
             return []
 
-        all_decisions = all_decisions_result.decisions()
         parsed_configs = []
 
-        for dc_name, decision in all_decisions.items():
-            decision_error = decision.err()
-            if decision_error:
-                logger.info(
-                    f"Encountered error for dynamic config: {dc_name} in decider.get_all_values(): {decision_error}"
-                )
-                continue
+        for feature_name, val in values.items():
+            parsed_configs.append(self._value_to_dc_dict(feature_name, val))
 
-            value_dict = decision.value_dict()
+        return parsed_configs
 
-            if value_dict:
-                parsed_configs.append(value_dict)
+    def _get_decision(
+        self,
+        experiment_name: str,
+        ctx: Dict[str, Any],
+    ) -> Optional[Decision]:
+        if self._internal is None:
+            logger.error("RustDecider is None--did not initialize.")
+            return None
 
-        return parsed_configs
+        try:
+            return self._internal.choose(experiment_name, ctx)
+        except FeatureNotFoundException as exc:
+            logger.debug(str(exc))
+            return None
+        except DeciderException as exc:
+            logger.info(str(exc))
+            return None
+
+    def _get_all_decisions(
+        self, ctx: Dict[str, Any], bucketing_field_filter: Optional[str] = None
+    ) -> Optional[Dict[str, Decision]]:
+        if self._internal is None:
+            logger.error("RustDecider is None--did not initialize.")
+            return None
+
+        try:
+            return self._internal.choose_all(ctx, bucketing_field_filter)
+        except DeciderException as exc:
+            logger.info(str(exc))
+            return None
+
+    def _get_dynamic_config_value(
+        self,
+        feature_name: str,
+        default: Any,
+        dc_type: Type[T],
+        get_fn: Callable[..., Type[T]],
+    ) -> T:
+        if self._internal is None:
+            logger.error("rs_decider is None--did not initialize.")
+            return default
+
+        ctx = self._decider_context.to_dict()
+
+        try:
+            value = get_fn(feature_name=feature_name, context=ctx)
+        except FeatureNotFoundException as exc:
+            logger.debug(str(exc))
+            return default
+        except ValueTypeMismatchException as exc:
+            logger.info(str(exc))
+            return default
+        except DeciderException as exc:
+            logger.info(str(exc))
+            return default
+
+        try:
+            return dc_type(value)  # type: ignore [call-arg]
+        except TypeError:
+            return default
+
+    def _value_to_dc_dict(self, feature_name: str, value: Optional[Any]) -> Dict[str, Any]:
+        return {
+            "name": feature_name,
+            "value": value,
+            "type": "" if value is None else TYPE_STR_LOOKUP[type(value)],
+        }
 
     def get_experiment(self, experiment_name: str) -> Optional[ExperimentConfig]:
-        """Get an :py:class:`~reddit_decider.ExperimentConfig` `dataclass <https://github.com/reddit/experiments.py/blob/728a9501faceab7072f9d62f4e391fa4c34a68b1/reddit_decider/__init__.py#L39-L47>`_
+        """Get an :py:class:`~reddit_decider.ExperimentConfig` `dataclass <https://github.com/reddit/experiments.py/blob/develop/reddit_decider/__init__.py#L44>`_
         representation of an experiment or :code:`None` if not found.
 
         :param experiment_name: Name of the experiment to be fetched.
 
-        :return: an :py:class:`~reddit_decider.ExperimentConfig` `dataclass <https://github.com/reddit/experiments.py/blob/728a9501faceab7072f9d62f4e391fa4c34a68b1/reddit_decider/__init__.py#L39-L47>`_
+        :return: an :py:class:`~reddit_decider.ExperimentConfig` `dataclass <https://github.com/reddit/experiments.py/blob/develop/reddit_decider/__init__.py#L44>`_
             representation of an experiment if found, else :code:`None`.
         """
-        decider = self._get_decider()
-        if decider is None:
+        if self._internal is None:
+            logger.error("RustDecider is None--did not initialize.")
             return None
 
-        experiment = decider.get_experiment(experiment_name)
-        error = experiment.err()
-        if error:
-            # sending to debug logger to avoid printing "Feature x not found." logs
-            logger.debug(f"Encountered error in decider.get_experiment(): {error}")
+        try:
+            feature = self._internal.get_feature(experiment_name)
+        except FeatureNotFoundException as exc:
+            logger.debug(str(exc))
             return None
-
-        exp_dict = experiment.val()
-
-        if exp_dict is None:
+        except DeciderException as exc:
+            logger.info(str(exc))
             return None
 
         return ExperimentConfig(
-            id=int(exp_dict.get("id", 0)),
-            name=exp_dict.get("name"),
-            version=str(exp_dict.get("version")),
-            bucket_val=exp_dict.get("variant_set", {}).get("bucket_val"),
-            start_ts=exp_dict.get("variant_set", {}).get("start_ts"),
-            stop_ts=exp_dict.get("variant_set", {}).get("stop_ts"),
-            owner=exp_dict.get("owner"),
+            id=feature.id,
+            name=feature.name,
+            version=str(feature.version),
+            bucket_val=feature.bucket_val,
+            start_ts=feature.start_ts,
+            stop_ts=feature.stop_ts,
+            owner=feature.owner,
+            emit_event=feature.emit_event,
         )
 
 
 class DeciderContextFactory(ContextFactory):
     """Decider client context factory.
 
     This factory will attach a new
@@ -1022,38 +942,38 @@
                 logger.info(
                     f"{k}: {v} value in `request_field_extractor()` dict is not one of type: [None, int, float, str, bool] and is removed."
                 )
                 del parsed_extracted_fields[k]
         return parsed_extracted_fields
 
     def _minimal_decider(
-        self, name: str, span: Span, parsed_extracted_fields: Optional[Dict] = None
+        self,
+        internal: Optional[RustDecider],
+        name: str,
+        span: Span,
+        parsed_extracted_fields: Optional[Dict] = None,
     ) -> Decider:
         return Decider(
             decider_context=DeciderContext(extracted_fields=parsed_extracted_fields),
-            config_watcher=self._filewatcher,
+            internal=internal,
             server_span=span,
             context_name=name,
             event_logger=self._event_logger,
         )
 
     def make_object_for_context(self, name: str, span: Span) -> Decider:
-        decider = None
+        rs_decider = None
         try:
-            decider = self._filewatcher.get_data()
+            rs_decider = self._filewatcher.get_data()
         except WatchedFileNotAvailableError as exc:
-            logger.error("Experiment config file unavailable: %s", str(exc))
-        except TypeError as exc:
-            logger.error("Could not load experiment config: %s", str(exc))
-
-        validate_decider(decider)
+            logger.error(f"Experiment config file unavailable: {exc}")
 
         if span is None:
             logger.debug("`span` is `None` in reddit_decider `make_object_for_context()`.")
-            return self._minimal_decider(name=name, span=span)
+            return self._minimal_decider(internal=rs_decider, name=name, span=span)
 
         request = None
         parsed_extracted_fields = None
         try:
             request = span.context
 
             if self._request_field_extractor:
@@ -1068,29 +988,38 @@
             )
 
         ec = None
         try:
             # if `edge_context` is inaccessible, bail early
             if request is None:
                 return self._minimal_decider(
-                    name=name, span=span, parsed_extracted_fields=parsed_extracted_fields
+                    internal=rs_decider,
+                    name=name,
+                    span=span,
+                    parsed_extracted_fields=parsed_extracted_fields,
                 )
 
             ec = request.edge_context
 
             if ec is None:
                 return self._minimal_decider(
-                    name=name, span=span, parsed_extracted_fields=parsed_extracted_fields
+                    internal=rs_decider,
+                    name=name,
+                    span=span,
+                    parsed_extracted_fields=parsed_extracted_fields,
                 )
         except Exception as exc:
             logger.info(
                 f"Unable to access `request.edge_context` in `make_object_for_context()`. details: {exc}"
             )
             return self._minimal_decider(
-                name=name, span=span, parsed_extracted_fields=parsed_extracted_fields
+                internal=rs_decider,
+                name=name,
+                span=span,
+                parsed_extracted_fields=parsed_extracted_fields,
             )
 
         # All fields below are derived from `edge_context`
 
         user_id = None
         logged_in = None
         cookie_created_timestamp = None
@@ -1178,22 +1107,21 @@
                 oauth_client_id=oauth_client_id,
                 cookie_created_timestamp=cookie_created_timestamp,
                 loid_created_timestamp=loid_created_timestamp,
                 extracted_fields=parsed_extracted_fields,
             )
         except Exception as exc:
             logger.warning(
-                "Could not create full DeciderContext() (defaulting to empty DeciderContext()): %s",
-                str(exc),
+                f"Could not create full DeciderContext() (defaulting to empty DeciderContext()): {exc}"
             )
             decider_context = DeciderContext()
 
         return Decider(
             decider_context=decider_context,
-            config_watcher=self._filewatcher,
+            internal=rs_decider,
             server_span=span,
             context_name=name,
             event_logger=self._event_logger,
         )
 
 
 class DeciderClient(config.Parser):
@@ -1251,15 +1179,15 @@
     Supported config keys:
 
         ``path`` (optional)
             The path to the experiment configuration file generated by the
             experiment configuration fetcher daemon.
         ``timeout`` (optional)
             The time that we should wait for the file specified by ``path`` to
-            exist.  Defaults to `None` which is `infinite`.
+            exist.  Defaults to `None` which is not blocking.
         ``backoff`` (optional)
             The base amount of time for exponential backoff when trying to find the
             experiments config file. Defaults to no backoff between tries.
 
     :param app_config: The application configuration which should have
         settings for the decider client.
     :param event_logger: The EventLogger to be used to log bucketing events.
```

### Comparing `reddit_experiments-1.3.9/reddit_experiments/__init__.py` & `reddit_experiments-1.4.0/reddit_experiments/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# DEPRECATED: please migrate to `reddit_decider` module.
+#
+# see docs for upgrade instructions:
+#   https://reddit-experiments.readthedocs.io/en/latest/#integrate-reddit-experiments-into-baseplate-service
 import json
 import logging
 import warnings
 
 from enum import Enum
 from typing import Dict
 from typing import Optional
@@ -121,14 +125,19 @@
         except WatchedFileNotAvailableError as exc:
             logger.warning("Experiment config unavailable: %s", str(exc))
         except TypeError as exc:
             logger.warning("Could not load experiment config: %s", str(exc))
         return {}
 
     def _get_experiment(self, name: str) -> Optional[Experiment]:
+        warn_deprecated(
+            "`_get_experiment()` in `reddit_experiments` module is deprecated, "
+            "use `get_experiment()` from `reddit_decider` module instead."
+        )
+
         if name in self._global_cache:
             return self._global_cache[name]
 
         if self._cfg_data is None:
             warn_deprecated("config_watcher will be removed in Baseplate 2.0.")
             self._cfg_data = self._get_config()
 
@@ -151,20 +160,26 @@
         """
         if self._cfg_data is None:
             self._cfg_data = self._config_watcher.get_data()
         experiment_names = list(self._cfg_data.keys())
         return experiment_names
 
     def is_valid_experiment(self, name: str) -> bool:
-        """Return true if the provided experiment name is a valid experiment.
+        """DEPRECATED.
+
+        Return true if the provided experiment name is a valid experiment.
 
         :param name: Name of the experiment you want to check.
 
         :return: Whether or not a particular experiment is valid.
         """
+        warn_deprecated(
+            "`is_valid_experiment()` in `reddit_experiments` module is deprecated, "
+            "use `get_experiment()` from `reddit_decider` module instead."
+        )
         return self._get_experiment(name) is not None
 
     @overload
     def variant(
         self,
         *,
         name: str,
@@ -189,15 +204,17 @@
         self,
         experiment_name: Optional[str] = None,
         user: Optional[User] = None,
         bucketing_event_override: Optional[bool] = None,
         name: Optional[str] = None,  # DEPRECATED
         **kwargs: str,
     ) -> Optional[str]:
-        r"""Return which variant, if any, is active.
+        r"""DEPRECATED.
+
+        Return which variant, if any, is active.
 
         If a variant is active, a bucketing event will be logged to the event
         pipeline unless any one of the following conditions are met:
 
         1. bucketing_event_override is set to False.
         2. The experiment specified by "name" explicitly disables bucketing
            events.
@@ -231,14 +248,19 @@
         :param kwargs:  Arguments that will be passed to experiment.variant to
             determine bucketing, targeting, and overrides. These values will also
             be passed to the logger.
 
         :return: Variant name if a variant is active, None otherwise.
 
         """
+        warn_deprecated(
+            "`variant()` in `reddit_experiments` module is deprecated, "
+            "use `get_variant*()` API from `reddit_decider` module instead."
+        )
+
         experiment_name = experiment_name or name
         assert experiment_name
         if name:
             warn_deprecated(
                 f"The 'name' parameter on 'variant' method is deprecated, use 'experiment_name' instead. (name={name})"
             )
         experiment = self._get_experiment(experiment_name)
@@ -287,24 +309,35 @@
             self._already_bucketed.add(bucketing_id)
 
         return variant
 
     def expose(
         self, experiment_name: str, variant_name: str, user: Optional[User] = None, **kwargs: str
     ) -> None:
-        """Log an event to indicate that a user has been exposed to an experimental treatment.
+        """DEPRECATED.
+
+        Log an event to indicate that a user has been exposed to an experimental treatment.
 
         :param experiment_name: Name of the experiment that was exposed.
         :param variant_name: Name of the variant that was exposed.
         :param user: User object for the user you want to check the experiment
             variant for. If unset, it is expected that user_id and logged_in values
             will be set in the keyword arguments.
         :param kwargs: Additional arguments that will be passed to logger.
 
         """
+        warn_deprecated(
+            "`expose()` in `reddit_experiments` module is deprecated, "
+            "for manual exposure use `expose()` API from `reddit_decider` module instead "
+            "(or use auto-exposure provided in `get_variant()`)."
+        )
+
+        if variant_name is None or variant_name == "":
+            return
+
         experiment = self._get_experiment(experiment_name)
 
         if experiment is None:
             return
 
         inputs = dict(kwargs)
 
@@ -321,58 +354,71 @@
             event_type=EventType.EXPOSE,
             inputs=inputs,
             span=self._span,
         )
 
 
 class ExperimentsClient(config.Parser):
-    """Configure an experiments client.
+    """DEPRECATED.
+
+    Configure an experiments client.
 
     This is meant to be used with
     :py:meth:`baseplate.Baseplate.configure_context`.
 
     See :py:func:`experiments_client_from_config` for available configuration settings.
 
     :param event_logger: The EventLogger instance to be used to log bucketing events.
 
     """
 
     def __init__(self, event_logger: EventLogger):
+        warn_deprecated(
+            "`ExperimentsClient` class in `reddit_experiments` module is deprecated, "
+            "use `DeciderClient` class from `reddit_decider` module instead."
+        )
         self.event_logger = event_logger
 
     def parse(self, key_path: str, raw_config: config.RawConfig) -> ExperimentsContextFactory:
         return experiments_client_from_config(raw_config, self.event_logger, prefix=f"{key_path}.")
 
 
 def experiments_client_from_config(
     app_config: config.RawConfig, event_logger: EventLogger, prefix: str = "experiments."
 ) -> ExperimentsContextFactory:
-    """Configure and return an :py:class:`ExperimentsContextFactory` object.
+    """DEPRECATED.
+
+    Configure and return an :py:class:`ExperimentsContextFactory` object.
 
     The keys used in your app's :code:`some_config.ini` file should be prefixed, e.g.
     ``experiments.path``, etc.
 
     Supported config keys:
 
         ``path`` (optional)
             The path to the experiment configuration file generated by the
             experiment configuration fetcher daemon.
         ``timeout`` (optional)
             The time that we should wait for the file specified by ``path`` to
-            exist.  Defaults to `None` which is `infinite`.
+            exist.  (defaults to not blocking).
         ``backoff`` (optional)
             The base amount of time for exponential backoff when trying to find the
             experiments config file. Defaults to no backoff between tries.
 
     :param raw_config: The application configuration which should have
         settings for the experiments client.
     :param event_logger: The EventLogger to be used to log bucketing events.
     :param prefix: the prefix used to filter keys (defaults to "experiments.").
 
     """
+    warn_deprecated(
+        "`experiments_client_from_config()` in `reddit_experiments` module is deprecated, "
+        "use `decider_client_from_config()` class from `reddit_decider` module instead."
+    )
+
     assert prefix.endswith(".")
     config_prefix = prefix[:-1]
 
     cfg = config.parse_config(
         app_config,
         {
             config_prefix: {
```

### Comparing `reddit_experiments-1.3.9/reddit_experiments/providers/__init__.py` & `reddit_experiments-1.4.0/reddit_experiments/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/providers/base.py` & `reddit_experiments-1.4.0/reddit_experiments/providers/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/providers/feature_flag.py` & `reddit_experiments-1.4.0/reddit_experiments/providers/feature_flag.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/providers/forced_variant.py` & `reddit_experiments-1.4.0/reddit_experiments/providers/forced_variant.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/providers/r2.py` & `reddit_experiments-1.4.0/reddit_experiments/providers/r2.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/providers/simple_experiment.py` & `reddit_experiments-1.4.0/reddit_experiments/providers/simple_experiment.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/targeting/tree_targeting.py` & `reddit_experiments-1.4.0/reddit_experiments/targeting/tree_targeting.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/variant_sets/base.py` & `reddit_experiments-1.4.0/reddit_experiments/variant_sets/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/variant_sets/multi_variant_set.py` & `reddit_experiments-1.4.0/reddit_experiments/variant_sets/multi_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/variant_sets/range_variant_set.py` & `reddit_experiments-1.4.0/reddit_experiments/variant_sets/range_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/variant_sets/rollout_variant_set.py` & `reddit_experiments-1.4.0/reddit_experiments/variant_sets/rollout_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments/variant_sets/single_variant_set.py` & `reddit_experiments-1.4.0/reddit_experiments/variant_sets/single_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/reddit_experiments.egg-info/PKG-INFO` & `reddit_experiments-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reddit-experiments
-Version: 1.3.9
+Name: reddit_experiments
+Version: 1.4.0
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
         
@@ -21,15 +21,15 @@
         $ pip install reddit-experiments
         ```
         
         Add the client to your application's Baseplate context:
         
         ```python
          from reddit_decider import decider_client_from_config
-         
+        
          decider = decider_client_from_config(
              app_config=app_config,
              event_logger=ExperimentLogger(),
              request_field_extractor=decider_field_extractor,
          )
          baseplate.add_to_context("decider", decider)
         ```
@@ -38,15 +38,16 @@
         
         ```python
         def my_method(request):
            if request.decider.get_variant("foo") == "bar":
                pass
         ```
         
-        See [the documentation] for more information.
+        See [the documentation] for more information (documentation builds can be found [here](https://readthedocs.org/projects/reddit-experiments/builds/))
+        .
         
         [the documentation]: https://reddit-experiments.readthedocs.io/
         
         ## Development
         
         A Dockerfile is provided to get a development environment running. To use it,
         build the base Docker image:
```

### Comparing `reddit_experiments-1.3.9/reddit_experiments.egg-info/SOURCES.txt` & `reddit_experiments-1.4.0/reddit_experiments.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/images/ddg-logo.png
 docs/images/favicon.png
 docs/legacy/index.rst
 reddit_decider/__init__.py
+reddit_decider/py.typed
 reddit_experiments/__init__.py
 reddit_experiments/py.typed
 reddit_experiments.egg-info/PKG-INFO
 reddit_experiments.egg-info/SOURCES.txt
 reddit_experiments.egg-info/dependency_links.txt
 reddit_experiments.egg-info/requires.txt
 reddit_experiments.egg-info/top_level.txt
```

### Comparing `reddit_experiments-1.3.9/requirements-transitive.txt` & `reddit_experiments-1.4.0/requirements-transitive.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 chardet==4.0.0
 click==7.1.2
 coverage==5.3.1
 gevent==21.12.0
 greenlet==1.1.1
 idna==2.10
 imagesize==1.2.0
+importlib-metadata==4.13.0
 iniconfig==1.1.1
 Jinja2==2.11.2
 MarkupSafe==1.1.1
 mccabe==0.6.1
 mypy-extensions==0.4.3
 packaging==20.8
 pathspec==0.8.1
```

### Comparing `reddit_experiments-1.3.9/setup.cfg` & `reddit_experiments-1.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -21,11 +21,14 @@
 no_implicit_optional = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_return_any = False
 no_implicit_reexport = True
 strict_equality = True
 
+[mypy-rust_decider]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `reddit_experiments-1.3.9/setup.py` & `reddit_experiments-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     use_scm_version=True,
     packages=find_packages(),
     python_requires=">=3.7",
     setup_requires=["setuptools_scm"],
     install_requires=[
         "baseplate>=2.0.0a1,<3.0",
         "reddit-edgecontext>=1.0.0a3,<2.0",
-        "reddit-decider>=1.2.18,<2.0",
+        "reddit-decider~=1.2.32",
         "typing_extensions>=3.10.0.0,<5.0",
     ],
-    package_data={"reddit_experiments": ["py.typed"]},
+    package_data={"reddit_experiments": ["py.typed"], "reddit_decider": ["py.typed"]},
     zip_safe=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `reddit_experiments-1.3.9/tests/decider_tests.py` & `reddit_experiments-1.4.0/tests/decider_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import json
 import logging
 import tempfile
 import unittest
+import warnings
 
 from unittest import mock
 
 from baseplate import RequestContext
 from baseplate import ServerSpan
 from baseplate.lib.events import DebugLogger
 from baseplate.lib.file_watcher import FileWatcher
@@ -19,30 +20,33 @@
 from reddit_decider import EventType
 from reddit_decider import init_decider_parser
 
 logger = logging.getLogger()
 
 USER_ID = "t2_1234"
 IS_LOGGED_IN = True
-AUTH_CLIENT_ID = "token"
-COUNTRY_CODE = "US"
-DEVICE_ID = "abc"
-COOKIE_CREATED_TIMESTAMP = 1234
-LOID_CREATED_TIMESTAMP = 123456
-LOCALE_CODE = "us_en"
-ORIGIN_SERVICE = "origin"
+AD_ACCOUNT_ID = "t2_4321"
 APP_NAME = "ios"
 APP_VERSION = "0.0.0.0"
+AUTH_CLIENT_ID = "token"
 BUILD_NUMBER = 1
+BUSINESS_ID = "t_some"
 CANONICAL_URL = "www.test.com"
+COOKIE_CREATED_TIMESTAMP = 1234
+COUNTRY_CODE = "US"
+DEVICE_ID = "abc"
 EVENT_FIELDS = {
     "user_id": USER_ID,
     "logged_in": IS_LOGGED_IN,
     "cookie_created_timestamp": COOKIE_CREATED_TIMESTAMP,
 }
+LOID_CREATED_TIMESTAMP = 123456
+LOCALE_CODE = "us_en"
+ORIGIN_SERVICE = "origin"
+SUBREDDIT_ID = "t5_123abc"
 
 
 @contextlib.contextmanager
 def create_temp_config_file(contents):
     with tempfile.NamedTemporaryFile() as f:
         f.write(json.dumps(contents).encode())
         f.seek(0)
@@ -54,14 +58,30 @@
         "app_name": APP_NAME,
         "app_version": APP_VERSION,
         "build_number": BUILD_NUMBER,
         "canonical_url": CANONICAL_URL,
     }
 
 
+def setup_decider(file_name, decider_context, mock_span, event_logger):
+    try:
+        rs_decider = init_decider_parser(file_name)
+    except Exception as e:
+        print(e)
+        rs_decider = None
+
+    return Decider(
+        decider_context=decider_context,
+        internal=rs_decider,
+        server_span=mock_span,
+        context_name="test",
+        event_logger=event_logger,
+    )
+
+
 def first_occurrence_of_key_in(array, dict_key, name):
     return next((v for v in array if v[dict_key] == name), None)
 
 
 @mock.patch("reddit_decider.FileWatcher")
 class DeciderClientFromConfigTests(unittest.TestCase):
     def setUp(self):
@@ -131,15 +151,15 @@
                 self.event_logger,
                 prefix="experiments.",
                 request_field_extractor=decider_field_extractor,
             )
         with self.assertLogs(logger, logging.WARN) as captured:
             # ensure no warnings are printed except for the dummy one
             # https://stackoverflow.com/a/61381576/4260179
-            logger.warn("Dummy warning")
+            logger.warning("Dummy warning")
             decider = decider_ctx_factory.make_object_for_context(name="test", span=self.mock_span)
             assert len(captured.records) == 1
             self.assertEqual(["WARNING:root:Dummy warning"], captured.output)
 
         self.assertIsInstance(decider, Decider)
 
         decider_context = getattr(decider, "_decider_context")
@@ -208,15 +228,15 @@
                 self.event_logger,
                 prefix="experiments.",
                 request_field_extractor=decider_field_extractor,
             )
         with self.assertLogs(logger, logging.WARN) as captured:
             # ensure no warnings are printed except for the dummy one
             # https://stackoverflow.com/a/61381576/4260179
-            logger.warn("Dummy warning")
+            logger.warning("Dummy warning")
 
             decider = decider_ctx_factory.make_object_for_context(name="test", span=None)
             assert len(captured.records) == 1
             self.assertEqual(["WARNING:root:Dummy warning"], captured.output)
 
         self.assertIsInstance(decider, Decider)
 
@@ -380,25 +400,14 @@
             device_id=DEVICE_ID,
             oauth_client_id=AUTH_CLIENT_ID,
             cookie_created_timestamp=COOKIE_CREATED_TIMESTAMP,
             loid_created_timestamp=LOID_CREATED_TIMESTAMP,
             extracted_fields=decider_field_extractor(_request=None),
         )
 
-    def setup_decider(self, file_name, decider_context):
-        filewatcher = FileWatcher(path=file_name, parser=init_decider_parser, timeout=2, backoff=2)
-
-        return Decider(
-            decider_context=decider_context,
-            config_watcher=filewatcher,
-            server_span=self.mock_span,
-            context_name="test",
-            event_logger=self.event_logger,
-        )
-
     def assert_exposure_event_fields(
         self,
         experiment_name: str,
         variant: str,
         event_fields: dict,
         bucket_val: str = "user_id",
         identifier: str = USER_ID,
@@ -439,108 +448,155 @@
         self.assertEqual(getattr(event_fields["experiment"], "name"), cfg["name"])
         self.assertEqual(getattr(event_fields["experiment"], "owner"), cfg["owner"])
         self.assertEqual(getattr(event_fields["experiment"], "version"), cfg["version"])
         self.assertEqual(getattr(event_fields["experiment"], "bucket_val"), bucket_val)
 
     def test_get_variant(self):
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant(experiment_name="exp_1")
             self.assertEqual(variant, "variant_4")
 
             # exposure assertions
             self.assertEqual(self.event_logger.log.call_count, 1)
             event_fields = self.event_logger.log.call_args[1]
             self.assert_exposure_event_fields(
                 experiment_name="exp_1", variant=variant, event_fields=event_fields
             )
 
-    def test_none_returned_on_variant_call_with_bad_id(self):
+    def test_none_returned_on_get_variant_call_with_bad_id(self):
         config = {
             "test": {
                 "id": "1",
                 "name": "test",
                 "owner": "test_owner",
                 "type": "r2",
                 "version": "1",
                 "start_ts": 0,
                 "stop_ts": 0,
                 "experiment": {
                     "id": 1,
                     "name": "test",
+                    "experiment_version": 1,
                     "variants": [
                         {"range_start": 0.0, "range_end": 0.2, "name": "active"},
                         {"range_start": 0.2, "range_end": 0.4, "name": "control_1"},
                         {"range_start": 0.4, "range_end": 0.6, "name": "control_2"},
                         {"range_start": 0.6, "range_end": 0.8, "name": "variant_3"},
                     ],
                 },
             }
         }
         with create_temp_config_file(config) as f:
-            decider = self.setup_decider(f.name, self.minimal_decider_context)
-
             with self.assertLogs() as captured:
+                decider = setup_decider(
+                    f, self.minimal_decider_context, self.mock_span, self.event_logger
+                )
                 variant = decider.get_variant("test")
 
                 self.assertEqual(variant, None)
                 self.assertEqual(self.event_logger.log.call_count, 0)
 
                 assert any(
-                    'Rust decider has initialization error: Decider initialization failed: Json error: "invalid type: string \\"1\\"'
+                    "Partially loaded Decider: 1 features failed to load: {'test': 'invalid type: string \"1\", expected u32'}"
                     in x.getMessage()
                     for x in captured.records
                 )
 
     def test_none_returned_on_get_variant_call_with_no_experiment_data(self):
         config = {
             "test": {
                 "id": 1,
                 "name": "test",
                 "owner": "test_owner",
-                "type": "r2",
+                "type": "dynamic_config",
                 "version": "1",
                 "start_ts": 0,
                 "stop_ts": 0,
             }
         }
         with create_temp_config_file(config) as f:
-            decider = self.setup_decider(f.name, self.minimal_decider_context)
+            decider = setup_decider(
+                f, self.minimal_decider_context, self.mock_span, self.event_logger
+            )
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant("test")
             self.assertEqual(variant, None)
 
+    def test_get_variant_calls_with_partial_data(self):
+        config = {
+            "test": {
+                "id": 1,
+                "name": "test",
+                "owner": "test_owner",
+                "type": "dynamic_config",
+                "version": "1",
+                "start_ts": 0,
+                "stop_ts": 0,
+            }
+        }
+        self.exp_base_config.update(config)
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
+            # get_variant_for_identifier()
+            variant = decider.get_variant_for_identifier("test", USER_ID, "user_id")
+            self.assertEqual(variant, None)
+
+            variant = decider.get_variant_for_identifier("exp_1", USER_ID, "user_id")
+            self.assertEqual(variant, "variant_4")
+
+            # get_variant()
+            variant = decider.get_variant("test")
+            self.assertEqual(variant, None)
+
+            variant = decider.get_variant("exp_1")
+            self.assertEqual(variant, "variant_4")
+
     def test_none_returned_on_get_variant_call_with_experiment_not_found(self):
         with create_temp_config_file({}) as f:
-            decider = self.setup_decider(f.name, self.minimal_decider_context)
+            decider = setup_decider(
+                f, self.minimal_decider_context, self.mock_span, self.event_logger
+            )
 
             self.assertEqual(self.event_logger.log.call_count, 0)
-            variant = decider.get_variant("anything")
+            with self.assertLogs(logger, logging.DEBUG) as captured:
+                variant = decider.get_variant("anything")
+
+                assert any(
+                    'Feature "anything" not found.' in x.getMessage() for x in captured.records
+                )
             self.assertEqual(variant, None)
 
+            # no exposures should be triggered
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
     def test_get_variant_without_expose(self):
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_without_expose(experiment_name="exp_1")
             self.assertEqual(variant, "variant_4")
 
             # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_get_variant_without_expose_for_holdout_exposure(self):
         self.exp_base_config["exp_1"].update({"parent_hg_name": "hg"})
         self.exp_base_config.update(self.parent_hg_config)
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_without_expose(experiment_name="exp_1")
             # user is part of Holdout (100% bucketing), so `None` is returned
             self.assertEqual(variant, None)
 
             # exposure assertions
@@ -548,21 +604,39 @@
             event_fields = self.event_logger.log.call_args[1]
 
             # `variant == None` for holdout but event will fire with `variant == "holdout"` for analysis
             self.assert_exposure_event_fields(
                 experiment_name="hg", variant="holdout", event_fields=event_fields
             )
 
+    def test_none_returned_on_get_variant_without_expose_call_with_experiment_not_found(self):
+        with create_temp_config_file({}) as f:
+            decider = setup_decider(
+                f, self.minimal_decider_context, self.mock_span, self.event_logger
+            )
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            with self.assertLogs(logger, logging.DEBUG) as captured:
+                variant = decider.get_variant_without_expose("anything")
+
+                assert any(
+                    'Feature "anything" not found.' in x.getMessage() for x in captured.records
+                )
+            self.assertEqual(variant, None)
+
+            # no exposures should be triggered
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
     def test_get_variant_for_identifier_user_id(self):
         identifier = USER_ID
         bucket_val = "user_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier(
                 experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
             self.assertEqual(variant, "variant_4")
 
@@ -581,15 +655,15 @@
 
     def test_get_variant_for_identifier_canonical_url(self):
         identifier = CANONICAL_URL
         bucket_val = "canonical_url"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier(
                 experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
             self.assertEqual(variant, "variant_3")
 
@@ -609,15 +683,15 @@
 
     def test_get_variant_for_identifier_device_id(self):
         identifier = DEVICE_ID
         bucket_val = "device_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier(
                 experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
             self.assertEqual(variant, "variant_3")
 
@@ -631,84 +705,169 @@
                 bucket_val=bucket_val,
                 identifier=identifier,
             )
 
             # `identifier` passed to correct event field of experiment's `bucket_val` config
             self.assertEqual(event_fields["device_id"], identifier)
 
-    def test_get_variant_for_identifier_wrong_bucket_val(self):
-        identifier = USER_ID
-        bucket_val = "device_id"
+    def test_get_variant_for_identifier_subreddit_id(self):
+        identifier = SUBREDDIT_ID
+        bucket_val = "subreddit_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
-            with self.assertLogs() as captured:
-                # `identifier_type="canonical_url"`, which doesn't match `bucket_val` of `device_id`
-                variant = decider.get_variant_for_identifier(
-                    experiment_name="exp_1", identifier=identifier, identifier_type="canonical_url"
-                )
-                # `None` is returned since `identifier_type` doesn't match `bucket_val` in experiment-config json
-                self.assertEqual(variant, None)
-                # exposure isn't emitted either
-                self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_for_identifier(
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
+            )
+            self.assertEqual(variant, "control_1")
 
-                assert any(
-                    'Requested identifier_type: "canonical_url" is incompatible with experiment\'s bucket_val = device_id.'
-                    in x.getMessage()
-                    for x in captured.records
-                )
+            # exposure assertions
+            self.assertEqual(self.event_logger.log.call_count, 1)
+            event_fields = self.event_logger.log.call_args[1]
+            self.assert_minimal_exposure_event_fields(
+                experiment_name="exp_1",
+                variant=variant,
+                event_fields=event_fields,
+                bucket_val=bucket_val,
+                identifier=identifier,
+            )
+
+            # `identifier` passed to correct event field of experiment's `bucket_val` config
+            self.assertEqual(event_fields["subreddit_id"], identifier)
+
+    def test_get_variant_for_identifier_ad_account_id(self):
+        identifier = AD_ACCOUNT_ID
+        bucket_val = "ad_account_id"
+        self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_for_identifier(
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
+            )
+            self.assertEqual(variant, "variant_2")
+
+            # exposure assertions
+            self.assertEqual(self.event_logger.log.call_count, 1)
+            event_fields = self.event_logger.log.call_args[1]
+            self.assert_minimal_exposure_event_fields(
+                experiment_name="exp_1",
+                variant=variant,
+                event_fields=event_fields,
+                bucket_val=bucket_val,
+                identifier=identifier,
+            )
+
+            # `identifier` passed to correct event field of experiment's `bucket_val` config
+            self.assertEqual(event_fields["ad_account_id"], identifier)
+
+    def test_get_variant_for_identifier_business_id(self):
+        identifier = BUSINESS_ID
+        bucket_val = "business_id"
+        self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_for_identifier(
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
+            )
+            self.assertEqual(variant, "control_2")
+
+            # exposure assertions
+            self.assertEqual(self.event_logger.log.call_count, 1)
+            event_fields = self.event_logger.log.call_args[1]
+            self.assert_minimal_exposure_event_fields(
+                experiment_name="exp_1",
+                variant=variant,
+                event_fields=event_fields,
+                bucket_val=bucket_val,
+                identifier=identifier,
+            )
+
+            # `identifier` passed to correct event field of experiment's `bucket_val` config
+            self.assertEqual(event_fields["business_id"], identifier)
 
     def test_get_variant_for_identifier_bogus_identifier_type(self):
         identifier = "anything"
         identifier_type = "blah"
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.minimal_decider_context)
+            decider = setup_decider(
+                f, self.minimal_decider_context, self.mock_span, self.event_logger
+            )
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             with self.assertLogs() as captured:
                 variant = decider.get_variant_for_identifier(
                     experiment_name="exp_1", identifier=identifier, identifier_type=identifier_type
                 )
 
                 self.assertEqual(variant, None)
 
                 assert any(
-                    "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url']."
+                    "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url', 'subreddit_id', 'ad_account_id', 'business_id']."
                     in x.getMessage()
                     for x in captured.records
                 )
 
         # exposure isn't emitted either
         self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_expose(self):
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = "variant_4"
             decider.expose("exp_1", variant)
 
             # exposure assertions
             self.assertEqual(self.event_logger.log.call_count, 1)
             event_fields = self.event_logger.log.call_args[1]
             self.assert_exposure_event_fields(
                 experiment_name="exp_1", variant=variant, event_fields=event_fields
             )
 
+    def test_feature_rollout_does_not_expose(self):
+        self.exp_base_config["exp_1"].update({"emit_event": False})
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = "variant_4"
+            decider.expose("exp_1", variant)
+
+            # exposure not fired
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
+    def test_expose_without_variant_name(self):
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f.name, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
+            decider.expose("exp_1", None)
+
+            # exposure assertions
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
     def test_get_variant_for_identifier_without_expose_user_id(self):
         identifier = USER_ID
         bucket_val = "user_id"
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier_without_expose(
                 experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
             self.assertEqual(variant, "variant_4")
 
@@ -719,15 +878,15 @@
         identifier = USER_ID
         bucket_val = "user_id"
 
         self.exp_base_config["exp_1"].update({"parent_hg_name": "hg"})
         self.exp_base_config.update(self.parent_hg_config)
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier_without_expose(
                 experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
             # user is part of Holdout (100% bucketing), so `None` is returned
             self.assertEqual(variant, None)
@@ -737,108 +896,129 @@
             event_fields = self.event_logger.log.call_args[1]
 
             # `variant == None` for holdout but event will fire with `variant == "holdout"` for analysis
             self.assert_minimal_exposure_event_fields(
                 experiment_name="hg", variant="holdout", event_fields=event_fields
             )
 
-    def test_get_variant_for_identifier_without_expose_for_holdout_exposure_wrong_bucket_val(self):
+    def test_get_variant_for_identifier_without_expose_canonical_url(self):
+        identifier = CANONICAL_URL
+        bucket_val = "canonical_url"
+        self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_for_identifier_without_expose(
+                experiment_name="exp_1", identifier=identifier, identifier_type="canonical_url"
+            )
+            self.assertEqual(variant, "variant_3")
+
+            # no exposures should be triggered
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
+    def test_get_variant_for_identifier_without_expose_device_id(self):
         identifier = DEVICE_ID
         bucket_val = "device_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
-        self.exp_base_config["exp_1"].update({"parent_hg_name": "hg"})
-        self.parent_hg_config["hg"]["experiment"].update({"bucket_val": bucket_val})
-        self.exp_base_config.update(self.parent_hg_config)
-
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
-            # `identifier_type="canonical_url"`, which doesn't match `bucket_val` of `device_id`
+            variant = decider.get_variant_for_identifier_without_expose(
+                experiment_name="exp_1", identifier=identifier, identifier_type="device_id"
+            )
+            self.assertEqual(variant, "variant_3")
+
+            # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
-            with self.assertLogs() as captured:
-                variant = decider.get_variant_for_identifier_without_expose(
-                    experiment_name="exp_1", identifier=identifier, identifier_type="canonical_url"
-                )
-                # `None` is returned since `identifier_type` doesn't match `bucket_val` in experiment-config json
-                self.assertEqual(variant, None)
 
-                assert any(
-                    'Encountered error in decider.choose(): Requested identifier_type: "canonical_url" is incompatible with experiment\'s bucket_val = device_id.'
-                    in x.getMessage()
-                    for x in captured.records
-                )
+    def test_get_variant_for_identifier_without_expose_subreddit_id(self):
+        identifier = SUBREDDIT_ID
+        bucket_val = "subreddit_id"
+        self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_for_identifier_without_expose(
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
+            )
+            self.assertEqual(variant, "control_1")
 
-    def test_get_variant_for_identifier_without_expose_canonical_url(self):
-        identifier = CANONICAL_URL
-        bucket_val = "canonical_url"
+            # no exposures should be triggered
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
+    def test_get_variant_for_identifier_without_expose_ad_account_id(self):
+        identifier = AD_ACCOUNT_ID
+        bucket_val = "ad_account_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier_without_expose(
-                experiment_name="exp_1", identifier=identifier, identifier_type="canonical_url"
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
-            self.assertEqual(variant, "variant_3")
+            self.assertEqual(variant, "variant_2")
 
             # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
 
-    def test_get_variant_for_identifier_without_expose_device_id(self):
-        identifier = DEVICE_ID
-        bucket_val = "device_id"
+    def test_get_variant_for_identifier_without_expose_business_id(self):
+        identifier = BUSINESS_ID
+        bucket_val = "business_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_for_identifier_without_expose(
-                experiment_name="exp_1", identifier=identifier, identifier_type="device_id"
+                experiment_name="exp_1", identifier=identifier, identifier_type=bucket_val
             )
-            self.assertEqual(variant, "variant_3")
+            self.assertEqual(variant, "control_2")
 
             # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_get_variant_for_identifier_without_expose_bogus_identifier_type(self):
         identifier = "anything"
         identifier_type = "blah"
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             with self.assertLogs() as captured:
                 variant = decider.get_variant_for_identifier_without_expose(
                     experiment_name="exp_1", identifier=identifier, identifier_type=identifier_type
                 )
 
                 self.assertEqual(variant, None)
 
                 assert any(
-                    "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url']."
+                    "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url', 'subreddit_id', 'ad_account_id', 'business_id']."
                     in x.getMessage()
                     for x in captured.records
                 )
 
             # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_get_all_variants_without_expose(self):
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_without_expose()
 
             self.assertEqual(len(variant_arr), len(self.exp_base_config))
             self.assertEqual(
                 first_occurrence_of_key_in(variant_arr, "experimentName", "exp_1"),
@@ -861,15 +1041,15 @@
         self.exp_base_config["exp_1"].update({"parent_hg_name": "hg"})
         self.exp_base_config.update(self.parent_hg_config)
 
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_without_expose()
 
             # "exp_1" returns variant None (due to "hg") and is excluded from the response arr
             self.assertEqual(len(variant_arr), len(self.exp_base_config) - 1)
             self.assertEqual(
@@ -893,23 +1073,53 @@
             event_fields = self.event_logger.log.call_args[1]
 
             # `variant == None` for holdout but event will fire with `variant == "holdout"` for analysis
             self.assert_exposure_event_fields(
                 experiment_name="hg", variant="holdout", event_fields=event_fields
             )
 
+    def test_get_all_variants_without_expose_ctx_missing_device_id(self):
+        # no device_id in ctx
+        dc = DeciderContext(user_id=USER_ID)
+
+        self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": "device_id"})
+        self.exp_base_config.update(self.additional_two_exp)
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
+            decision_arr = decider.get_all_variants_without_expose()
+
+            # device_id experiment not bucketed since
+            # device_id is missing in ctx
+            self.assertEqual(len(decision_arr), 2)
+
+            self.assertEqual(
+                first_occurrence_of_key_in(decision_arr, "experimentName", "e1"),
+                {"id": 6, "name": "e1treat", "version": "4", "experimentName": "e1"},
+            )
+            self.assertEqual(
+                first_occurrence_of_key_in(decision_arr, "experimentName", "e2"),
+                {"id": 7, "name": "e2treat", "version": "5", "experimentName": "e2"},
+            )
+
+            # no exposures should be triggered
+            self.assertEqual(self.event_logger.log.call_count, 0)
+
     def test_get_all_variants_for_identifier_without_expose_user_id(self):
         identifier = USER_ID
         bucket_val = "user_id"
 
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
             self.assertEqual(len(variant_arr), len(self.exp_base_config))
@@ -935,15 +1145,17 @@
 
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
         # alter `bucket_val` on exp_1 to induce err() due to `identifier_type` mismatch
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": "device_id"})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.minimal_decider_context)
+            decider = setup_decider(
+                f, self.minimal_decider_context, self.mock_span, self.event_logger
+            )
 
             self.assertEqual(self.event_logger.log.call_count, 0)
 
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
@@ -972,15 +1184,15 @@
         self.exp_base_config["exp_1"].update({"parent_hg_name": "hg"})
         self.exp_base_config.update(self.parent_hg_config)
 
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
             # "exp_1" returns variant None (due to "hg") and is excluded from the response dict
@@ -1017,15 +1229,15 @@
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         for exp_name in self.exp_base_config.keys():
             self.exp_base_config[exp_name]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
             self.assertEqual(len(variant_arr), len(self.exp_base_config))
@@ -1056,15 +1268,15 @@
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         for exp_name in self.exp_base_config.keys():
             self.exp_base_config[exp_name]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
             # "exp_1" returns variant None (due to "hg") and is excluded from the response dict
@@ -1101,38 +1313,37 @@
     def test_get_all_variants_for_identifier_without_expose_canonical_url(self):
         identifier = CANONICAL_URL
         bucket_val = "canonical_url"
 
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
-        for exp_name in self.exp_base_config.keys():
+        # update 2 of 3 experiments to have bucket_val: 'canonical_url'
+        # so that the 3rd one is filtered out
+        for exp_name in list(self.exp_base_config.keys())[0:2]:
             self.exp_base_config[exp_name]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
-            self.assertEqual(len(variant_arr), len(self.exp_base_config))
+            # non-canonical_url experiment is not included in result
+            self.assertEqual(len(variant_arr), 2)
             self.assertEqual(
                 first_occurrence_of_key_in(variant_arr, "experimentName", "exp_1"),
                 {"id": 1, "name": "variant_3", "version": "2", "experimentName": "exp_1"},
             )
             self.assertEqual(
                 first_occurrence_of_key_in(variant_arr, "experimentName", "e1"),
                 {"id": 6, "name": "e1treat", "version": "4", "experimentName": "e1"},
             )
-            self.assertEqual(
-                first_occurrence_of_key_in(variant_arr, "experimentName", "e2"),
-                {"id": 7, "name": "e2treat", "version": "5", "experimentName": "e2"},
-            )
 
             # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_get_all_variants_for_identifier_without_expose_canonical_url_with_hg(self):
         identifier = CANONICAL_URL
         bucket_val = "canonical_url"
@@ -1144,15 +1355,15 @@
         # add 2 more experiments
         self.exp_base_config.update(self.additional_two_exp)
 
         for exp_name in self.exp_base_config.keys():
             self.exp_base_config[exp_name]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant_arr = decider.get_all_variants_for_identifier_without_expose(
                 identifier=identifier, identifier_type=bucket_val
             )
 
             # "exp_1" returns variant None (due to "hg") and is excluded from the response dict
@@ -1188,37 +1399,37 @@
 
     def test_get_all_variants_for_identifier_without_expose_bogus_identifier_type(self):
         identifier = "anything"
         # use non-supported `identifier_type`
         identifier_type = "blah"
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
 
             with self.assertLogs() as captured:
                 variant_arr = decider.get_all_variants_for_identifier_without_expose(
                     identifier=identifier, identifier_type="blah"
                 )
 
                 self.assertEqual(len(variant_arr), 0)
 
                 assert any(
-                    "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url']."
+                    "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url', 'subreddit_id', 'ad_account_id', 'business_id']."
                     in x.getMessage()
                     for x in captured.records
                 )
 
             # no exposures should be triggered
             self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_get_variant_with_exposure_kwargs(self):
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             exp_kwargs = {"foo": "test_1", "bar": "test_2"}
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant(experiment_name="exp_1", **exp_kwargs)
             self.assertEqual(variant, "variant_4")
 
             # exposure assertions
@@ -1235,37 +1446,71 @@
             self.assertEqual(event_fields["inputs"]["foo"], exp_kwargs["foo"])
             self.assertEqual(event_fields["inputs"]["bar"], exp_kwargs["bar"])
 
     def test_get_variant_with_disabled_exp(self):
         self.exp_base_config["exp_1"].update({"enabled": False})
 
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant(experiment_name="exp_1")
             self.assertEqual(variant, None)
 
             # exposure assertions
             self.assertEqual(self.event_logger.log.call_count, 0)
 
     def test_get_experiment(self):
         with create_temp_config_file(self.exp_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             experiment = decider.get_experiment("exp_1")
 
             cfg = self.exp_base_config["exp_1"]
             self.assertEqual(experiment.id, cfg["id"])
             self.assertEqual(experiment.name, cfg["name"])
             self.assertEqual(experiment.version, cfg["version"])
             self.assertEqual(experiment.bucket_val, cfg["experiment"]["bucket_val"])
             self.assertEqual(experiment.start_ts, cfg["start_ts"])
             self.assertEqual(experiment.stop_ts, cfg["stop_ts"])
             self.assertEqual(experiment.owner, cfg["owner"])
+            self.assertEqual(experiment.emit_event, True)
+
+    def test_get_variant_without_expose_with_HG_as_control_1_and_child_returns_none_does_expose(
+        self,
+    ):
+        self.exp_base_config["exp_1"].update({"parent_hg_name": "hg"})
+        # force child "exp_1" to return `None`
+        self.exp_base_config["exp_1"]["experiment"]["variants"] = [
+            {"name": "control_1", "size": 0.0, "range_end": 0.0, "range_start": 0.0},
+        ]
+
+        self.exp_base_config.update(self.parent_hg_config)
+        # force "hg" to bucket "control_1"
+        self.exp_base_config["hg"]["experiment"]["variants"] = [
+            {"name": "control_1", "size": 1.00, "range_end": 1.0, "range_start": 0},
+            {"name": "holdout", "size": 0.00, "range_end": 0.0, "range_start": 0.00},
+        ]
+
+        with create_temp_config_file(self.exp_base_config) as f:
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
+
+            self.assertEqual(self.event_logger.log.call_count, 0)
+            variant = decider.get_variant_without_expose("exp_1")
+
+            assert variant == None
+
+            # exposure from control_1 of "hg"
+            self.assertEqual(self.event_logger.log.call_count, 1)
+            event_fields = self.event_logger.log.call_args[1]
+
+            # `variant == None` for child but event will fire with `variant == "control_1"` for analysis
+            self.assert_exposure_event_fields(
+                experiment_name="hg", variant="control_1", event_fields=event_fields
+            )
 
 
 class TestDeciderGetDynamicConfig(unittest.TestCase):
     def setUp(self):
         super().setUp()
         self.event_logger = mock.Mock(spec=DebugLogger)
         self.mock_span = mock.MagicMock(spec=ServerSpan)
@@ -1295,76 +1540,65 @@
             user_is_employee=True,
             device_id=DEVICE_ID,
             oauth_client_id=AUTH_CLIENT_ID,
             cookie_created_timestamp=COOKIE_CREATED_TIMESTAMP,
             loid_created_timestamp=LOID_CREATED_TIMESTAMP,
         )
 
-    def setup_decider(self, file_name, decider_context):
-        filewatcher = FileWatcher(path=file_name, parser=init_decider_parser, timeout=2, backoff=2)
-
-        return Decider(
-            decider_context=decider_context,
-            config_watcher=filewatcher,
-            server_span=self.mock_span,
-            context_name="test",
-            event_logger=self.event_logger,
-        )
-
     def test_get_bool(self):
         self.dc_base_config["dc_1"].update({"value_type": "Boolean", "value": True})
 
         with create_temp_config_file(self.dc_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             res = decider.get_bool("dc_1")
             self.assertEqual(res, True)
             res = decider.get_float("dc_1")
             self.assertEqual(res, 0.0)
 
     def test_get_int(self):
         self.dc_base_config["dc_1"].update({"value_type": "Integer", "value": 7})
 
         with create_temp_config_file(self.dc_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             res = decider.get_int("dc_1")
             self.assertEqual(res, 7)
             res = decider.get_float("dc_1")
             self.assertEqual(res, 7.0)
 
     def test_get_float(self):
         self.dc_base_config["dc_1"].update({"value_type": "Float", "value": 4.20})
 
         with create_temp_config_file(self.dc_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             res = decider.get_float("dc_1")
             self.assertEqual(res, 4.20)
             res = decider.get_int("dc_1")
             self.assertEqual(res, 0)
 
     def test_get_string(self):
         self.dc_base_config["dc_1"].update({"value_type": "Text", "value": "helloworld!"})
 
         with create_temp_config_file(self.dc_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             res = decider.get_string("dc_1")
             self.assertEqual(res, "helloworld!")
             res = decider.get_int("dc_1")
             self.assertEqual(res, 0)
 
     def test_get_map(self):
         self.dc_base_config["dc_1"].update(
             {"value_type": "Map", "value": {"key": "value", "another_key": "another_value"}}
         )
 
         with create_temp_config_file(self.dc_base_config) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             res = decider.get_map("dc_1")
             self.assertEqual(res, dict({"key": "value", "another_key": "another_value"}))
             res = decider.get_string("dc_1")
             self.assertEqual(res, "")
 
     def test_get_all_values(self):
@@ -1521,17 +1755,16 @@
         experiments_cfg.update(cfg_missing_string)
         experiments_cfg.update(cfg_missing_text)
         experiments_cfg.update(cfg_missing_map)
 
         # missing "value_type" field
         experiments_cfg.update(missing_value_type_cfg)
 
-        print(experiments_cfg)
         with create_temp_config_file(experiments_cfg) as f:
-            decider = self.setup_decider(f.name, self.dc)
+            decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             configs = decider.get_all_dynamic_configs()
 
             # 6 correct DCs, 6 DCs w/ values set to respective defaults
             # 1 `missing_value_type_cfg` which sets "type" to empty string
             # (3 regular experiments are excluded)
             self.assertEqual(len(configs), 13)
@@ -1608,15 +1841,14 @@
 
             missing_map_val_res = first_occurrence_of_key_in(configs, "name", "dc_missing_map")
             self.assertEqual(
                 missing_map_val_res,
                 {"name": "dc_missing_map", "value": {}, "type": "map"},
             )
 
-            # set "type" to empty string if "value_type" is missing on cfg
             missing_map_val_res = first_occurrence_of_key_in(
                 configs, "name", "dc_missing_value_type"
             )
             self.assertEqual(
                 missing_map_val_res,
-                {"name": "dc_missing_value_type", "value": False, "type": ""},
+                {"name": "dc_missing_value_type", "value": False, "type": "boolean"},
             )
```

### Comparing `reddit_experiments-1.3.9/tests/experiment_tests.py` & `reddit_experiments-1.4.0/tests/experiment_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.mock_span.trace_id = "123456"
         self.user_name = "gary"
         self.mock_authentication_token = mock.Mock(spec=AuthenticationToken)
         self.mock_authentication_token.subject = "t2_1"
         self.mock_authentication_token.user_roles = set()
         self.user = User(
             authentication_token=self.mock_authentication_token,
-            loid="t2_1",
+            loid_="t2_1",
             cookie_created_ms=10000,
         )
 
     def test_bucketing_event_fields(self):
         self.mock_filewatcher.get_data.return_value = {
             "test": {
                 "id": 1,
@@ -255,14 +255,46 @@
         self.assertNotEqual(event_fields["span"], None)
 
         self.assertEqual(getattr(event_fields["experiment"], "id"), 1)
         self.assertEqual(getattr(event_fields["experiment"], "name"), "test")
         self.assertEqual(getattr(event_fields["experiment"], "owner"), "test_owner")
         self.assertEqual(getattr(event_fields["experiment"], "version"), "1")
 
+    def test_expose_without_variant_name(self):
+        cfg_data = {
+            "test": {
+                "id": 1,
+                "name": "test",
+                "owner": "test_owner",
+                "type": "r2",
+                "version": "1",
+                "start_ts": time.time() - THIRTY_DAYS,
+                "stop_ts": time.time() + THIRTY_DAYS,
+                "experiment": {
+                    "id": 1,
+                    "name": "test",
+                    "variants": {"active": 10, "control_1": 10, "control_2": 10},
+                },
+            }
+        }
+        experiments = Experiments(
+            config_watcher=self.mock_filewatcher,
+            server_span=self.mock_span,
+            context_name="test",
+            cfg_data=cfg_data,
+            global_cache={},
+            event_logger=self.event_logger,
+        )
+
+        self.assertEqual(self.event_logger.log.call_count, 0)
+
+        experiments.expose("test", variant_name=None, user=self.user, app_name="r2")
+
+        self.assertEqual(self.event_logger.log.call_count, 0)
+
     def test_that_override_true_has_no_effect_with_cfg_data(self):
         cfg_data = {
             "test": {
                 "id": 1,
                 "name": "test",
                 "owner": "test",
                 "type": "r2",
```

### Comparing `reddit_experiments-1.3.9/tests/providers/feature_flag_tests.py` & `reddit_experiments-1.4.0/tests/providers/feature_flag_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/forced_variant_tests.py` & `reddit_experiments-1.4.0/tests/providers/forced_variant_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/r2_tests.py` & `reddit_experiments-1.4.0/tests/providers/r2_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/simple_experiment_tests.py` & `reddit_experiments-1.4.0/tests/providers/simple_experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/variant_sets/multi_variant_set_tests.py` & `reddit_experiments-1.4.0/tests/providers/variant_sets/multi_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/variant_sets/range_variant_set_tests.py` & `reddit_experiments-1.4.0/tests/providers/variant_sets/range_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/variant_sets/rollout_variant_set_tests.py` & `reddit_experiments-1.4.0/tests/providers/variant_sets/rollout_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/providers/variant_sets/single_variant_set_tests.py` & `reddit_experiments-1.4.0/tests/providers/variant_sets/single_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/range_variant_tests/data/original_zk_config.json` & `reddit_experiments-1.4.0/tests/range_variant_tests/data/original_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/range_variant_tests/data/output.json` & `reddit_experiments-1.4.0/tests/range_variant_tests/data/output.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/range_variant_tests/data/range_variant_zk_config.json` & `reddit_experiments-1.4.0/tests/range_variant_tests/data/range_variant_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.3.9/tests/range_variant_tests/range_variant_parity_tests.py` & `reddit_experiments-1.4.0/tests/range_variant_tests/range_variant_parity_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 class TestExperiments(unittest.TestCase):
     def setUp(self):
         super().setUp()
         with open(ORIGINAL_ZK_CONFIG_FILE, "r") as f:
             self.original_zk_config = json.load(f)
         with open(RANGE_VARIANT_ZK_CONFIG_FILE, "r") as f:
+            self.range_variant_zk_file = f
             self.range_variant_zk_config = json.load(f)
         self.mock_filewatcher = mock.Mock(spec=FileWatcher)
         self.mock_span = mock.MagicMock(spec=ServerSpan)
         self.mock_span.context = None
         self.mock_span.trace_id = "123456"
         self.mock_authentication_token = mock.Mock(spec=AuthenticationToken)
         self.mock_authentication_token.user_roles = set()
@@ -46,29 +47,27 @@
         rv_experiments = Experiments(
             config_watcher=self.mock_filewatcher,
             server_span=self.mock_span,
             context_name="test",
             cfg_data=self.range_variant_zk_config,
         )
 
-        filewatcher = FileWatcher(
-            path=RANGE_VARIANT_ZK_CONFIG_FILE, parser=init_decider_parser, timeout=2, backoff=2
-        )
+        rs_decider = init_decider_parser(self.range_variant_zk_file)
         extracted_fields = {"app_name": "", "build_number": 0}
 
         # results = {}
         for experiment_name in self.original_zk_config.keys():
             for i in range(NUMBER_OF_TEST_USERS):
                 uuid = "t2_" + str(i)
 
                 # experiments sdk
                 self.mock_authentication_token.subject = uuid
                 user = User(
                     authentication_token=self.mock_authentication_token,
-                    loid=uuid,
+                    loid_=uuid,
                     cookie_created_ms=10000,
                 )
 
                 og_variant = original_experiments.variant(
                     experiment_name, user=user, **extracted_fields
                 )
                 rv_variant = rv_experiments.variant(experiment_name, user=user, **extracted_fields)
@@ -82,15 +81,15 @@
                 self.assertEqual(og_variant, rv_variant)
 
                 # decider sdk
                 decider_context = DeciderContext(user_id=uuid, extracted_fields=extracted_fields)
 
                 decider = Decider(
                     decider_context=decider_context,
-                    config_watcher=filewatcher,
+                    internal=rs_decider,
                     server_span=self.mock_span,
                     context_name="test",
                     event_logger=self.event_logger,
                 )
 
                 decider_variant = decider.get_variant(experiment_name=experiment_name)
```

### Comparing `reddit_experiments-1.3.9/tests/targeting/tree_targeting_tests.py` & `reddit_experiments-1.4.0/tests/targeting/tree_targeting_tests.py`

 * *Files identical despite different names*


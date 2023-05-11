# Comparing `tmp/substrafl-0.35.1rc1.tar.gz` & `tmp/substrafl-0.36.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.35.1rc1.tar", last modified: Tue Apr 11 14:52:27 2023, max compression
+gzip compressed data, was "substrafl-0.36.0rc1.tar", last modified: Thu May 11 14:30:53 2023, max compression
```

## Comparing `substrafl-0.35.1rc1.tar` & `substrafl-0.36.0rc1.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.042597 substrafl-0.35.1rc1/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.042597 substrafl-0.35.1rc1/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18027 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.046597 substrafl-0.35.1rc1/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/register/generate_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.050597 substrafl-0.35.1rc1/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14974 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-04-11 14:52:21.000000 substrafl-0.35.1rc1/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:52:27.042597 substrafl-0.35.1rc1/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-11 14:52:27.000000 substrafl-0.35.1rc1/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 14:52:26.000000 substrafl-0.35.1rc1/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.552012 substrafl-0.36.0rc1/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.552012 substrafl-0.36.0rc1/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/register/generate_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.556012 substrafl-0.36.0rc1/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/fed_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-11 14:30:47.000000 substrafl-0.36.0rc1/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:30:53.552012 substrafl-0.36.0rc1/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 14:30:53.000000 substrafl-0.36.0rc1/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.35.1rc1/LICENSE` & `substrafl-0.36.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/PKG-INFO` & `substrafl-0.36.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.35.1rc1
+Version: 0.36.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.35.1rc1/README.md` & `substrafl-0.36.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/pyproject.toml` & `substrafl-0.36.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/setup.py` & `substrafl-0.36.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,26 +38,27 @@
     packages=find_packages(exclude=["tests*", "benchmark*"]),
     # Not compatible with substratools 0.8.0 because
     # that release is private and in the Docker container
     # it has access only to the public PyPi
     install_requires=[
         "numpy>=1.20.3,!=1.24.*",
         "cloudpickle>=1.6.0",
-        "substra~=0.43.0",
+        "substra~=0.44.0",
         "substratools~=0.20.0",
         "pydantic>=1.9.0",
         "pip>=21.2",
         "wheel",
         "six",
         "packaging",
     ],
     extras_require={
         "dev": [
             "pytest>=6.2.4",
             "pytest-cov>=2.12.0",
+            "pytest-mock",
             "pre-commit>=2.13.0",
             "types-PyYAML>=6.0.0",
             "torch>=1.9.1,!=1.12.0",  # bug in 1.12.0 (https://github.com/pytorch/pytorch/pull/80345)
             "nbmake>=1.1",
             "docker",
         ],
     },
```

### Comparing `substrafl-0.35.1rc1/substrafl/__init__.py` & `substrafl-0.36.0rc1/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/algo.py` & `substrafl-0.36.0rc1/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from torch import __version__ as torch_version
 
 from substrafl.algorithms.pytorch.torch_fed_avg_algo import TorchFedAvgAlgo
+from substrafl.algorithms.pytorch.torch_fed_pca_algo import TorchFedPCAAlgo
 from substrafl.algorithms.pytorch.torch_newton_raphson_algo import TorchNewtonRaphsonAlgo
 from substrafl.algorithms.pytorch.torch_scaffold_algo import TorchScaffoldAlgo
 from substrafl.algorithms.pytorch.torch_single_organization_algo import TorchSingleOrganizationAlgo
 from substrafl.exceptions import UnsupportedPytorchVersionError
 
 if torch_version == "1.12.0":
     raise UnsupportedPytorchVersionError(
         "Please use an other pytorch version. There is a regression bug in torch 1.12.0, that impacts optimizers that "
         "have been pickled and unpickled. "
         "This bug occurs for Adam optimizer for example (but not for SGD). Here is a link to one issue covering it: "
         "https://github.com/pytorch/pytorch/pull/80345"
     )
 
 
-__all__ = ["TorchFedAvgAlgo", "TorchSingleOrganizationAlgo", "TorchScaffoldAlgo", "TorchNewtonRaphsonAlgo"]
+__all__ = [
+    "TorchFedAvgAlgo",
+    "TorchFedPCAAlgo",
+    "TorchSingleOrganizationAlgo",
+    "TorchScaffoldAlgo",
+    "TorchNewtonRaphsonAlgo",
+]
```

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         shared_state: Any = None,
     ) -> Any:
         # Must be implemented in the child class
         raise NotImplementedError()
 
     @remote_data
     def predict(self, datasamples: Any, shared_state: Any = None, predictions_path: os.PathLike = None) -> Any:
-        """Executes the following operations:
+        """Execute the following operations:
 
             * Create the test torch dataset.
             * Execute and return the results of the ``self._local_predict`` method
 
         Args:
             datasamples (typing.Any): Input data
             shared_state (typing.Any): Latest train task shared state (output of the train method)
@@ -118,18 +118,18 @@
             predictions_path (os.PathLike): destination file to save predictions.
         """
         if predictions_path is not None:
             np.save(predictions_path, predictions)
             shutil.move(str(predictions_path) + ".npy", predictions_path)
 
     def _local_predict(self, predict_dataset: torch.utils.data.Dataset, predictions_path):
-        """Executes the following operations:
+        """Execute the following operations:
 
             * Create the torch dataloader using the index generator batch size.
-            * Sets the model to `eval` mode
+            * Set the model to `eval` mode
             * Save the predictions using the
               :py:func:`~substrafl.algorithms.pytorch.torch_base_algo.TorchAlgo._save_predictions` function.
 
         Args:
             predict_dataset (torch.utils.data.Dataset): predict_dataset build from the x returned by the opener.
 
         Important:
@@ -240,15 +240,15 @@
             device = torch.device("cuda")
         return device
 
     def _update_from_checkpoint(self, path: Path) -> dict:
         """Load the checkpoint and update the internal state
         from it.
         Pop the values from the checkpoint so that we can ensure that it is empty at the
-        end, ie all the values have been used.
+        end, i.e. all the values have been used.
 
         Args:
             path (pathlib.Path): path where the checkpoint is saved
 
         Returns:
             dict: checkpoint
```

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,24 +245,24 @@
             loss += l2_reg
 
             current_batch_size = len(x_batch)
 
             self._update_gradients_and_hessian(loss, current_batch_size)
 
     def _local_predict(self, predict_dataset: torch.utils.data.Dataset, predictions_path):
-        """Executes the following operations:
+        """Execute the following operations:
 
             * Create the torch dataloader using the batch size given at the ``__init__`` of the class
-            * Sets the model to `eval` mode
-            * Returns the predictions
+            * Set the model to `eval` mode
+            * Return the predictions
 
         Args:
             predict_dataset (torch.utils.data.Dataset): predict_dataset build from the x returned by the opener.
         """
-        dataloader_batchsize = self._batch_size or len(predict_dataset)
+        dataloader_batchsize = min(self._batch_size, len(predict_dataset)) if self._batch_size else len(predict_dataset)
         predict_loader = torch.utils.data.DataLoader(predict_dataset, batch_size=dataloader_batchsize)
 
         self._model.eval()
 
         predictions = torch.Tensor([])
         with torch.inference_mode():
             for x in predict_loader:
```

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.36.0rc1/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
     return parameters
 
 
 def increment_parameters(
     model: torch.nn.Module,
     updates: List[torch.nn.parameter.Parameter],
+    *,
     with_batch_norm_parameters: bool,
     updates_multiplier: float = 1.0,
 ):
     """Add the given update to the model parameters. If with_batch_norm_parameters is set to True, the operation
     will include the running mean and the running variance of the batch norm layers (in this case, they must be
     included in the given update). This function modifies the given model internally and therefore returns nothing.
```

### Comparing `substrafl-0.35.1rc1/substrafl/dependency.py` & `substrafl-0.36.0rc1/substrafl/dependency.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/evaluation_strategy.py` & `substrafl-0.36.0rc1/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/exceptions.py` & `substrafl-0.36.0rc1/substrafl/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
 
 class EmptySharedStatesError(Exception):
     """The shared_states is empty. Ensure that the train method of the algorithm returns a
     StrategySharedState object."""
 
 
+class ExistingRegisteredMetricError(Exception):
+    """A metric with the same name is already registered."""
+
+
 class IncompatibleAlgoStrategyError(Exception):
     """This algo is not compatible with this strategy."""
 
 
 class IndexGeneratorSampleNoneError(Exception):
     """Try to use the index generator without setting the number of samples."""
 
@@ -39,14 +43,18 @@
     """The index generator has not been updated properly."""
 
 
 class InvalidPathError(Exception):
     """Invalid path."""
 
 
+class InvalidMetricIdentifierError(Exception):
+    """A metric name or identifier cannot be a SubstraFL Outputidentifier."""
+
+
 class KeyMetadataError(Exception):
     """``substrafl_version``, ``substra_version`` and ``substratools_version`` keys can't be added
     to the experiment metadata."""
 
 
 class LenMetadataError(Exception):
     """Too long additional metadata passed to the execute_experiment function to be shown on the Substra WebApp."""
```

### Comparing `substrafl-0.35.1rc1/substrafl/experiment.py` & `substrafl-0.36.0rc1/substrafl/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,75 +31,82 @@
 def _register_operations(
     client: substra.Client,
     train_data_nodes: List[TrainDataNode],
     aggregation_node: Optional[AggregationNode],
     evaluation_strategy: Optional[EvaluationStrategy],
     dependencies: Dependency,
 ) -> Tuple[List[dict], Dict[RemoteStruct, OperationKey]]:
-    """Register the operations in Substra: define the algorithms we need and submit them
+    """Register the operations in Substra: define the functions we need and submit them
 
     Args:
         client (substra.Client): substra client
         train_data_nodes (typing.List[TrainDataNode]): list of train data nodes
         aggregation_node (typing.Optional[AggregationNode]): the aggregation node for
             centralized strategies
         evaluation_strategy (typing.Optional[EvaluationStrategy]): the evaluation strategy
             if there is one dependencies
-        (Dependency): dependencies of the train algo
+        (Dependency): dependencies of the experiment
 
     Returns:
         typing.Tuple[typing.List[dict], typing.Dict[RemoteStruct, OperationKey]]:
         tasks, operation_cache
     """
     # `register_operations` methods from the different organizations store the id of the already registered
-    # algorithm so we don't add them twice
+    # functions so we don't add them twice
     operation_cache = dict()
-    predict_algo_cache = dict()
+    predict_function_cache = dict()
+    test_function_cache = dict()
     tasks = list()
 
     train_data_organizations_id = {train_data_node.organization_id for train_data_node in train_data_nodes}
     aggregation_organization_id = {aggregation_node.organization_id} if aggregation_node is not None else set()
     test_data_organizations_ids = (
         evaluation_strategy.test_data_nodes_org_ids if evaluation_strategy is not None else set()
     )
 
     authorized_ids = list(train_data_organizations_id | aggregation_organization_id | test_data_organizations_ids)
     permissions = substra.sdk.schemas.Permissions(public=False, authorized_ids=authorized_ids)
 
     for train_data_node in train_data_nodes:
         operation_cache = train_data_node.register_operations(
-            client,
-            permissions,
+            client=client,
+            permissions=permissions,
             cache=operation_cache,
             dependencies=dependencies,
         )
 
         if train_data_node.init_task is not None:
             tasks += [train_data_node.init_task]
 
         tasks += train_data_node.tasks
 
     if evaluation_strategy is not None:
         for test_data_node in evaluation_strategy.test_data_nodes:
-            predict_algo_cache = test_data_node.register_predict_operations(
-                client,
-                permissions,
-                cache=predict_algo_cache,
+            predict_function_cache = test_data_node.register_predict_operations(
+                client=client,
+                permissions=permissions,
+                cache=predict_function_cache,
+                dependencies=dependencies,
+            )
+            test_function_cache = test_data_node.register_test_operations(
+                client=client,
+                permissions=permissions,
+                cache=test_function_cache,
                 dependencies=dependencies,
             )
 
             tasks += test_data_node.predicttasks
             tasks += test_data_node.testtasks
 
     # The aggregation operation is defined in the strategy, its dependencies are
     # the strategy dependencies
     if aggregation_node is not None:
         operation_cache = aggregation_node.register_operations(
-            client,
-            permissions,
+            client=client,
+            permissions=permissions,
             cache=operation_cache,
             dependencies=dependencies,
         )
 
         tasks += aggregation_node.tasks
 
     return tasks, operation_cache
@@ -204,58 +211,59 @@
         "substra_version": substra.__version__,
         "substratools_version": substratools.__version__,
         "python_version": python_version(),
     }
 
 
 def execute_experiment(
+    *,
     client: substra.Client,
     strategy: Strategy,
     train_data_nodes: List[TrainDataNode],
     num_rounds: int,
     experiment_folder: Union[str, Path],
     aggregation_node: Optional[AggregationNode] = None,
     evaluation_strategy: Optional[EvaluationStrategy] = None,
     dependencies: Optional[Dependency] = None,
     clean_models: bool = True,
     name: Optional[str] = None,
     additional_metadata: Optional[Dict] = None,
     task_submission_batch_size: int = 500,
 ) -> substra.sdk.models.ComputePlan:
     """Run a complete experiment. This will train (on the `train_data_nodes`) and test (on the
-    `test_data_nodes`) your `algo` with the specified `strategy` `n_rounds` times and return the
+    `test_data_nodes`) the specified `strategy` `n_rounds` times and return the
     compute plan object from the Substra platform.
 
-    In substrafl, operations are linked to each other statically before being submitted to substra.
+    In SubstraFL, operations are linked to each other statically before being submitted to Substra.
 
     The execution of:
 
         - the `self.perform_round` method from the passed strategy **num_rounds** times
         - the `self.predict` methods from the passed strategy
 
     generate the static graph of operations.
 
-    Each element necessary for those operations (Tasks and Algorithms)
+    Each element necessary for those operations (Tasks and Functions)
     is registered to the Substra platform thanks to the specified client.
 
     Finally, the compute plan is sent and executed.
 
     The experiment summary is saved in `experiment_folder`, with the name format `{timestamp}_{compute_plan.key}.json`
 
     Args:
         client (substra.Client): A substra client to interact with the Substra platform
-        strategy (Strategy): The strategy by which your algorithm will be executed
+        strategy (Strategy): The strategy that will be executed
         train_data_nodes (typing.List[TrainDataNode]): List of the nodes where training on data
             occurs evaluation_strategy (EvaluationStrategy, Optional): If None performance will not be measured at all.
             Otherwise measuring of performance will follow the EvaluationStrategy. Defaults to None.
         aggregation_node (typing.Optional[AggregationNode]): For centralized strategy, the aggregation
             node, where all the shared tasks occurs else None.
         num_rounds (int): The number of time your strategy will be executed
-        dependencies (Dependency, Optional): Dependencies of the algorithm. It must be defined from
-            the substrafl Dependency class. Defaults None.
+        dependencies (Dependency, Optional): Dependencies of the experiment. It must be defined from
+            the SubstraFL Dependency class. Defaults None.
         experiment_folder (typing.Union[str, pathlib.Path]): path to the folder where the experiment summary is saved.
         clean_models (bool): Clean the intermediary models on the Substra platform. Set it to False
             if you want to download or re-use intermediary models. This causes the disk space to fill
             quickly so should be set to True unless needed. Defaults to True.
         name (str, Optional): Optional name chosen by the user to identify the compute plan. If None,
             the compute plan name is set to the timestamp.
         additional_metadata(dict, typing.Optional): Optional dictionary of metadata to be passed to the Substra WebApp.
@@ -273,15 +281,15 @@
     aggregation_node = copy.deepcopy(aggregation_node)
     strategy = copy.deepcopy(strategy)
     evaluation_strategy = copy.deepcopy(evaluation_strategy)
 
     train_organization_ids = [train_data_node.organization_id for train_data_node in train_data_nodes]
 
     if len(train_organization_ids) != len(set(train_organization_ids)):
-        raise ValueError("Training multiple algorithms on the same organization is not supported right now.")
+        raise ValueError("Training multiple functions on the same organization is not supported right now.")
 
     if evaluation_strategy is not None:
         _check_evaluation_strategy(evaluation_strategy, num_rounds)
         # Reset the evaluation strategy
         evaluation_strategy.restart_rounds()
 
     cp_metadata = dict()
@@ -302,15 +310,15 @@
         aggregation_node=aggregation_node,
         evaluation_strategy=evaluation_strategy,
         num_rounds=num_rounds,
         clean_models=clean_models,
     )
 
     # Computation graph is created
-    logger.info("Registering the algorithm to Substra.")
+    logger.info("Registering the functions to Substra.")
     tasks, operation_cache = _register_operations(
         client=client,
         train_data_nodes=train_data_nodes,
         aggregation_node=aggregation_node,
         evaluation_strategy=evaluation_strategy,
         dependencies=dependencies,
     )
```

### Comparing `substrafl-0.35.1rc1/substrafl/index_generator/base.py` & `substrafl-0.36.0rc1/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/index_generator/np_index_generator.py` & `substrafl-0.36.0rc1/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/logger.py` & `substrafl-0.36.0rc1/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/model_loading.py` & `substrafl-0.36.0rc1/substrafl/model_loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,28 +121,28 @@
         raise LoadAlgoFileNotFoundError(
             ", ".join(missing) + f" not found within the provided input folder `{folder}`.\n" + end_of_msg
         )
 
     return metadata
 
 
-def _get_composite_from_round(client: substra.Client, compute_plan_key: str, round_idx: int) -> substra.models.Task:
-    """Return the composite train task:
+def _get_train_task_from_round(client: substra.Client, compute_plan_key: str, round_idx: int) -> substra.models.Task:
+    """Return the train task:
 
         - hosted on the given client organization
         - belonging to the given compute plan
         - of the given round_idx
 
     Args:
-        client (substra.Client): Substra client where to fetch the composite train task from.
-        compute_plan_key (str): Compute plan key to fetch the composite from.
-        round_idx (int): Round of the strategy to fetch the composite from.
+        client (substra.Client): Substra client where to fetch the train task from.
+        compute_plan_key (str): Compute plan key to fetch the train task from.
+        round_idx (int): Round of the strategy to fetch the train task from.
 
     Returns:
-        substra.models.Task: The composite matching the given requirements.
+        substra.models.Task: The train task matching the given requirements.
     """
     org_id = client.organization_info().organization_id
 
     filters = {
         "compute_plan_key": [compute_plan_key],
         "worker": [org_id],
         "metadata": [{"key": "round_idx", "type": "is", "value": str(round_idx)}],
@@ -169,15 +169,15 @@
 
     return local_train_task
 
 
 def _load_algo(algo_path: Path, extraction_folder: Path) -> Any:
     """Load into memory a serialized (and compressed (.tar.gz)) substrafl algo within the given algo_path.
     This kind of file is usually the result of the ``substra.Client.download_function`` function applied to
-    a composite train task being part of a Substrafl experiment.
+    a train task being part of a Substrafl experiment.
 
     Args:
         algo_path (Path): A file being the tar.gz compression of a substrafl RemoteStruct algorithm
         extraction_folder (Path): Where to unpack the folder.
 
     Returns:
         Any: The loaded substrafl object into memory.
@@ -192,14 +192,15 @@
 
     my_algo = remote_struct.get_instance()
 
     return my_algo
 
 
 def download_algo_files(
+    *,
     client: substra.Client,
     compute_plan_key: str,
     dest_folder: os.PathLike,
     round_idx: Optional[int] = None,
 ):
     """Download all the files needed to load the model:
 
@@ -212,58 +213,55 @@
     Those files are:
 
         - the function used for this task
         - the output local state of the task
         - a metadata.json
 
     Important:
-        This function supports only strategies with one composite traintask for a given organization and round.
+        This function supports only strategies with one train task for a given organization and round.
 
     Args:
         client (substra.Client): Substra client where to fetch the model from.
         compute_plan_key (str): Compute plan key to fetch the model from.
         dest_folder (os.PathLike): Folder where to download the files.
         round_idx (Optional[int], None): Round of the strategy to fetch the model from. If set to ``None``,
             the last round will be used. (Defaults to None).
 
     Raises:
         NotImplementedError: The given compute plan must have been submitted to Substra through the
             :func:`~substrafl.experiment.execute_experiment` function.
-        TrainTaskNotFoundError: If no composite matches the given requirements.
+        TrainTaskNotFoundError: If no train task matches the given requirements.
         MultipleTrainTaskError: The experiment to get the model from can't have multiple
             TrainDataNodes hosted on the same organization. In practice this means the presence of multiple
-            composite train tasks with the same round number on the same rank.
+            train tasks with the same round number on the same rank.
         UnfinishedTrainTaskError: The task from which the files are trying to be downloaded is not done.
     """
     compute_plan = client.get_compute_plan(compute_plan_key)
 
     _check_environment_compatibility(metadata=compute_plan.metadata)
 
     folder = Path(dest_folder)
     folder.mkdir(exist_ok=True, parents=True)
 
     if round_idx is None:
         round_idx = compute_plan.metadata["num_rounds"]
 
-    # Get the composite associated to user inputs
-    composite_traintask = _get_composite_from_round(
-        client=client, compute_plan_key=compute_plan_key, round_idx=round_idx
-    )
+    # Get the train task associated to user inputs
+    train_task = _get_train_task_from_round(client=client, compute_plan_key=compute_plan_key, round_idx=round_idx)
 
-    if composite_traintask.status is not Status.done:
+    if train_task.status is not Status.done:
         raise UnfinishedTrainTaskError(
-            f"Can't download algo files form task {composite_traintask.key} as it is "
-            f"in status {composite_traintask.status}"
+            f"Can't download algo files form task {train_task.key} as it is " f"in status {train_task.status}"
         )
 
-    algo_file = client.download_function(composite_traintask.function.key, destination_folder=folder)
+    algo_file = client.download_function(train_task.function.key, destination_folder=folder)
 
     # Get the associated head model (local state)
     local_state_file = client.download_model_from_task(
-        composite_traintask.key, folder=folder, identifier=OutputIdentifiers.local
+        train_task.key, folder=folder, identifier=OutputIdentifiers.local
     )
 
     # Environment requirements and local state path
     metadata = {k: v for k, v in compute_plan.metadata.items() if k in REQUIRED_KEYS}
     metadata[LOCAL_STATE_DICT_KEY] = str(local_state_file.relative_to(folder))
     metadata[ALGO_DICT_KEY] = str(algo_file.relative_to(folder))
     metadata_path = folder / METADATA_FILE
```

### Comparing `substrafl-0.35.1rc1/substrafl/nodes/__init__.py` & `substrafl-0.36.0rc1/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/nodes/aggregation_node.py` & `substrafl-0.36.0rc1/substrafl/nodes/aggregation_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     data operations.
     The result is sent to the ``TrainDataNode`` and/or ``TestDataNode`` data operations.
     """
 
     def update_states(
         self,
         operation: RemoteOperation,
+        *,
         round_idx: int,
         authorized_ids: Set[str],
         clean_models: bool = False,
     ) -> SharedStateRef:
         """Adding an aggregated task to the list of operations to be executed by the node during the compute plan.
         This is done in a static way, nothing is submitted to substra.
         This is why the function key is a RemoteStruct (substrafl local reference of the algorithm)
@@ -96,14 +97,15 @@
 
         self.tasks.append(aggregate_task)
 
         return SharedStateRef(key=op_id)
 
     def register_operations(
         self,
+        *,
         client: substra.Client,
         permissions: substra.sdk.schemas.Permissions,
         cache: Dict[RemoteStruct, OperationKey],
         dependencies: Dependency,
     ) -> Dict[RemoteStruct, OperationKey]:
         """Define the functions for each operation and submit the aggregated task to substra.
```

### Comparing `substrafl-0.35.1rc1/substrafl/nodes/node.py` & `substrafl-0.36.0rc1/substrafl/nodes/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 
 class InputIdentifiers(str, Enum):
     local = "local"
     shared = "shared"
     model = "model"
     models = "models"
     predictions = "predictions"
-    performance = "performance"
     opener = "opener"
     datasamples = "datasamples"
     rank = "rank"
     X = "X"
     y = "y"
 
 
 class OutputIdentifiers(str, Enum):
     local = "local"
     shared = "shared"
     model = "model"
     predictions = "predictions"
-    performance = "performance"
 
 
 class Node:
     def __init__(self, organization_id: str):
         self.organization_id = organization_id
         self.tasks: List[Dict] = []
```

### Comparing `substrafl-0.35.1rc1/substrafl/nodes/train_data_node.py` & `substrafl-0.36.0rc1/substrafl/nodes/train_data_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
         self.init_task = None
 
         super().__init__(organization_id)
 
     def init_states(
         self,
+        *,
         operation: RemoteOperation,
         round_idx: int,
         authorized_ids: Set[str],
         clean_models: bool = False,
     ) -> LocalStateRef:
         op_id = str(uuid.uuid4())
 
@@ -76,21 +77,22 @@
         self.init_task = init_task
 
         return LocalStateRef(key=op_id, init=True)
 
     def update_states(
         self,
         operation: RemoteDataOperation,
+        *,
         round_idx: int,
         authorized_ids: Set[str],
         aggregation_id: Optional[str] = None,
         clean_models: bool = False,
         local_state: Optional[LocalStateRef] = None,
     ) -> Tuple[LocalStateRef, SharedStateRef]:
-        """Adding a composite train task to the list of operations to
+        """Adding a train task to the list of operations to
         be executed by the node during the compute plan. This is done in a static
         way, nothing is submitted to substra.
         This is why the function key is a RemoteStruct (substrafl local reference of the algorithm)
         and not a substra function_key as nothing has been submitted yet.
 
         Args:
             operation (RemoteDataOperation): Automatically generated structure returned by
@@ -153,15 +155,15 @@
                     parent_task_output_identifier=OutputIdentifiers.shared,
                 )
             ]
 
         else:
             shared_inputs = []
 
-        composite_traintask = substra.schemas.ComputePlanTaskSpec(
+        train_task = substra.schemas.ComputePlanTaskSpec(
             function_key=str(uuid.uuid4()),  # bogus function key
             task_id=op_id,
             inputs=data_inputs + local_inputs + shared_inputs,
             outputs={
                 OutputIdentifiers.shared: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(
                         public=False,
@@ -177,29 +179,30 @@
             metadata={
                 "round_idx": round_idx,
             },
             tag="train",
             worker=self.organization_id,
         ).dict()
 
-        composite_traintask.pop("function_key")
-        composite_traintask["remote_operation"] = operation.remote_struct
+        train_task.pop("function_key")
+        train_task["remote_operation"] = operation.remote_struct
 
-        self.tasks.append(composite_traintask)
+        self.tasks.append(train_task)
 
         return LocalStateRef(op_id), SharedStateRef(op_id)
 
     def register_operations(
         self,
+        *,
         client: substra.Client,
         permissions: substra.sdk.schemas.Permissions,
         cache: Dict[RemoteStruct, OperationKey],
         dependencies: Dependency,
     ) -> Dict[RemoteStruct, OperationKey]:
-        """Define the functions for each operation and submit the composite traintask to substra.
+        """Define the functions for each operation and submit the train task to substra.
 
         Go through every operation in the computation graph, check what function they use (identified by their
         RemoteStruct id), submit it to substra and save `RemoteStruct : function_key` into the `cache`
         (where function_key is the returned function key by substra.)
         If two tasks depend on the same function, the function won't be added twice to substra as this method check
         if a function has already been submitted to substra before adding it.
```

### Comparing `substrafl-0.35.1rc1/substrafl/remote/decorators.py` & `substrafl-0.36.0rc1/substrafl/remote/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     """
 
     @wraps(method)
     def remote_method_inner(
         self,
         data_samples: Optional[List[str]] = None,
         shared_state: Any = None,
+        *,
         _skip: bool = False,
         _algo_name: Optional[str] = None,
         **method_parameters,
     ) -> RemoteDataOperation:
         """
         Args:
             data_samples (List[str]): The data samples paths. Defaults to None.
@@ -113,14 +114,15 @@
         method (Callable): Method to wrap so that it is executed on the remote server
     """
 
     @wraps(method)
     def remote_method_inner(
         self,
         shared_states: Optional[List] = None,
+        *,
         _skip: bool = False,
         _algo_name: Optional[str] = None,
         **method_parameters,
     ) -> RemoteOperation:
         if _skip:
             return method(self=self, shared_states=shared_states, **method_parameters)
```

### Comparing `substrafl-0.35.1rc1/substrafl/remote/operations.py` & `substrafl-0.36.0rc1/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/remote/register/generate_wheel.py` & `substrafl-0.36.0rc1/substrafl/remote/register/generate_wheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List
 
 logger = logging.getLogger(__name__)
 
 LOCAL_WHEELS_FOLDER = Path.home() / ".substrafl"
 
 
-def local_lib_wheels(lib_modules: List, operation_dir: Path, python_major_minor: str, dest_dir: str) -> str:
+def local_lib_wheels(lib_modules: List, *, operation_dir: Path, python_major_minor: str, dest_dir: str) -> str:
     """Prepares the private modules from lib_modules list to be installed in a Docker image and generates the
     appropriated install command for a dockerfile. It first creates the wheel for each library. Each of the
     libraries must be already installed in the correct version locally. Use command:
     ``pip install -e library-name`` in the directory of each library.
 
     This allows one user to use custom version of the passed modules.
 
@@ -87,15 +87,15 @@
             + f"RUN python{python_major_minor} -m pip install {force_reinstall}{wheel_name}\n"
         )
         install_cmds.append(install_cmd)
 
     return "\n".join(install_cmds)
 
 
-def pypi_lib_wheels(lib_modules: List, operation_dir: Path, python_major_minor: str, dest_dir: str) -> str:
+def pypi_lib_wheels(lib_modules: List, *, operation_dir: Path, python_major_minor: str, dest_dir: str) -> str:
     """Retrieves lib_modules' wheels to be installed in a Docker image and generates
     the appropriated install command for a dockerfile.
 
     Args:
         lib_modules (list): list of modules to be installed.
         operation_dir (pathlib.Path): PosixPath to the operation directory
         python_major_minor (str): version which is to be used in the dockerfile. Eg: '3.8'
```

### Comparing `substrafl-0.35.1rc1/substrafl/remote/register/register.py` & `substrafl-0.36.0rc1/substrafl/remote/register/register.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Create the Substra function assets and register them to the platform.
 """
-import inspect
 import logging
 import os
 import shutil
 import tarfile
 import tempfile
 import typing
 import warnings
@@ -17,15 +16,14 @@
 import substratools
 from packaging import version
 
 import substrafl
 from substrafl import exceptions
 from substrafl.dependency import Dependency
 from substrafl.nodes.node import InputIdentifiers
-from substrafl.nodes.node import OutputIdentifiers
 from substrafl.remote.register.generate_wheel import local_lib_wheels
 from substrafl.remote.register.generate_wheel import pypi_lib_wheels
 from substrafl.remote.remote_struct import RemoteStruct
 from substrafl.remote.substratools_methods import RemoteMethod
 
 logger = logging.getLogger(__name__)
 
@@ -277,14 +275,15 @@
     archive_path = operation_dir / "function.tar.gz"
     _create_archive(archive_path=archive_path, src_path=operation_dir)
 
     return archive_path, description_path
 
 
 def register_function(
+    *,
     client: substra.Client,
     remote_struct: RemoteStruct,
     permissions: substra.sdk.schemas.Permissions,
     inputs: typing.List[substra.sdk.schemas.FunctionInputSpec],
     outputs: typing.List[substra.sdk.schemas.FunctionOutputSpec],
     dependencies: Dependency,
 ) -> str:
@@ -318,80 +317,37 @@
                 permissions=permissions,
                 metadata=dict(),
             )
         )
         return key
 
 
-def _check_metric_function(metric_function: typing.Callable):
-    """Function to check the type and the signature of a given metric function.
-
-    Args:
-        metric_function (typing.Callable): function to check.
-
-    Raises:
-        exceptions.MetricFunctionTypeError: metric_function must be of type "function"
-        exceptions.MetricFunctionSignatureError: metric_function must ONLY contains
-            datasamples and predictions_path as parameters
-    """
-
-    if not inspect.isfunction(metric_function):
-        raise exceptions.MetricFunctionTypeError("The metric_function() must be of type function.")
-
-    signature = inspect.signature(metric_function)
-    parameters = signature.parameters
-
-    if "datasamples" not in parameters:
-        raise exceptions.MetricFunctionSignatureError(
-            "The metric_function() function must contain datasamples as parameter."
-        )
-    elif "predictions_path" not in parameters:
-        raise exceptions.MetricFunctionSignatureError(
-            "The metric_function() function must contain predictions_path as parameter."
-        )
-    elif len(parameters) != 2:
-        raise exceptions.MetricFunctionSignatureError(
-            """The metric_function() function must ONLY contains datasamples and predictions_path as
-            parameters."""
-        )
-
-
-def add_metric(
+def register_metrics(
+    *,
     client: substra.Client,
-    permissions: substra.sdk.schemas.Permissions,
     dependencies: Dependency,
-    metric_function: typing.Callable,
-    metric_name: typing.Optional[str] = None,
-) -> str:
-    """Adds a metric to the Substra platform using the given metric function as the
+    permissions: substra.sdk.schemas.Permissions,
+    metric_functions: typing.Dict[str, typing.Callable],
+):
+    """Adds a function to the Substra platform using the given metric functions as the
     function to register.
-    The metric function must be of type function, and its signature must ONLY contains
+    Each metric function must be of type function, and their signature must ONLY contains
     `datasamples` and `predictions_path` as parameters. An error is raised otherwise.
 
     Args:
         client (substra.Client): The substra client.
         permissions (substra.sdk.schemas.Permissions): Permissions for the metric function.
         dependencies (Dependency): Metric function dependencies.
-        metric_function (typing.Callable): function to compute the score from the datasamples and the predictions.
-            This function is registered in substra as a metric.
-        metric_name (str, Optional): Optional name chosen by the user to identify the metric. If None,
-            the metric name is set to the 'metric_{metric_function.__name__}'.
+        metric_functions (typing.Dict[str, typing.Callable]): functions to compute the score from the datasamples and
+            the predictions. These functions are registered in substra as one function.
 
     Returns:
-        str: The key of the function created from the metric function.
+        str: Substra function containing all the given metric functions.
     """
 
-    _check_metric_function(metric_function=metric_function)
-
-    class Metric:
-        def score(self, datasamples, predictions_path, _skip=True):
-            # The _skip argument is needed to match the default signature of methods executed
-            # on substratools_methods.py.
-            return metric_function(datasamples=datasamples, predictions_path=predictions_path)
-
     inputs_metrics = [
         substra.sdk.schemas.FunctionInputSpec(
             identifier=InputIdentifiers.datasamples,
             kind=substra.sdk.schemas.AssetKind.data_sample,
             optional=False,
             multiple=True,
         ),
@@ -407,28 +363,38 @@
             optional=False,
             multiple=False,
         ),
     ]
 
     outputs_metrics = [
         substra.sdk.schemas.FunctionOutputSpec(
-            identifier=OutputIdentifiers.performance,
+            identifier=metric_function_id,
             kind=substra.sdk.schemas.AssetKind.performance,
             multiple=False,
         )
+        for metric_function_id in metric_functions
     ]
 
+    class Metric:
+        def score(self, datasamples, predictions_path, _skip=True):
+            # The _skip argument is needed to match the default signature of methods executed
+            # on substratools_methods.py.
+            return {
+                metric_function_id: metric_function(datasamples=datasamples, predictions_path=predictions_path)
+                for metric_function_id, metric_function in metric_functions.items()
+            }
+
     remote_struct = RemoteStruct(
         cls=Metric,
         cls_args=[],
         cls_kwargs={},
         remote_cls=RemoteMethod,
         method_name="score",
         method_parameters={},
-        algo_name=metric_name or "metric_" + metric_function.__name__,
+        algo_name="Evaluating",
     )
 
     key = register_function(
         client=client,
         remote_struct=remote_struct,
         permissions=permissions,
         inputs=inputs_metrics,
```

### Comparing `substrafl-0.35.1rc1/substrafl/remote/remote_struct.py` & `substrafl-0.36.0rc1/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.36.0rc1/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.35.1rc1/substrafl/remote/substratools_methods.py` & `substrafl-0.36.0rc1/substrafl/remote/substratools_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,16 +84,19 @@
 
         if OutputIdentifiers.model in outputs:
             self.save_model(method_output, outputs[OutputIdentifiers.model])
 
         elif OutputIdentifiers.shared in outputs:
             self.save_model(method_output, outputs[OutputIdentifiers.shared])
 
-        elif OutputIdentifiers.performance in outputs:
-            tools.save_performance(method_output, outputs[OutputIdentifiers.performance])
+        else:
+            for output_id in outputs:
+                # The performances are the only identifier user defined.
+                if output_id not in list(OutputIdentifiers):
+                    tools.save_performance(method_output[output_id], outputs[output_id])
 
     def generic_function(
         self,
         inputs: TypedDict,
         outputs: TypedDict,  # outputs contains a dict where keys are identifiers and values are paths on disk
         task_properties: TypedDict,
     ) -> None:
```

### Comparing `substrafl-0.35.1rc1/substrafl/schemas.py` & `substrafl-0.36.0rc1/substrafl/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 import pydantic
 
 
 class StrategyName(str, Enum):
     FEDERATED_AVERAGING = "Federated Averaging"
+    FEDERATED_PCA = "Federated PCA"
     SCAFFOLD = "Scaffold"
     SINGLE_ORGANIZATION = "Single organization"
     NEWTON_RAPHSON = "Newton Raphson"
 
 
 class _Model(pydantic.BaseModel):
     """Base model configuration"""
@@ -33,14 +34,30 @@
     received by the aggregate function in the federated averaging strategy.
     """
 
     n_samples: int
     parameters_update: List[np.ndarray]
 
 
+class FedPCAAveragedState(_Model):
+    """Shared state sent by the aggregate_organization in the federated
+    PCA strategy."""
+
+    avg_parameters_update: List[np.ndarray]
+
+
+class FedPCASharedState(_Model):
+    """Shared state returned by the train method of the algorithm for each client,
+    received by the aggregate function in the federated PCA strategy.
+    """
+
+    n_samples: int
+    parameters_update: List[np.ndarray]
+
+
 class ScaffoldSharedState(_Model):
     """Shared state returned by the train method of the algorithm for each client
     (e.g. algorithms.pytorch.scaffold.train)
 
     Args:
         parameters_update (typing.List[numpy.ndarray]): the weight update of the client
             (delta between fine-tuned weights and previous weights)
```

### Comparing `substrafl-0.35.1rc1/substrafl/strategies/fed_avg.py` & `substrafl-0.36.0rc1/substrafl/strategies/fed_avg.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         Returns:
             StrategyName: Name of the strategy
         """
         return StrategyName.FEDERATED_AVERAGING
 
     def perform_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         aggregation_node: AggregationNode,
         round_idx: int,
         clean_models: bool,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """One round of the Federated Averaging strategy consists in:
@@ -105,15 +106,15 @@
                 round_idx=0,
                 aggregation_id=aggregation_node.organization_id,
                 additional_orgs_permissions=additional_orgs_permissions or set(),
                 clean_models=clean_models,
             )
 
         current_aggregation = aggregation_node.update_states(
-            self.avg_shared_states(shared_states=self._shared_states, _algo_name="Aggregating"),
+            operation=self.avg_shared_states(shared_states=self._shared_states, _algo_name="Aggregating"),
             round_idx=round_idx,
             authorized_ids=set([train_data_node.organization_id for train_data_node in train_data_nodes]),
             clean_models=clean_models,
         )
 
         self._perform_local_updates(
             train_data_nodes=train_data_nodes,
@@ -152,15 +153,15 @@
             assert self._local_states is not None, "Cannot predict if no training has been done beforehand."
             local_state = self._local_states[node_index]
 
             test_data_node.update_states(
                 traintask_id=local_state.key,
                 operation=self.algo.predict(
                     data_samples=test_data_node.test_data_sample_keys,
-                    _algo_name=f"Testing with {self.algo.__class__.__name__}",
+                    _algo_name=f"Predicting with {self.algo.__class__.__name__}",
                 ),
                 round_idx=round_idx,
             )  # Init state for testtask
 
     @remote
     def avg_shared_states(self, shared_states: List[FedAvgSharedState]) -> FedAvgAveragedState:
         """Compute the weighted average of all elements returned by the train
@@ -193,29 +194,24 @@
             without the passed key "n_samples".
         """
         if len(shared_states) == 0:
             raise EmptySharedStatesError(
                 "Your shared_states is empty. Please ensure that "
                 "the train method of your algorithm returns a FedAvgSharedState object."
             )
-
+        parameters_update_len = len(shared_states[0].parameters_update)
         assert all(
-            [
-                len(shared_state.parameters_update) == len(shared_states[0].parameters_update)
-                for shared_state in shared_states
-            ]
+            [len(shared_state.parameters_update) == parameters_update_len for shared_state in shared_states]
         ), "Not the same number of layers for every input parameters."
 
         n_all_samples = sum([state.n_samples for state in shared_states])
 
-        averaged_states = list()
-        for idx in range(len(shared_states[0].parameters_update)):
-            states = list()
-            for state in shared_states:
-                states.append(state.parameters_update[idx] * (state.n_samples / n_all_samples))
+        averaged_states = []
+        for idx in range(parameters_update_len):
+            states = [state.parameters_update[idx] * (state.n_samples / n_all_samples) for state in shared_states]
             averaged_states.append(np.sum(states, axis=0))
 
         return FedAvgAveragedState(avg_parameters_update=averaged_states)
 
     def _perform_local_updates(
         self,
         train_data_nodes: List[TrainDataNode],
@@ -241,18 +237,18 @@
                 space to fill quickly so should be set to True unless needed.
         """
 
         next_local_states = []
         next_shared_states = []
 
         for i, node in enumerate(train_data_nodes):
-            # define composite tasks (do not submit yet)
-            # for each composite task give description of Algo instead of a key for an algo
+            # define train tasks (do not submit yet)
+            # for each train task give description of Algo instead of a key for an algo
             next_local_state, next_shared_state = node.update_states(
-                self.algo.train(
+                operation=self.algo.train(
                     node.data_sample_keys,
                     shared_state=current_aggregation,
                     _algo_name=f"Training with {self.algo.__class__.__name__}",
                 ),
                 local_state=self._local_states[i] if self._local_states is not None else None,
                 round_idx=round_idx,
                 authorized_ids=set([node.organization_id]) | additional_orgs_permissions,
```

### Comparing `substrafl-0.35.1rc1/substrafl/strategies/newton_raphson.py` & `substrafl-0.36.0rc1/substrafl/strategies/newton_raphson.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         Returns:
             StrategyName: Name of the strategy
         """
         return StrategyName.NEWTON_RAPHSON
 
     def perform_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         aggregation_node: AggregationNode,
         round_idx: int,
         clean_models: bool,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """One round of the Newton-Raphson strategy consists in:
@@ -110,15 +111,15 @@
                 round_idx=0,
                 aggregation_id=aggregation_node.organization_id,
                 additional_orgs_permissions=additional_orgs_permissions or set(),
                 clean_models=clean_models,
             )
 
         current_aggregation = aggregation_node.update_states(
-            self.compute_averaged_states(
+            operation=self.compute_averaged_states(
                 shared_states=self._shared_states,
                 _algo_name="Aggregating",
             ),
             round_idx=round_idx,
             authorized_ids=set([train_data_node.organization_id for train_data_node in train_data_nodes]),
             clean_models=clean_models,
         )
@@ -253,18 +254,18 @@
                 space to fill quickly so should be set to True unless needed.
         """
 
         next_local_states = []
         next_shared_states = []
 
         for i, node in enumerate(train_data_nodes):
-            # define composite tasks (do not submit yet)
-            # for each composite task give description of Algo instead of a key for an algo
+            # define train tasks (do not submit yet)
+            # for each train task give description of Algo instead of a key for an algo
             next_local_state, next_shared_state = node.update_states(
-                self.algo.train(
+                operation=self.algo.train(
                     node.data_sample_keys,
                     shared_state=current_aggregation,
                     _algo_name=f"Training with {self.algo.__class__.__name__}",
                 ),
                 local_state=self._local_states[i] if self._local_states is not None else None,
                 round_idx=round_idx,
                 authorized_ids=set([node.organization_id]) | additional_orgs_permissions,
@@ -306,15 +307,15 @@
 
             assert self._local_states is not None, "Cannot predict if no training has been done beforehand."
             local_state = self._local_states[node_index]
 
             test_data_node.update_states(
                 operation=self.algo.predict(
                     data_samples=test_data_node.test_data_sample_keys,
-                    _algo_name=f"Testing with {self.algo.__class__.__name__}",
+                    _algo_name=f"Predicting with {self.algo.__class__.__name__}",
                 ),
                 traintask_id=local_state.key,
                 round_idx=round_idx,
             )  # Init state for testtask
 
     def _check_shared_states(self, shared_states: List[NewtonRaphsonSharedState]):
         """Check the Newton Raphson assumptions.
```

### Comparing `substrafl-0.35.1rc1/substrafl/strategies/scaffold.py` & `substrafl-0.36.0rc1/substrafl/strategies/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         Returns:
             StrategyName: Name of the strategy
         """
         return StrategyName.SCAFFOLD
 
     def perform_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         aggregation_node: AggregationNode,
         round_idx: int,
         clean_models: bool,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """One round of the Scaffold strategy consists in:
@@ -96,15 +97,15 @@
                 round_idx=0,
                 aggregation_id=aggregation_node.organization_id,
                 additional_orgs_permissions=additional_orgs_permissions or set(),
                 clean_models=clean_models,
             )
 
         current_aggregation = aggregation_node.update_states(
-            self.avg_shared_states(shared_states=self._shared_states, _algo_name="Aggregating"),
+            operation=self.avg_shared_states(shared_states=self._shared_states, _algo_name="Aggregating"),
             round_idx=round_idx,
             authorized_ids=set([train_data_node.organization_id for train_data_node in train_data_nodes]),
             clean_models=clean_models,
         )
 
         self._perform_local_updates(
             train_data_nodes=train_data_nodes,
@@ -142,15 +143,15 @@
 
             assert self._local_states is not None, "Cannot predict if no training has been done beforehand."
             local_state = self._local_states[node_index]
 
             test_data_node.update_states(
                 operation=self.algo.predict(
                     data_samples=test_data_node.test_data_sample_keys,
-                    _algo_name=f"Testing with {self.algo.__class__.__name__}",
+                    _algo_name=f"Predicting with {self.algo.__class__.__name__}",
                 ),
                 traintask_id=local_state.key,
                 round_idx=round_idx,
             )  # Init state for testtask
 
     def _check_shared_states(self, shared_states: List[ScaffoldSharedState]):
         """Check the Scaffold assumptions: server_control_variate, parameters_update and server_control_variate have the
@@ -348,18 +349,18 @@
                 space to fill quickly so should be set to True unless needed.
         """
 
         next_local_states = []
         next_shared_states = []
 
         for i, node in enumerate(train_data_nodes):
-            # define composite tasks (do not submit yet)
-            # for each composite task give description of Algo instead of a key for an algo
+            # define train tasks (do not submit yet)
+            # for each train task give description of Algo instead of a key for an algo
             next_local_state, next_shared_state = node.update_states(
-                self.algo.train(
+                operation=self.algo.train(
                     node.data_sample_keys,
                     shared_state=current_aggregation,
                     _algo_name=f"Training with {self.algo.__class__.__name__}",
                 ),
                 local_state=self._local_states[i] if self._local_states is not None else None,
                 round_idx=round_idx,
                 authorized_ids=set([node.organization_id]) | additional_orgs_permissions,
```

### Comparing `substrafl-0.35.1rc1/substrafl/strategies/single_organization.py` & `substrafl-0.36.0rc1/substrafl/strategies/single_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         Returns:
             StrategyName: Name of the strategy
         """
         return StrategyName.SINGLE_ORGANIZATION
 
     def initialization_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         clean_models: bool,
         round_idx: Optional[int] = 0,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """Call the initialize function of the algo on each train node.
 
@@ -64,26 +65,27 @@
         if n_train_data_nodes != 1:
             raise ValueError(
                 "One organization strategy can only be used with one train_data_node"
                 f" but {n_train_data_nodes} were passed."
             )
 
         next_local_state = train_data_nodes[0].init_states(
-            self.algo.initialize(
+            operation=self.algo.initialize(
                 _algo_name=f"Initializing with {self.algo.__class__.__name__}",
             ),
             round_idx=round_idx,
             authorized_ids=set([train_data_nodes[0].organization_id]) | additional_orgs_permissions,
             clean_models=clean_models,
         )
 
         self.local_state = next_local_state
 
     def perform_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         round_idx: int,
         clean_models: bool,
         aggregation_node: Optional[AggregationNode] = None,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """One round of the SingleOrganization strategy: perform a local update (train on n mini-batches) of the models
@@ -107,18 +109,18 @@
         n_train_data_nodes = len(train_data_nodes)
         if n_train_data_nodes != 1:
             raise ValueError(
                 "One organization strategy can only be used with one train_data_node"
                 f" but {n_train_data_nodes} were passed."
             )
 
-        # define composite tasks (do not submit yet)
-        # for each composite task give description of Algo instead of a key for an algo
+        # define train tasks (do not submit yet)
+        # for each train task give description of Algo instead of a key for an algo
         next_local_state, _ = train_data_nodes[0].update_states(
-            self.algo.train(
+            operation=self.algo.train(
                 train_data_nodes[0].data_sample_keys,
                 shared_state=None,
                 _algo_name=f"Training with {self.algo.__class__.__name__}",
             ),
             local_state=self.local_state,
             round_idx=round_idx,
             authorized_ids=set([train_data_nodes[0].organization_id]) | additional_orgs_permissions or set(),
@@ -150,11 +152,11 @@
 
         for test_data_node in test_data_nodes:
             # Init state for testtask
             test_data_node.update_states(
                 traintask_id=self.local_state.key,
                 operation=self.algo.predict(
                     data_samples=test_data_node.test_data_sample_keys,
-                    _algo_name=f"Testing with {self.algo.__class__.__name__}",
+                    _algo_name=f"Predicting with {self.algo.__class__.__name__}",
                 ),
                 round_idx=round_idx,
             )  # Init state for testtask
```

### Comparing `substrafl-0.35.1rc1/substrafl/strategies/strategy.py` & `substrafl-0.36.0rc1/substrafl/strategies/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         Returns:
             StrategyName: Name of the strategy
         """
         raise NotImplementedError
 
     def initialization_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         clean_models: bool,
         round_idx: Optional[int] = 0,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """Call the initialize function of the algo on each train node.
 
@@ -79,30 +80,31 @@
             round_idx (typing.Optional[int]): index of the round. Defaults to 0.
             additional_orgs_permissions (typing.Optional[set]): Additional permissions to give to the model outputs
                 after training, in order to test the model on an other organization. Default to None
         """
         next_local_states = []
 
         for node in train_data_nodes:
-            # define composite tasks (do not submit yet)
-            # for each composite task give description of Algo instead of a key for an algo
+            # define train tasks (do not submit yet)
+            # for each train task give description of Algo instead of a key for an algo
             next_local_state = node.init_states(
-                self.algo.initialize(
+                operation=self.algo.initialize(
                     _algo_name=f"Initializing with {self.algo.__class__.__name__}",
                 ),
                 round_idx=round_idx,
                 authorized_ids=set([node.organization_id]) | additional_orgs_permissions,
                 clean_models=clean_models,
             )
             next_local_states.append(next_local_state)
         self._local_states = next_local_states
 
     @abstractmethod
     def perform_round(
         self,
+        *,
         train_data_nodes: List[TrainDataNode],
         aggregation_node: Optional[AggregationNode],
         round_idx: int,
         clean_models: bool,
         additional_orgs_permissions: Optional[set] = None,
     ):
         """Perform one round of the strategy
```

### Comparing `substrafl-0.35.1rc1/substrafl.egg-info/PKG-INFO` & `substrafl-0.36.0rc1/substrafl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.35.1rc1
+Version: 0.36.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.35.1rc1/substrafl.egg-info/SOURCES.txt` & `substrafl-0.36.0rc1/substrafl.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 substrafl.egg-info/requires.txt
 substrafl.egg-info/top_level.txt
 substrafl/algorithms/__init__.py
 substrafl/algorithms/algo.py
 substrafl/algorithms/pytorch/__init__.py
 substrafl/algorithms/pytorch/torch_base_algo.py
 substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+substrafl/algorithms/pytorch/torch_fed_pca_algo.py
 substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
 substrafl/algorithms/pytorch/torch_scaffold_algo.py
 substrafl/algorithms/pytorch/torch_single_organization_algo.py
 substrafl/algorithms/pytorch/weight_manager.py
 substrafl/index_generator/__init__.py
 substrafl/index_generator/base.py
 substrafl/index_generator/np_index_generator.py
@@ -45,11 +46,12 @@
 substrafl/remote/register/generate_wheel.py
 substrafl/remote/register/register.py
 substrafl/remote/serializers/__init__.py
 substrafl/remote/serializers/pickle_serializer.py
 substrafl/remote/serializers/serializer.py
 substrafl/strategies/__init__.py
 substrafl/strategies/fed_avg.py
+substrafl/strategies/fed_pca.py
 substrafl/strategies/newton_raphson.py
 substrafl/strategies/scaffold.py
 substrafl/strategies/single_organization.py
 substrafl/strategies/strategy.py
```


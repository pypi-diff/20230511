# Comparing `tmp/gurobi-machinelearning-1.2.0a1.tar.gz` & `tmp/gurobi-machinelearning-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.2.0a1.tar", last modified: Mon Apr 17 13:54:59 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.2.1.tar", last modified: Wed May 10 22:14:50 2023, max compression
```

## Comparing `gurobi-machinelearning-1.2.0a1.tar` & `gurobi-machinelearning-1.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.031154 gurobi-machinelearning-1.2.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 13:54:51.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/base_predictor_constr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.768843 gurobi-machinelearning-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-10 22:14:50.768843 gurobi-machinelearning-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 22:14:50.768843 gurobi-machinelearning-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.764843 gurobi-machinelearning-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.764843 gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-10 22:14:50.000000 gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-10 22:14:50.000000 gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:14:50.000000 gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 22:14:50.000000 gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 22:14:50.000000 gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.764843 gurobi-machinelearning-1.2.1/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-10 22:14:43.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.764843 gurobi-machinelearning-1.2.1/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.764843 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/base_predictor_constr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.768843 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.768843 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:14:50.768843 gurobi-machinelearning-1.2.1/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-10 22:14:41.000000 gurobi-machinelearning-1.2.1/src/gurobi_ml/torch/sequential.py
```

### Comparing `gurobi-machinelearning-1.2.0a1/LICENSE` & `gurobi-machinelearning-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/PKG-INFO` & `gurobi-machinelearning-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.2.0a1
+Version: 1.2.1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.2.0a1/README.md` & `gurobi-machinelearning-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/pyproject.toml` & `gurobi-machinelearning-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.2.0a1"
+version = "1.2.1"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.2.0a1
+Version: 1.2.1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.2.1/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "411376135a2001b5fcd3f57261b51ab673e94761"
+GIT_HASH = "627a44da6f89bbad46916a14c92c9c73741d914c"
 
 
 def get_versions():
     """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
```

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/add_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/keras/keras.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/_var_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/get_convertor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/layers.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/neural_net.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/modeling/submodel.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/register_user_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/registered_predictors.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 """Module for formulating a column transformer in a :gurobipy:`gurobipy model <Model>`."""
 
 import gurobipy as gp
 
+from ..exceptions import NoModel
 from .preprocessing import sklearn_transformers
 from .skgetter import SKtransformer
 
 
 class ColumnTransformerConstr(SKtransformer):
     """Class to model a fitted :external+sklearn:py:class:`sklearn.compose.ColumnTransformer` with gurobipy.
 
@@ -66,20 +67,22 @@
         for name, trans, cols in column_transform.transformers_:
             if trans == "passthrough":
                 transformed.append(_input.loc[:, cols])
             elif trans == "drop":
                 pass
             else:
                 data = _input.loc[:, cols]
-                anyvar = any(
+                any_var = any(
                     map(lambda i: isinstance(i, gp.Var), data.to_numpy().ravel())
                 )
-                if anyvar:
-                    if name in transformers:
+                if any_var:
+                    try:
                         trans_constr = transformers[name](self._gp_model, trans, data)
+                    except KeyError:
+                        raise NoModel(name, "No implementation found")
                     transformed.append(trans_constr.output.tolist())
                 else:
                     transformed.append(trans.transform(_input.loc[:, cols]))
         self._output = column_transform._hstack(transformed)
 
 
 def add_column_transformer_constr(gp_model, column_transformer, input_vars, **kwargs):
```

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/decision_tree_regressor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/sklearn/skgetter.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.2.1/src/gurobi_ml/torch/sequential.py`

 * *Files identical despite different names*


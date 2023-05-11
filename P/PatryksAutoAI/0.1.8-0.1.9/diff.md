# Comparing `tmp/PatryksAutoAI-0.1.8.tar.gz` & `tmp/PatryksAutoAI-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.1.8.tar", last modified: Thu May 11 13:46:37 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.1.9.tar", last modified: Thu May 11 13:51:00 2023, max compression
```

## Comparing `PatryksAutoAI-0.1.8.tar` & `PatryksAutoAI-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.717548 PatryksAutoAI-0.1.8/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.713548 PatryksAutoAI-0.1.8/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.713548 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.713548 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7947 2023-05-10 18:02:26.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6311 2023-05-10 18:02:28.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5276 2023-05-10 18:02:20.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5947 2023-05-10 18:02:52.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2243 2023-05-10 18:02:51.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7272 2023-05-10 18:02:49.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2339 2023-05-10 18:02:48.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4864 2023-05-10 18:02:47.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6342 2023-05-10 18:02:46.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2358 2023-05-10 18:08:42.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2293 2023-05-10 18:02:44.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5742 2023-05-10 18:02:41.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.713548 PatryksAutoAI-0.1.8/Machine_Learning_Classes/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.713548 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       83 2023-05-10 18:02:07.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.713548 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      225 2023-05-11 13:46:02.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6127 2023-05-11 13:46:03.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2592 2023-05-11 13:30:17.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6046 2023-05-11 13:30:24.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2519 2023-05-11 13:30:28.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5478 2023-05-11 13:30:34.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2809 2023-05-11 13:30:39.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2642 2023-05-11 13:30:43.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7242 2023-05-11 13:30:49.000000 PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 13:46:37.717548 PatryksAutoAI-0.1.8/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:46:37.717548 PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 13:46:37.000000 PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-11 13:46:37.000000 PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-11 13:46:37.000000 PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-11 13:46:37.000000 PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-11 13:46:37.000000 PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-11 13:46:37.717548 PatryksAutoAI-0.1.8/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-11 13:46:16.000000 PatryksAutoAI-0.1.8/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.480383 PatryksAutoAI-0.1.9/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.480383 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7947 2023-05-10 18:02:26.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6311 2023-05-10 18:02:28.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5276 2023-05-10 18:02:20.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5947 2023-05-10 18:02:52.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2243 2023-05-10 18:02:51.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7272 2023-05-10 18:02:49.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2339 2023-05-10 18:02:48.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4864 2023-05-10 18:02:47.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6342 2023-05-10 18:02:46.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2358 2023-05-10 18:08:42.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2293 2023-05-10 18:02:44.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5742 2023-05-10 18:02:41.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/Machine_Learning_Classes/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       83 2023-05-10 18:02:07.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      225 2023-05-11 13:46:02.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6116 2023-05-11 13:50:02.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2581 2023-05-11 13:50:07.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6035 2023-05-11 13:50:11.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2508 2023-05-11 13:50:14.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5467 2023-05-11 13:50:18.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2798 2023-05-11 13:50:21.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2631 2023-05-11 13:50:24.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7231 2023-05-11 13:50:32.000000 PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 13:51:00.000000 PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-11 13:51:00.000000 PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-11 13:51:00.000000 PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-11 13:51:00.000000 PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-11 13:51:00.000000 PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-11 13:51:00.484383 PatryksAutoAI-0.1.9/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-11 13:50:52.000000 PatryksAutoAI-0.1.9/setup.py
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/metrics.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/cat.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/extra_trees.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/hist_gradient.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/kneighbours.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/light_lgb.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/linear_svc.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/logistic_regression.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/random_forest.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/svc.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/classification/models/xgb.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/model_data/model_data.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/metrics_regression.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/cat.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import mean_squared_error,r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 from catboost import CatBoostRegressor
 import numpy as np
 import optuna
 
 
 class Cat(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/elastic_net.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/elastic_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 from sklearn.linear_model import ElasticNet
 import numpy as np
 
 class ElasticNetM(Metrics):
     def __init__(self):
         self.model = None
         self.parameters = None
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/gradient_boosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.metrics import mean_squared_error,r2_score
 from sklearn.ensemble import GradientBoostingRegressor
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 import numpy as np
 import optuna
 
 
 class GradientBoosting(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/lasso.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/lasso.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import mean_squared_error,r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 from sklearn.linear_model import Lasso
 import numpy as np
 
 class LassoM(Metrics):
     def __init__(self):
         self.model = None
         self.parameters = None
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/lgb.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/lgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import mean_squared_error,r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 import lightgbm as lgb
 import numpy as np
 import optuna
 
 class LGB(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/sgd.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/sgd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import mean_squared_error,r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 from sklearn.linear_model import SGDRegressor
 import numpy as np
 
 class SGD(Metrics):
     def __init__(self):
         self.model = None
         self.parameters = None
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/svr.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/svr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import mean_squared_error,r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 from sklearn.svm import SVR
 import numpy as np
 
 
 class SVRM(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.8/Machine_Learning_Classes/regression/models/xgb.py` & `PatryksAutoAI-0.1.9/Machine_Learning_Classes/regression/models/xgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from sklearn.metrics import mean_squared_error,r2_score
-from regression.metrics_regression import Metrics
+from metrics_regression import Metrics
 import xgboost as xgb
 import numpy as np
 import optuna
 
 class XGB(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.8/PKG-INFO` & `PatryksAutoAI-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.8
+Version: 0.1.9
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.8
+Version: 0.1.9
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.8/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.1.9/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.8/setup.py` & `PatryksAutoAI-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```


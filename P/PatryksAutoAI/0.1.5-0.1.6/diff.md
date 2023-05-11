# Comparing `tmp/PatryksAutoAI-0.1.5.tar.gz` & `tmp/PatryksAutoAI-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.1.5.tar", last modified: Wed May 10 18:09:12 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.1.6.tar", last modified: Wed May 10 18:19:11 2023, max compression
```

## Comparing `PatryksAutoAI-0.1.5.tar` & `PatryksAutoAI-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.040288 PatryksAutoAI-0.1.5/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.012288 PatryksAutoAI-0.1.5/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.016288 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.024288 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7947 2023-05-10 18:02:26.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6311 2023-05-10 18:02:28.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5276 2023-05-10 18:02:20.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5947 2023-05-10 18:02:52.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2243 2023-05-10 18:02:51.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7272 2023-05-10 18:02:49.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2339 2023-05-10 18:02:48.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4864 2023-05-10 18:02:47.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6342 2023-05-10 18:02:46.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2358 2023-05-10 18:08:42.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2293 2023-05-10 18:02:44.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5742 2023-05-10 18:02:41.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.028288 PatryksAutoAI-0.1.5/Machine_Learning_Classes/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.028288 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       83 2023-05-10 18:02:07.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.036288 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      175 2023-05-10 17:52:36.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5997 2023-05-10 18:02:14.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2755 2023-05-10 18:02:16.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6103 2023-05-10 18:02:37.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2663 2023-05-10 18:02:36.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5470 2023-05-10 18:02:35.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2953 2023-05-10 18:02:34.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2787 2023-05-10 18:02:33.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7232 2023-05-10 18:02:30.000000 PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 18:09:12.036288 PatryksAutoAI-0.1.5/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:09:12.036288 PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 18:09:11.000000 PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-10 18:09:11.000000 PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 18:09:11.000000 PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 18:09:11.000000 PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 18:09:11.000000 PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 18:09:12.040288 PatryksAutoAI-0.1.5/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 18:08:46.000000 PatryksAutoAI-0.1.5/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.805988 PatryksAutoAI-0.1.6/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.805988 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.813988 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7947 2023-05-10 18:02:26.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6311 2023-05-10 18:02:28.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5276 2023-05-10 18:02:20.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5947 2023-05-10 18:02:52.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2243 2023-05-10 18:02:51.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7272 2023-05-10 18:02:49.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2339 2023-05-10 18:02:48.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4864 2023-05-10 18:02:47.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6342 2023-05-10 18:02:46.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2358 2023-05-10 18:08:42.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2293 2023-05-10 18:02:44.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5742 2023-05-10 18:02:41.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/Machine_Learning_Classes/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       83 2023-05-10 18:02:07.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      175 2023-05-10 17:52:36.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5997 2023-05-10 18:17:56.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2755 2023-05-10 18:18:03.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6103 2023-05-10 18:18:13.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2663 2023-05-10 18:18:18.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5470 2023-05-10 18:18:25.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2953 2023-05-10 18:18:32.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2787 2023-05-10 18:18:39.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7232 2023-05-10 18:18:46.000000 PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 18:19:11.000000 PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-10 18:19:11.000000 PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 18:19:11.000000 PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 18:19:11.000000 PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 18:19:11.000000 PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 18:19:11.817988 PatryksAutoAI-0.1.6/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 18:18:51.000000 PatryksAutoAI-0.1.6/setup.py
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/metrics.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/cat.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/extra_trees.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/hist_gradient.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/kneighbours.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/light_lgb.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/linear_svc.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/logistic_regression.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/random_forest.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/svc.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/classification/models/xgb.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/model_data/model_data.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/metrics_regression.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/cat.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/cat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from catboost import CatBoostRegressor
 import numpy as np
 import optuna
 
 
 class Cat(Metrics):
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/elastic_net.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/elastic_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.linear_model import ElasticNet
 import numpy as np
 
 class ElasticNetM(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/gradient_boosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.metrics import mean_squared_error
 from sklearn.ensemble import GradientBoostingRegressor
-from sklearn.model_selection import GridSearchCV, train_test_split
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 import numpy as np
 import optuna
 
 
 class GradientBoosting(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/lasso.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/lasso.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.linear_model import Lasso
 import numpy as np
 
 class LassoM(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/lgb.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/lgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 import lightgbm as lgb
 import numpy as np
 import optuna
 
 class LGB(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/sgd.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/sgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.linear_model import SGDRegressor
 import numpy as np
 
 class SGD(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/svr.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/svr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.svm import SVR
 import numpy as np
 
 
 class SVRM(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.5/Machine_Learning_Classes/regression/models/xgb.py` & `PatryksAutoAI-0.1.6/Machine_Learning_Classes/regression/models/xgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sklearn.model_selection import GridSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error,KFold
+from sklearn.model_selection import GridSearchCV, train_test_split,KFold
+from sklearn.metrics import mean_squared_error
 from Machine_Learning_Classes.regression.metrics_regression import Metrics
 import xgboost as xgb
 import numpy as np
 import optuna
 
 class XGB(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.5/PKG-INFO` & `PatryksAutoAI-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.5
+Version: 0.1.6
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.5
+Version: 0.1.6
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.5/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.1.6/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.5/setup.py` & `PatryksAutoAI-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```


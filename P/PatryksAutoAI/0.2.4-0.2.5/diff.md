# Comparing `tmp/PatryksAutoAI-0.2.4.tar.gz` & `tmp/PatryksAutoAI-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.2.4.tar", last modified: Thu May 11 14:41:37 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.2.5.tar", last modified: Thu May 11 14:50:34 2023, max compression
```

## Comparing `PatryksAutoAI-0.2.4.tar` & `PatryksAutoAI-0.2.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.889041 PatryksAutoAI-0.2.4/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.889041 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7909 2023-05-11 13:58:25.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6273 2023-05-11 13:59:08.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5238 2023-05-11 13:59:11.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5909 2023-05-11 13:59:15.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7234 2023-05-11 13:59:20.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4826 2023-05-11 13:59:26.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6304 2023-05-11 13:59:30.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5702 2023-05-11 13:59:04.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/Machine_Learning_Classes/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-11 14:03:31.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-11 14:13:19.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6118 2023-05-11 13:59:46.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2583 2023-05-11 14:00:02.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6037 2023-05-11 13:57:48.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2510 2023-05-11 13:57:51.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5469 2023-05-11 13:57:54.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2800 2023-05-11 13:57:58.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 13:58:01.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7214 2023-05-11 14:41:11.000000 PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 14:41:37.000000 PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-11 14:41:37.000000 PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-11 14:41:37.000000 PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-11 14:41:37.000000 PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-11 14:41:37.000000 PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-11 14:41:37.893041 PatryksAutoAI-0.2.4/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-11 14:41:22.000000 PatryksAutoAI-0.2.4/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.969186 PatryksAutoAI-0.2.5/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.965186 PatryksAutoAI-0.2.5/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.965186 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.965186 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7909 2023-05-11 13:58:25.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6273 2023-05-11 13:59:08.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5238 2023-05-11 13:59:11.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5909 2023-05-11 13:59:15.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7234 2023-05-11 13:59:20.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4826 2023-05-11 13:59:26.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6304 2023-05-11 13:59:30.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5702 2023-05-11 13:59:04.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.965186 PatryksAutoAI-0.2.5/Machine_Learning_Classes/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.965186 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-11 14:03:31.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.969186 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-11 14:13:19.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6118 2023-05-11 13:59:46.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2583 2023-05-11 14:00:02.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6037 2023-05-11 13:57:48.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2510 2023-05-11 13:57:51.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5469 2023-05-11 13:57:54.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2800 2023-05-11 13:57:58.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 13:58:01.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7214 2023-05-11 14:49:30.000000 PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 14:50:34.969186 PatryksAutoAI-0.2.5/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-11 14:50:34.969186 PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-11 14:50:34.000000 PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-11 14:50:34.000000 PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-11 14:50:34.000000 PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-11 14:50:34.000000 PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-11 14:50:34.000000 PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-11 14:50:34.969186 PatryksAutoAI-0.2.5/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-11 14:50:28.000000 PatryksAutoAI-0.2.5/setup.py
```

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/metrics.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/cat.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/extra_trees.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/hist_gradient.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/kneighbours.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/light_lgb.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/linear_svc.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/logistic_regression.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/random_forest.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/svc.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/classification/models/xgb.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/model_data/model_data.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/metrics_regression.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/cat.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/elastic_net.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/lasso.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/lgb.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/sgd.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/svr.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/Machine_Learning_Classes/regression/models/xgb.py` & `PatryksAutoAI-0.2.5/Machine_Learning_Classes/regression/models/xgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 'n_estimators': trial.suggest_int('n_estimators', params["n_estimators"][0], params["n_estimators"][1]),
                 'max_depth': trial.suggest_int('max_depth', params["max_depth"][0], params["max_depth"][1]),
                 'learning_rate': trial.suggest_float('learning_rate', params['learning_rate'][0], params['learning_rate'][1]),
                 'subsample': trial.suggest_float('subsample', params['subsample'][0], params['subsample'][1]),
                 'colsample_bytree': trial.suggest_float('colsample_bytree', params['colsample_bytree'][0], params['colsample_bytree'][1]),
                 'gamma': trial.suggest_float('gamma', params['gamma'][0], params['gamma'][1]),
                 'min_child_weight': trial.suggest_int('min_child_weight', params['min_child_weight'][0], params['min_child_weight'][1]),
-                'scale_pos_weight': trial.suggest_float('scale_pos_weight', params['scale_pos_weight'][0], params['scale_pos_weight'][1]),
+                'pos_scale_weight': trial.suggest_float('pos_scale_weight', params['pos_scale_weight'][0], params['pos_scale_weight'][1]),
                 'max_delta_step': trial.suggest_int('max_delta_step', params['max_delta_step'][0], params['max_delta_step'][1]),
                 'seed': params['seed'],
                 'num_boost_round': params["num_boost_round"],
                 'verbosity': params['verbosity']
             }
             xgb_model= xgb.train(param, dtrain)
             y_pred = xgb_model.predict(dtest)
```

### Comparing `PatryksAutoAI-0.2.4/PKG-INFO` & `PatryksAutoAI-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.2.4
+Version: 0.2.5
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.2.4
+Version: 0.2.5
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.2.4/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.2.5/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.2.4/setup.py` & `PatryksAutoAI-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```


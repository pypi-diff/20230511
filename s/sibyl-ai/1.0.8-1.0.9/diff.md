# Comparing `tmp/sibyl-ai-1.0.8.tar.gz` & `tmp/sibyl-ai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sibyl-ai-1.0.8.tar", last modified: Fri Oct 29 07:12:41 2021, max compression
+gzip compressed data, was "dist\sibyl-ai-1.0.9.tar", last modified: Sun Dec 19 08:43:07 2021, max compression
```

## Comparing `sibyl-ai-1.0.8.tar` & `sibyl-ai-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-10-29 07:12:41.958000 sibyl-ai-1.0.8/
--rw-rw-rw-   0        0        0       51 2021-08-30 08:07:57.000000 sibyl-ai-1.0.8/.gitignore
--rw-rw-rw-   0        0        0      331 2021-10-29 07:12:41.920000 sibyl-ai-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4012 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/readme.md
--rw-rw-rw-   0        0        0      123 2021-09-24 07:24:40.000000 sibyl-ai-1.0.8/requirements.txt
--rw-rw-rw-   0        0        0      100 2021-10-29 07:12:41.952000 sibyl-ai-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      669 2021-10-29 07:12:31.000000 sibyl-ai-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-29 07:12:40.548000 sibyl-ai-1.0.8/sibyl/
--rw-rw-rw-   0        0        0        0 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/sibyl/__init__.py
--rw-rw-rw-   0        0        0     6074 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/sibyl/dataexplorer.py
-drwxrwxrwx   0        0        0        0 2021-10-29 07:12:40.689000 sibyl-ai-1.0.8/sibyl/encoders/
--rw-rw-rw-   0        0        0        0 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/sibyl/encoders/__init__.py
--rw-rw-rw-   0        0        0     3629 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/sibyl/encoders/omniencoder.py
--rw-rw-rw-   0        0        0      722 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/sibyl/example_automl.py
--rw-rw-rw-   0        0        0     1269 2021-10-27 10:33:45.000000 sibyl-ai-1.0.8/sibyl/example_customsteps.py
-drwxrwxrwx   0        0        0        0 2021-10-29 07:12:41.474000 sibyl-ai-1.0.8/sibyl/models/
--rw-rw-rw-   0        0        0        0 2021-07-16 05:31:03.000000 sibyl-ai-1.0.8/sibyl/models/__init__.py
--rw-rw-rw-   0        0        0     1788 2021-09-27 05:21:04.000000 sibyl-ai-1.0.8/sibyl/models/catboostwrapper.py
--rw-rw-rw-   0        0        0     6407 2021-10-27 10:51:25.000000 sibyl-ai-1.0.8/sibyl/models/kerasdense.py
--rw-rw-rw-   0        0        0      945 2021-10-29 07:11:00.000000 sibyl-ai-1.0.8/sibyl/models/lightgbmwrapper.py
--rw-rw-rw-   0        0        0     7310 2021-09-21 13:55:51.000000 sibyl-ai-1.0.8/sibyl/predictor.py
-drwxrwxrwx   0        0        0        0 2021-10-29 07:12:41.803000 sibyl-ai-1.0.8/sibyl_ai.egg-info/
--rw-rw-rw-   0        0        0      331 2021-10-29 07:12:36.000000 sibyl-ai-1.0.8/sibyl_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2021-10-29 07:12:38.000000 sibyl-ai-1.0.8/sibyl_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-29 07:12:37.000000 sibyl-ai-1.0.8/sibyl_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2021-10-29 07:12:37.000000 sibyl-ai-1.0.8/sibyl_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-10-29 07:12:37.000000 sibyl-ai-1.0.8/sibyl_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-12-19 08:43:07.138000 sibyl-ai-1.0.9/
+-rw-rw-rw-   0        0        0       51 2021-08-30 08:08:07.000000 sibyl-ai-1.0.9/.gitignore
+-rw-rw-rw-   0        0        0      331 2021-12-19 08:43:07.120000 sibyl-ai-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4029 2021-12-14 13:21:32.000000 sibyl-ai-1.0.9/readme.md
+-rw-rw-rw-   0        0        0      123 2021-09-24 07:24:50.000000 sibyl-ai-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0      100 2021-12-19 08:43:07.134000 sibyl-ai-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      669 2021-12-19 08:37:00.000000 sibyl-ai-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-19 08:43:06.795000 sibyl-ai-1.0.9/sibyl/
+-rw-rw-rw-   0        0        0        0 2021-07-16 05:31:03.000000 sibyl-ai-1.0.9/sibyl/__init__.py
+-rw-rw-rw-   0        0        0     6074 2021-07-16 05:31:03.000000 sibyl-ai-1.0.9/sibyl/dataexplorer.py
+drwxrwxrwx   0        0        0        0 2021-12-19 08:43:06.844000 sibyl-ai-1.0.9/sibyl/encoders/
+-rw-rw-rw-   0        0        0        0 2021-07-16 05:31:03.000000 sibyl-ai-1.0.9/sibyl/encoders/__init__.py
+-rw-rw-rw-   0        0        0     3629 2021-07-16 05:31:03.000000 sibyl-ai-1.0.9/sibyl/encoders/omniencoder.py
+-rw-rw-rw-   0        0        0      722 2021-07-16 05:31:03.000000 sibyl-ai-1.0.9/sibyl/example_automl.py
+-rw-rw-rw-   0        0        0     1270 2021-12-14 13:21:32.000000 sibyl-ai-1.0.9/sibyl/example_customsteps.py
+drwxrwxrwx   0        0        0        0 2021-12-19 08:43:06.968000 sibyl-ai-1.0.9/sibyl/models/
+-rw-rw-rw-   0        0        0        0 2021-07-16 05:31:03.000000 sibyl-ai-1.0.9/sibyl/models/__init__.py
+-rw-rw-rw-   0        0        0     1788 2021-09-27 05:21:17.000000 sibyl-ai-1.0.9/sibyl/models/catboostwrapper.py
+-rw-rw-rw-   0        0        0     8894 2021-12-15 08:32:56.000000 sibyl-ai-1.0.9/sibyl/models/kerasmodels.py
+-rw-rw-rw-   0        0        0      945 2021-11-25 02:27:30.000000 sibyl-ai-1.0.9/sibyl/models/lightgbmwrapper.py
+-rw-rw-rw-   0        0        0     7311 2021-12-14 13:21:33.000000 sibyl-ai-1.0.9/sibyl/predictor.py
+drwxrwxrwx   0        0        0        0 2021-12-19 08:43:07.103000 sibyl-ai-1.0.9/sibyl_ai.egg-info/
+-rw-rw-rw-   0        0        0      331 2021-12-19 08:43:05.000000 sibyl-ai-1.0.9/sibyl_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2021-12-19 08:43:05.000000 sibyl-ai-1.0.9/sibyl_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-19 08:43:05.000000 sibyl-ai-1.0.9/sibyl_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2021-12-19 08:43:05.000000 sibyl-ai-1.0.9/sibyl_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-12-19 08:43:05.000000 sibyl-ai-1.0.9/sibyl_ai.egg-info/top_level.txt
```

### Comparing `sibyl-ai-1.0.8/readme.md` & `sibyl-ai-1.0.9/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,23 +57,24 @@
 
 ```python
 from sklearn import datasets
 from sklearn.decomposition import PCA
 from sklearn.model_selection import train_test_split
 
 from sibyl import predictor as pred
-from sibyl.models import kerasdense as kd
+from sibyl.models import kerasmodels as kd
 
 STEPS = [("preprocessing", PCA()),
          ("model", kd.KerasDenseClassifier(n_iter_no_change=1,
                                            epochs=1000))]
 
 SEARCH_PARAMS = {"preprocessing__n_components": [None, 0.99, 0.90],
                  "model__units": [(64,), (64, 64), (64, 64, 64)],
                  "model__batch_norm": [True, False]}
 
 X, y = datasets.fetch_openml('mnist_784', version=1, return_X_y=True)
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
 predclf = pred.SibylClassifier(steps=STEPS)
-predclf.search(X_train, y_train, params=SEARCH_PARAMS)  # RandomizedGridSearchCV available but also fit method is available
+predclf.search(X_train, y_train,
+               params=SEARCH_PARAMS)  # RandomizedGridSearchCV available but also fit method is available
 print(f"Test score: {predclf.score(X_test, y_test):.4f}")
 ```
```

### Comparing `sibyl-ai-1.0.8/setup.py` & `sibyl-ai-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(
     name="sibyl-ai",
-    version="1.0.8",
+    version="1.0.9",
     author="Francesco Baldisserri",
     author_email="fbaldisserri@gmail.com",
     packages=find_packages(include=["sibyl", "sibyl.models", "sibyl.encoders"]),
     install_requires=["joblib","numpy","pandas","scipy","scikit-learn",
                       "tensorflow","catboost","seaborn", "lightgbm",
                       "matplotlib"],
     description="Wrapper for SKLearn Pipeline with Auto ML features",
```

### Comparing `sibyl-ai-1.0.8/sibyl/dataexplorer.py` & `sibyl-ai-1.0.9/sibyl/dataexplorer.py`

 * *Files identical despite different names*

### Comparing `sibyl-ai-1.0.8/sibyl/encoders/omniencoder.py` & `sibyl-ai-1.0.9/sibyl/encoders/omniencoder.py`

 * *Files identical despite different names*

### Comparing `sibyl-ai-1.0.8/sibyl/example_automl.py` & `sibyl-ai-1.0.9/sibyl/example_automl.py`

 * *Files identical despite different names*

### Comparing `sibyl-ai-1.0.8/sibyl/example_customsteps.py` & `sibyl-ai-1.0.9/sibyl/example_customsteps.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from sklearn import datasets
 from sklearn.decomposition import PCA
 from sklearn.model_selection import train_test_split
 
 from sibyl import predictor as pred
-from sibyl.models import kerasdense as kd
+from sibyl.models import kerasmodels as kd
 
 STEPS = [("preprocessing", PCA()),
          ("model", kd.KerasDenseClassifier(n_iter_no_change=1,
                                            val_split=0.2,
                                            epochs=10))]
 
 SEARCH_PARAMS = {"preprocessing__n_components": [None, 0.99, 0.90],
```

### Comparing `sibyl-ai-1.0.8/sibyl/models/catboostwrapper.py` & `sibyl-ai-1.0.9/sibyl/models/catboostwrapper.py`

 * *Files identical despite different names*

### Comparing `sibyl-ai-1.0.8/sibyl/models/lightgbmwrapper.py` & `sibyl-ai-1.0.9/sibyl/models/lightgbmwrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class LGBMRegressorWrapper(lgb.LGBMRegressor):
     def fit(self, x, y):
         rounds = int(log10(self.n_estimators))
         x_train, x_val, y_train, y_val = train_test_split(x, y, test_size=0.2)
         return super().fit(x_train, y_train, eval_set=[(x_val, y_val)],
-                           callbacks=[lgb.early_stopping(rounds, verbose=False)])
+                           verbose=False, callbacks=[lgb.early_stopping(rounds)])
 
 
 class LGBMClassifierWrapper(lgb.LGBMClassifier):
     def fit(self, x, y):
         rounds = int(log10(self.n_estimators))
         x_train, x_val, y_train, y_val = train_test_split(x, y, test_size=0.2)
         return super().fit(x_train, y_train, eval_set=[(x_val, y_val)],
-                           callbacks=[lgb.early_stopping(rounds, verbose=False)])
+                           verbose=False, callbacks=[lgb.early_stopping(rounds)])
```

### Comparing `sibyl-ai-1.0.8/sibyl/predictor.py` & `sibyl-ai-1.0.9/sibyl/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.decomposition import PCA
 from sklearn.model_selection import RandomizedSearchCV
 from sklearn.metrics import accuracy_score, r2_score, make_scorer
 
 from sibyl.encoders.omniencoder import OmniEncoder
-from sibyl.models.kerasdense import KerasDenseRegressor, KerasDenseClassifier
+from sibyl.models.kerasmodels import KerasDenseRegressor, KerasDenseClassifier
 
 PARAMS = {"pca__n_components": [None, 0.99, 0.90],
           "model__units": [(64,), (64, 64), (64, 64, 64)],
           "model__batch_norm": [True, False]}
 
 
 class SibylBase(Pipeline):
```


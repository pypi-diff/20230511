# Comparing `tmp/crepes-0.2.0.tar.gz` & `tmp/crepes-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepes-0.2.0.tar", last modified: Fri Apr 28 07:58:51 2023, max compression
+gzip compressed data, was "crepes-0.3.0.tar", last modified: Thu May 11 12:50:32 2023, max compression
```

## Comparing `crepes-0.2.0.tar` & `crepes-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/
--rw-rw-r--   0 henke     (1000) henke     (1000)     1459 2023-04-28 07:57:14.000000 crepes-0.2.0/LICENSE
--rw-rw-r--   0 henke     (1000) henke     (1000)    15213 2023-04-28 07:58:51.491480 crepes-0.2.0/PKG-INFO
--rw-rw-r--   0 henke     (1000) henke     (1000)    14690 2023-04-28 07:32:04.000000 crepes-0.2.0/README.md
--rw-rw-r--   0 henke     (1000) henke     (1000)      106 2022-06-28 07:30:29.000000 crepes-0.2.0/pyproject.toml
--rw-rw-r--   0 henke     (1000) henke     (1000)       38 2023-04-28 07:58:51.491480 crepes-0.2.0/setup.cfg
--rw-rw-r--   0 henke     (1000) henke     (1000)      865 2023-04-12 14:34:32.000000 crepes-0.2.0/setup.py
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/src/
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/src/crepes/
--rw-rw-r--   0 henke     (1000) henke     (1000)      104 2023-04-12 11:57:09.000000 crepes-0.2.0/src/crepes/__init__.py
--rw-rw-r--   0 henke     (1000) henke     (1000)    42079 2023-04-27 16:41:21.000000 crepes-0.2.0/src/crepes/base.py
--rw-rw-r--   0 henke     (1000) henke     (1000)     8365 2023-04-27 15:14:46.000000 crepes-0.2.0/src/crepes/fillings.py
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/src/crepes.egg-info/
--rw-rw-r--   0 henke     (1000) henke     (1000)    15213 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/PKG-INFO
--rw-rw-r--   0 henke     (1000) henke     (1000)      275 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/SOURCES.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)        1 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/dependency_links.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)       13 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/requires.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)        7 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/top_level.txt
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-05-11 12:50:32.122882 crepes-0.3.0/
+-rw-rw-r--   0 henke     (1000) henke     (1000)     1459 2023-05-08 10:22:43.000000 crepes-0.3.0/LICENSE
+-rw-rw-r--   0 henke     (1000) henke     (1000)    15436 2023-05-11 12:50:32.122882 crepes-0.3.0/PKG-INFO
+-rw-rw-r--   0 henke     (1000) henke     (1000)    14913 2023-05-11 08:30:12.000000 crepes-0.3.0/README.md
+-rw-rw-r--   0 henke     (1000) henke     (1000)      106 2023-05-08 10:22:43.000000 crepes-0.3.0/pyproject.toml
+-rw-rw-r--   0 henke     (1000) henke     (1000)       38 2023-05-11 12:50:32.122882 crepes-0.3.0/setup.cfg
+-rw-rw-r--   0 henke     (1000) henke     (1000)      865 2023-05-08 14:28:34.000000 crepes-0.3.0/setup.py
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-05-11 12:50:32.122882 crepes-0.3.0/src/
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-05-11 12:50:32.122882 crepes-0.3.0/src/crepes/
+-rw-rw-r--   0 henke     (1000) henke     (1000)      104 2023-05-08 10:22:43.000000 crepes-0.3.0/src/crepes/__init__.py
+-rw-rw-r--   0 henke     (1000) henke     (1000)    42079 2023-05-10 08:30:26.000000 crepes-0.3.0/src/crepes/base.py
+-rw-rw-r--   0 henke     (1000) henke     (1000)    17418 2023-05-11 08:59:22.000000 crepes-0.3.0/src/crepes/fillings.py
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-05-11 12:50:32.122882 crepes-0.3.0/src/crepes.egg-info/
+-rw-rw-r--   0 henke     (1000) henke     (1000)    15436 2023-05-11 12:50:32.000000 crepes-0.3.0/src/crepes.egg-info/PKG-INFO
+-rw-rw-r--   0 henke     (1000) henke     (1000)      275 2023-05-11 12:50:32.000000 crepes-0.3.0/src/crepes.egg-info/SOURCES.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)        1 2023-05-11 12:50:32.000000 crepes-0.3.0/src/crepes.egg-info/dependency_links.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)       13 2023-05-11 12:50:32.000000 crepes-0.3.0/src/crepes.egg-info/requires.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)        7 2023-05-11 12:50:32.000000 crepes-0.3.0/src/crepes.egg-info/top_level.txt
```

### Comparing `crepes-0.2.0/LICENSE` & `crepes-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crepes-0.2.0/PKG-INFO` & `crepes-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepes
-Version: 0.2.0
+Version: 0.3.0
 Summary: Conformal regressors and predictive systems (crepes)
 Home-page: https://github.com/henrikbostrom/crepes
 Author: Henrik Boström
 Author-email: bostromh@kth.se
 Project-URL: Bug Tracker, https://github.com//henrikbostrom/crepes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -17,33 +17,39 @@
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
 The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
 
 ## Installation
 
-Install with:
+From [PyPI](https://pypi.org/project/crepes/)
 
 ```bash
 pip install crepes
 ```
 
+From [conda-forge](https://anaconda.org/conda-forge/crepes)
+
+```bash
+conda install -c conda-forge crepes
+```
+
 ## Documentation
 
 For complete documentation of the `crepes` package, see [here](https://crepes.readthedocs.io/en/latest/).
 
 ## Quickstart
 
 ### Conformal regressors
 
-We first import the main class and two helper functions:
+We first import the main class from `crepes` and a helper class and function from `crepes.fillings`:
 
 ```python
 from crepes import ConformalRegressor
-from crepes.fillings import sigma_knn, binning
+from crepes.fillings import DifficultyEstimator, binning
 ```
 
 We will illustrate the above using a dataset from [www.openml.org](https://www.openml.org) and a `RandomForestRegressor` from [sklearn](https://scikit-learn.org):
 
 ```python
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
@@ -109,48 +115,51 @@
        [ 567114.77, 1044561.67],
        [  16067.02,  493513.92],
        [  97103.35,  574550.25]])
 ```
 
 The above intervals are not normalized, i.e., they are all of the same size (at least before they are cut). We could make the intervals more informative through normalization using difficulty estimates; more difficult instances will be assigned wider intervals.
 
-We will use the helper function `sigma_knn` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
+We will use a `DifficultyEstimator` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
 
 ```python
-sigmas_cal = sigma_knn(X=X_cal, X_ref=X_prop_train, y_ref=y_prop_train)
+de = DifficultyEstimator()
+de.fit(X_prop_train, y=y_prop_train)
+
+sigmas_cal = de.apply(X_cal)
 ```
 
 The difficulty estimates and residuals of the calibration examples can now be used to form a normalized conformal regressor:
 
 ```python
 cr_norm = ConformalRegressor()
 cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
 ```
 
-To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same helper function. 
+To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same difficulty estimator as for the calibration set:
 
 ```python
-sigmas_test = sigma_knn(X=X_test, X_ref=X_prop_train, y_ref=y_prop_train)
+sigmas_test = de.apply(X_test)
 ```
 
 Now we can obtain the prediction intervals, using the point predictions and difficulty estimates for the test set:
 
 ```python
 intervals_norm = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test, 
                                  y_min=0)
 ```
 
 ```numpy
-array([[205959.07517616, 576004.92482384],
-       [133206.86035366, 438925.51964634],
-       [291925.81345507, 879201.32654493],
+array([[ 226719.06607977,  555244.93392023],
+       [ 173767.90753715,  398364.47246285],
+       [ 124690.70166966, 1046436.43833034],
        ...,
-       [622212.95112744, 989463.48887256],
-       [ 98805.77755066, 410775.16244934],
-       [197248.38670265, 474405.21329735]])
+       [ 607949.71540572, 1003726.72459428],
+       [ 188671.3752278 ,  320909.5647722 ],
+       [ 145340.39076824,  526313.20923176]])
 ```
 
 Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no information on the expected error should instead lead to more uniformly distributed interval sizes.
 
 A Mondrian conformal regressor can be used to address these problems, by dividing the object space into non-overlapping so-called Mondrian categories, and forming a (standard) conformal regressor for each category. The category membership of the objects can be provided as an additional argument, named `bins`, for the `fit` method.
 
 Here we will use the helper function `binning` to form Mondrian categories by equal-sized binning of the difficulty estimates; the function will return labels for the calibration objects as well as thresholds for the bins, which are later to be used when binning the test objects:
@@ -188,15 +197,15 @@
        [ 140587.46,  531066.14]])
 ```
 
 ### Conformal predictive systems
 
 The interface to a `ConformalPredictiveSystem` is very similar to that of a conformal regressor; by providing just the residuals, we get a standard conformal predictive system, by providing also difficulty estimates, we get a normalized conformal predictive system and by providing labels for Mondrian categories (bins), we get a Mondrian conformal predictive system.
 
-The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain calibrated point predictions, as well as p values for given target values.
+The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain percentiles, calibrated point predictions, as well as p-values for given target values.
 
 Let us fit a Mondrian normalized conformal predictive system, using the above residuals and difficulty estimates (sigmas), and where the Mondrian categories (bins) are formed using the point predictions for the calibration set:
 
 ```python
 from crepes import ConformalPredictiveSystem
 
 bins_cal, bin_thresholds = binning(values=y_hat_cal, bins=5)
@@ -220,40 +229,40 @@
                                   bins=bins_test,
                                   lower_percentiles=2.5,
                                   higher_percentiles=97.5,
                                   y_min=0)
 ```
 
 ```numpy
-array([[ 226536.76784152,  519404.56955659],
-       [ 170043.51497485,  376524.37491457],
-       [ 192376.08061079,  994115.461665  ],
+array([[ 245826.3422693 ,  517315.83618985],
+       [ 145348.03415848,  392968.15587997],
+       [ 148774.65461212, 1034300.84195976],
        ...,
-       [ 594183.11971763, 1010273.54816378],
-       [ 186478.52365968,  308050.53035102],
-       [ 167498.01540504,  485813.1329371 ]])
+       [ 589200.5725957 , 1057013.89102007],
+       [ 171938.29382952,  317732.31611141],
+       [ 167498.01540504,  482328.98552632]])
 ```
 
-We can also get the p values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
+We can also get the p-values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
 
 ```python
 p_values = cps_mond_norm.predict(y_hat=y_hat_test,
                                  sigmas=sigmas_test,
                                  bins=bins_test,
                                  y=y_test)
 ```
 
 ```numpy
-array([[0.98298087],
-       [0.90125379],
-       [0.41770673],
+array([[0.98603614],
+       [0.87178256],
+       [0.44201984],
        ...,
-       [0.04659288],
-       [0.07914733],
-       [0.31090332]])
+       [0.05688804],
+       [0.09473604],
+       [0.31069913]])
 ```
 
 We may request that the predict method returns the full conformal predictive distribution (CPD) for each test instance, as defined by the threshold values, by setting `return_cpds=True`. The format of the distributions vary with the type of conformal predictive system; for a standard and normalized CPS, the output is an array with a row for each test instance and a column for each calibration instance (residual), while for a Mondrian CPS, the default output is a vector containing one CPD per test instance, since the number of values may vary between categories.
 
 ```python
 cpds = cps_mond_norm.predict(y_hat=y_hat_test,
                              sigmas=sigmas_test,
```

### Comparing `crepes-0.2.0/README.md` & `crepes-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,39 @@
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
 The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
 
 ## Installation
 
-Install with:
+From [PyPI](https://pypi.org/project/crepes/)
 
 ```bash
 pip install crepes
 ```
 
+From [conda-forge](https://anaconda.org/conda-forge/crepes)
+
+```bash
+conda install -c conda-forge crepes
+```
+
 ## Documentation
 
 For complete documentation of the `crepes` package, see [here](https://crepes.readthedocs.io/en/latest/).
 
 ## Quickstart
 
 ### Conformal regressors
 
-We first import the main class and two helper functions:
+We first import the main class from `crepes` and a helper class and function from `crepes.fillings`:
 
 ```python
 from crepes import ConformalRegressor
-from crepes.fillings import sigma_knn, binning
+from crepes.fillings import DifficultyEstimator, binning
 ```
 
 We will illustrate the above using a dataset from [www.openml.org](https://www.openml.org) and a `RandomForestRegressor` from [sklearn](https://scikit-learn.org):
 
 ```python
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
@@ -94,48 +100,51 @@
        [ 567114.77, 1044561.67],
        [  16067.02,  493513.92],
        [  97103.35,  574550.25]])
 ```
 
 The above intervals are not normalized, i.e., they are all of the same size (at least before they are cut). We could make the intervals more informative through normalization using difficulty estimates; more difficult instances will be assigned wider intervals.
 
-We will use the helper function `sigma_knn` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
+We will use a `DifficultyEstimator` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
 
 ```python
-sigmas_cal = sigma_knn(X=X_cal, X_ref=X_prop_train, y_ref=y_prop_train)
+de = DifficultyEstimator()
+de.fit(X_prop_train, y=y_prop_train)
+
+sigmas_cal = de.apply(X_cal)
 ```
 
 The difficulty estimates and residuals of the calibration examples can now be used to form a normalized conformal regressor:
 
 ```python
 cr_norm = ConformalRegressor()
 cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
 ```
 
-To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same helper function. 
+To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same difficulty estimator as for the calibration set:
 
 ```python
-sigmas_test = sigma_knn(X=X_test, X_ref=X_prop_train, y_ref=y_prop_train)
+sigmas_test = de.apply(X_test)
 ```
 
 Now we can obtain the prediction intervals, using the point predictions and difficulty estimates for the test set:
 
 ```python
 intervals_norm = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test, 
                                  y_min=0)
 ```
 
 ```numpy
-array([[205959.07517616, 576004.92482384],
-       [133206.86035366, 438925.51964634],
-       [291925.81345507, 879201.32654493],
-       ...,
-       [622212.95112744, 989463.48887256],
-       [ 98805.77755066, 410775.16244934],
-       [197248.38670265, 474405.21329735]])
+array([[ 226719.06607977,  555244.93392023],
+       [ 173767.90753715,  398364.47246285],
+       [ 124690.70166966, 1046436.43833034],
+       ...,
+       [ 607949.71540572, 1003726.72459428],
+       [ 188671.3752278 ,  320909.5647722 ],
+       [ 145340.39076824,  526313.20923176]])
 ```
 
 Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no information on the expected error should instead lead to more uniformly distributed interval sizes.
 
 A Mondrian conformal regressor can be used to address these problems, by dividing the object space into non-overlapping so-called Mondrian categories, and forming a (standard) conformal regressor for each category. The category membership of the objects can be provided as an additional argument, named `bins`, for the `fit` method.
 
 Here we will use the helper function `binning` to form Mondrian categories by equal-sized binning of the difficulty estimates; the function will return labels for the calibration objects as well as thresholds for the bins, which are later to be used when binning the test objects:
@@ -173,15 +182,15 @@
        [ 140587.46,  531066.14]])
 ```
 
 ### Conformal predictive systems
 
 The interface to a `ConformalPredictiveSystem` is very similar to that of a conformal regressor; by providing just the residuals, we get a standard conformal predictive system, by providing also difficulty estimates, we get a normalized conformal predictive system and by providing labels for Mondrian categories (bins), we get a Mondrian conformal predictive system.
 
-The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain calibrated point predictions, as well as p values for given target values.
+The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain percentiles, calibrated point predictions, as well as p-values for given target values.
 
 Let us fit a Mondrian normalized conformal predictive system, using the above residuals and difficulty estimates (sigmas), and where the Mondrian categories (bins) are formed using the point predictions for the calibration set:
 
 ```python
 from crepes import ConformalPredictiveSystem
 
 bins_cal, bin_thresholds = binning(values=y_hat_cal, bins=5)
@@ -205,40 +214,40 @@
                                   bins=bins_test,
                                   lower_percentiles=2.5,
                                   higher_percentiles=97.5,
                                   y_min=0)
 ```
 
 ```numpy
-array([[ 226536.76784152,  519404.56955659],
-       [ 170043.51497485,  376524.37491457],
-       [ 192376.08061079,  994115.461665  ],
+array([[ 245826.3422693 ,  517315.83618985],
+       [ 145348.03415848,  392968.15587997],
+       [ 148774.65461212, 1034300.84195976],
        ...,
-       [ 594183.11971763, 1010273.54816378],
-       [ 186478.52365968,  308050.53035102],
-       [ 167498.01540504,  485813.1329371 ]])
+       [ 589200.5725957 , 1057013.89102007],
+       [ 171938.29382952,  317732.31611141],
+       [ 167498.01540504,  482328.98552632]])
 ```
 
-We can also get the p values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
+We can also get the p-values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
 
 ```python
 p_values = cps_mond_norm.predict(y_hat=y_hat_test,
                                  sigmas=sigmas_test,
                                  bins=bins_test,
                                  y=y_test)
 ```
 
 ```numpy
-array([[0.98298087],
-       [0.90125379],
-       [0.41770673],
-       ...,
-       [0.04659288],
-       [0.07914733],
-       [0.31090332]])
+array([[0.98603614],
+       [0.87178256],
+       [0.44201984],
+       ...,
+       [0.05688804],
+       [0.09473604],
+       [0.31069913]])
 ```
 
 We may request that the predict method returns the full conformal predictive distribution (CPD) for each test instance, as defined by the threshold values, by setting `return_cpds=True`. The format of the distributions vary with the type of conformal predictive system; for a standard and normalized CPS, the output is an array with a row for each test instance and a column for each calibration instance (residual), while for a Mondrian CPS, the default output is a vector containing one CPD per test instance, since the number of values may vary between categories.
 
 ```python
 cpds = cps_mond_norm.predict(y_hat=y_hat_test,
                              sigmas=sigmas_test,
```

### Comparing `crepes-0.2.0/setup.py` & `crepes-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crepes",
-    version="0.2.0",
+    version="0.3.0",
     author="Henrik Boström",
     author_email="bostromh@kth.se",
     description="Conformal regressors and predictive systems (crepes)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henrikbostrom/crepes",
     project_urls={
```

### Comparing `crepes-0.2.0/src/crepes/base.py` & `crepes-0.3.0/src/crepes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 Author: Henrik Boström (bostromh@kth.se)
 
 Copyright 2023 Henrik Boström
 
 License: BSD 3 clause
 """
 
+__version__ = "0.3.0"
+
 import numpy as np
 import pandas as pd
 import time
 import warnings
 
 warnings.simplefilter("always", UserWarning)
 
-__version__ = "0.2.0"
-
 class ConformalPredictor():
     """
     The class contains two sub-classes: ConformalRegressor 
     and ConformalPredictiveSystem.
     """
     
     def __init__(self):
```

### Comparing `crepes-0.2.0/src/crepes.egg-info/PKG-INFO` & `crepes-0.3.0/src/crepes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepes
-Version: 0.2.0
+Version: 0.3.0
 Summary: Conformal regressors and predictive systems (crepes)
 Home-page: https://github.com/henrikbostrom/crepes
 Author: Henrik Boström
 Author-email: bostromh@kth.se
 Project-URL: Bug Tracker, https://github.com//henrikbostrom/crepes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -17,33 +17,39 @@
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
 The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
 
 ## Installation
 
-Install with:
+From [PyPI](https://pypi.org/project/crepes/)
 
 ```bash
 pip install crepes
 ```
 
+From [conda-forge](https://anaconda.org/conda-forge/crepes)
+
+```bash
+conda install -c conda-forge crepes
+```
+
 ## Documentation
 
 For complete documentation of the `crepes` package, see [here](https://crepes.readthedocs.io/en/latest/).
 
 ## Quickstart
 
 ### Conformal regressors
 
-We first import the main class and two helper functions:
+We first import the main class from `crepes` and a helper class and function from `crepes.fillings`:
 
 ```python
 from crepes import ConformalRegressor
-from crepes.fillings import sigma_knn, binning
+from crepes.fillings import DifficultyEstimator, binning
 ```
 
 We will illustrate the above using a dataset from [www.openml.org](https://www.openml.org) and a `RandomForestRegressor` from [sklearn](https://scikit-learn.org):
 
 ```python
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
@@ -109,48 +115,51 @@
        [ 567114.77, 1044561.67],
        [  16067.02,  493513.92],
        [  97103.35,  574550.25]])
 ```
 
 The above intervals are not normalized, i.e., they are all of the same size (at least before they are cut). We could make the intervals more informative through normalization using difficulty estimates; more difficult instances will be assigned wider intervals.
 
-We will use the helper function `sigma_knn` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
+We will use a `DifficultyEstimator` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
 
 ```python
-sigmas_cal = sigma_knn(X=X_cal, X_ref=X_prop_train, y_ref=y_prop_train)
+de = DifficultyEstimator()
+de.fit(X_prop_train, y=y_prop_train)
+
+sigmas_cal = de.apply(X_cal)
 ```
 
 The difficulty estimates and residuals of the calibration examples can now be used to form a normalized conformal regressor:
 
 ```python
 cr_norm = ConformalRegressor()
 cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
 ```
 
-To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same helper function. 
+To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same difficulty estimator as for the calibration set:
 
 ```python
-sigmas_test = sigma_knn(X=X_test, X_ref=X_prop_train, y_ref=y_prop_train)
+sigmas_test = de.apply(X_test)
 ```
 
 Now we can obtain the prediction intervals, using the point predictions and difficulty estimates for the test set:
 
 ```python
 intervals_norm = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test, 
                                  y_min=0)
 ```
 
 ```numpy
-array([[205959.07517616, 576004.92482384],
-       [133206.86035366, 438925.51964634],
-       [291925.81345507, 879201.32654493],
+array([[ 226719.06607977,  555244.93392023],
+       [ 173767.90753715,  398364.47246285],
+       [ 124690.70166966, 1046436.43833034],
        ...,
-       [622212.95112744, 989463.48887256],
-       [ 98805.77755066, 410775.16244934],
-       [197248.38670265, 474405.21329735]])
+       [ 607949.71540572, 1003726.72459428],
+       [ 188671.3752278 ,  320909.5647722 ],
+       [ 145340.39076824,  526313.20923176]])
 ```
 
 Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no information on the expected error should instead lead to more uniformly distributed interval sizes.
 
 A Mondrian conformal regressor can be used to address these problems, by dividing the object space into non-overlapping so-called Mondrian categories, and forming a (standard) conformal regressor for each category. The category membership of the objects can be provided as an additional argument, named `bins`, for the `fit` method.
 
 Here we will use the helper function `binning` to form Mondrian categories by equal-sized binning of the difficulty estimates; the function will return labels for the calibration objects as well as thresholds for the bins, which are later to be used when binning the test objects:
@@ -188,15 +197,15 @@
        [ 140587.46,  531066.14]])
 ```
 
 ### Conformal predictive systems
 
 The interface to a `ConformalPredictiveSystem` is very similar to that of a conformal regressor; by providing just the residuals, we get a standard conformal predictive system, by providing also difficulty estimates, we get a normalized conformal predictive system and by providing labels for Mondrian categories (bins), we get a Mondrian conformal predictive system.
 
-The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain calibrated point predictions, as well as p values for given target values.
+The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain percentiles, calibrated point predictions, as well as p-values for given target values.
 
 Let us fit a Mondrian normalized conformal predictive system, using the above residuals and difficulty estimates (sigmas), and where the Mondrian categories (bins) are formed using the point predictions for the calibration set:
 
 ```python
 from crepes import ConformalPredictiveSystem
 
 bins_cal, bin_thresholds = binning(values=y_hat_cal, bins=5)
@@ -220,40 +229,40 @@
                                   bins=bins_test,
                                   lower_percentiles=2.5,
                                   higher_percentiles=97.5,
                                   y_min=0)
 ```
 
 ```numpy
-array([[ 226536.76784152,  519404.56955659],
-       [ 170043.51497485,  376524.37491457],
-       [ 192376.08061079,  994115.461665  ],
+array([[ 245826.3422693 ,  517315.83618985],
+       [ 145348.03415848,  392968.15587997],
+       [ 148774.65461212, 1034300.84195976],
        ...,
-       [ 594183.11971763, 1010273.54816378],
-       [ 186478.52365968,  308050.53035102],
-       [ 167498.01540504,  485813.1329371 ]])
+       [ 589200.5725957 , 1057013.89102007],
+       [ 171938.29382952,  317732.31611141],
+       [ 167498.01540504,  482328.98552632]])
 ```
 
-We can also get the p values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
+We can also get the p-values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
 
 ```python
 p_values = cps_mond_norm.predict(y_hat=y_hat_test,
                                  sigmas=sigmas_test,
                                  bins=bins_test,
                                  y=y_test)
 ```
 
 ```numpy
-array([[0.98298087],
-       [0.90125379],
-       [0.41770673],
+array([[0.98603614],
+       [0.87178256],
+       [0.44201984],
        ...,
-       [0.04659288],
-       [0.07914733],
-       [0.31090332]])
+       [0.05688804],
+       [0.09473604],
+       [0.31069913]])
 ```
 
 We may request that the predict method returns the full conformal predictive distribution (CPD) for each test instance, as defined by the threshold values, by setting `return_cpds=True`. The format of the distributions vary with the type of conformal predictive system; for a standard and normalized CPS, the output is an array with a row for each test instance and a column for each calibration instance (residual), while for a Mondrian CPS, the default output is a vector containing one CPD per test instance, since the number of values may vary between categories.
 
 ```python
 cpds = cps_mond_norm.predict(y_hat=y_hat_test,
                              sigmas=sigmas_test,
```


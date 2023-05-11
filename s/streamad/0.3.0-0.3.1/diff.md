# Comparing `tmp/streamad-0.3.0.tar.gz` & `tmp/streamad-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamad-0.3.0.tar", last modified: Thu Sep 22 09:51:16 2022, max compression
+gzip compressed data, was "streamad-0.3.1.tar", max compression
```

## Comparing `streamad-0.3.0.tar` & `streamad-0.3.1.tar`

### file list

```diff
@@ -1,55 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.918632 streamad-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11321 2022-09-22 09:51:05.000000 streamad-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-22 09:51:05.000000 streamad-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10108 2022-09-22 09:51:16.918632 streamad-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9208 2022-09-22 09:51:05.000000 streamad-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-22 09:51:05.000000 streamad-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 09:51:16.918632 streamad-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-09-22 09:51:05.000000 streamad-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.914632 streamad-0.3.0/streamad/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.914632 streamad-0.3.0/streamad/base/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/base/detector.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/base/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.914632 streamad-0.3.0/streamad/evaluate/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/evaluate/numenta_aware_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/evaluate/point_aware_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/evaluate/series_aware_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10422 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/evaluate/ts_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.918632 streamad-0.3.0/streamad/model/
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/KNN_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/Mad_Dectector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/OCSVM_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/SArima_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/SR_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/hstree_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/loda_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/random_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/rrcf_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/rshash_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)    12812 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/spot_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/xStream_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/zscore_Detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     5011 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/model/zspot_Detector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.918632 streamad-0.3.0/streamad/process/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/process/tdigest_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/process/vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/process/weight_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/process/zscore_calibrator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.918632 streamad-0.3.0/streamad/util/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/util/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/util/math_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/util/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/util/stream_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-22 09:51:05.000000 streamad-0.3.0/streamad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 09:51:16.914632 streamad-0.3.0/streamad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10108 2022-09-22 09:51:16.000000 streamad-0.3.0/streamad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-09-22 09:51:16.000000 streamad-0.3.0/streamad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 09:51:16.000000 streamad-0.3.0/streamad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-22 09:51:16.000000 streamad-0.3.0/streamad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-22 09:51:16.000000 streamad-0.3.0/streamad.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11321 2023-05-11 10:09:44.850711 streamad-0.3.1/LICENSE
+-rw-r--r--   0        0        0     9162 2023-05-11 10:09:44.850711 streamad-0.3.1/README.md
+-rw-r--r--   0        0        0      587 2023-05-11 10:09:44.962712 streamad-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      316 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/__init__.py
+-rw-r--r--   0        0        0      112 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/base/__init__.py
+-rw-r--r--   0        0        0     3012 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/base/detector.py
+-rw-r--r--   0        0        0      542 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/base/metrics.py
+-rw-r--r--   0        0        0      252 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/evaluate/__init__.py
+-rw-r--r--   0        0        0     1374 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/evaluate/numenta_aware_metrics.py
+-rw-r--r--   0        0        0     1338 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/evaluate/point_aware_metrics.py
+-rw-r--r--   0        0        0     1777 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/evaluate/series_aware_metrics.py
+-rw-r--r--   0        0        0    10678 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/evaluate/ts_metrics.py
+-rw-r--r--   0        0        0      890 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/meta.yaml
+-rw-r--r--   0        0        0     1652 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/KNN_Detector.py
+-rw-r--r--   0        0        0     1141 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/Mad_Dectector.py
+-rw-r--r--   0        0        0     1368 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/OCSVM_Detector.py
+-rw-r--r--   0        0        0     2420 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/SArima_Detector.py
+-rw-r--r--   0        0        0     3485 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/SR_Detector.py
+-rw-r--r--   0        0        0      888 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/__init__.py
+-rw-r--r--   0        0        0     4577 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/hstree_Detector.py
+-rw-r--r--   0        0        0     4315 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/loda_Detector.py
+-rw-r--r--   0        0        0      447 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/random_Detector.py
+-rw-r--r--   0        0        0     2340 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/rrcf_Detector.py
+-rw-r--r--   0        0        0     4318 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/rshash_Detector.py
+-rw-r--r--   0        0        0    12936 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/spot_Detector.py
+-rw-r--r--   0        0        0     6776 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/xStream_Detector.py
+-rw-r--r--   0        0        0     1026 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/zscore_Detector.py
+-rw-r--r--   0        0        0     7249 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/model/zspot_Detector.py
+-rw-r--r--   0        0        0      288 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/process/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/process/tdigest_calibrator.py
+-rw-r--r--   0        0        0     1115 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/process/vote_ensemble.py
+-rw-r--r--   0        0        0     1511 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/process/weight_ensemble.py
+-rw-r--r--   0        0        0     2341 2023-05-11 10:09:44.962712 streamad-0.3.1/streamad/process/zscore_calibrator.py
+-rw-r--r--   0        0        0      476 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/__init__.py
+-rw-r--r--   0        0        0    40309 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/data/multiDS.csv
+-rw-r--r--   0        0        0    39240 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/data/uniDS.csv
+-rw-r--r--   0        0        0     2493 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/dataset.py
+-rw-r--r--   0        0        0     5552 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/math_toolkit.py
+-rw-r--r--   0        0        0     2397 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/plot.py
+-rw-r--r--   0        0        0      719 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/util/stream_generator.py
+-rw-r--r--   0        0        0       42 2023-05-11 10:09:44.966712 streamad-0.3.1/streamad/version.py
+-rw-r--r--   0        0        0    10210 1970-01-01 00:00:00.000000 streamad-0.3.1/PKG-INFO
```

### Comparing `streamad-0.3.0/LICENSE` & `streamad-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/PKG-INFO` & `streamad-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: streamad
-Version: 0.3.0
-Summary: An anomaly detection package for data streams.
-Home-page: https://github.com/Fengrui-Liu/StreamAD
-Author: liufr
-Author-email: liufengrui18z@ict.ac.cn
-License: UNKNOWN
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # StreamAD
 
 ![StreamAD Logo](docs/source/images/logo_htmlwithname.svg)
 
 
 
 Anomaly detection for data streams/time series. Detectors process the univariate or multivariate data one by one to simulte a real-time scene.
@@ -97,15 +73,14 @@
 
 If you want to detect multivarite time series with these models, you need to apply them on each feature separately.
 
 | Model Example                                                                                                     | API Usage                                                                                                         | Paper                                                                                                                                                                                                         |
 | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [KNNCAD](https://streamad.readthedocs.io/en/latest/example/univariate.html#knncad-detector)                       | [streamad.model.KNNDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#knndetector)       | [Conformalized density- and distance-based anomaly detection in time-series data](https://arxiv.org/abs/1608.04585)                                                                                           |
 | [SPOT](https://streamad.readthedocs.io/en/latest/example/univariate.html#spot-detector)                           | [streamad.model.SpotDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#spotdetector)     | [Anomaly detection in streams with extreme value theory](https://dl.acm.org/doi/10.1145/3097983.3098144)                                                                                                      |
-| [RRCF](https://streamad.readthedocs.io/en/latest/example/univariate.html#rrcf-detector)                           | [streamad.model.RrcfDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#rrcfdetector)     | [Robust random cut forest based anomaly detection on streams](http://proceedings.mlr.press/v48/guha16.pdf)                                                                                                    |
 | [Spectral Residual](https://streamad.readthedocs.io/en/latest/example/univariate.html#spectral-residual-detector) | [streamad.model.SRDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#srdetector)         | [Time-series anomaly detection service at microsoft](https://arxiv.org/abs/1906.03821)                                                                                                                        |
 | [Z score](https://streamad.readthedocs.io/en/latest/example/univariate.html#z-score-detector)                     | [streamad.model.ZScoreDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#zscoredetector) | [Standard score](https://en.wikipedia.org/wiki/Standard_score)                                                                                                                                                |
 | [One-class SVM](https://streamad.readthedocs.io/en/latest/example/univariate.html#one-class-svm-detector)         | [streamad.model.OCSVMDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#ocsvmdetector)   | [One-class SVM](https://en.wikipedia.org/w/index.php?title=One-class_classification&oldid=1098733917)                                                                                                         |
 | [MAD](https://streamad.readthedocs.io/en/latest/example/univariate.html#median-absolute-deviation-detector)       | [streamad.model.MadDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#maddetector)       | [Median absolute deviation](https://www.influxdata.com/blog/anomaly-detection-with-median-absolute-deviation/#:~:text=How%20Median%20Absolute%20Deviation%20algorithm,time%20series%20at%20that%20timestamp/) |
 | [SARIMAX](https://streamad.readthedocs.io/en/latest/example/univariate.html#seasonal-arima-detector)              | [streamad.model.SArimaDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#sarimadetector) | [Seasonal Arima Detector](https://www.statsmodels.org/dev/generated/statsmodels.tsa.statespace.sarimax.SARIMAX.html?highlight=sarimax#statsmodels.tsa.statespace.sarimax.SARIMAX)                             |
 
 ### For multivariate time series
@@ -116,9 +91,8 @@
 
 | Models Example                                                                                         | API Usage                                                                                                          | Paper                                                                                                                                                                     |
 | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [xStream](https://streamad.readthedocs.io/en/latest/example/multivariate.html#xstream-detector)        | [streamad.model.xStramDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#xstreamdetector) | [Xstream: outlier detection in feature-evolving data streams](http://www.kdd.org/kdd2018/accepted-papers/view/xstream-outlier-detection-in-feature-evolving-data-streams) |
 | [RShash](https://streamad.readthedocs.io/en/latest/example/multivariate.html#rshash-detector)          | [streamad.model.RShashDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#rshashdetector)  | [Subspace Outlier Detection in Linear Time with Randomized Hashing](https://ieeexplore.ieee.org/document/7837870)                                                         |
 | [HSTree](https://streamad.readthedocs.io/en/latest/example/multivariate.html#half-space-tree-detector) | [streamad.model.HSTreeDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#hstreedetector)  | [Fast Anomaly Detection for Streaming Data](https://www.ijcai.org/Proceedings/11/Papers/254.pdf)                                                                          |
 | [LODA](https://streamad.readthedocs.io/en/latest/example/multivariate.html#loda-detector)              | [streamad.model.LodaDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#lodadetector)      | [Lightweight on-line detector of anomalies](https://link.springer.com/article/10.1007/s10994-015-5521-0)                                                                  |
-
-
+| [RRCF](https://streamad.readthedocs.io/en/latest/example/univariate.html#rrcf-detector)                | [streamad.model.RrcfDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#rrcfdetector)      | [Robust random cut forest based anomaly detection on streams](http://proceedings.mlr.press/v48/guha16.pdf)                                                                |
```

### Comparing `streamad-0.3.0/README.md` & `streamad-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: streamad
+Version: 0.3.1
+Summary: An anomaly detection package for data streams.
+License: Apache Software License
+Author: Fengrui-Liu
+Author-email: liufengrui18z@ict.ac.cn
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fast-histogram (>=0.11,<0.12)
+Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: plotly (>=5.14.1,<6.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
+Requires-Dist: rrcf (>=0.4.4,<0.5.0)
+Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
+Requires-Dist: scipy (>=1.3.1,<2.0.0)
+Requires-Dist: statsmodels (==0.13.5)
+Requires-Dist: tdigest (>=0.5.2.2,<0.6.0.0)
+Description-Content-Type: text/markdown
+
 # StreamAD
 
 ![StreamAD Logo](docs/source/images/logo_htmlwithname.svg)
 
 
 
 Anomaly detection for data streams/time series. Detectors process the univariate or multivariate data one by one to simulte a real-time scene.
@@ -73,15 +101,14 @@
 
 If you want to detect multivarite time series with these models, you need to apply them on each feature separately.
 
 | Model Example                                                                                                     | API Usage                                                                                                         | Paper                                                                                                                                                                                                         |
 | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [KNNCAD](https://streamad.readthedocs.io/en/latest/example/univariate.html#knncad-detector)                       | [streamad.model.KNNDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#knndetector)       | [Conformalized density- and distance-based anomaly detection in time-series data](https://arxiv.org/abs/1608.04585)                                                                                           |
 | [SPOT](https://streamad.readthedocs.io/en/latest/example/univariate.html#spot-detector)                           | [streamad.model.SpotDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#spotdetector)     | [Anomaly detection in streams with extreme value theory](https://dl.acm.org/doi/10.1145/3097983.3098144)                                                                                                      |
-| [RRCF](https://streamad.readthedocs.io/en/latest/example/univariate.html#rrcf-detector)                           | [streamad.model.RrcfDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#rrcfdetector)     | [Robust random cut forest based anomaly detection on streams](http://proceedings.mlr.press/v48/guha16.pdf)                                                                                                    |
 | [Spectral Residual](https://streamad.readthedocs.io/en/latest/example/univariate.html#spectral-residual-detector) | [streamad.model.SRDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#srdetector)         | [Time-series anomaly detection service at microsoft](https://arxiv.org/abs/1906.03821)                                                                                                                        |
 | [Z score](https://streamad.readthedocs.io/en/latest/example/univariate.html#z-score-detector)                     | [streamad.model.ZScoreDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#zscoredetector) | [Standard score](https://en.wikipedia.org/wiki/Standard_score)                                                                                                                                                |
 | [One-class SVM](https://streamad.readthedocs.io/en/latest/example/univariate.html#one-class-svm-detector)         | [streamad.model.OCSVMDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#ocsvmdetector)   | [One-class SVM](https://en.wikipedia.org/w/index.php?title=One-class_classification&oldid=1098733917)                                                                                                         |
 | [MAD](https://streamad.readthedocs.io/en/latest/example/univariate.html#median-absolute-deviation-detector)       | [streamad.model.MadDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#maddetector)       | [Median absolute deviation](https://www.influxdata.com/blog/anomaly-detection-with-median-absolute-deviation/#:~:text=How%20Median%20Absolute%20Deviation%20algorithm,time%20series%20at%20that%20timestamp/) |
 | [SARIMAX](https://streamad.readthedocs.io/en/latest/example/univariate.html#seasonal-arima-detector)              | [streamad.model.SArimaDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#sarimadetector) | [Seasonal Arima Detector](https://www.statsmodels.org/dev/generated/statsmodels.tsa.statespace.sarimax.SARIMAX.html?highlight=sarimax#statsmodels.tsa.statespace.sarimax.SARIMAX)                             |
 
 ### For multivariate time series
@@ -92,7 +119,9 @@
 
 | Models Example                                                                                         | API Usage                                                                                                          | Paper                                                                                                                                                                     |
 | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [xStream](https://streamad.readthedocs.io/en/latest/example/multivariate.html#xstream-detector)        | [streamad.model.xStramDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#xstreamdetector) | [Xstream: outlier detection in feature-evolving data streams](http://www.kdd.org/kdd2018/accepted-papers/view/xstream-outlier-detection-in-feature-evolving-data-streams) |
 | [RShash](https://streamad.readthedocs.io/en/latest/example/multivariate.html#rshash-detector)          | [streamad.model.RShashDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#rshashdetector)  | [Subspace Outlier Detection in Linear Time with Randomized Hashing](https://ieeexplore.ieee.org/document/7837870)                                                         |
 | [HSTree](https://streamad.readthedocs.io/en/latest/example/multivariate.html#half-space-tree-detector) | [streamad.model.HSTreeDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#hstreedetector)  | [Fast Anomaly Detection for Streaming Data](https://www.ijcai.org/Proceedings/11/Papers/254.pdf)                                                                          |
 | [LODA](https://streamad.readthedocs.io/en/latest/example/multivariate.html#loda-detector)              | [streamad.model.LodaDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#lodadetector)      | [Lightweight on-line detector of anomalies](https://link.springer.com/article/10.1007/s10994-015-5521-0)                                                                  |
+| [RRCF](https://streamad.readthedocs.io/en/latest/example/univariate.html#rrcf-detector)                | [streamad.model.RrcfDetector](https://streamad.readthedocs.io/en/latest/api/streamad.model.html#rrcfdetector)      | [Robust random cut forest based anomaly detection on streams](http://proceedings.mlr.press/v48/guha16.pdf)                                                                |
+
```

### Comparing `streamad-0.3.0/streamad/base/detector.py` & `streamad-0.3.1/streamad/base/detector.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,36 +5,38 @@
 
 
 class BaseDetector(ABC):
     """Abstract class for Detector, supporting for customize detector."""
 
     def __init__(
         self,
-        window_len: int = 100,
+        window_len: int = 50,
         detrend: bool = False,
-        detrend_len: int = 20,
+        detrend_len: int = 10,
         data_type: str = "multivariate",
+        score_first: bool = False,
     ):
         """Initialize the attributes of the BaseDetector class
 
 
         Args:
-            window_len (int, optional): Length of window for observations. Defaults to 100.
+            window_len (int, optional): Length of window for observations. Defaults to 50.
             detrend (bool, optional): Data is detrended by subtracting the mean. Defaults to True.
-            detrend_len (int, optional): Length of data for reference to detrend. Defaults to 20.
+            detrend_len (int, optional): Length of data for reference to detrend. Defaults to 10.
             data_type (str, optional): Multi/Univariate data type. Defaults to "multivariate".
         """
 
         self.data_type = data_type
         self.index = -1
         self.detrend = detrend
         self.window_len = window_len
         self.detrend_len = detrend_len
         self.window = deque(maxlen=self.window_len)
         self.detrend_window = deque(maxlen=self.detrend_len)
+        self.score_first = score_first
 
     def _check(self, X) -> bool:
         """Check whether the detector can handle the data."""
         x_shape = X.shape[0]
 
         if self.data_type == "univariate":
             assert x_shape == 1, "The data is not univariate."
@@ -57,24 +59,22 @@
         """
 
         self.detrend_window.append(X)
 
         return X - np.mean(self.detrend_window, axis=0)
 
     @abstractmethod
-    def fit(self, X: np.ndarray):
-
+    def fit(self, X: np.ndarray, timestamp: int = None):
         return NotImplementedError
 
     @abstractmethod
-    def score(self, X: np.ndarray) -> float:
-
+    def score(self, X: np.ndarray, timestamp: int = None) -> float:
         return NotImplementedError
 
-    def fit_score(self, X: np.ndarray) -> float:
+    def fit_score(self, X: np.ndarray, timestamp: int = None) -> float:
         """Fit one observation and calculate its anomaly score.
 
         Args:
             X (np.ndarray): Data of current observation.
 
         Returns:
             float: Anomaly score. A high score indicates a high degree of anomaly.
@@ -82,13 +82,17 @@
 
         check_flag = self._check(X)
         if not check_flag:
             return None
         X = self._detrend(X) if self.detrend else X
 
         if self.index < self.window_len:
-            self.fit(X)
+            self.fit(X, timestamp)
             return None
 
-        score = self.fit(X).score(X)
+        if self.score_first:
+            score = self.score(X, timestamp)
+            self.fit(X, timestamp)
+        else:
+            score = self.fit(X, timestamp).score(X, timestamp)
 
         return float(abs(score))
```

### Comparing `streamad-0.3.0/streamad/base/metrics.py` & `streamad-0.3.1/streamad/base/metrics.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/evaluate/numenta_aware_metrics.py` & `streamad-0.3.1/streamad/evaluate/numenta_aware_metrics.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/evaluate/point_aware_metrics.py` & `streamad-0.3.1/streamad/evaluate/point_aware_metrics.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/evaluate/series_aware_metrics.py` & `streamad-0.3.1/streamad/evaluate/series_aware_metrics.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/evaluate/ts_metrics.py` & `streamad-0.3.1/streamad/evaluate/ts_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,18 +215,22 @@
                         -1, 1
                     ),
                 ]
             )
 
             real_anomalies_ = np.argwhere(values_real == 1).ravel()
             real_anomalies_shift_forward = self._shift(
-                real_anomalies_, 1, fill_value=real_anomalies_[0]
+                real_anomalies_,
+                1,
+                fill_value=real_anomalies_[0] if len(real_anomalies_) else 0,
             )
             real_anomalies_shift_backward = self._shift(
-                real_anomalies_, -1, fill_value=real_anomalies_[-1]
+                real_anomalies_,
+                -1,
+                fill_value=real_anomalies_[-1] if len(real_anomalies_) else 0,
             )
             real_anomalies_start = np.argwhere(
                 (real_anomalies_shift_forward - real_anomalies_) != -1
             ).ravel()
             real_anomalies_finish = np.argwhere(
                 (real_anomalies_ - real_anomalies_shift_backward) != -1
             ).ravel()
@@ -239,18 +243,22 @@
 
         elif self.metric_option == "numenta":
             predicted_anomalies = np.argwhere(values_pred == 1).repeat(
                 2, axis=1
             )
             real_anomalies_ = np.argwhere(values_real == 1).ravel()
             real_anomalies_shift_forward = self._shift(
-                real_anomalies_, 1, fill_value=real_anomalies_[0]
+                real_anomalies_,
+                1,
+                fill_value=real_anomalies_[0] if len(real_anomalies_) else 0,
             )
             real_anomalies_shift_backward = self._shift(
-                real_anomalies_, -1, fill_value=real_anomalies_[-1]
+                real_anomalies_,
+                -1,
+                fill_value=real_anomalies_[-1] if len(real_anomalies_) else 0,
             )
             real_anomalies_start = np.argwhere(
                 (real_anomalies_shift_forward - real_anomalies_) != -1
             ).ravel()
             real_anomalies_finish = np.argwhere(
                 (real_anomalies_ - real_anomalies_shift_backward) != -1
             ).ravel()
```

### Comparing `streamad-0.3.0/streamad/model/KNN_Detector.py` & `streamad-0.3.1/streamad/model/KNN_Detector.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
         assert (
             k_neighbor < self.buffer.maxlen
         ), "k_neighbor must be less than the length of buffer"
 
         self.k = k_neighbor
 
-    def fit(self, X: np.ndarray):
+    def fit(self, X: np.ndarray, timestamp: int = None):
 
         self.window.append(X[0])
 
         if len(self.window) == self.window.maxlen:
             self.buffer.append(deepcopy(self.window))
 
         return self
 
-    def score(self, X) -> float:
+    def score(self, X: np.ndarray, timestamp: int = None) -> float:
 
         window = deepcopy(self.window)
         window.pop()
         window.append(X[0])
 
         try:
             dist = cdist(np.array([window]), self.buffer, metric="mahalanobis")[
```

### Comparing `streamad-0.3.0/streamad/model/Mad_Dectector.py` & `streamad-0.3.1/streamad/model/Mad_Dectector.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 
 
 class MadDetector(BaseDetector):
     def __init__(self, **kwargs):
         """Median Absolute Deviation Detector :cite: `InfluxDB:MAD`.
 
         Args:
-            window_len (int, optional): Length of sliding window. Defaults to 10.
+            window_len (int, optional): Length of sliding window. Defaults to 50.
             threshold (float, optional): threshold to decide a anomaly data. Defaults to 3.0.
 
         parameters:
             scale_factor : Multiple relationship between standard deviation and absolute median difference under normal distribution.
 
         """
         super().__init__(data_type="univariate", **kwargs)
         self.scale_factor = 1.4826
 
-    def fit(self, X: np.ndarray) -> None:
+    def fit(self, X: np.ndarray, timestamp: int = None):
         self.window.append(X[0])
 
         return self
 
-    def score(self, X: np.ndarray) -> float:
-
+    def score(self, X: np.ndarray, timestamp: int = None):
         ori_median = np.median(self.window)
         abs_diff = np.abs(self.window - ori_median)
         mad = self.scale_factor * np.median(abs_diff)
         score = np.divide(
             abs_diff[-1], mad, out=np.array(abs_diff[-1] / 1e-5), where=mad != 0
         )
```

### Comparing `streamad-0.3.0/streamad/model/OCSVM_Detector.py` & `streamad-0.3.1/streamad/model/OCSVM_Detector.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,22 +21,22 @@
             kernel (str, optional): The kernel type to be used in the algorithm. Defaults to "rbf".
         """
         super().__init__(data_type="multivariate", **kwargs)
         self.nu = nu
         self.kernel = kernel
         self.model = None
 
-    def fit(self, X: np.ndarray):
+    def fit(self, X: np.ndarray, timestamp: int = None):
 
         self.window.append(X)
         if self.index >= self.window_len:
             self.model = OneClassSVM(
                 gamma="scale", nu=self.nu, kernel=self.kernel
             )
             self.model.fit(list(self.window))
 
         return self
 
-    def score(self, X: np.ndarray) -> float:
+    def score(self, X: np.ndarray, timestamp: int = None):
 
         score = self.model.decision_function(X.reshape(1, -1))
         return abs(score)
```

### Comparing `streamad-0.3.0/streamad/model/SArima_Detector.py` & `streamad-0.3.1/streamad/model/SArima_Detector.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 
 class SArimaDetector(BaseDetector):
     def __init__(self, **kwargs):
         """Auto Regressive Integrated Moving Averages Detector :cite:`durbin2012time`
 
         Args:
-            window_len (int, optional): Length of sliding window. Defaults to 200.
+            window_len (int, optional): Length of sliding window. Defaults to 50.
         """
         super().__init__(data_type="univariate", **kwargs)
         self.best_result = None
         self.best_model = None
         self.best_order = None
         self.best_seasonal_order = None
 
     def _init_fit(self):
-
         best_aic = float("inf")
         p = d = q = range(0, 2)
         pdq = list(itertools.product(p, d, q))
         seasonal_pdq = [
             (x[0], x[1], x[2], 12) for x in list(itertools.product(p, d, q))
         ]
         for param in pdq:
@@ -44,27 +43,25 @@
                     self.best_model = model
                     best_aic = aic
                     self.best_order = param
                     self.best_seasonal_order = param_seasonal
 
         self.best_result = self.best_model.fit(disp=0)
 
-    def fit(self, X: np.ndarray) -> None:
-
+    def fit(self, X: np.ndarray, timestamp: int = None):
         self.window.append(X[0])
         if self.index == self.window_len:
             self._init_fit()
 
         if self.index > self.window_len:
             self.best_result = self.best_result.append(X)
 
         return self
 
-    def score(self, X: np.ndarray) -> float:
-
+    def score(self, X: np.ndarray, timestamp: int = None):
         pred_uc = self.best_result.get_forecast(steps=1)
 
         pred_ci = pred_uc.conf_int()
         pred_mid = (pred_ci[0, 0] + pred_ci[0, 1]) / 2
         pred_range = pred_ci[0, 1] - pred_ci[0, 0]
 
         if pred_ci[0, 0] > X:
```

### Comparing `streamad-0.3.0/streamad/model/SR_Detector.py` & `streamad-0.3.1/streamad/model/SR_Detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,63 +13,60 @@
         ahead_len: int = 10,
         mag_num: int = 5,
         **kwargs
     ):
         """Spectral Residual Detector :cite:`DBLP:conf/kdd/RenXWYHKXYTZ19`.
 
         Args:
-            window_len (int, optional): Length of sliding window. Defaults to 100.
+            window_len (int, optional): Length of sliding window. Defaults to 50.
             extend_len (int, optional): Length to be extended, for FFT transforme. Defaults to 5.
             ahead_len (int, optional): Length to look ahead for references. Defaults to 10.
             mag_num (int, optional): Number of FFT magnitude. Defaults to 5.
         """
         super().__init__(data_type="univariate", **kwargs)
         self.extend_len = extend_len
         assert ahead_len > 1, "ahead_len must be greater than 1"
         self.ahead_len = ahead_len
         self.mag_num = mag_num
 
-    def fit(self, X):
+    def fit(self, X: np.ndarray, timestamp: int = None):
         self.window.append(X[0])
 
         return self
 
-    def score(self, X):
-
+    def score(self, X: np.ndarray, timestamp: int = None) -> float:
         window = deepcopy(self.window)
 
         window.pop()
         window.append(X[0])
 
         extended_window = self._extend_window(window)
 
         mags = self._sr_transform(extended_window)
         anomaly_scores = self._spectral_score(mags)
 
         return anomaly_scores[-1 - self.extend_len]
 
     def _spectral_score(self, mags):
-
         avg_mag = self._average_filter(mags, n=self.mag_num * 10)
         safeDivisors = np.clip(avg_mag, EPS, avg_mag.max())
 
         raw_scores = np.divide(
             np.abs(mags - avg_mag),
             safeDivisors,
             out=np.zeros_like(mags),
             where=safeDivisors != 0,
         )
         scores = np.clip(raw_scores / 10.0, 0, 1.0)
 
         return scores
 
     def _sr_transform(self, window):
-
         trans = np.fft.fft(window)
-        mag = np.sqrt(trans.real ** 2 + trans.imag ** 2)
+        mag = np.sqrt(trans.real**2 + trans.imag**2)
         eps_index = np.where(mag <= EPS)[0]
         mag[eps_index] = EPS
 
         mag_log = np.log(mag)
         mag_log[eps_index] = 0
 
         spectral = np.exp(
@@ -80,15 +77,15 @@
         trans.imag = trans.imag * spectral / mag
 
         trans.real[eps_index] = 0
         trans.imag[eps_index] = 0
 
         wave_r = np.fft.ifft(trans)
 
-        mag = np.sqrt(wave_r.real ** 2, wave_r.imag ** 2)
+        mag = np.sqrt(wave_r.real**2, wave_r.imag**2)
 
         return mag
 
     def _average_filter(self, values, n=3):
         if n >= len(values):
             n = len(values)
 
@@ -98,25 +95,23 @@
 
         for i in range(1, n):
             res[i] /= i + 1
 
         return res
 
     def _extend_window(self, window):
-
         predicted_window = [
             self._predict_next(list(window)[-self.ahead_len : -1])
         ] * self.extend_len
 
         extended_window = np.concatenate((window, predicted_window), axis=0)
 
         return extended_window
 
     def _predict_next(self, ahead_window):
-
         assert (
             len(ahead_window) > 1
         ), "ahead window must have at least 2 elements"
 
         ele_last = ahead_window[-1]
         n = len(ahead_window)
```

### Comparing `streamad-0.3.0/streamad/model/__init__.py` & `streamad-0.3.1/streamad/model/__init__.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/model/hstree_Detector.py` & `streamad-0.3.1/streamad/model/hstree_Detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import numpy as np
 from streamad.base import BaseDetector
 from streamad.util import StreamStatistic
 
 
 class Leaf:
     def __init__(
-        self, left=None, right=None, depth=0,
+        self,
+        left=None,
+        right=None,
+        depth=0,
     ):
         self.left = left
         self.right = right
         self.r = 0
         self.l = 0
         self.split_attrib = 0
         self.split_value = 0.0
         self.k = depth
 
 
 class HSTreeDetector(BaseDetector):
-    def __init__(self, tree_height: int = 10, tree_num: int = 100, **kwargs):
+    def __init__(self, tree_height: int = 10, tree_num: int = 20, **kwargs):
         """Half space tree detectors. :cite:`DBLP:conf/ijcai/TanTL11`.
 
         Args:
             tree_height (int, optional): Height of a half space tree. Defaults to 10.
-            tree_num (int, optional): Totla number of the trees. Defaults to 100.
+            tree_num (int, optional): Totla number of the trees. Defaults to 20.
         """
         super().__init__(data_type="multivariate", **kwargs)
         self.tree_height = tree_height
         self.tree_num = tree_num
         self.forest = []
         self.data_stats = StreamStatistic()
 
@@ -77,23 +80,23 @@
     def _reset_tree(self, tree):
         if tree:
             tree.r = tree.l
             tree.l = 0
             self._reset_tree(tree.left)
             self._reset_tree(tree.right)
 
-    def fit(self, X: np.ndarray) -> None:
-
+    def fit(self, X: np.ndarray, timestamp: int = None):
         self.data_stats.update(X)
 
         X_normalized = np.divide(
             X - self.data_stats.get_min(),
             self.data_stats.get_max() - self.data_stats.get_min(),
-            out=np.zeros_like(X),
+            out=np.zeros_like(X, dtype=float),
             where=self.data_stats.get_max() - self.data_stats.get_min() != 0,
+            dtype=float,
         )
         X_normalized[np.abs(X_normalized) == np.inf] = 0
 
         if self.dimensions is None:
             self.dimensions = len(X)
             for _ in range(self.tree_num):
                 max_arr, min_arr = self._generate_max_min()
@@ -109,22 +112,21 @@
                     self._reset_tree(tree)
 
             for tree in self.forest:
                 self._update_tree_mass(tree, X_normalized, False)
 
         return self
 
-    def score(self, X: np.ndarray) -> float:
-
+    def score(self, X: np.ndarray, timestamp: int = None) -> float:
         score = 0.0
 
         X_normalized = np.divide(
             X - self.data_stats.get_min(),
             self.data_stats.get_max() - self.data_stats.get_min(),
-            out=np.zeros_like(X),
+            out=np.zeros_like(X, dtype=float),
             where=self.data_stats.get_max() - self.data_stats.get_min() != 0,
         )
         X_normalized[np.abs(X_normalized) == np.inf] = 0
 
         for tree in self.forest:
             score += self._score_tree(tree, X_normalized, 0)
 
@@ -133,15 +135,15 @@
         return float(score)
 
     def _score_tree(self, tree, X, k):
         s = 0
         if not tree:
             return s
 
-        s += tree.r * (2 ** k)
+        s += tree.r * (2**k)
 
         if X[tree.split_attrib] > tree.split_value:
             tree_new = tree.right
         else:
             tree_new = tree.left
 
         s += self._score_tree(tree_new, X, k + 1)
```

### Comparing `streamad-0.3.0/streamad/model/rshash_Detector.py` & `streamad-0.3.1/streamad/model/rshash_Detector.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from streamad.base import BaseDetector
 from streamad.util import StreamStatistic
 from collections import deque
 
 
 class RShashDetector(BaseDetector):
     def __init__(
-        self, decay=0.015, components_num=100, hash_num: int = 10, **kwargs
+        self, decay=0.015, components_num=10, hash_num: int = 10, **kwargs
     ):
         """Multivariate RSHashDetector :cite:`DBLP:conf/icdm/SatheA16`.
 
         Args:
-            window_len (int, optional): Length of data to burn in/init. Defaults to 150.
+            window_len (int, optional): Length of data to burn in/init. Defaults to 50.
             decay (float, optional): Decay ratio. Defaults to 0.015.
-            components_num (int, optional): Number of components. Defaults to 100.
+            components_num (int, optional): Number of components. Defaults to 10.
             hash_num (int, optional): Number of hash functions. Defaults to 10.
         """
         super().__init__(data_type="multivariate", **kwargs)
 
         self.decay = decay
         self.data_stats = StreamStatistic()
 
@@ -31,46 +31,45 @@
         self.f = np.random.uniform(
             low=1.0 / np.sqrt(self.effective_s),
             high=1 - (1.0 / np.sqrt(self.effective_s)),
             size=self.components_num,
         )
 
     def _burn_in(self):
-
         # Normalized the init data
         buffer = np.array(self.window)
         buffer_normalized = np.divide(
             buffer - self.data_stats.get_min(),
             self.data_stats.get_max() - self.data_stats.get_min(),
-            out=np.zeros_like(buffer),
+            out=np.zeros_like(buffer).astype(float),
             where=self.data_stats.get_max() - self.data_stats.get_min() != 0,
         )
         buffer_normalized[np.abs(buffer_normalized) == np.inf] = 0
 
         for r in range(self.components_num):
             for i in range(buffer.shape[0]):
                 Y = np.floor(
                     (buffer_normalized[i, :] + np.array(self.alpha[r]))
                     / self.f[r]
                 )
 
-                mod_entry = np.insert(Y, 0, r)
+                # mod_entry = np.insert(Y, 0, r)
+                mod_entry = np.concatenate(([r], Y))
                 mod_entry = tuple(mod_entry.astype(int))
 
                 for w in range(self.hash_num):
                     try:
                         value = self.cmsketches[w][mod_entry]
                     except KeyError:
                         value = (0, 0)
 
                     value = (0, value[1] + 1)
                     self.cmsketches[w][mod_entry] = value
 
-    def fit(self, X):
-
+    def fit(self, X: np.ndarray, timestamp: int = None):
         if self.index == 0:
             self.alpha = [
                 np.random.uniform(low=0, high=self.f[r], size=len(X))
                 for r in range(self.components_num)
             ]
 
         self.data_stats.update(X)
@@ -80,29 +79,29 @@
 
         if len(self.window) < self.window.maxlen:
             self.window.append(X)
             return self
 
         return self
 
-    def score(self, X):
-
+    def score(self, X: np.ndarray, timestamp: int = None) -> float:
         X_normalized = np.divide(
             X - self.data_stats.get_min(),
             self.data_stats.get_max() - self.data_stats.get_min(),
-            out=np.zeros_like(X),
+            out=np.zeros_like(X).astype(float),
             where=self.data_stats.get_max() - self.data_stats.get_min() != 0,
         )
         X_normalized[np.abs(X_normalized) == np.inf] = 0
 
         score_instance = 0
 
         for r in range(self.components_num):
             Y = np.floor((X_normalized + np.array(self.alpha[r])) / self.f[r])
-            mod_entry = np.insert(Y, 0, r)
+            # mod_entry = np.insert(Y, 0, r)
+            mod_entry = np.concatenate(([r], Y))
             mod_entry = tuple(mod_entry.astype(int))
 
             c = []
 
             for w in range(len(self.cmsketches)):
                 try:
                     value = self.cmsketches[w][mod_entry]
```

### Comparing `streamad-0.3.0/streamad/model/spot_Detector.py` & `streamad-0.3.1/streamad/model/spot_Detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,15 +232,14 @@
             )
         else:
             L = n * (1 + log(abs(Y.mean()) + 1e-8))
 
         return L
 
     def _quantile(self, side, gamma, sigma):
-
         if side == "up":
             r = self.window_len * self.prob / self.num_threshold[side]
             # r = 1000 * self.prob
 
             if gamma != 0:
                 return self.init_threshold["up"] + (sigma / gamma) * (
                     pow(r, -gamma) - 1
@@ -257,22 +256,20 @@
                 )
             else:
                 return self.init_threshold["down"] + sigma * log(r)
         else:
             raise ValueError("The side is not right")
 
     def _init_drift(self, verbose=False):
-
         for side in ["up", "down"]:
             self._update_one_side(side)
 
         return self
 
     def _update_one_side(self, side: str):
-
         if side == "up":
             candidates = (
                 list(self.window) + self.history_peaks[side]
                 if self.global_memory
                 else list(self.window)
             )
 
@@ -312,28 +309,27 @@
             np.mean(self.back_mean_window)
             if self.back_mean_window.maxlen > 0
             else np.array(0.0)
         )
 
         return X - back_mean
 
-    def fit(self, X: np.ndarray):
+    def fit(self, X: np.ndarray, timestamp: int = None):
         X = float(X[0])
 
         self.back_mean_window.append(X)
 
         if self.index >= self.back_mean_len:
             self.normal_X = self._cal_back_mean(X)
             self.window.append(self.normal_X)
 
         if self.index == self.window_len:
             self._init_drift()
 
         if self.index >= self.window_len:
-
             last_X = (
                 self.window[-2]
                 if self.back_mean_len == 0
                 else (X - self.window[-1])
             )
 
             if (
@@ -346,23 +342,24 @@
             ):
                 return self
 
             if self.normal_X > self.init_threshold["up"]:
                 self._update_one_side("up")
 
             elif self.normal_X < self.init_threshold["down"]:
-
                 self._update_one_side("down")
 
         return self
 
-    def score(self, X: np.ndarray) -> float:
-
+    def score(self, X: np.ndarray, timestamp: int = None):
         X = float(X[0])
 
+        # if self.score_first:
+        #     last_X = self._cal_back_mean(X)
+        # else:
         last_X = (
             self.window[-2]
             if self.back_mean_len == 0
             else (X - self.window[-1])
         )
 
         if (
```

### Comparing `streamad-0.3.0/streamad/model/xStream_Detector.py` & `streamad-0.3.1/streamad/model/xStream_Detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 from streamad.base import BaseDetector
 import numpy as np
 import mmh3
+from math import floor
 
 
 class xStreamDetector(BaseDetector):
     def __init__(
         self,
-        n_components: int = 50,
-        n_chains: int = 50,
-        depth: int = 25,
-        **kwargs
+        n_components: int = 8,
+        n_chains: int = 8,
+        depth: int = 8,
+        **kwargs,
     ):
         """Multivariate xStreamDetector :cite:`DBLP:conf/kdd/ManzoorLA18`.
 
         Args:
             n_components (int, optional): Number of streamhash projection, similar to feature numbers. Defaults to 50.
-            n_chains (int, optional): Number of half-space chains. Defaults to 100.
-            depth (int, optional): Maximum depth for each chain. Defaults to 25.
+            n_chains (int, optional): Number of half-space chains. Defaults to 8.
+            depth (int, optional): Maximum depth for each chain. Defaults to 8.
         """
 
         super().__init__(data_type="multivariate", **kwargs)
         self.projector = StreamhashProjector(
             num_components=n_components, density=1 / 3.0
         )
         self.cur_window = []
         self.ref_window = []
 
         delta = np.ones(n_components) * 0.5
         self.hs_chains = _hsChains(
             deltamax=delta, n_chains=n_chains, depth=depth
         )
 
-    def fit(self, X: np.ndarray):
-
+    def fit(self, X: np.ndarray, timestamp: int = None):
         projected_X = self.projector.transform(X)
         self.cur_window.append(projected_X)
         self.hs_chains.fit(projected_X)
 
         self.ref_window = self.cur_window
         self.cur_window = []
 
         deltamax = np.ptp(self.ref_window, axis=0) / 2.0
         deltamax[np.abs(deltamax) <= 0.0001] = 1.0
 
         self.hs_chains.set_deltamax(deltamax=deltamax)
-        self.hs_chains.next_window()
 
         return self
 
-    def score(self, X: np.ndarray) -> float:
-
+    def score(self, X: np.ndarray, timestamp: int = None):
         projected_X = self.projector.transform(X)
 
         score = -1.0 * self.hs_chains.score_chains(projected_X)
 
         return score
 
 
 class _Chain:
     def __init__(self, deltamax, depth):
-
         self.depth = depth
         self.deltamax = deltamax
         self.rand = np.random.rand(len(deltamax))
         self.rand_shift = self.rand * deltamax
         self.cmsketch_ref = [{} for _ in range(depth)] * depth
-        self.cmsketch_cur = [{} for _ in range(depth)] * depth
         self.is_first_window = True
         self.fs = [np.random.randint(0, len(deltamax)) for _ in range(depth)]
 
-    def bincount(self, X):
+    @staticmethod
+    def float_to_int(x):
+        return x // 1
 
+    def bincount(self, X):
         scores = np.zeros(self.depth)
         prebins = np.zeros(X.shape[0], dtype=float)
         depthcount = np.zeros(len(self.deltamax), dtype=int)
         for depth in range(self.depth):
             f = self.fs[depth]
             depthcount[f] += 1
             if depthcount[f] == 1:
@@ -82,112 +81,98 @@
             else:
                 prebins[f] = (
                     2.0 * prebins[f] - self.rand_shift[f] / self.deltamax[f]
                 )
 
             cmsketch = self.cmsketch_ref[depth]
 
-            for prebin in prebins:
+            l = tuple(map(floor, prebins))
 
-                l = int(prebin)
-                if l in cmsketch:
-                    scores[depth] = cmsketch[l]
-                else:
-                    scores[depth] = 0.0
+            if l in cmsketch:
+                scores[depth] = cmsketch[l]
+            else:
+                scores[depth] = 0.0
 
         return scores
 
     def score(self, X):
-
         scores = self.bincount(X)
 
         depths = np.arange(1, self.depth + 1)
 
         scores = np.log2(1.0 + scores) + depths
         return np.min(scores)
 
     def fit(self, X):
-
         prebins = np.zeros(X.shape, dtype=float)
         depthcount = np.zeros(len(self.deltamax), dtype=int)
         for depth in range(self.depth):
             f = self.fs[depth]
             depthcount[f] += 1
 
             if depthcount[f] == 1:
                 prebins[f] = (X[f] + self.rand_shift[f]) / self.deltamax[f]
             else:
                 prebins[f] = (
                     2.0 * prebins[f] - self.rand_shift[f] / self.deltamax[f]
                 )
 
             if self.is_first_window:
-
                 cmsketch = self.cmsketch_ref[depth]
-                for prebin in prebins:
 
-                    l = int(prebin)
+                l = tuple(map(floor, prebins))
 
-                    if l not in cmsketch:
-                        cmsketch[l] = 0
-                    cmsketch[l] += 1
+                if l not in cmsketch:
+                    cmsketch[l] = 0
+                cmsketch[l] += 1
 
                 self.cmsketch_ref[depth] = cmsketch
-                self.cmsketch_cur[depth] = cmsketch
             else:
-                cmsketch = self.cmsketch_cur[depth]
-                for prebin in prebins:
-                    l = int(prebin)
-
-                    if l not in cmsketch:
-                        cmsketch[l] = 0
-                    cmsketch[l] += 1
-                self.cmsketch_cur[depth] = cmsketch
+                cmsketch = self.cmsketch_ref[depth]
 
-        return self
+                l = tuple(map(floor, prebins))
 
-    def next_window(self):
-        self.is_first_window = False
-        self.cmsketch_ref = self.cmsketch_cur
-        self.cmsketch_cur = [{} for _ in range(self.depth)] * self.depth
+                if l not in cmsketch:
+                    cmsketch[l] = 0
+                cmsketch[l] += 1
+                self.cmsketch_ref[depth] = cmsketch
+
+        return self
 
 
 class _hsChains:
     def __init__(self, deltamax, n_chains: int = 100, depth: int = 25) -> None:
         self.nchains = n_chains
         self.depth = depth
         self.chains = [_Chain(deltamax, depth) for _ in range(n_chains)]
 
     def score_chains(self, X):
-
         scores = 0
         for chain in self.chains:
             scores += chain.score(X)
 
         scores = float(scores) / float(self.nchains)
 
         return scores
 
     def fit(self, X):
-        for chain in self.chains:
-            chain.fit(X)
-
-    def next_window(self):
-        for chain in self.chains:
-            chain.next_window()
+        # for chain in self.chains:
+        #     chain.fit(X)
+        list(map(lambda x: x.fit(X), self.chains))
 
     def set_deltamax(self, deltamax):
+        # list(map(lambda x: x.deltamax = deltamax, self.chains))
+        # list(map(lambda x: x.rand_shift = x.rand * deltamax, self.chains))
         for chain in self.chains:
             chain.deltamax = deltamax
             chain.rand_shift = chain.rand * deltamax
 
 
 class StreamhashProjector:
     def __init__(self, num_components, density=1 / 3.0):
-
         self.keys = np.arange(0, num_components, 1)
         self.constant = np.sqrt(1.0 / density) / np.sqrt(num_components)
         self.density = density
         self.n_components = num_components
 
     def transform(self, X):
         """Projects particular (next) timestep's vector to (possibly) lower dimensional space.
@@ -210,16 +195,37 @@
         )
 
         Y = np.dot(X, R.T).squeeze()
 
         return Y
 
     def _hash_string(self, k, s):
-
-        hash_value = int(mmh3.hash(s, signed=False, seed=k)) / (2.0 ** 32 - 1)
+        hash_value = int(mmh3.hash(s, signed=False, seed=k)) / (2.0**32 - 1)
         s = self.density
         if hash_value <= s / 2.0:
             return -1 * self.constant
         elif hash_value <= s:
             return self.constant
         else:
             return 0
+
+
+if __name__ == "__main__":
+    import cProfile
+    from line_profiler import LineProfiler
+
+    lp = LineProfiler()
+
+    model = xStreamDetector()
+
+    lp.add_function(_Chain.fit)
+    lp.add_function(_Chain.score)
+    lp.add_function(_Chain.bincount)
+    # lp.add_function(model.fit)
+    # lp.add_function(model.score)
+    lp_wrapper = lp(model.fit_score)
+
+    for i in range(1500):
+        # lp_wrapper(np.array([i]))
+        model.fit_score(np.array([i]))
+
+    lp.print_stats()
```

### Comparing `streamad-0.3.0/streamad/model/zscore_Detector.py` & `streamad-0.3.1/streamad/model/zscore_Detector.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 
 
 class ZScoreDetector(BaseDetector):
     def __init__(self, is_global: bool = False, **kwargs):
         """Univariate Z-Score Detecto :cite:`enwiki:1086685336`
 
         Args:
-            window_len (int, optional):  Length of the window for reference. Defaults to 100.
+            window_len (int, optional):  Length of the window for reference. Defaults to 50.
             is_global (bool, optional): Whether to detect anomalies from a global view. Defaults to False.
         """
         super().__init__(data_type="univariate", **kwargs)
 
         self.stat = StreamStatistic(
             is_global=is_global, window_len=self.window_len
         )
 
-    def fit(self, X: np.ndarray):
+    def fit(self, X: np.ndarray, timestamp: int = None):
         self.stat.update(X[0])
         return self
 
-    def score(self, X: np.ndarray):
-
+    def score(self, X: np.ndarray, timestamp: int = None):
         mean = self.stat.get_mean()
         std = self.stat.get_std()
 
         score = np.divide(
             (X[0] - mean), std, out=np.zeros_like(X[0]), where=std != 0
         )
```

### Comparing `streamad-0.3.0/streamad/process/tdigest_calibrator.py` & `streamad-0.3.1/streamad/process/tdigest_calibrator.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/process/vote_ensemble.py` & `streamad-0.3.1/streamad/process/vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/process/weight_ensemble.py` & `streamad-0.3.1/streamad/process/weight_ensemble.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/process/zscore_calibrator.py` & `streamad-0.3.1/streamad/process/zscore_calibrator.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/util/dataset.py` & `streamad-0.3.1/streamad/util/dataset.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/util/math_toolkit.py` & `streamad-0.3.1/streamad/util/math_toolkit.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/util/plot.py` & `streamad-0.3.1/streamad/util/plot.py`

 * *Files identical despite different names*

### Comparing `streamad-0.3.0/streamad/util/stream_generator.py` & `streamad-0.3.1/streamad/util/stream_generator.py`

 * *Files identical despite different names*


# Comparing `tmp/graphomaly-0.2.8.tar.gz` & `tmp/graphomaly-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphomaly-0.2.8.tar", last modified: Fri Apr 14 14:03:41 2023, max compression
+gzip compressed data, was "graphomaly-0.3.tar", last modified: Thu May 11 18:14:46 2023, max compression
```

## Comparing `graphomaly-0.2.8.tar` & `graphomaly-0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.746382 graphomaly-0.2.8/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      718 2021-10-11 19:50:38.000000 graphomaly-0.2.8/LICENSE
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-14 14:03:41.746382 graphomaly-0.2.8/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1955 2022-05-03 07:20:54.000000 graphomaly-0.2.8/README.md
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.739715 graphomaly-0.2.8/graphomaly/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       43 2022-03-01 20:47:00.000000 graphomaly-0.2.8/graphomaly/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    31674 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/estimator.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25465 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/grid_search.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.743048 graphomaly-0.2.8/graphomaly/models/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       46 2022-02-27 21:19:37.000000 graphomaly-0.2.8/graphomaly/models/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    24065 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/models/autoencoder.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2684 2022-02-27 21:07:58.000000 graphomaly-0.2.8/graphomaly/models/base_model.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7950 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/models/dictlearn.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7111 2022-05-03 07:25:03.000000 graphomaly-0.2.8/graphomaly/models/models.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      731 2022-02-27 21:06:44.000000 graphomaly-0.2.8/graphomaly/models/sklearn.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    26574 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/models/vae.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4813 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/normalizations.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.743048 graphomaly-0.2.8/graphomaly/preprocessing/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-02-27 22:16:17.000000 graphomaly-0.2.8/graphomaly/preprocessing/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8556 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/egonet.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.743048 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4642 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/historical_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    18634 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/statistical_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12728 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/time_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5112 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_difference_transformer.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8427 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_statistical_transformer.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9538 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_time_transformers.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    33228 2022-09-27 19:49:32.000000 graphomaly-0.2.8/graphomaly/preprocessing/graph_to_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9095 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/graph_to_spectrum_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7204 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/rwalk.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6850 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/spectrum.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6129 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/preprocessing/transactions_to_graph.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    36401 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/voting.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.746382 graphomaly-0.2.8/graphomaly.egg-info/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1494 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/SOURCES.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/dependency_links.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      176 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/requires.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       11 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/top_level.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       99 2021-10-11 19:50:38.000000 graphomaly-0.2.8/pyproject.toml
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1188 2023-04-14 14:03:41.746382 graphomaly-0.2.8/setup.cfg
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.746382 graphomaly-0.2.8/tests/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1619 2022-03-31 19:27:11.000000 graphomaly-0.2.8/tests/test_dl.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1501 2022-05-03 07:20:54.000000 graphomaly-0.2.8/tests/test_fe_time.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1991 2022-04-02 17:39:48.000000 graphomaly-0.2.8/tests/test_graphomaly_ctor.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1035 2022-04-02 17:24:08.000000 graphomaly-0.2.8/tests/test_synthetic.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1023 2022-04-02 17:10:58.000000 graphomaly-0.2.8/tests/test_synthetic_gridsearch.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3264 2022-05-03 07:20:54.000000 graphomaly-0.2.8/tests/test_synthetic_preprocessing.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1084 2022-04-02 15:48:52.000000 graphomaly-0.2.8/tests/test_synthetic_voting.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1722 2022-03-15 18:50:57.000000 graphomaly-0.2.8/tests/test_tf_save.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1535 2022-03-01 23:27:25.000000 graphomaly-0.2.8/tests/test_voting.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.228444 graphomaly-0.3/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      718 2021-10-11 19:50:38.000000 graphomaly-0.3/LICENSE
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3154 2023-05-11 18:14:46.228444 graphomaly-0.3/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2367 2023-05-11 17:56:03.000000 graphomaly-0.3/README.md
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.225110 graphomaly-0.3/graphomaly/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       43 2022-03-01 20:47:00.000000 graphomaly-0.3/graphomaly/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    34446 2023-05-11 17:44:22.000000 graphomaly-0.3/graphomaly/estimator.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25465 2023-04-12 14:59:15.000000 graphomaly-0.3/graphomaly/grid_search.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.225110 graphomaly-0.3/graphomaly/models/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       46 2022-02-27 21:19:37.000000 graphomaly-0.3/graphomaly/models/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    24282 2023-05-07 13:02:29.000000 graphomaly-0.3/graphomaly/models/autoencoder.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2684 2022-02-27 21:07:58.000000 graphomaly-0.3/graphomaly/models/base_model.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7950 2023-04-12 14:59:15.000000 graphomaly-0.3/graphomaly/models/dictlearn.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7111 2022-05-03 07:25:03.000000 graphomaly-0.3/graphomaly/models/models.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      731 2022-02-27 21:06:44.000000 graphomaly-0.3/graphomaly/models/sklearn.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    26884 2023-05-07 13:02:29.000000 graphomaly-0.3/graphomaly/models/vae.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4813 2023-04-12 14:59:15.000000 graphomaly-0.3/graphomaly/normalizations.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.225110 graphomaly-0.3/graphomaly/preprocessing/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-02-27 22:16:17.000000 graphomaly-0.3/graphomaly/preprocessing/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8556 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/egonet.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.225110 graphomaly-0.3/graphomaly/preprocessing/fe_base/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_base/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4642 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_base/historical_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    18634 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_base/statistical_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12728 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_base/time_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5112 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_difference_transformer.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8427 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_statistical_transformer.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9538 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/fe_time_transformers.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    34054 2023-05-07 13:02:29.000000 graphomaly-0.3/graphomaly/preprocessing/graph_to_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9095 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/graph_to_spectrum_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7204 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/rwalk.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6850 2022-05-03 07:20:54.000000 graphomaly-0.3/graphomaly/preprocessing/spectrum.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6129 2023-04-12 14:59:15.000000 graphomaly-0.3/graphomaly/preprocessing/transactions_to_graph.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    37278 2023-05-11 17:44:22.000000 graphomaly-0.3/graphomaly/voting.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.225110 graphomaly-0.3/graphomaly.egg-info/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3154 2023-05-11 18:14:46.000000 graphomaly-0.3/graphomaly.egg-info/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1494 2023-05-11 18:14:46.000000 graphomaly-0.3/graphomaly.egg-info/SOURCES.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2023-05-11 18:14:46.000000 graphomaly-0.3/graphomaly.egg-info/dependency_links.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      176 2023-05-11 18:14:46.000000 graphomaly-0.3/graphomaly.egg-info/requires.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       11 2023-05-11 18:14:46.000000 graphomaly-0.3/graphomaly.egg-info/top_level.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       99 2021-10-11 19:50:38.000000 graphomaly-0.3/pyproject.toml
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1262 2023-05-11 18:14:46.228444 graphomaly-0.3/setup.cfg
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-05-11 18:14:46.228444 graphomaly-0.3/tests/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1619 2022-03-31 19:27:11.000000 graphomaly-0.3/tests/test_dl.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1501 2022-05-03 07:20:54.000000 graphomaly-0.3/tests/test_fe_time.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1991 2022-04-02 17:39:48.000000 graphomaly-0.3/tests/test_graphomaly_ctor.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1035 2022-04-02 17:24:08.000000 graphomaly-0.3/tests/test_synthetic.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1023 2022-04-02 17:10:58.000000 graphomaly-0.3/tests/test_synthetic_gridsearch.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3264 2022-05-03 07:20:54.000000 graphomaly-0.3/tests/test_synthetic_preprocessing.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1084 2022-04-02 15:48:52.000000 graphomaly-0.3/tests/test_synthetic_voting.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1722 2022-03-15 18:50:57.000000 graphomaly-0.3/tests/test_tf_save.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1535 2022-03-01 23:27:25.000000 graphomaly-0.3/tests/test_voting.py
```

### Comparing `graphomaly-0.2.8/LICENSE` & `graphomaly-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/PKG-INFO` & `graphomaly-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: graphomaly
-Version: 0.2.8
-Summary: software package for anomaly detection in graphs modeling financial transactions
+Version: 0.3
+Summary: Anomaly detection in graphs modeling financial transactions and computer networks.
 Home-page: https://gitlab.com/unibuc/graphomaly/graphomaly
-Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
+Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu, Nicolae Cleju, Andrei Iulian Hîji
 Author-email: graphomaly@fmi.unibuc.ro
 Project-URL: Bug Tracker, https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
-Keywords: anomaly detection,graphs,financial transactions,machine learning,security
+Keywords: anomaly detection,graphs,financial transactions,computer networks,abnormal behavior,machine learning,security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Graphomaly
 
-The Anti-Money Laundering (AML) tool. Find abnormal data in graph and network structures.
+Automatic tool for Anti-Money Laundering (AML) and  detecting abnormal behavior in computer networks. Find abnormal data in graph and network structures.
 
 Official package documentation [here](https://unibuc.gitlab.io/graphomaly/graphomaly/).
 
-This work was supported by the [Graphomaly Research Grant](http://graphomaly.upb.ro/).
+This work was initially supported by the [Graphomaly Research Grant](http://graphomaly.upb.ro/) and later partially supported by the [Netalert Research Grant](https://cs.unibuc.ro/~pirofti/netalert.html).
 
 ## Installation and setup
 Install via pip from the [PyPi repository](https://pypi.org/project/graphomaly/):
 ```
 pip install graphomaly
 ```
 
 or for the latest changes not yet in the official release:
 ```
 pip install git+https://gitlab.com/unibuc/graphomaly/graphomaly
 ```
 
+Install via docker from the [DockerHub repository](https://hub.docker.com/r/pirofti/graphomaly)
+```
+docker pull pirofti/graphomaly
+```
+For using the GPU pull the dedicated image:
+```
+docker pull pirofti/graphomaly:latest_gpu
+```
+
 ## Usage
 
 The package follows the [sklearn](https://scikit-learn.org/) API and can be included in your projects via
 ```
 from graphomaly.estimator import GraphomalyEstimator
 ```
 which will provide you with a standard scikit-learn estimator that you can use in your pipeline.
```

### Comparing `graphomaly-0.2.8/README.md` & `graphomaly-0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 # Graphomaly
 
-The Anti-Money Laundering (AML) tool. Find abnormal data in graph and network structures.
+Automatic tool for Anti-Money Laundering (AML) and  detecting abnormal behavior in computer networks. Find abnormal data in graph and network structures.
 
 Official package documentation [here](https://unibuc.gitlab.io/graphomaly/graphomaly/).
 
-This work was supported by the [Graphomaly Research Grant](http://graphomaly.upb.ro/).
+This work was initially supported by the [Graphomaly Research Grant](http://graphomaly.upb.ro/) and later partially supported by the [Netalert Research Grant](https://cs.unibuc.ro/~pirofti/netalert.html).
 
 ## Installation and setup
 Install via pip from the [PyPi repository](https://pypi.org/project/graphomaly/):
 ```
 pip install graphomaly
 ```
 
 or for the latest changes not yet in the official release:
 ```
 pip install git+https://gitlab.com/unibuc/graphomaly/graphomaly
 ```
 
+Install via docker from the [DockerHub repository](https://hub.docker.com/r/pirofti/graphomaly)
+```
+docker pull pirofti/graphomaly
+```
+For using the GPU pull the dedicated image:
+```
+docker pull pirofti/graphomaly:latest_gpu
+```
+
 ## Usage
 
 The package follows the [sklearn](https://scikit-learn.org/) API and can be included in your projects via
 ```
 from graphomaly.estimator import GraphomalyEstimator
 ```
 which will provide you with a standard scikit-learn estimator that you can use in your pipeline.
```

### Comparing `graphomaly-0.2.8/graphomaly/estimator.py` & `graphomaly-0.3/graphomaly/estimator.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import numpy as np
 import pandas as pd
 import pprint
 import yaml
 from attrdict import AttrDict
 from sklearn.base import BaseEstimator
 from sklearn.preprocessing import MinMaxScaler, MaxAbsScaler, RobustScaler, StandardScaler
+from threading import Lock
 
 from .grid_search import GridSearch
 from .models import ModelsLoader
 from .preprocessing.egonet import EgonetFeatures
 from .preprocessing.rwalk import RwalkFeatures
 from .preprocessing.spectrum import SpectrumFeatures
 from .preprocessing.transactions_to_graph import Transactions2Graph
@@ -83,27 +84,27 @@
     voting_normalization: string, default="unify"
         Score normalization method to use.
         See the `VotingClassifier` from `graphomaly.voting` for more details.
 
     voting_combine: string, default="average"
         Score combining method to use.
         See the `VotingClassifier` from `graphomaly.voting` for more details.
-        
+
     voting_contamination_rate: float, default=0.001
         Contamination rate to use for soft voting. Applies to the combined score.
-        
+
     timeout_fit: float or None, default=None
         Maximum timeout (in seconds) for fitting one estimator in the grid search. When None, timeout is disabled.
-        
+
     scaling_type: string, dict  or None, default=None
         Apply scaling to input data. String, dict or None.
         Can be a string: one of `'MinMaxScaler'`, `'MaxAbsScaler'`,`'RobustScaler'`, `'StandardScaler'`
         or a dict with (key, value) = (estimator name, string), to specify scaling per algorithm.
         Scaler is fit when running fit().
-        
+
     Attributes
     ----------
     config: attrdict
         if `config_file` was used, this contains the read configuration parameters
 
     config_file: string
         user provided configuration file
@@ -248,55 +249,58 @@
                 #self.voting = self.config.voting
                 # Set individual voting parameters from config
                 self.voting = self.config.voting.method if 'method' in self.config.voting else self.voting   # self.voting is a string
                 self.voting_normalization = self.config.voting.normalization if 'normalization' in self.config.voting else self.voting_normalization
                 self.voting_combine = self.config.voting.combine if 'combine' in self.config.voting else self.voting_combine
                 self.voting_contamination_rate = self.config.voting.contamination_rate if 'contamination_rate' in self.config.voting else self.voting_contamination_rate
 
+        # Ovewrite individual contamination_rate with the global voting_contamination_rate
+        for estim_name, estim_fitkw in self.models_fit_kwargs.items():
+            estim_fitkw['contamination'] = self.voting_contamination_rate
 
         os.makedirs(self.results_path, exist_ok=True)
 
         self._get_models_list()
 
         # Create `scaling_type` dict for estimators
         #
         # `Scaling_type` handling:
         # - if constructor argument `scaling_type` is provided, it is used for all estimators
         # - otherwise, use values from config file
         #   - use the individual `scaling_type` defined for each estimator
         #   - otherwise, use the global scaling_type in the file, if provided
         # `scaling-type` can be a string, or a dict with key = estimators and value = string
-        
+
         self.scaling_type_dict = {}
         if isinstance(self.scaling_type, dict):
             # If already a dict, use as is, but check that all algorithms are specified
             algs_missing = [alg for alg in self.models_list if alg not in self.scaling_type]
             if len(algs_missing) != 0:
                 raise ValueError(f"scaling_type is given as a dict, but not all algorithms are specified ({algs_missing})")
 
             self.scaling_type_dict = self.scaling_type
         elif self.scaling_type is not None:
             # Same scaling for all estimators
             self.scaling_type_dict = {algorithm:self.scaling_type for algorithm in self.models_list}
         else:
             # Use values from config file, if exists
-            
+
             for algorithm in self.models_list:
 
                 if self.models_fit_kwargs is not None and 'scaling_type' in self.models_fit_kwargs[algorithm]:
                         scal = self.models_fit_kwargs[algorithm]['scaling_type']
                 elif hasattr(self, 'config') and 'scaling_type' in self.config:
                         scal = self.config['scaling_type']
                 else:
                     scal = None
-                
+
                 self.scaling_type_dict[algorithm] = scal
 
         logger.info(f"Scaling configuration: {pprint.pformat(self.scaling_type_dict)}")
-        
+
         # Clean fit_kwargs of any `scaling_type` parameter, regardless if used or not,
         #  so it doesn't reach the actual estimator object
         if self.models_fit_kwargs is not None:
             for algorithm in self.models_list:
                 self.models_fit_kwargs[algorithm].pop('scaling_type', None)
 
     def load(self):
@@ -537,19 +541,19 @@
         X: array-like of shape (n_samples, n_features)
             samples on which to perform anomaly detection
 
         voting: string
             Voting method. See `graphomaly.voting` for available options.
 
         normalization: string
-            Normalization method for individual estimator's scores. 
+            Normalization method for individual estimator's scores.
             See `graphomaly.voting` for available options.
 
         combine: string
-            Combination method of estimator's scores. 
+            Combination method of estimator's scores.
             See `graphomaly.voting` for available options.
 
 
         Returns
         -------
         y: array-like of shape (n_samples, ) or list(array-like of shape (n_samples, ))
             If combine == 'no', returns a list of predicted labels for each underlying estimator. The estimator order is the same as returned by get_estimator_params()
@@ -571,19 +575,19 @@
 
         Parameters
         ----------
         X: array-like of shape (n_samples, n_features)
             samples on which to perform anomaly detection
 
         normalization: string
-            Normalization method for individual estimator's scores. 
+            Normalization method for individual estimator's scores.
             See `graphomaly.voting` for available options.
 
         combine: string
-            Combination method of estimator's scores. 
+            Combination method of estimator's scores.
             See `graphomaly.voting` for available options.
 
         Returns
         -------
         y: array-like of shape (n_samples, n_classes) or list(array-like of shape (n_samples, n_classes))
             If combine == 'no', returns a list of predicted_probas for each underlying estimator. The estimator order is the same as returned by get_estimator_params()
             If combine != 'no', returns the combined predicted_probas
@@ -603,15 +607,15 @@
         X: array-like of shape (n_samples, n_features)
             samples on which to perform anomaly detection
 
         voting: string
             Voting method. See `graphomaly.voting` for available options.
 
         normalization: string
-            Normalization method for individual estimator's scores. 
+            Normalization method for individual estimator's scores.
             See `graphomaly.voting` for available options.
 
         Returns
         -------
         y: array-like of shape (n_samples, )
             The predicted labels
 
@@ -658,41 +662,44 @@
         See also
         --------
         tests.test_synthetic_gridsearch:
             example of performing parameter tuning
             on a small subset of methods and parameters list.
         """
 
+        # Save the input X before scaling
+        X_input = X
+
         for algorithm in self.models_list:
             model_kwargs, fit_kwargs = self._get_params(algorithm, X.shape[1])
 
             # Merge 'common' kwargs, with lower priority
             if 'common' in self.models_fit_kwargs:
                 fit_kwargs = {**self.models_fit_kwargs['common'], **fit_kwargs}
 
             # Create and fit scaler object. Same scaler will be used in later calls to predict() and predict_proba()
             #
             # Scaling cannot be done in preprocessing(), because there we don't know if we preprocess the data
-            # in order to (i) fit, where we need to learn a new scaler, (ii) predict, where we just need to use the old scaler, 
+            # in order to (i) fit, where we need to learn a new scaler, (ii) predict, where we just need to use the old scaler,
             # or (iii) refit, where we have an old scaler but we don't want to use it
 
-            # TODO: X scaling is repeatedly applied on same array X. Should copy X every time?
+            # Apply on original X, not on the X transformed at the previous iteration.
 
             if self.scaling_type_dict[algorithm] == "MinMaxScaler":
-                self.scalers_[algorithm] = MinMaxScaler().fit(X)
-                X = self.scalers_[algorithm].transform(X)
+                self.scalers_[algorithm] = MinMaxScaler().fit(X_input)
+                X = self.scalers_[algorithm].transform(X_input)
             elif self.scaling_type_dict[algorithm]  == "MaxAbsScaler":
-                self.scalers_[algorithm] = MaxAbsScaler().fit(X)
-                X = self.scalers_[algorithm].transform(X)
+                self.scalers_[algorithm] = MaxAbsScaler().fit(X_input)
+                X = self.scalers_[algorithm].transform(X_input)
             elif self.scaling_type_dict[algorithm]  == "RobustScaler":
-                self.scalers_[algorithm] = RobustScaler().fit(X)
-                X = self.scalers_[algorithm].transform(X)
+                self.scalers_[algorithm] = RobustScaler().fit(X_input)
+                X = self.scalers_[algorithm].transform(X_input)
             elif self.scaling_type_dict[algorithm]  == "StandardScaler":
-                self.scalers_[algorithm] = StandardScaler().fit(X)
-                X = self.scalers_[algorithm].transform(X)
+                self.scalers_[algorithm] = StandardScaler().fit(X_input)
+                X = self.scalers_[algorithm].transform(X_input)
 
             clf = ModelsLoader.get(algorithm, **model_kwargs)
             if hasattr(clf, "save"):  # tf model detected
                 clf_type = "tensorflow"
             else:
                 clf_type = "sklearn"
 
@@ -728,24 +735,24 @@
                     f"{search.best_params_}"
                 )
 
         # Initialize the VotingClassifier object
         # Some estimators might be None (e.g. no fit() for specified model actually finished in time). Keep only the non-None ones.
         voting_estimators = [(name, obj) for name, obj in zip(self.models_list, self.models) if obj is not None]
 
-        self.voter = VotingClassifier(estimators=voting_estimators, 
-                voting=self.voting, 
-                normalization=self.voting_normalization, 
-                combine=self.voting_combine, 
+        self.voter = VotingClassifier(estimators=voting_estimators,
+                voting=self.voting,
+                normalization=self.voting_normalization,
+                combine=self.voting_combine,
                 contamination_rate=self.voting_contamination_rate,
                 available_normalizations=[self.voting_normalization],
                 available_combines=[self.voting_combine],
                 scalers=self.scalers_)
-       
-        self.voter.fit(X,y)
+
+        self.voter.fit(X_input,y)
 
         return self
 
     def decision_function(self, X):
         """Calls decision_function(X) for all the contained estimators, and returns all the results.
 
         Parameters
@@ -773,15 +780,15 @@
             A list of tuples (estimator_name, estimator.get_params(), for all estimators.
         """
 
         # Some estimators might be None (e.g. no fit() for specified model actually finished in time). Keep only the non-None ones.
         voting_estimators = [(name, obj.get_params()) for name, obj in zip(self.models_list, self.models) if obj is not None]
 
         return voting_estimators
-    
+
     def scale_for_estimator(self, X, estimator_name):
         """Scale data for given estimator
 
         Args:
             X (ndarray): Data matrix
             estimator_name (str): Name of estimator
 
@@ -799,8 +806,79 @@
         return X
 
     def save(self, filepath):
         joblib.dump(self, filepath)
 
     @classmethod
     def load(cls, filepath):
-        return joblib.load(filepath)
+        return joblib.load(filepath)
+
+
+class GraphomalySafeEstimator:
+    """Wrapper to ensure that training the estimator can be done in parallel
+    with predicting.
+
+    Internally delegates the training to a second GraphomalyEstimator object,
+    so that the original GraphomalyEstimator can keep predicting().
+    When training is done, the first estimator re-loads the trained
+    estimators from the disk.
+
+    There are two locks:
+
+    1. Memory lock:
+      - guards the estimator objects loaded in the memory
+      - ensures that `load_cached()`, `predict()` and `predict_proba()`
+        are mutually exclusive when they access the object
+    2. Folder lock:
+      - guards the folder where the individual estimators are saved during training
+      - ensures that `fit()`, `refit()` and `load_cached()` are mutually exclusive
+
+    `fit()` and `refit()` need only the Folder lock.
+    `predict()` and `predict_proba()` need only the Memory lock.
+    `load_cached()` needs both the Memory lock and the Folder lock .
+
+    One of (`fit()` or `refit()`) can run in parallel
+    with one of (`predict()` and `predict_proba()`)
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        self.predictor = GraphomalyEstimator(*args, **kwargs)
+        self.trainer   = GraphomalyEstimator(*args, **kwargs)
+
+        self.memory_lock = Lock()
+        self.folder_lock = Lock()
+
+    def fit(self, *args, **kwargs):
+        with self.folder_lock:
+            self.trainer.fit(*args, **kwargs)
+
+        # Acquires lock internally
+        return self.load_cached(*args, **kwargs)
+
+    def refit(self, *args, **kwargs):
+        with self.folder_lock:
+            self.trainer.refit(*args, **kwargs)
+
+        # Acquires lock internally
+        return self.load_cached(*args, **kwargs)
+
+    def load_cached(self, *args, **kwargs):
+        with self.memory_lock, self.folder_lock:
+            return self.predictor.load_cached(*args, **kwargs)
+
+    def predict(self, *args, **kwargs):
+        with self.memory_lock:
+            return self.predictor.predict(*args, **kwargs)
+
+    def predict_proba(self, *args, **kwargs):
+        with self.memory_lock:
+            return self.predictor.predict_proba(*args, **kwargs)
+
+    def preprocess(self, *args, **kwargs):
+        return self.predictor.preprocess(*args, **kwargs)
+
+    def get_estimator_params(self, *args, **kwargs):
+        return self.predictor.get_estimator_params(*args, **kwargs)
+
+    @property
+    def _model_is_fitted(self):
+        return self.predictor._model_is_fitted
```

### Comparing `graphomaly-0.2.8/graphomaly/grid_search.py` & `graphomaly-0.3/graphomaly/grid_search.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/models/autoencoder.py` & `graphomaly-0.3/graphomaly/models/autoencoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 from tensorflow.keras import activations, layers
 from tensorflow.keras.regularizers import L2
 from tensorflow.keras.callbacks import EarlyStopping, ReduceLROnPlateau
 
 
 @tf.keras.utils.register_keras_serializable()
 class Autoencoder(tf.keras.Model):
-    """Autoencoder model introduced by Aggarwal C. [1]_
+    """Autoencoder model introduced by Aggarwal C. [Aggarwal2015]_
 
     Parameters
     ----------
     encoder_neurons : list
-        The number of neurons per encoder layers. 
+        The number of neurons per encoder layers.
         Values > 1 are absolute, values <= 1 are relative to input size (e.g. [0.8, 0.4])
 
     decoder_neurons : list
-        The number of neurons per decoder layers. 
+        The number of neurons per decoder layers.
         Values > 1 are absolute, values <= 1 are relative to input size (e.g. [0.8, 0.4])
 
     activation_function : str or callable, default='tanh'
         The activation function for all layers.
-        See `Keras doc <https://keras.io/api/layers/activations/>`_.
+        See `Keras doc <https://keras.io/api/layers/activations/>`__.
 
     l2_regularizer : float in (0., 1), default=0.1
         The regularization factor for L2 regularizer for all layers.
 
     dropout : float in (0., 1), default=0.2
         Dropout rate for all hidden layers.
 
@@ -55,78 +55,78 @@
 
     contamination : float, default=0.1
         The contamination rate used for computing the reconstruction error
         threshold. Used if threshold is not set.
 
     optimizer: str or callable, default='adam'
         The optimizer algorithm of the neural network.
-        See `Keras doc <https://keras.io/api/optimizers/>`_.
+        See `Keras doc <https://keras.io/api/optimizers/>`__.
 
     loss: str or callable, default='mse'
         The loss function of the neural network.
-        See `Keras doc <https://keras.io/api/losses/>`_.
+        See `Keras doc <https://keras.io/api/losses/>`__.
 
     epochs: int, default=1000
         Maximum number of epochs for network training.
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
-        
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
+
     batch_size: int, default=10000
         Batch size used for training.
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
     shuffle: boolean, default=True
         Shuffle data before each epoch during training.
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
     validation_size: float, default==0.1
         Amount of training set used for validation.
-        See `validation_split` argument of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See `validation_split` argument of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
     learning_rate : float, default==0.001
         Gradient step size used in training.
         Depends on the optimizer used.
 
     verbose: int or str, default='auto'
         Print training progress. Can be 0, 1, or 'auto'
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
     es_monitor: str or None, default='val_loss'
         Quantity to monitor for early stopping of training.
         Use None to disable EarlyStopping.
-        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`__.
 
     es_patience: int, default=50
         Early Stopping: how many epochs to wait before stop.
-        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`__.
 
-    redlr_monitor: str or None, default='val_loss'                  
+    redlr_monitor: str or None, default='val_loss'
         Quantity to monitor for "Reduce Learning Rate on Plateau" during training.
         Use None to disable ReduceLROnPlateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     redlr_learning_rate_reduce_factor: float, default=0.2
-        Factor for reducing learning rate when plateau is detected. Must be < 1. 
+        Factor for reducing learning rate when plateau is detected. Must be < 1.
         Use None to disable ReduceLROnPlateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     redlr_learning_rate_min: float, default=0.00001
         Minimum learning rate allowed when reducing learning rate on plateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     redlr_patience: int, default=10
         How many epochs to wait before reducing learning rate on plateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     savename_key_len: int, default=3
         When saving the model, restrict key length in the name to this many characters.
 
     Attributes
     ----------
     decision_scores_ : array-like of shape (n_samples,)
-        The raw outlier scores for the training data, i.e. the reconstruction errors. 
+        The raw outlier scores for the training data, i.e. the reconstruction errors.
         The anomalies have a larger error score.
 
     history_ : Keras Object
         The training history of the model.
 
     labels_ : list of int (0 or 1)
         The binary labels for the training data. 0 means inliers and 1 means
@@ -139,15 +139,15 @@
         The actual number of neurons per encoder layers, if decoder_neurons is relative
 
     decoder_neurons_ : list
         The actual number of neurons per decoder layers, if decoder_neurons is relative
 
     References
     ----------
-    .. [1] Aggarwal C. (2015) Outlier Analysis. In: Data Mining. Springer,
+    .. [Aggarwal2015] Aggarwal C. (2015) Outlier Analysis. In: Data Mining. Springer,
         Cham. https://doi.org/10.1007/978-3-319-14142-8_8
     """
 
     def __init__(
         self,
         encoder_neurons = None,
         decoder_neurons = None,
@@ -233,20 +233,20 @@
         params.update(attributes)
         return params
 
     @classmethod
     def from_config(cls, config):
         """Instantiates an object based on a config dict returned by get_config()
         """
-        
+
         # Extract attributes from `config` and set later, they cannot be passed to __init__()
         attrs = ["classes", "threshold_", "decision_scores_", "history_", "labels_"]
         attrs_dict = {attr: config.pop(attr) for attr in attrs}
 
-        # Instantiate with the remaining keys        
+        # Instantiate with the remaining keys
         instance = cls(**config)
 
         # Set attributes
         for attr, value in attrs_dict.items():
             setattr(instance, attr, value)
 
         return instance
@@ -284,14 +284,16 @@
             decoder_layers.append(linear_layer)
             decoder_layers.append(dropout_layer)
 
         self.encoder = tf.keras.Sequential(encoder_layers, name="encoder")
         self.decoder = tf.keras.Sequential(decoder_layers[:-1], name="decoder")
 
     def call(self, inputs):
+        """Runs the model on the input data.
+        """
         if inputs.shape[1] != self.decoder_neurons_[-1]:
             raise ValueError(
                 "Expected the number of features to be equal to "
                 "the number of neurons on the last decoder layer. "
                 f"But found: {inputs.shape[1]} features and "
                 f"{self.decoder_neurons_[-1]} neurons."
             )
@@ -323,32 +325,33 @@
             The reconstruction error scores.
         """
         preds = super().predict(X)
         return Autoencoder._compute_scores(X, preds)
 
     def predict_proba(self, X=None, method="linear", thresh=None):
         """Compute a distribution probability on the reconstuction errors
-        predicted for the samples passed as parameter. 
+        predicted for the samples passed as parameter.
 
         This does not modify the object. Use for prediction, not fitting.
 
         If X is not None, the errors are computed for the data in X
-        If X is None, assume the erorrs are already available in self.decision_scores_
+        If X is None, assume the erorrs are already available in `self.decision_scores_`
 
         Parameters
         ----------
         X : array-like of shape (num_samples, num_features)
             The samples for which to compute the probabilities.
 
         method : {'linear', 'hard', 'quantile'}, default='linear'
-            The method used for score normalization. 
-            'linear': scale scores to [0, 1] range. Default.
-            'hard': hard thresholding with a given threshold `thresh`, return binary scores. If `thresh` is None, use self.threshold_ instead.
-            'quantile': hard thresholding using the given quantile in `thresh`, 
-                        e.g. thresh=0.1 assigns 0 to the smallest 10% errors, and 1 to the largest 90% errors.
+                 The method used for score normalization. Possible values:
+
+                 - 'linear': scale scores to [0, 1] range. Default.
+                 - 'hard': hard thresholding with a given threshold `thresh`, return binary scores. If `thresh` is None, use `self.threshold_` instead.
+                 - 'quantile': hard thresholding using the given quantile in `thresh`,
+                   e.g. thresh=0.1 assigns 0 to the smallest 10% errors, and 1 to the largest 90% errors.
 
         Returns
         -------
         ndarray of shape (num_samples, )
             The probabilities for each class (normal prob on dimension 0,
             anomaly prob on dimension 1).
         """
@@ -380,14 +383,15 @@
             raise ValueError(
                 f"method={method}, thresh={thresh} is not a valid combination for probability conversion."
             )
 
         return probs
 
     def set_params(self, **kwargs):
+        """Set estimator parameters"""
         for key, value in kwargs.items():
             setattr(self, key, value)
         return self
 
     def get_params(self, deep=True):
         """Returns all parameters of the estimator. Needed for Scikit-learn compatibility
         """
@@ -415,18 +419,19 @@
             "redlr_learning_rate_reduce_factor": self.redlr_learning_rate_reduce_factor,
             "redlr_learning_rate_min": self.redlr_learning_rate_min,
             "redlr_patience": self.redlr_patience,
             "savename_key_len": self.savename_key_len
         }
 
     def fit(self, X, y=None, **kwargs):
+        """Fits the model on the data provided."""
 
         self.set_params(**kwargs)
 
-        # When the last decoder layer has size 1, the values are relative. 
+        # When the last decoder layer has size 1, the values are relative.
         # Scale the numbers by input size.
         # Note the trailing underscore_!
         input_size = X.shape[1]
         if round(self.decoder_neurons[-1]) == 1:
             self.encoder_neurons_ = [round(v * input_size) for v in self.encoder_neurons]
             self.decoder_neurons_ = [round(v * input_size) for v in self.decoder_neurons]
             logger.info(f'Layer size was relative, actual sizes are: encoder: {self.encoder_neurons_}, decoder: {self.decoder_neurons_}')
@@ -452,15 +457,15 @@
 
         # - Reduce learning-rate on plateau
         if hasattr(self, 'redlr_monitor') and hasattr(self, 'redlr_learning_rate_reduce_factor'):
             redlr_learning_rate_min = \
                 self.redlr_learning_rate_min if hasattr(self, 'redlr_learning_rate_min') else 0    # defaults to 0
             redlr_patience = \
                 self.redlr_patience if hasattr(self, 'redlr_patience') else 10   # defaults to 10
-            callbacks.append(ReduceLROnPlateau(monitor=self.redlr_monitor, factor=self.redlr_learning_rate_reduce_factor, 
+            callbacks.append(ReduceLROnPlateau(monitor=self.redlr_monitor, factor=self.redlr_learning_rate_reduce_factor,
                                             patience=redlr_patience, min_lr=redlr_learning_rate_min))
 
         # Train!
         self.history_ = (
             super()
             .fit(
                 X,
@@ -504,14 +509,15 @@
         """
 
         pred_score = self.decision_function(X)
         labels = (pred_score > self.threshold_).astype("int")
         return labels
 
     def fit_predict(self, X, y=None):
+        """Run fit() and the predict()"""
         # Fit already does prediction internally, and the labels are in labels_
         return self.fit(X, y).labels_
 
     def _check_parameters(self):
         if not isinstance(self.encoder_neurons, list):
             raise TypeError(
                 "Expected encoder_neurons to have type list, but "
```

### Comparing `graphomaly-0.2.8/graphomaly/models/base_model.py` & `graphomaly-0.3/graphomaly/models/base_model.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/models/dictlearn.py` & `graphomaly-0.3/graphomaly/models/dictlearn.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/models/models.py` & `graphomaly-0.3/graphomaly/models/models.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/models/sklearn.py` & `graphomaly-0.3/graphomaly/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/models/vae.py` & `graphomaly-0.3/graphomaly/models/vae.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,39 +25,39 @@
 from tensorflow.keras import activations, layers
 from tensorflow.keras.regularizers import L2
 from tensorflow.keras.callbacks import EarlyStopping, ReduceLROnPlateau
 
 
 @tf.keras.utils.register_keras_serializable()
 class VAE(tf.keras.Model):
-    """Variational Autoencoder model introduced by Kingma et al. [2]_
+    """Variational Autoencoder model introduced by Kingma et al. [Kingma2013]_
 
     Parameters
     ----------
     encoder_neurons : list
-        The number of neurons per encoder layers. 
+        The number of neurons per encoder layers.
         Values > 1 are absolute, values <= 1 are relative to input size (e.g. [0.8, 0.4])
 
     decoder_neurons : list
-        The number of neurons per decoder layers. 
+        The number of neurons per decoder layers.
         Values > 1 are absolute, values <= 1 are relative to input size (e.g. [0.8, 0.4])
 
 
     input_dim : int or None
         The number of features (input dimension).
         If None, the input dimension is taken from the input data.
 
     latent_dim : int or None
-        The dimension of the latent space. 
+        The dimension of the latent space.
         A value >1 is absolute, a value <=1 is relative to input_dimension.
         If None, latent_dim is taken as the last value from `encoder_neurons` argument.
 
     activation_function : str or callable, default='tanh'
         The activation function for all layers.
-        See `Keras doc <https://keras.io/api/layers/activations/>`_.
+        See `Keras doc <https://keras.io/api/layers/activations/>`__.
 
     l2_regularizer : float in (0., 1), default=0.1
         The regularization factor for L2 regularizer for all layers.
 
     dropout : float in (0., 1), default=0.2
         Dropout rate for all hidden layers.
 
@@ -67,78 +67,78 @@
 
     contamination : float, default=0.1
         The contamination rate used for computing the reconstruction error
         threshold. Used if threshold is not set.
 
     optimizer: str or callable, default='adam'
         The optimizer algorithm of the neural network.
-        See `Keras doc <https://keras.io/api/optimizers/>`_.
+        See `Keras doc <https://keras.io/api/optimizers/>`__.
 
     loss: str or callable, default='mse'
         The loss function of the neural network.
-        See `Keras doc <https://keras.io/api/losses/>`_.
+        See `Keras doc <https://keras.io/api/losses/>`__.
 
     epochs: int, default=1000
         Maximum number of epochs for network training.
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
-        
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
+
     batch_size: int, default=10000
         Batch size used for training.
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
     shuffle: boolean, default=True
         Shuffle data before each epoch during training.
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
-    validation_size: float, default==0.1
+    validation_size: float, default=0.1
         Amount of training set used for validation.
-        See `validation_split` argument of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See `validation_split` argument of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
-    learning_rate : float, default==0.001
+    learning_rate: float, default=0.001
         Gradient step size used in training.
         Depends on the optimizer used.
 
     verbose: int or str, default='auto'
         Print training progress. Can be 0, 1, or 'auto'
-        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`_.
+        See arguments of fit() method in `Keras doc <https://keras.io/api/models/model_training_apis/>`__.
 
     es_monitor: str or None, default='val_loss'
         Quantity to monitor for early stopping of training.
         Use None to disable EarlyStopping.
-        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`__.
 
     es_patience: int, default=50
         Early Stopping: how many epochs to wait before stop.
-        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/early_stopping/>`__.
 
-    redlr_monitor: str or None, default='val_loss'                  
+    redlr_monitor: str or None, default='val_loss'
         Quantity to monitor for "Reduce Learning Rate on Plateau" during training.
         Use None to disable ReduceLROnPlateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     redlr_learning_rate_reduce_factor: float, default=0.2
-        Factor for reducing learning rate when plateau is detected. Must be < 1. 
+        Factor for reducing learning rate when plateau is detected. Must be < 1.
         Use None to disable ReduceLROnPlateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     redlr_learning_rate_min: float, default=0.00001
         Minimum learning rate allowed when reducing learning rate on plateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     redlr_patience: int, default=10
         How many epochs to wait before reducing learning rate on plateau.
-        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`_.
+        See `Keras doc <https://keras.io/api/callbacks/reduce_lr_on_plateau/>`__.
 
     savename_key_len: int, default=3
         When saving the model, restrict key length in the name to this many characters.
 
     Attributes
     ----------
     decision_scores_ : array-like of shape (n_samples,)
-        The raw outlier scores for the training data, i.e. the reconstruction errors. 
+        The raw outlier scores for the training data, i.e. the reconstruction errors.
         The anomalies have a larger error score.
 
     history_ : Keras Object
         The training history of the model.
 
     labels_ : list of integers (0 or 1)
         The binary labels for the training data. 0 means inliers and 1 means
@@ -154,15 +154,15 @@
         The actual number of neurons per decoder layers, if decoder_neurons is relative
 
     latent_dim_ : list
         The actual latent dimension, if latent_dim is relative
 
     References
     ----------
-    .. [2] Kingma, Diederik P., and Max Welling. "Auto-encoding variational
+    .. [Kingma2013] Kingma, Diederik P., and Max Welling. "Auto-encoding variational
         bayes." arXiv preprint arXiv:1312.6114 (2013).
     """
 
     def __init__(
         self,
         encoder_neurons = [],
         decoder_neurons = [],
@@ -256,20 +256,20 @@
         params.update(attributes)
         return params
 
     @classmethod
     def from_config(cls, config):
         """Instantiates an object based on a config dict returned by get_config()
         """
-        
+
         # Extract attributes from `config` and set later, they cannot be passed to __init__()
         attrs = ["classes", "threshold_", "decision_scores_", "history_", "labels_"]
         attrs_dict = {attr: config.pop(attr) for attr in attrs}
 
-        # Instantiate with the remaining keys        
+        # Instantiate with the remaining keys
         instance = cls(**config)
 
         # Set attributes
         for attr, value in attrs_dict.items():
             setattr(instance, attr, value)
 
         return instance
@@ -314,14 +314,16 @@
             # The last layer should have no subsequent dropout
             if ilayer < len(self.decoder_neurons_)-1:
                 outputs = layers.Dropout(self.dropout)(outputs)
 
         self.decoder = tf.keras.Model(latent_inputs, outputs, name="decoder")
 
     def call(self, inputs):
+        """Runs the model on the input data.
+        """
         if inputs.shape[1] != self.decoder_neurons_[-1]:
             raise ValueError(
                 "Expected the number of features to be equal to "
                 "the number of neurons on the last decoder layer. "
                 f"But found: {inputs.shape[1]} features and "
                 f"{self.decoder_neurons_[-1]} neurons."
             )
@@ -334,15 +336,15 @@
         kl_loss = -0.5 * tf.reduce_mean(
             z_log_var - tf.square(z_mean) - tf.exp(z_log_var) + 1
         )
         self.add_loss(kl_loss)
         return reconstructed
 
     def summary(self):
-        """Print Autoencoder architecture on components."""
+        """Print VAE architecture on components."""
         print(self.encoder.summary())
         print(self.decoder.summary())
 
     def decision_function(self, X):
         """Compute the reconstruction errors for some samples.
         The anomalies have a larger error score.
 
@@ -359,32 +361,33 @@
             The reconstruction error scores.
         """
         preds = super().predict(X)
         return VAE._compute_scores(X, preds)
 
     def predict_proba(self, X=None, method="linear", thresh=None):
         """Compute a distribution probability on the reconstuction errors
-        predicted for the samples passed as parameter. 
+        predicted for the samples passed as parameter.
 
         This does not modify the object. Use for prediction, not fitting.
 
         If X is not None, the errors are computed for the data in X
         If X is None, assume the erorrs are already available in self.decision_scores_
 
         Parameters
         ----------
         X : array-like of shape (num_samples, num_features)
             The samples for which to compute the probabilities.
 
         method : {'linear', 'hard', 'quantile'}, default='linear'
-            The method used for score normalization. 
-            'linear': scale scores to [0, 1] range. Default.
-            'hard': hard thresholding with a given threshold `thresh`, return binary scores. If `thresh` is None, use self.threshold_ instead.
-            'quantile': hard thresholding using the given quantile in `thresh`, 
-                        e.g. thresh=0.1 assigns 0 to the smallest 10% errors, and 1 to the largest 90% errors.
+                 The method used for score normalization. Possible values:
+
+                 - 'linear': scale scores to [0, 1] range. Default.
+                 - 'hard': hard thresholding with a given threshold `thresh`, return binary scores. If `thresh` is None, use self.threshold_ instead.
+                 - 'quantile': hard thresholding using the given quantile in `thresh`,
+                   e.g. thresh=0.1 assigns 0 to the smallest 10% errors, and 1 to the largest 90% errors.
 
         Returns
         -------
         ndarray of shape (num_samples, )
             The probabilities for each class (normal prob on dimension 0,
             anomaly prob on dimension 1).
         """
@@ -416,14 +419,15 @@
             raise ValueError(
                 f"method={method}, thresh={thresh} is not a valid combination for probability conversion."
             )
 
         return probs
 
     def set_params(self, **kwargs):
+        """Set estimator parameters"""
         for key, value in kwargs.items():
             setattr(self, key, value)
         return self
 
     def get_params(self, deep=True):
         """Returns all parameters of the estimator. Needed for Scikit-learn compatibility
         """
@@ -453,26 +457,27 @@
             "redlr_learning_rate_reduce_factor": self.redlr_learning_rate_reduce_factor,
             "redlr_learning_rate_min": self.redlr_learning_rate_min,
             "redlr_patience": self.redlr_patience,
             "savename_key_len": self.savename_key_len
         }
 
     def fit(self, X, y=None, **kwargs):
+        """Fits the model on the data provided."""
 
         self.set_params(**kwargs)
 
         # Overwrite `input_dim`` if not explicitly set
         if self.input_dim is None:
             self.input_dim = X.shape[1]
 
         # Overwrite `latent_dim` if not explicitly set
         if self.latent_dim is None:
             self.latent_dim = self.encoder_neurons[-1]
 
-        # When the last decoder layer has size 1, the values are relative. 
+        # When the last decoder layer has size 1, the values are relative.
         # Scale the numbers by input size.
         # Note the trailing _ !
         if round(self.decoder_neurons[-1]) == 1:
             self.encoder_neurons_ = [round(v * self.input_dim) for v in self.encoder_neurons]
             self.decoder_neurons_ = [round(v * self.input_dim) for v in self.decoder_neurons]
             self.latent_dim_      = round(self.latent_dim * self.input_dim)
             logger.info(f'Layer sizes were relative, actual sizes are: encoder: {self.encoder_neurons_}, decoder: {self.decoder_neurons_}, latent_dim: {self.latent_dim_}')
@@ -499,15 +504,15 @@
 
         # - Reduce learning-rate on plateau
         if hasattr(self, 'redlr_monitor') and hasattr(self, 'redlr_learning_rate_reduce_factor'):
             redlr_learning_rate_min = \
                 self.redlr_learning_rate_min if hasattr(self, 'redlr_learning_rate_min') else 0    # defaults to 0
             redlr_patience = \
                 self.redlr_patience if hasattr(self, 'redlr_patience') else 10   # defaults to 10
-            callbacks.append(ReduceLROnPlateau(monitor=self.redlr_monitor, factor=self.redlr_learning_rate_reduce_factor, 
+            callbacks.append(ReduceLROnPlateau(monitor=self.redlr_monitor, factor=self.redlr_learning_rate_reduce_factor,
                                             patience=redlr_patience, min_lr=redlr_learning_rate_min))
 
         # Train!
         self.history_ = (
             super()
             .fit(
                 X,
@@ -551,14 +556,15 @@
         """
 
         pred_score = self.decision_function(X)
         labels = (pred_score > self.threshold_).astype("int")
         return labels
 
     def fit_predict(self, X, y=None):
+        """Runs fit() and then predict()"""
         # Fit already does prediction internally, and the labels are in labels_
         return self.fit(X, y).labels_
 
     def _check_parameters(self):
         if not isinstance(self.encoder_neurons, list):
             raise TypeError(
                 "Expected encoder_neurons to have type list, but "
@@ -636,14 +642,17 @@
 
     @staticmethod
     def _compute_scores(X, Y):
         return np.sqrt(np.sum(np.square(Y - X), axis=1))
 
 
 class Sampling(layers.Layer):
+    """Helper class to implement sampling as a Keras layer
+    """
     def call(self, inputs):
+        """Apply the layer to the inputs"""
         z_mean, z_log_var = inputs
         batch = K.shape(z_mean)[0]  # batch size
         dim = K.int_shape(z_mean)[1]  # latent dimension
         epsilon = K.random_normal(shape=(batch, dim))  # mean=0, std=1.0
 
         return z_mean + K.exp(0.5 * z_log_var) * epsilon
```

### Comparing `graphomaly-0.2.8/graphomaly/normalizations.py` & `graphomaly-0.3/graphomaly/normalizations.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/egonet.py` & `graphomaly-0.3/graphomaly/preprocessing/egonet.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/fe_base/historical_features.py` & `graphomaly-0.3/graphomaly/preprocessing/fe_base/historical_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/fe_base/statistical_features.py` & `graphomaly-0.3/graphomaly/preprocessing/fe_base/statistical_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/fe_base/time_features.py` & `graphomaly-0.3/graphomaly/preprocessing/fe_base/time_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/fe_difference_transformer.py` & `graphomaly-0.3/graphomaly/preprocessing/fe_difference_transformer.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/fe_statistical_transformer.py` & `graphomaly-0.3/graphomaly/preprocessing/fe_statistical_transformer.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/fe_time_transformers.py` & `graphomaly-0.3/graphomaly/preprocessing/fe_time_transformers.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/graph_to_features.py` & `graphomaly-0.3/graphomaly/preprocessing/graph_to_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -272,14 +272,27 @@
         # (a lonely node is connected only with a single edge to the central node of the egonet)
         enodes = []
         i_ego = 0
         for nn in Gs:
             if Gs.degree(nn) > 1:  # keep only nodes that have more than one neighbor
                 enodes.append(nn)
                 i_ego += 1
+
+        # There is a case when egonet looks like this :
+        #           degree: DiDegreeView({273172446621881.0: 3, 198112242249590.0: 1})
+        #           edges: OutEdgeView([(273172446621881.0, 273172446621881.0), (198112242249590.0, 273172446621881.0)])
+        #           in_edges: InEdgeView([(198112242249590.0, 273172446621881.0), (273172446621881.0, 273172446621881.0)])
+        #           out_edges: OutEdgeView([(273172446621881.0, 273172446621881.0), (198112242249590.0, 273172446621881.0)])
+        # And the current node is 198112242249590.0
+        # As the degree of the current node is 1, it won't be added to the enodes list
+        # This means that the reduced egonet doesn t contain the "ego" anymore
+        # So the reduced egonet is empty
+        if node not in enodes:
+            i_ego = 0
+
         # if something left in the egonet (i.e., not a star)
         if i_ego > 0:
             Gs = Gs.subgraph(enodes[0:i_ego])  # the reduced egonet
 
             # Repeat the same operations as for the full egonet
             # In and out degree, total number of edges (they are smaller now, of course)
             node_features[row, feat_egored_degree_in] = Gs.in_degree(node)
```

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/graph_to_spectrum_features.py` & `graphomaly-0.3/graphomaly/preprocessing/graph_to_spectrum_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/rwalk.py` & `graphomaly-0.3/graphomaly/preprocessing/rwalk.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/spectrum.py` & `graphomaly-0.3/graphomaly/preprocessing/spectrum.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/preprocessing/transactions_to_graph.py` & `graphomaly-0.3/graphomaly/preprocessing/transactions_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/graphomaly/voting.py` & `graphomaly-0.3/graphomaly/voting.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,30 +40,30 @@
 #  Ensemble:
 #    predict():           ensemble prediction            input X, output labels, combined
 #    predict_proba():     ensemble score                 input X, output scores, combined
 #
 #  Individual estimators:
 #    transform():         individual prediction/scores     input X, output labels or scores, each. Wrapper of _predict() or _collect_probas()
 #      _predict():        individual prediction            input X, output labels, each
-#      _collect_probas(): individual scores                input X, output scores, each   
+#      _collect_probas(): individual scores                input X, output scores, each
 #==========================================
 
 class VotingClassifier(ClassifierMixin, _BaseVoting):
     """Ensemble voting of multiple estimators
 
     How to use VotingClassifier:
 
     Ensemble:
 
     - predict():           ensemble prediction            input X, output labels, combined
     - predict_proba():     ensemble score                 input X, output scores, combined
 
     Individual estimators:
 
-    - transform():         individual prediction/scores     input X, output labels or scores, each. 
+    - transform():         individual prediction/scores     input X, output labels or scores, each.
                            Wrapper of _predict() or _collect_probas()
     - _predict():          individual prediction            input X, output labels, each
     - _collect_probas():   individual scores                input X, output scores, each
     """
 
     # Class-level option lists
     available_normalizations = ['raw', 'default', 'linear', 'unify', 'gaussian', 'standard']  # and 'no'
@@ -115,39 +115,39 @@
 
         Returns
         -------
         self: object
             Fitted VotingClassifier object.
         """
 
-        self.estimators_ = []    
+        self.estimators_ = []
         self.normalizers_ = []   # Will store a list of dicts with fitted normalizers
         self.threshold_dict_ = {}
 
         for clf_name, clf in self.estimators:
-            
+
             # Scale data
-            X = self.scale_for_estimator(X, clf_name)
+            Xscaled = self.scale_for_estimator(X, clf_name)
 
-            if not self._model_is_fitted(clf, X[0]):
-                clf.fit(X)
+            if not self._model_is_fitted(clf, Xscaled[0]):
+                clf.fit(Xscaled)
             self.estimators_.append(clf)
 
         #self.__sklearn_is_fitted__() # ?
 
         # Fit individual normalizers
         self.fit_normalizers(X)
 
         # Fit thresholds for combination
         self.fit_threshold(X)
 
         return self
 
     def fit_normalizers(self, X):
-        """Train the outlier scores normalizers on samples in `X`. 
+        """Train the outlier scores normalizers on samples in `X`.
         Normalizers are used in voting to bring scores from all models in the same range.
 
         Parameters
         ----------
         X: array-like of shape (n_samples, n_features)
             samples on which to fit the methods
 
@@ -161,19 +161,19 @@
 
             # Compute decision scores for each estimator
             if hasattr(clf, 'decision_scores_'):
                 logger.debug(f"VotingClassifier fit(): using {est_name} decision_scores_")
                 decision_scores = clf.decision_scores_
             else:
                 logger.debug(f"VotingClassifier fit(): computing decision scores for {est_name}")
-                X = self.scale_for_estimator(X, est_name)
-                decision_scores = cached_decision_function(clf, X)
+                Xscaled = self.scale_for_estimator(X, est_name)
+                decision_scores = cached_decision_function(clf, Xscaled)
             decision_scores = np.reshape(decision_scores, (-1,1))
 
-            # Fit different normalizers for each estimator, 
+            # Fit different normalizers for each estimator,
             # and append them to the normalizers list
             normalizers = {}
             normalizers['raw'] = StandardScaler(with_mean=False, with_std=False)  # does nothing
             normalizers['raw'].fit(decision_scores)
             normalizers['linear'] = MinMaxScaler()
             normalizers['linear'].fit(decision_scores)
             normalizers['unify'] = GaussScalingTransformer()
@@ -202,19 +202,20 @@
             Fitted VotingClassifier object.
         """
 
         # Fit threshold for each tuple (normalization, combine)
         # It's not very efficient to call predict_proba for all possible combinations. Turn on caching?
         for norm, comb in itertools.product(self.available_normalizations, self.available_combines):
             try:
-                combined_score = self.predict_proba(X, normalization=norm, combine=comb)[:,1]
+                combined_score = self.predict_proba(X, normalization=norm, combine=comb,
+                                                    use_decision_scores=True)[:,1]
                 self.threshold_dict_[(norm, comb)] = np.quantile(combined_score, 1-self.contamination_rate)
             except Exception as e:
                 logger.warning(f'Caught exception in fit_threshold(), norm={norm}, comb={comb}, exception: {e}')
-        
+
         logger.debug(f'self.threshold_dict_ = {self.threshold_dict_}')
 
         return self
 
     def _model_is_fitted(self, model, X):
         """Checks if model object has any attributes ending with an underscore.
 
@@ -335,62 +336,74 @@
         return maj
 
     def fit_predict(self, X, y):
         """Call fit() and then predict()
         """
         return self.fit(X, y).predict(X)
 
-    def _collect_probas(self, X, normalization=None):
+    def _collect_probas(self, X, normalization=None, use_decision_scores = False):
         """Collect results estimators predict_probas(), with configurable normalizations
+
+        If use_decision_scores is True, we skip calling predict_proba() or
+        decision_function() and we collect the estimators' decision_scores_,
+        which are then regularized explicitly.
+        Use this option only when fitting for the train data, not for the test data.
         """
 
         # return np.asarray([clf.predict_proba(X) for clf in self.estimators_])
 
         probas = []
         for (method_name, method_obj),normalizers in zip(self.estimators, self.normalizers_):
 
             # Decide which normalization method to use for scores
             # Use provided argument or fallback to self.normalization
             normalization = normalization if normalization is not None else self.normalization
-            
+
             # We could also pass a dictionary indicating normalization type for each method
             if isinstance(normalization, dict):
                 if method_name in self.normalization:
                     normalization = self.normalization[method_name]
                 elif 'default' in self.normalization:
                     normalization = self.normalization['default']
                 else:
                     raise ValueError(f"Normalization {normalization} not understood")
 
             # Scale data
-            X = self.scale_for_estimator(X, method_name)
+            Xscaled = self.scale_for_estimator(X, method_name)
 
             # Get probas
-            done = False 
-            
+            done = False
+
             # Attempt to use estimator's predict_proba() with method 'linear' or 'unify'
-            if (normalization == 'default' or normalization == 'linear' or normalization == 'unify') and hasattr(method_obj, 'predict_proba'):
+            if not use_decision_scores and \
+               (normalization == 'default' or normalization == 'linear' or normalization == 'unify') and \
+               hasattr(method_obj, 'predict_proba'):
 
                 try:
                     logger.debug(f'Voting {self.voting}: predict_proba({normalization}): {method_obj}')
                     if normalization == 'default':
                         #probas_pred = method_obj.predict_proba(X)
-                        probas_pred = cached_predict_proba(obj=method_obj, X=X)
+                        probas_pred = cached_predict_proba(obj=method_obj, X=Xscaled)
                     else:
                         #probas_pred = method_obj.predict_proba(X, method=normalization)
-                        probas_pred = cached_predict_proba(obj=method_obj, X=X, method=normalization)
+                        probas_pred = cached_predict_proba(obj=method_obj, X=Xscaled, method=normalization)
                     done = True
                 except Exception as e:
                     logger.debug(f'_collect_probas(): Caught exception: {e}')
 
-            # Attempt to use decision_function() and regularize explicitly
+            # Attempt to regularize explicitly the decision scores
+            # Get them either from clf.decision_scores_ or with clf.decision_function()
             if not done:
-                logger.debug(f'Voting {self.voting}: decision_function(): {method_obj}')
-                #decision_scores = method_obj.decision_function(X).reshape(-1, 1)
-                decision_scores = cached_decision_function(obj=method_obj, X=X).reshape(-1, 1)
+                if use_decision_scores:
+                    logger.debug(f'Voting {self.voting}: collecting decision_scores_ for: {method_obj}')
+                    decision_scores = method_obj.decision_scores_.reshape(-1, 1)  # Make sure to reshape(-1,1)
+                else:
+                    logger.debug(f'Voting {self.voting}: decision_function(): {method_obj}')
+                    #decision_scores = method_obj.decision_function(X).reshape(-1, 1)
+                    decision_scores = cached_decision_function(obj=method_obj, X=Xscaled).reshape(-1, 1)
 
                 # 'raw' => provide raw scores, without transformation
                 if normalization == 'raw':
                     probas_pred = decision_scores
                 else:
                     # Regularize scores
                     if normalization == 'linear':
@@ -408,70 +421,71 @@
 
                 done = True
 
             if done:
                 probas.append(probas_pred)
 
         return np.asarray(probas, dtype="float32")
-        
+
     def _check_voting(self):
         if self.voting == "hard":
             raise AttributeError(
                 f"predict_proba is not available when voting={repr(self.voting)}"
             )
         return True
 
     def _predict(self, X):
         """Collect labels predicted by each underlying estimator.
-        
+
         Results are always in the same order as estimators.
         """
         y = []
         for method in self.estimators:
             logger.debug(f'Voting {self.voting}: predict(): {method}')
 
             # Scale
-            X = self.scale_for_estimator(X, method[0])
+            Xscaled = self.scale_for_estimator(X, method[0])
 
             #y_pred = method[1].predict(X)
-            y_pred = cached_predict(obj=method[1], X=X)
+            y_pred = cached_predict(obj=method[1], X=Xscaled)
             if y_pred.ndim > 1:  # saved tf autoencoders
-                _, y_pred, _ = self.__fix_saved_tf_scores(X, method)
+                _, y_pred, _ = self.__fix_saved_tf_scores(X, method)  # This scales internally
             y.append(y_pred)
         return np.asarray(y, dtype="int").T
 
     @available_if(_check_voting)
-    def predict_proba(self, X, normalization=None, combine=None):
+    def predict_proba(self, X, normalization=None, combine=None,
+                      use_decision_scores=False):
         """Compute probabilities of possible outcomes for samples in X.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The input samples.
         normalization: str
             How to transform the individual scores of each estimator. Passed to _collect_probas() internally.
         combine: str
             How to combine the transformed scores of each estimator
             'average' (or None), 'maximization', 'median', 'aom', 'mao', 'no'
-            If 'no', a list of underlying probas for each estimator is returned, without any combination. 
+            If 'no', a list of underlying probas for each estimator is returned, without any combination.
             The estimator order is the same as in initialization.
 
         Returns
         -------
         avg : array-like of shape (n_samples, n_classes)
             Weighted average probability for each class per sample.
         """
 
-        # Set default combination method to 'average', if not provided    
+        # Set default combination method to 'average', if not provided
         combine = combine if combine is not None else self.combine
-    
+
         check_is_fitted(self)
 
         # Collect transformed scores (i.e. normalized) from all estimators
-        scores_norm = self._collect_probas(X, normalization=normalization)
+        scores_norm = self._collect_probas(X, normalization=normalization, use_decision_scores=use_decision_scores)
 
         # If we don't combine the scores, just return now
         if combine == 'no':
             proba = scores_norm
 
         else:
             # Keep only the outlier scores (for class 1), since this is what pyod combiners expect
@@ -491,15 +505,15 @@
             elif combine == "aom":
                 proba = aom(scores_norm, int(len(self.estimators_) / 2))
             elif combine == "moa":
                 proba = moa(scores_norm, int(len(self.estimators_) / 2))
 
             # Add the first column, so the return has two columns like the normal predict_proba()'s
             proba = np.stack((1-proba, proba)).T
-            
+
         return proba
 
     def transform(self, X, voting=None, normalization=None, flatten_transform=None):
         """Return class labels or probabilities for X for each estimator.
 
         Parameters
         ----------
@@ -562,31 +576,31 @@
 # Provide memoized versions of predict(), predict_proba() and decision_function(), based on joblib
 #=======================
 
 # Decorators to turn exceptions into outputs and re-raise later
 
 def wrap_exception(func, excclass=Exception):
     """Decorator around to catch a possible Exception and return it as an output
-    
-    Given a function func() which returns `output`, 
+
+    Given a function func() which returns `output`,
     the decorated function wrap_exception(func) will return a tuple (output, exception):
     - either (output, None) if no exception was caught
     - either (None, exception) if exc `exception` was caught
 
     Args:
         func (__type__): Wrapped function
         excclass (class): Exception class to catch
     """
     def wrapper(*args, **kwargs):
         try:
             output = func(*args, **kwargs)
         except excclass as e:
             return None, e
         return output, None
-    
+
     return wrapper
 
 def unwrap_exception(func):
     """Decorator to raise an exception-turned-output by wrap_exception()
 
     Given a function func() which returns (output, exception), unwrap_exception will either
     - return output, if exception is None
@@ -663,15 +677,15 @@
         obj (_type_): Object
         X (_type_): Data to call predict() on
         idobj (_type_, optional): Alternative unique for `obj`, used for caching. Defaults to None.
 
     Returns:
         Result of obj.decision_function(X, **kwargs)
     """
-    
+
     logger.debug(f"Using cached decision_function() with id: {idobj}")
     return wrap_exception(obj.decision_function)(X, **kwargs)
 
 
 # Decorator to log a cache hit or miss
 
 def log_cache_hit(func, logger, funcname='function'):
@@ -681,15 +695,15 @@
         func (__type__): A joblib cached function returned by joblib.Memory.cache()
         logger (Logger): A logger object
         funcname (str, optional): Optional name of the function used for logging. Defaults to 'function'.
     """
     def wrapper(*args, **kwargs):
         cache_message = 'Cache hit' if func.check_call_in_cache(*args, **kwargs) else 'Cache new'
         logger.debug(cache_message + f' when calling cached {funcname}, arguments: {args}; {kwargs}' )
-        
+
         return func(*args, **kwargs)
     return wrapper
 
 
 # Internal cached function wrappers
 # By default, caching is disabled (location=None)
 # `obj` object is always ignored, hashing is actually done on a separate argument `idobj`
@@ -700,42 +714,42 @@
 # - this is called by _function_clf_xxx(), as wrap_exception(obj.xxx())
 # - this is cached by cache() decorator (caching the tuple (output, exception))
 # - log_cache_hit() just prints a cache hit or miss message ahead
 # - unwrap_exception() splits (output, exception) and raises back the exception, if any, or returns output
 
 _cached_predict_noobj = unwrap_exception(
                             log_cache_hit(
-                                joblib.Memory(location=None).cache(_function_clf_predict, ignore=['obj']), 
+                                joblib.Memory(location=None).cache(_function_clf_predict, ignore=['obj']),
                                 logger, 'predict() (ignore obj)'
                                 )
                         )
 
 _cached_predict_proba_noobj =   unwrap_exception(
                                     log_cache_hit(
-                                        joblib.Memory(location=None).cache(_function_clf_predict_proba, ignore=['obj']), 
+                                        joblib.Memory(location=None).cache(_function_clf_predict_proba, ignore=['obj']),
                                         logger, 'predict_proba() (ignore obj)'
                                     )
                                 )
 
 _cached_decision_function_noobj    =    unwrap_exception(
                                             log_cache_hit(
-                                                joblib.Memory(location=None).cache(_function_clf_decision_function, ignore=['obj']), 
+                                                joblib.Memory(location=None).cache(_function_clf_decision_function, ignore=['obj']),
                                                 logger, 'decision_function() (ignore obj)'
                                                 )
                                         )
 
 # Top-level cached functions. These are the functions to call from outside
 #       cached_predict(obj, X, ...)
 #       cached_predict_proba(obj, X, ...)
 #       cached_decision_function(obj, X, ...)
 
 def cached_predict(obj, X, **kwargs):
     """Calls obj.predict(X, **kwargs), with caching (memoization).
 
-    TF-based models are cached based on the model weights. 
+    TF-based models are cached based on the model weights.
     All other models are cached based on their params, as returned by get_params().
 
     Args:
         obj (_type_): Object
         X (_type_): Input data
 
     Returns:
@@ -751,15 +765,15 @@
         idobj = (obj.__class__, obj.get_params())
 
     return _cached_predict_noobj(obj, X, idobj=idobj, **kwargs)
 
 def cached_predict_proba(obj, X, **kwargs):
     """Calls obj.predict_proba(X, **kwargs), with caching (memoization).
 
-    TF-based models are cached based on the model weights. 
+    TF-based models are cached based on the model weights.
     All other models are cached based on their params, as returned by get_params().
 
     Args:
         obj (_type_): Object
         X (_type_): Input data
 
     Returns:
@@ -769,21 +783,21 @@
     logger.debug(f"Inside cached_predict_proba(), object type: {type(obj)}")
 
     # Decide what uniquely identifying traits to be used for caching. Whole objects might not be pickable (e.g. tensorflow)
     if isinstance(obj, Autoencoder) or isinstance(obj, VAE):
         idobj=(obj.__class__, obj.get_weights())
     else:
         idobj = (obj.__class__, obj.get_params())
-    
+
     return _cached_predict_proba_noobj(obj, X, idobj=idobj, **kwargs)
 
 def cached_decision_function(obj, X, **kwargs):
     """Calls obj.decision_function(X, **kwargs), with caching (memoization).
 
-    TF-based models are cached based on (class, model weights). 
+    TF-based models are cached based on (class, model weights).
     All other models are cached based on (class, params), params being returned by get_params().
 
     Args:
         obj (_type_): Object
         X (_type_): Input data
 
     Returns:
@@ -859,28 +873,28 @@
     global _cached_predict_noobj
     global _cached_predict_proba_noobj
     global _cached_decision_function_noobj
 
     # Recreate cached function handles, with new joblib arguments
     _cached_predict_noobj = unwrap_exception(
                                 log_cache_hit(
-                                    joblib.Memory(**kwargs).cache(_function_clf_predict, ignore=['obj']), 
+                                    joblib.Memory(**kwargs).cache(_function_clf_predict, ignore=['obj']),
                                     logger, 'predict() (ignore obj)'
                                     )
                             )
 
     _cached_predict_proba_noobj =   unwrap_exception(
                                         log_cache_hit(
-                                            joblib.Memory(**kwargs).cache(_function_clf_predict_proba, ignore=['obj']), 
+                                            joblib.Memory(**kwargs).cache(_function_clf_predict_proba, ignore=['obj']),
                                             logger, 'predict_proba() (ignore obj)'
                                         )
                                     )
 
     _cached_decision_function_noobj    =    unwrap_exception(
                                                 log_cache_hit(
-                                                    joblib.Memory(**kwargs).cache(_function_clf_decision_function, ignore=['obj']), 
+                                                    joblib.Memory(**kwargs).cache(_function_clf_decision_function, ignore=['obj']),
                                                     logger, 'decision_function() (ignore obj)'
                                                     )
-                                            )    
+                                            )
     logger.info(f"Set joblib cache parameters to {kwargs['location']}")
 
-#=======================
+#=======================
```

### Comparing `graphomaly-0.2.8/graphomaly.egg-info/PKG-INFO` & `graphomaly-0.3/graphomaly.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: graphomaly
-Version: 0.2.8
-Summary: software package for anomaly detection in graphs modeling financial transactions
+Version: 0.3
+Summary: Anomaly detection in graphs modeling financial transactions and computer networks.
 Home-page: https://gitlab.com/unibuc/graphomaly/graphomaly
-Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
+Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu, Nicolae Cleju, Andrei Iulian Hîji
 Author-email: graphomaly@fmi.unibuc.ro
 Project-URL: Bug Tracker, https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
-Keywords: anomaly detection,graphs,financial transactions,machine learning,security
+Keywords: anomaly detection,graphs,financial transactions,computer networks,abnormal behavior,machine learning,security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Graphomaly
 
-The Anti-Money Laundering (AML) tool. Find abnormal data in graph and network structures.
+Automatic tool for Anti-Money Laundering (AML) and  detecting abnormal behavior in computer networks. Find abnormal data in graph and network structures.
 
 Official package documentation [here](https://unibuc.gitlab.io/graphomaly/graphomaly/).
 
-This work was supported by the [Graphomaly Research Grant](http://graphomaly.upb.ro/).
+This work was initially supported by the [Graphomaly Research Grant](http://graphomaly.upb.ro/) and later partially supported by the [Netalert Research Grant](https://cs.unibuc.ro/~pirofti/netalert.html).
 
 ## Installation and setup
 Install via pip from the [PyPi repository](https://pypi.org/project/graphomaly/):
 ```
 pip install graphomaly
 ```
 
 or for the latest changes not yet in the official release:
 ```
 pip install git+https://gitlab.com/unibuc/graphomaly/graphomaly
 ```
 
+Install via docker from the [DockerHub repository](https://hub.docker.com/r/pirofti/graphomaly)
+```
+docker pull pirofti/graphomaly
+```
+For using the GPU pull the dedicated image:
+```
+docker pull pirofti/graphomaly:latest_gpu
+```
+
 ## Usage
 
 The package follows the [sklearn](https://scikit-learn.org/) API and can be included in your projects via
 ```
 from graphomaly.estimator import GraphomalyEstimator
 ```
 which will provide you with a standard scikit-learn estimator that you can use in your pipeline.
```

### Comparing `graphomaly-0.2.8/graphomaly.egg-info/SOURCES.txt` & `graphomaly-0.3/graphomaly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/setup.cfg` & `graphomaly-0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = graphomaly
-version = 0.2.8
-author = Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
+version = 0.3
+author = Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu, Nicolae Cleju, Andrei Iulian Hîji
 author_email = graphomaly@fmi.unibuc.ro
-description = software package for anomaly detection in graphs modeling financial transactions
+description = Anomaly detection in graphs modeling financial transactions and computer networks.
 long_description = file: README.md
 long_description_content_type = text/markdown
-keywords = anomaly detection, graphs, financial transactions, machine learning, security
+keywords = anomaly detection, graphs, financial transactions, computer networks, abnormal behavior, machine learning, security
 url = https://gitlab.com/unibuc/graphomaly/graphomaly
 project_urls = 
 	Bug Tracker = https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
```

### Comparing `graphomaly-0.2.8/tests/test_dl.py` & `graphomaly-0.3/tests/test_dl.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_fe_time.py` & `graphomaly-0.3/tests/test_fe_time.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_graphomaly_ctor.py` & `graphomaly-0.3/tests/test_graphomaly_ctor.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_synthetic.py` & `graphomaly-0.3/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_synthetic_gridsearch.py` & `graphomaly-0.3/tests/test_synthetic_gridsearch.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_synthetic_preprocessing.py` & `graphomaly-0.3/tests/test_synthetic_preprocessing.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_synthetic_voting.py` & `graphomaly-0.3/tests/test_synthetic_voting.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_tf_save.py` & `graphomaly-0.3/tests/test_tf_save.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.8/tests/test_voting.py` & `graphomaly-0.3/tests/test_voting.py`

 * *Files identical despite different names*


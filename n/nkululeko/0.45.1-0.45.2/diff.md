# Comparing `tmp/nkululeko-0.45.1.tar.gz` & `tmp/nkululeko-0.45.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.45.1.tar", last modified: Wed May 10 17:23:14 2023, max compression
+gzip compressed data, was "nkululeko-0.45.2.tar", last modified: Thu May 11 09:24:58 2023, max compression
```

## Comparing `nkululeko-0.45.1.tar` & `nkululeko-0.45.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-10 17:23:14.546830 nkululeko-0.45.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5725 2023-05-10 17:22:55.000000 nkululeko-0.45.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16754 2023-05-10 17:23:14.546830 nkululeko-0.45.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10476 2023-04-21 08:51:24.000000 nkululeko-0.45.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-10 17:23:14.546830 nkululeko-0.45.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.45.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.1/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.1/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.1/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-10 17:13:08.000000 nkululeko-0.45.1/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.1/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.1/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.1/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.45.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20426 2023-05-10 17:14:33.000000 nkululeko-0.45.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1873 2023-04-27 09:18:23.000000 nkululeko-0.45.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.45.1/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.1/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.1/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.1/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.1/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.1/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.1/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.1/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.1/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.1/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.1/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.1/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.1/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.1/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.1/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.1/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.1/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.1/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.1/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.1/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.1/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.1/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.1/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.1/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.1/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.1/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.1/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.1/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.1/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.1/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.1/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.45.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.1/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.45.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8174 2023-05-04 14:07:02.000000 nkululeko-0.45.1/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-10 17:23:14.546830 nkululeko-0.45.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16754 2023-05-10 17:23:14.000000 nkululeko-0.45.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-10 17:23:14.000000 nkululeko-0.45.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-10 17:23:14.000000 nkululeko-0.45.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-10 17:23:14.000000 nkululeko-0.45.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-10 17:23:14.000000 nkululeko-0.45.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-05-10 17:23:14.546830 nkululeko-0.45.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.45.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 09:24:58.971481 nkululeko-0.45.2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5810 2023-05-11 09:20:49.000000 nkululeko-0.45.2/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.2/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16700 2023-05-11 09:24:58.971481 nkululeko-0.45.2/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10337 2023-05-11 07:49:43.000000 nkululeko-0.45.2/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 09:24:58.971481 nkululeko-0.45.2/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.45.2/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.2/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.2/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.2/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.2/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-11 09:19:51.000000 nkululeko-0.45.2/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.2/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.2/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.2/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.45.2/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.2/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20481 2023-05-11 09:16:07.000000 nkululeko-0.45.2/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1934 2023-05-11 09:14:55.000000 nkululeko-0.45.2/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.45.2/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.2/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.2/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.2/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.2/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.2/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.2/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.2/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.2/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.2/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.2/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.2/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.2/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.2/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.2/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.2/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.2/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.2/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.2/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.2/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.2/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.2/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.2/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.2/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.2/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.2/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.2/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.2/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.2/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.2/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.2/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.2/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.2/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.45.2/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.2/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.2/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.2/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.2/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.2/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.45.2/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.2/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8381 2023-05-11 09:13:01.000000 nkululeko-0.45.2/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 09:24:58.971481 nkululeko-0.45.2/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16700 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.2/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-05-11 09:24:58.971481 nkululeko-0.45.2/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.45.2/setup.py
```

### Comparing `nkululeko-0.45.1/CHANGELOG.md` & `nkululeko-0.45.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 =========
 
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
+Version 0.45.2
+--------------
+* added sample_selection for sample distribution plots
+
 Version 0.45.1
 --------------
 * fixed dataframe.append bug
 
-
 Version 0.45.0
 --------------
 * added auddim as features
 * added FEATS store_format
 * added device use to feat_audmodel
 
 Version 0.44.1
```

### Comparing `nkululeko-0.45.1/LICENSE` & `nkululeko-0.45.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/PKG-INFO` & `nkululeko-0.45.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.1
+Version: 0.45.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -119,15 +119,14 @@
 * [Setting up a base nkululeko experiment](http://blog.syntheticspeech.de/2021/10/05/setting-up-a-base-nkululeko-experiment/)
 * [How to import a database](http://blog.syntheticspeech.de/2022/01/27/nkululeko-how-to-import-a-database/) 
 * [Comparing classifiers and features](http://blog.syntheticspeech.de/2021/10/05/nkululeko-comparing-classifiers-and-features/)
 * [Use Praat features](http://blog.syntheticspeech.de/2022/06/27/how-to-use-selected-features-from-praat-with-nkululeko/)
 * [Combine feature sets](http://blog.syntheticspeech.de/2022/06/30/how-to-combine-feature-sets-with-nkululeko/)
 * [Classifying continuous variables](http://blog.syntheticspeech.de/2022/01/26/nkululeko-classifying-continuous-variables/) 
 * [Try out / demo a trained model](http://blog.syntheticspeech.de/2022/01/24/nkululeko-try-out-demo-a-trained-model/) 
-* [Plot distributions of feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Perform cross database experiments](http://blog.syntheticspeech.de/2021/10/05/nkululeko-perform-cross-database-experiments/)
 * [Meta parameter optimization](http://blog.syntheticspeech.de/2021/09/03/perform-optimization-with-nkululeko/)
 * [How to set up wav2vec embedding](http://blog.syntheticspeech.de/2021/12/03/how-to-set-up-wav2vec-embedding-for-nkululeko/)
 * [How to soft-label a database](http://blog.syntheticspeech.de/2022/01/24/how-to-soft-label-a-database-with-nkululeko/) 
 * [Re-generate the progressing confusion matrix animation wit a different framerate](demos/plot_faster_anim.py)
 * [How to limit/filter a dataset](http://blog.syntheticspeech.de/2022/02/22/how-to-limit-a-dataset-with-nkululeko/)
 * [Specifying database disk location](http://blog.syntheticspeech.de/2022/02/21/specifying-database-disk-location-with-nkululeko/) 
@@ -213,19 +212,22 @@
 =========
 
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
+Version 0.45.2
+--------------
+* added sample_selection for sample distribution plots
+
 Version 0.45.1
 --------------
 * fixed dataframe.append bug
 
-
 Version 0.45.0
 --------------
 * added auddim as features
 * added FEATS store_format
 * added device use to feat_audmodel
 
 Version 0.44.1
```

### Comparing `nkululeko-0.45.1/README.md` & `nkululeko-0.45.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 * [Setting up a base nkululeko experiment](http://blog.syntheticspeech.de/2021/10/05/setting-up-a-base-nkululeko-experiment/)
 * [How to import a database](http://blog.syntheticspeech.de/2022/01/27/nkululeko-how-to-import-a-database/) 
 * [Comparing classifiers and features](http://blog.syntheticspeech.de/2021/10/05/nkululeko-comparing-classifiers-and-features/)
 * [Use Praat features](http://blog.syntheticspeech.de/2022/06/27/how-to-use-selected-features-from-praat-with-nkululeko/)
 * [Combine feature sets](http://blog.syntheticspeech.de/2022/06/30/how-to-combine-feature-sets-with-nkululeko/)
 * [Classifying continuous variables](http://blog.syntheticspeech.de/2022/01/26/nkululeko-classifying-continuous-variables/) 
 * [Try out / demo a trained model](http://blog.syntheticspeech.de/2022/01/24/nkululeko-try-out-demo-a-trained-model/) 
-* [Plot distributions of feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Perform cross database experiments](http://blog.syntheticspeech.de/2021/10/05/nkululeko-perform-cross-database-experiments/)
 * [Meta parameter optimization](http://blog.syntheticspeech.de/2021/09/03/perform-optimization-with-nkululeko/)
 * [How to set up wav2vec embedding](http://blog.syntheticspeech.de/2021/12/03/how-to-set-up-wav2vec-embedding-for-nkululeko/)
 * [How to soft-label a database](http://blog.syntheticspeech.de/2022/01/24/how-to-soft-label-a-database-with-nkululeko/) 
 * [Re-generate the progressing confusion matrix animation wit a different framerate](demos/plot_faster_anim.py)
 * [How to limit/filter a dataset](http://blog.syntheticspeech.de/2022/02/22/how-to-limit-a-dataset-with-nkululeko/)
 * [Specifying database disk location](http://blog.syntheticspeech.de/2022/02/21/specifying-database-disk-location-with-nkululeko/)
```

### Comparing `nkululeko-0.45.1/nkululeko/augment.py` & `nkululeko-0.45.2/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/augmenter.py` & `nkululeko-0.45.2/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/cacheddataset.py` & `nkululeko-0.45.2/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/dataset.py` & `nkululeko-0.45.2/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/dataset_csv.py` & `nkululeko-0.45.2/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/dataset_ravdess.py` & `nkululeko-0.45.2/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/demo.py` & `nkululeko-0.45.2/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/demo_predictor.py` & `nkululeko-0.45.2/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/experiment.py` & `nkululeko-0.45.2/nkululeko/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,25 +243,28 @@
             a[i] = random.choice(labels)
         df[self.target] = a
         return df
 
     def plot_distribution(self):
         """Plot the distribution of samples and speaker per target class and biological sex"""
         plot = Plots()
-        if self.util.exp_is_classification():
-            # self.df_train['labels'] = self.label_encoder.inverse_transform(self.df_train[self.target])
-            # if self.df_test.is_labeled:
-            #     self.df_test['labels'] = self.label_encoder.inverse_transform(self.df_test[self.target])
-            if self.df_test.shape[0] > 0:
-                plot.describe_df('dev_set', self.df_test, self.target, f'test_distplot')
-            plot.describe_df('train_set', self.df_train, self.target, f'train_distplot')
+        sample_selection = self.util.config_val('EXPL', 'sample_selection', 'all')
+        if sample_selection=='all':
+            df_labels = pd.concat([self.df_train, self.df_test])
+            self.util.copy_flags(self.df_train, df_labels)
+        elif sample_selection=='train':
+            df_labels = self.df_train
+            self.util.copy_flags(self.df_train, df_labels)
+        elif sample_selection=='test':
+            df_labels = self.df_test
+            self.util.copy_flags(self.df_test, df_labels)
         else:
-            if self.df_test.shape[0] > 0:
-                plot.describe_df('dev_set', self.df_test, self.target, f'test_distplot')
-            plot.describe_df('train_set', self.df_train, self.target, f'train_distplot')
+            self.util.error(f'unkown sample selection specifier {sample_selection}, should be [all | train | test]')
+
+        plot.describe_df(f'{sample_selection}_set', df_labels, self.target, f'{sample_selection}_distplot')
 
     def extract_test_feats(self):
         self.feats_test = pd.DataFrame()
         feats_name = "_".join(ast.literal_eval(glob_conf.config['DATA']['tests']))
         self.feature_extractor = FeatureExtractor() 
         self.feature_extractor.set_data(self.df_test, feats_name, 'test')
         self.feats_test = self.feature_extractor.extract()
@@ -299,37 +302,38 @@
     #     """Augment the train dataframe"""
     #     from nkululeko.augmenter import Augmenter
     #     augment_train = Augmenter(self.df_train)
     #     df_train_aug = augment_train.augment()
     #     self.df_train = self.df_train.append(df_train_aug)
 
 
-    def analyse_features(self):
+    def analyse_features(self, needs_feats):
         """
         Do a feature exploration
         
         """
 
         if self.util.config_val('EXPL', 'value_counts', False):
             self.plot_distribution()
-
+        if not needs_feats:
+            return
         sample_selection = self.util.config_val('EXPL', 'sample_selection', 'False')
         if sample_selection=='all':
             df_feats = pd.concat([self.feats_train, self.feats_test])
             df_labels = pd.concat([self.df_train, self.df_test])
         elif sample_selection=='train':
             df_feats = self.feats_train
             df_labels = self.df_train
         elif sample_selection=='test':
             df_feats = self.feats_test
             df_labels = self.df_test
         elif sample_selection=='False':
             pass
         else:
-            self.util.error(f'unkown feature_distribution specifier {sample_selection}, should be [all | train | test]')
+            self.util.error(f'unkown sample selection specifier {sample_selection}, should be [all | train | test]')
         if sample_selection in ('all', 'train', 'test'):
             feat_analyser = FeatureAnalyser(sample_selection, df_labels, df_feats)        
             feat_analyser.analyse()
 
         # check if a scatterplot should be done
         scatter_var = eval(self.util.config_val('EXPL', 'scatter', 'False'))
         if scatter_var:
```

### Comparing `nkululeko-0.45.1/nkululeko/explore.py` & `nkululeko-0.45.2/nkululeko/explore.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,21 @@
     util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
 
     plot_feats = eval(util.config_val('EXPL', 'feature_distributions', 'False'))
     tsne = eval(util.config_val('EXPL', 'tsne', 'False'))
     scatter = eval(util.config_val('EXPL', 'scatter', 'False'))
     model_type = util.config_val('EXPL', 'model', False)
     plot_tree = eval(util.config_val('EXPL', 'plot_tree', 'False'))
+    needs_feats = False
     if plot_feats or tsne or scatter or model_type or plot_tree: 
         # these investigations need features to explore
         expr.extract_feats()
-
+        needs_feats = True
     # explore
-    expr.analyse_features()
+    expr.analyse_features(needs_feats)
 
     print('DONE')
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
     main(cwd) # use this if you want to state the config file path on command line
```

### Comparing `nkululeko-0.45.1/nkululeko/feats_analyser.py` & `nkululeko-0.45.2/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_audmodel.py` & `nkululeko-0.45.2/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.45.2/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_clap.py` & `nkululeko-0.45.2/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_import.py` & `nkululeko-0.45.2/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_mld.py` & `nkululeko-0.45.2/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_opensmile.py` & `nkululeko-0.45.2/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_oxbow.py` & `nkululeko-0.45.2/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_praat.py` & `nkululeko-0.45.2/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_trill.py` & `nkululeko-0.45.2/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feats_wav2vec2.py` & `nkululeko-0.45.2/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feature_extractor.py` & `nkululeko-0.45.2/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/featureset.py` & `nkululeko-0.45.2/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/feinberg_praat.py` & `nkululeko-0.45.2/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/filter_data.py` & `nkululeko-0.45.2/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/loss_ccc.py` & `nkululeko-0.45.2/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/loss_softf1loss.py` & `nkululeko-0.45.2/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model.py` & `nkululeko-0.45.2/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_cnn.py` & `nkululeko-0.45.2/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_gmm.py` & `nkululeko-0.45.2/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_knn.py` & `nkululeko-0.45.2/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_knn_reg.py` & `nkululeko-0.45.2/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_mlp.py` & `nkululeko-0.45.2/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_mlp_regression.py` & `nkululeko-0.45.2/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/model_svm.py` & `nkululeko-0.45.2/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/modelrunner.py` & `nkululeko-0.45.2/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/nkululeko.py` & `nkululeko-0.45.2/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/plots.py` & `nkululeko-0.45.2/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/reporter.py` & `nkululeko-0.45.2/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/runmanager.py` & `nkululeko-0.45.2/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/scaler.py` & `nkululeko-0.45.2/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/test.py` & `nkululeko-0.45.2/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/test_predictor.py` & `nkululeko-0.45.2/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/nkululeko/util.py` & `nkululeko-0.45.2/nkululeko/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,8 +222,13 @@
             
     def get_store(self, name, format):
         if format == 'pkl':
             return pd.read_pickle(name)
         elif format == 'csv':
             return audformat.utils.read_csv(name)
         else:
-            self.error(f'unkown store format: {format}')
+            self.error(f'unkown store format: {format}')
+
+    def copy_flags(self, df_source, df_target):
+        df_target.is_labeled = df_source.is_labeled
+        df_target.got_gender = df_source.got_gender
+        df_target.got_speaker = df_source.got_speaker
```

### Comparing `nkululeko-0.45.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.45.2/nkululeko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.1
+Version: 0.45.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -119,15 +119,14 @@
 * [Setting up a base nkululeko experiment](http://blog.syntheticspeech.de/2021/10/05/setting-up-a-base-nkululeko-experiment/)
 * [How to import a database](http://blog.syntheticspeech.de/2022/01/27/nkululeko-how-to-import-a-database/) 
 * [Comparing classifiers and features](http://blog.syntheticspeech.de/2021/10/05/nkululeko-comparing-classifiers-and-features/)
 * [Use Praat features](http://blog.syntheticspeech.de/2022/06/27/how-to-use-selected-features-from-praat-with-nkululeko/)
 * [Combine feature sets](http://blog.syntheticspeech.de/2022/06/30/how-to-combine-feature-sets-with-nkululeko/)
 * [Classifying continuous variables](http://blog.syntheticspeech.de/2022/01/26/nkululeko-classifying-continuous-variables/) 
 * [Try out / demo a trained model](http://blog.syntheticspeech.de/2022/01/24/nkululeko-try-out-demo-a-trained-model/) 
-* [Plot distributions of feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Perform cross database experiments](http://blog.syntheticspeech.de/2021/10/05/nkululeko-perform-cross-database-experiments/)
 * [Meta parameter optimization](http://blog.syntheticspeech.de/2021/09/03/perform-optimization-with-nkululeko/)
 * [How to set up wav2vec embedding](http://blog.syntheticspeech.de/2021/12/03/how-to-set-up-wav2vec-embedding-for-nkululeko/)
 * [How to soft-label a database](http://blog.syntheticspeech.de/2022/01/24/how-to-soft-label-a-database-with-nkululeko/) 
 * [Re-generate the progressing confusion matrix animation wit a different framerate](demos/plot_faster_anim.py)
 * [How to limit/filter a dataset](http://blog.syntheticspeech.de/2022/02/22/how-to-limit-a-dataset-with-nkululeko/)
 * [Specifying database disk location](http://blog.syntheticspeech.de/2022/02/21/specifying-database-disk-location-with-nkululeko/) 
@@ -213,19 +212,22 @@
 =========
 
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
+Version 0.45.2
+--------------
+* added sample_selection for sample distribution plots
+
 Version 0.45.1
 --------------
 * fixed dataframe.append bug
 
-
 Version 0.45.0
 --------------
 * added auddim as features
 * added FEATS store_format
 * added device use to feat_audmodel
 
 Version 0.44.1
```

### Comparing `nkululeko-0.45.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.45.2/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.1/setup.cfg` & `nkululeko-0.45.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nkululeko
-version = 0.45.1
+version = 0.45.2
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers =
```


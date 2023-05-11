# Comparing `tmp/deepdriver-1.0.0.tar.gz` & `tmp/deepdriver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdriver-1.0.0.tar", last modified: Tue May  2 08:24:35 2023, max compression
+gzip compressed data, was "deepdriver-1.0.1.tar", last modified: Thu May 11 05:35:23 2023, max compression
```

## Comparing `deepdriver-1.0.0.tar` & `deepdriver-1.0.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.009162 deepdriver-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1068 2022-12-07 08:07:21.000000 deepdriver-1.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-17 09:07:55.000000 deepdriver-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-02 08:24:35.009162 deepdriver-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2022-12-07 05:37:47.000000 deepdriver-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.925181 deepdriver-1.0.0/deepdriver/
--rw-r--r--   0 root         (0) root         (0)     2379 2023-04-27 01:07:57.000000 deepdriver-1.0.0/deepdriver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.929180 deepdriver-1.0.0/deepdriver/cli/
--rw-r--r--   0 root         (0) root         (0)     7598 2023-03-03 05:46:36.000000 deepdriver-1.0.0/deepdriver/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     5531 2023-03-02 07:42:42.000000 deepdriver-1.0.0/deepdriver/cli/cli_ctx.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-03-03 05:46:36.000000 deepdriver-1.0.0/deepdriver/cli/cli_func.py
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-17 08:55:26.000000 deepdriver-1.0.0/deepdriver/client_secrets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.921182 deepdriver-1.0.0/deepdriver/intergration/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.929180 deepdriver-1.0.0/deepdriver/intergration/keras/
--rw-r--r--   0 root         (0) root         (0)      669 2023-01-09 04:01:37.000000 deepdriver-1.0.0/deepdriver/intergration/keras/keras.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.929180 deepdriver-1.0.0/deepdriver/intergration/torch/
--rw-r--r--   0 root         (0) root         (0)     5883 2023-02-27 05:51:16.000000 deepdriver-1.0.0/deepdriver/intergration/torch/torch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.941177 deepdriver-1.0.0/deepdriver/sdk/
--rw-r--r--   0 root         (0) root         (0)    18043 2023-04-27 00:59:22.000000 deepdriver-1.0.0/deepdriver/sdk/artifact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.949175 deepdriver-1.0.0/deepdriver/sdk/chart/
--rw-r--r--   0 root         (0) root         (0)      432 2023-01-30 05:49:33.000000 deepdriver-1.0.0/deepdriver/sdk/chart/bar.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/sdk/chart/chart.py
--rw-r--r--   0 root         (0) root         (0)     1592 2022-12-28 04:38:44.000000 deepdriver-1.0.0/deepdriver/sdk/chart/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-02-01 00:58:29.000000 deepdriver-1.0.0/deepdriver/sdk/chart/histogram.py
--rw-r--r--   0 root         (0) root         (0)      432 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/sdk/chart/line.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-01-09 04:01:37.000000 deepdriver-1.0.0/deepdriver/sdk/chart/roc_curve.py
--rw-r--r--   0 root         (0) root         (0)      441 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/sdk/chart/scatter.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-01-04 04:43:05.000000 deepdriver-1.0.0/deepdriver/sdk/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.957174 deepdriver-1.0.0/deepdriver/sdk/data_types/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-27 00:59:22.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/artifactEntryInfo.py
--rw-r--r--   0 root         (0) root         (0)      770 2023-04-27 00:59:22.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/artifactInfo.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-01-12 01:42:36.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/boundingBoxes.py
--rw-r--r--   0 root         (0) root         (0)     1249 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/dataFrame.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-01-17 07:38:01.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/experiment.py
--rw-r--r--   0 root         (0) root         (0)     5984 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/image.py
--rw-r--r--   0 root         (0) root         (0)     1278 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/media.py
--rw-r--r--   0 root         (0) root         (0)     6588 2023-04-27 01:46:07.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/run.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/table.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-11 05:06:20.000000 deepdriver-1.0.0/deepdriver/sdk/data_types/uploadInfo.py
--rw-r--r--   0 root         (0) root         (0)    12608 2023-05-02 06:02:23.000000 deepdriver-1.0.0/deepdriver/sdk/experiment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.973170 deepdriver-1.0.0/deepdriver/sdk/interface/
--rw-r--r--   0 root         (0) root         (0)     4487 2023-04-12 07:39:11.000000 deepdriver-1.0.0/deepdriver/sdk/interface/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-01-03 09:04:07.000000 deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface.proto
--rw-r--r--   0 root         (0) root         (0)     8738 2023-01-04 04:43:05.000000 deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14226 2023-01-04 04:43:05.000000 deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    13528 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    11588 2023-04-28 06:57:37.000000 deepdriver-1.0.0/deepdriver/sdk/interface/http_interface.py
--rw-r--r--   0 root         (0) root         (0)    17211 2023-05-02 06:46:12.000000 deepdriver-1.0.0/deepdriver/sdk/interface/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.965172 deepdriver-1.0.0/deepdriver/sdk/lib/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-01-09 04:01:37.000000 deepdriver-1.0.0/deepdriver/sdk/lib/lazyloader.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-04-26 06:06:23.000000 deepdriver-1.0.0/deepdriver/sdk/login.py
--rw-r--r--   0 root         (0) root         (0)     3527 2023-03-24 06:36:16.000000 deepdriver-1.0.0/deepdriver/sdk/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.965172 deepdriver-1.0.0/deepdriver/sdk/security/
--rw-r--r--   0 root         (0) root         (0)     3597 2023-04-05 07:02:49.000000 deepdriver-1.0.0/deepdriver/sdk/security/crypto.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-03-14 09:26:00.000000 deepdriver-1.0.0/deepdriver/sdk/setting.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-04-27 01:19:07.000000 deepdriver-1.0.0/deepdriver/sdk/util.py
--rw-r--r--   0 root         (0) root         (0)     8022 2023-02-28 05:40:47.000000 deepdriver-1.0.0/deepdriver/sdk/visualization.py
--rw-r--r--   0 root         (0) root         (0)     1379 2023-02-27 05:51:16.000000 deepdriver-1.0.0/deepdriver/sdk/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.001164 deepdriver-1.0.0/deepdriver/test/
--rw-r--r--   0 root         (0) root         (0)     8736 2023-02-27 05:51:16.000000 deepdriver-1.0.0/deepdriver/test/basic.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-03-07 08:49:42.000000 deepdriver-1.0.0/deepdriver/test/bokchi.pem
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.921182 deepdriver-1.0.0/deepdriver/test/cat_dog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.001164 deepdriver-1.0.0/deepdriver/test/cat_dog/cat/
--rw-r--r--   0 root         (0) root         (0)     7695 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/test/cat_dog/cat/cat.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.001164 deepdriver-1.0.0/deepdriver/test/cat_dog/dog/
--rw-r--r--   0 root         (0) root         (0)     7507 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/test/cat_dog/dog/dog.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.921182 deepdriver-1.0.0/deepdriver/test/cat_dog2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.001164 deepdriver-1.0.0/deepdriver/test/cat_dog2/cat/
--rw-r--r--   0 root         (0) root         (0)     7507 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/test/cat_dog2/cat/cat.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.001164 deepdriver-1.0.0/deepdriver/test/cat_dog2/dog/
--rw-r--r--   0 root         (0) root         (0)     7695 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/test/cat_dog2/dog/dog.png
--rw-r--r--   0 root         (0) root         (0)     1176 2023-03-07 08:49:42.000000 deepdriver-1.0.0/deepdriver/test/lgcns.crt
--rw-r--r--   0 root         (0) root         (0)    45787 2022-12-07 08:39:06.000000 deepdriver-1.0.0/deepdriver/test/plotly.ipynb
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-26 06:06:23.000000 deepdriver-1.0.0/deepdriver/test/setting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:35.005163 deepdriver-1.0.0/deepdriver/test/src/
--rw-r--r--   0 root         (0) root         (0)     7457 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/test/src/crpyt_test.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-01-19 06:21:19.000000 deepdriver-1.0.0/deepdriver/test/src/test.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-01-18 07:29:24.000000 deepdriver-1.0.0/deepdriver/test/test_alert.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/test/test_artifact.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-01-18 07:29:24.000000 deepdriver-1.0.0/deepdriver/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-04-26 06:06:23.000000 deepdriver-1.0.0/deepdriver/test/test_driver_init.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-02-27 05:51:16.000000 deepdriver-1.0.0/deepdriver/test/test_hpo.py
--rw-r--r--   0 root         (0) root         (0)     3587 2023-04-26 06:06:23.000000 deepdriver-1.0.0/deepdriver/test/test_https.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-02-27 05:51:16.000000 deepdriver-1.0.0/deepdriver/test/test_image.py
--rw-r--r--   0 root         (0) root         (0)     7988 2023-02-02 03:00:34.000000 deepdriver-1.0.0/deepdriver/test/test_intergration.py
--rw-r--r--   0 root         (0) root         (0)     3645 2023-04-10 08:48:27.000000 deepdriver-1.0.0/deepdriver/test/test_log.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-01-18 07:29:24.000000 deepdriver-1.0.0/deepdriver/test/test_multi_run.py
--rw-r--r--   0 root         (0) root         (0)     4905 2023-02-01 00:58:29.000000 deepdriver-1.0.0/deepdriver/test/test_visualize.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-02 08:24:22.000000 deepdriver-1.0.0/deepdriver/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:24:34.969171 deepdriver-1.0.0/deepdriver.egg-info/
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-02 08:24:34.000000 deepdriver-1.0.0/deepdriver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3862 2023-05-02 08:24:34.000000 deepdriver-1.0.0/deepdriver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 08:24:34.000000 deepdriver-1.0.0/deepdriver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-02 08:24:34.000000 deepdriver-1.0.0/deepdriver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-02 08:24:34.000000 deepdriver-1.0.0/deepdriver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-02 08:24:34.000000 deepdriver-1.0.0/deepdriver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      375 2023-04-26 10:55:40.000000 deepdriver-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 08:24:35.009162 deepdriver-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1756 2023-04-26 10:55:40.000000 deepdriver-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.399417 deepdriver-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1068 2022-12-07 08:07:21.000000 deepdriver-1.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-17 09:07:55.000000 deepdriver-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-11 05:35:23.399417 deepdriver-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2022-12-07 05:37:47.000000 deepdriver-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.339431 deepdriver-1.0.1/deepdriver/
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-04-27 01:07:57.000000 deepdriver-1.0.1/deepdriver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.343430 deepdriver-1.0.1/deepdriver/cli/
+-rw-r--r--   0 root         (0) root         (0)     7598 2023-03-03 05:46:36.000000 deepdriver-1.0.1/deepdriver/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2023-03-02 07:42:42.000000 deepdriver-1.0.1/deepdriver/cli/cli_ctx.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-03-03 05:46:36.000000 deepdriver-1.0.1/deepdriver/cli/cli_func.py
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-17 08:55:26.000000 deepdriver-1.0.1/deepdriver/client_secrets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.335432 deepdriver-1.0.1/deepdriver/intergration/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.343430 deepdriver-1.0.1/deepdriver/intergration/keras/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-01-09 04:01:37.000000 deepdriver-1.0.1/deepdriver/intergration/keras/keras.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.343430 deepdriver-1.0.1/deepdriver/intergration/torch/
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-02-27 05:51:16.000000 deepdriver-1.0.1/deepdriver/intergration/torch/torch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.351428 deepdriver-1.0.1/deepdriver/sdk/
+-rw-r--r--   0 root         (0) root         (0)    18043 2023-04-27 00:59:22.000000 deepdriver-1.0.1/deepdriver/sdk/artifact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.355428 deepdriver-1.0.1/deepdriver/sdk/chart/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-01-30 05:49:33.000000 deepdriver-1.0.1/deepdriver/sdk/chart/bar.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/sdk/chart/chart.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2022-12-28 04:38:44.000000 deepdriver-1.0.1/deepdriver/sdk/chart/confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-02-01 00:58:29.000000 deepdriver-1.0.1/deepdriver/sdk/chart/histogram.py
+-rw-r--r--   0 root         (0) root         (0)      432 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/sdk/chart/line.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-01-09 04:01:37.000000 deepdriver-1.0.1/deepdriver/sdk/chart/roc_curve.py
+-rw-r--r--   0 root         (0) root         (0)      441 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/sdk/chart/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-01-04 04:43:05.000000 deepdriver-1.0.1/deepdriver/sdk/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.367425 deepdriver-1.0.1/deepdriver/sdk/data_types/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-27 00:59:22.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/artifactEntryInfo.py
+-rw-r--r--   0 root         (0) root         (0)      770 2023-04-27 00:59:22.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/artifactInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-01-12 01:42:36.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/boundingBoxes.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/dataFrame.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-01-17 07:38:01.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/image.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/media.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-05-11 05:35:11.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/run.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/table.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-11 05:06:20.000000 deepdriver-1.0.1/deepdriver/sdk/data_types/uploadInfo.py
+-rw-r--r--   0 root         (0) root         (0)    12609 2023-05-11 05:35:11.000000 deepdriver-1.0.1/deepdriver/sdk/experiment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.375423 deepdriver-1.0.1/deepdriver/sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)     4487 2023-04-12 07:39:11.000000 deepdriver-1.0.1/deepdriver/sdk/interface/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-01-03 09:04:07.000000 deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface.proto
+-rw-r--r--   0 root         (0) root         (0)     8738 2023-01-04 04:43:05.000000 deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14226 2023-01-04 04:43:05.000000 deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    13528 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    11588 2023-04-28 06:57:37.000000 deepdriver-1.0.1/deepdriver/sdk/interface/http_interface.py
+-rw-r--r--   0 root         (0) root         (0)    17211 2023-05-02 06:46:12.000000 deepdriver-1.0.1/deepdriver/sdk/interface/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.371424 deepdriver-1.0.1/deepdriver/sdk/lib/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-01-09 04:01:37.000000 deepdriver-1.0.1/deepdriver/sdk/lib/lazyloader.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-04-26 06:06:23.000000 deepdriver-1.0.1/deepdriver/sdk/login.py
+-rw-r--r--   0 root         (0) root         (0)     3527 2023-03-24 06:36:16.000000 deepdriver-1.0.1/deepdriver/sdk/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.371424 deepdriver-1.0.1/deepdriver/sdk/security/
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-04-05 07:02:49.000000 deepdriver-1.0.1/deepdriver/sdk/security/crypto.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-03-14 09:26:00.000000 deepdriver-1.0.1/deepdriver/sdk/setting.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-04-27 01:19:07.000000 deepdriver-1.0.1/deepdriver/sdk/util.py
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-02-28 05:40:47.000000 deepdriver-1.0.1/deepdriver/sdk/visualization.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-02-27 05:51:16.000000 deepdriver-1.0.1/deepdriver/sdk/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.391419 deepdriver-1.0.1/deepdriver/test/
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-02-27 05:51:16.000000 deepdriver-1.0.1/deepdriver/test/basic.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-03-07 08:49:42.000000 deepdriver-1.0.1/deepdriver/test/bokchi.pem
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.335432 deepdriver-1.0.1/deepdriver/test/cat_dog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.391419 deepdriver-1.0.1/deepdriver/test/cat_dog/cat/
+-rw-r--r--   0 root         (0) root         (0)     7695 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/test/cat_dog/cat/cat.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.391419 deepdriver-1.0.1/deepdriver/test/cat_dog/dog/
+-rw-r--r--   0 root         (0) root         (0)     7507 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/test/cat_dog/dog/dog.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.335432 deepdriver-1.0.1/deepdriver/test/cat_dog2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.391419 deepdriver-1.0.1/deepdriver/test/cat_dog2/cat/
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/test/cat_dog2/cat/cat.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.391419 deepdriver-1.0.1/deepdriver/test/cat_dog2/dog/
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/test/cat_dog2/dog/dog.png
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-03-07 08:49:42.000000 deepdriver-1.0.1/deepdriver/test/lgcns.crt
+-rw-r--r--   0 root         (0) root         (0)    45787 2022-12-07 08:39:06.000000 deepdriver-1.0.1/deepdriver/test/plotly.ipynb
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-26 06:06:23.000000 deepdriver-1.0.1/deepdriver/test/setting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.395419 deepdriver-1.0.1/deepdriver/test/src/
+-rw-r--r--   0 root         (0) root         (0)     7457 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/test/src/crpyt_test.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-01-19 06:21:19.000000 deepdriver-1.0.1/deepdriver/test/src/test.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-01-18 07:29:24.000000 deepdriver-1.0.1/deepdriver/test/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/test/test_artifact.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-01-18 07:29:24.000000 deepdriver-1.0.1/deepdriver/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     4964 2023-05-11 05:35:11.000000 deepdriver-1.0.1/deepdriver/test/test_driver_init.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-02-27 05:51:16.000000 deepdriver-1.0.1/deepdriver/test/test_hpo.py
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-04-26 06:06:23.000000 deepdriver-1.0.1/deepdriver/test/test_https.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-02-27 05:51:16.000000 deepdriver-1.0.1/deepdriver/test/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     7988 2023-02-02 03:00:34.000000 deepdriver-1.0.1/deepdriver/test/test_intergration.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-04-10 08:48:27.000000 deepdriver-1.0.1/deepdriver/test/test_log.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-01-18 07:29:24.000000 deepdriver-1.0.1/deepdriver/test/test_multi_run.py
+-rw-r--r--   0 root         (0) root         (0)     4905 2023-02-01 00:58:29.000000 deepdriver-1.0.1/deepdriver/test/test_visualize.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-11 05:35:11.000000 deepdriver-1.0.1/deepdriver/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 05:35:23.371424 deepdriver-1.0.1/deepdriver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-11 05:35:23.000000 deepdriver-1.0.1/deepdriver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3862 2023-05-11 05:35:23.000000 deepdriver-1.0.1/deepdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 05:35:23.000000 deepdriver-1.0.1/deepdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-11 05:35:23.000000 deepdriver-1.0.1/deepdriver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-11 05:35:23.000000 deepdriver-1.0.1/deepdriver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 05:35:23.000000 deepdriver-1.0.1/deepdriver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      375 2023-04-26 10:55:40.000000 deepdriver-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 05:35:23.399417 deepdriver-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-04-26 10:55:40.000000 deepdriver-1.0.1/setup.py
```

### Comparing `deepdriver-1.0.0/LICENSE.txt` & `deepdriver-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/PKG-INFO` & `deepdriver-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdriver
-Version: 1.0.0
+Version: 1.0.1
 Summary: deepdriver experiments
 Home-page: https://bokchi.com
 Author: bokchi
 Author-email: molamola.bokchi@gmail.com
 Project-URL: bokchi git hub, https://github.com/molabokchi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepdriver-1.0.0/deepdriver/__init__.py` & `deepdriver-1.0.1/deepdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/cli/cli.py` & `deepdriver-1.0.1/deepdriver/cli/cli.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/cli/cli_ctx.py` & `deepdriver-1.0.1/deepdriver/cli/cli_ctx.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/cli/cli_func.py` & `deepdriver-1.0.1/deepdriver/cli/cli_func.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/intergration/keras/keras.py` & `deepdriver-1.0.1/deepdriver/intergration/keras/keras.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/intergration/torch/torch.py` & `deepdriver-1.0.1/deepdriver/intergration/torch/torch.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/artifact.py` & `deepdriver-1.0.1/deepdriver/sdk/artifact.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/chart/chart.py` & `deepdriver-1.0.1/deepdriver/sdk/chart/chart.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/chart/confusion_matrix.py` & `deepdriver-1.0.1/deepdriver/sdk/chart/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/chart/histogram.py` & `deepdriver-1.0.1/deepdriver/sdk/chart/histogram.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/chart/roc_curve.py` & `deepdriver-1.0.1/deepdriver/sdk/chart/roc_curve.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/config.py` & `deepdriver-1.0.1/deepdriver/sdk/config.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/artifactInfo.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/artifactInfo.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/boundingBoxes.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/boundingBoxes.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/dataFrame.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/dataFrame.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/experiment.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/experiment.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/image.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/image.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/media.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/media.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/run.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
 import time
 from assertpy import assert_that
 from typing import Dict, Tuple, TYPE_CHECKING
-
+from urllib.parse import urljoin
 from deepdriver import logger
 from deepdriver.sdk import util
 from deepdriver.sdk.interface import interface
 try:
     from deepdriver.sdk.interface.grpc_interface_pb2 import *
 except ImportError:
     pass
@@ -134,16 +134,20 @@
             "summary": {
                 "_runtime": time.time() - self.run_start_time,
                 "_step": self.log_step,
                 "_custom": _custom,
             },
         }
         resp = interface.finish(data)
+        if 'baseUrl' in resp and resp['baseUrl']:
+            report_url = urljoin(resp['baseUrl'], resp['shareLink'])
+        else:
+            report_url = urljoin(f"http://{interface.get_http_host_ip()}:9111", resp['shareLink'])
         if resp["result"] =="success":
             logger.info("run is finished!\n"
-                        f"report url={resp['shareLink']}\n")
+                        f"report url={report_url}\n")
         else:
             logger.error("run is not finished!\n")
         return resp["result"] == "success"
 
     def alert(self, title: str, level:str, message: str):
         return interface.send_alert(run_id=self.run_id, team_name=self.team_name, exp_name=self.exp_name, run_name=self.run_name, title=title, message=message, level=level)
```

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/table.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/table.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/data_types/uploadInfo.py` & `deepdriver-1.0.1/deepdriver/sdk/data_types/uploadInfo.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/experiment.py` & `deepdriver-1.0.1/deepdriver/sdk/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             return None
 
     rsp = interface.init(exp_name, team_name, run_name, config)
     if 'baseUrl' in rsp and rsp['baseUrl']:
         run_url = urljoin(rsp['baseUrl'], rsp['runUrl'])
     else:
         run_url = urljoin(f"http://{interface.get_http_host_ip()}:9111", rsp['runUrl'])
+
     run = Run(rsp["teamName"], rsp["expName"], rsp["runName"], rsp["runId"], run_url)
     logger.info("DeepDriver initialized\n"
                 f"Team Name={rsp['teamName']}\n"
                 f"Exp Name={rsp['expName']}\n"
                 f"Run Name={rsp['runName']}\n"
                 f"Run URL={run_url}"
                 )
```

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/file_upload.py` & `deepdriver-1.0.1/deepdriver/sdk/interface/file_upload.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface.proto` & `deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface.proto`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface_pb2.py` & `deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface_pb2.pyi` & `deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py` & `deepdriver-1.0.1/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/http_interface.py` & `deepdriver-1.0.1/deepdriver/sdk/interface/http_interface.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/interface/interface.py` & `deepdriver-1.0.1/deepdriver/sdk/interface/interface.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/lib/lazyloader.py` & `deepdriver-1.0.1/deepdriver/sdk/lib/lazyloader.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/login.py` & `deepdriver-1.0.1/deepdriver/sdk/login.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/run.py` & `deepdriver-1.0.1/deepdriver/sdk/run.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/security/crypto.py` & `deepdriver-1.0.1/deepdriver/sdk/security/crypto.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/setting.py` & `deepdriver-1.0.1/deepdriver/sdk/setting.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/util.py` & `deepdriver-1.0.1/deepdriver/sdk/util.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/visualization.py` & `deepdriver-1.0.1/deepdriver/sdk/visualization.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/sdk/watch.py` & `deepdriver-1.0.1/deepdriver/sdk/watch.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/basic.py` & `deepdriver-1.0.1/deepdriver/test/basic.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/bokchi.pem` & `deepdriver-1.0.1/deepdriver/test/bokchi.pem`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/cat_dog/cat/cat.png` & `deepdriver-1.0.1/deepdriver/test/cat_dog/cat/cat.png`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/cat_dog/dog/dog.png` & `deepdriver-1.0.1/deepdriver/test/cat_dog/dog/dog.png`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/cat_dog2/cat/cat.png` & `deepdriver-1.0.1/deepdriver/test/cat_dog2/cat/cat.png`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/cat_dog2/dog/dog.png` & `deepdriver-1.0.1/deepdriver/test/cat_dog2/dog/dog.png`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/lgcns.crt` & `deepdriver-1.0.1/deepdriver/test/lgcns.crt`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/plotly.ipynb` & `deepdriver-1.0.1/deepdriver/test/plotly.ipynb`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/src/crpyt_test.py` & `deepdriver-1.0.1/deepdriver/test/src/crpyt_test.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/src/test.py` & `deepdriver-1.0.1/deepdriver/test/src/test.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_alert.py` & `deepdriver-1.0.1/deepdriver/test/test_alert.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_artifact.py` & `deepdriver-1.0.1/deepdriver/test/test_artifact.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_config.py` & `deepdriver-1.0.1/deepdriver/test/test_config.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_driver_init.py` & `deepdriver-1.0.1/deepdriver/test/test_driver_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,20 @@
 
         # login success
         #deepdriver.setting(http_host=Setting.HTTP_HOST, grpc_host=Setting.GRPC_HOSt,  use_grpc_tls =True, use_https=True)
         #deepdriver.login_with()
         login_result = deepdriver.login(
             id=Setting.ID, pw=Setting.PW)
         self.assertTrue(login_result)
-        run = deepdriver.init(exp_name="test",
+        run = deepdriver.init(exp_name="test2",
                               config={'epoch': 10, 'batch_size': 64, 'hidden_layer': 128})
         image = deepdriver.Image("./cat_dog/cat/cat.png")
         print(image.to_json("image"))
         deepdriver.log({"image_str": image, "a": "b"})
+        deepdriver.finish()
 
     def test_host_setting(self):
         # http 로 시작하는 REST 주소
         deepdriver.setting(http_host="http://15.164.104.132:9011", grpc_host="15.164.104.132:19051")
         login_result = deepdriver.login(
             key=Setting.LOGIN_KEY)
```

### Comparing `deepdriver-1.0.0/deepdriver/test/test_hpo.py` & `deepdriver-1.0.1/deepdriver/test/test_hpo.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_https.py` & `deepdriver-1.0.1/deepdriver/test/test_https.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_image.py` & `deepdriver-1.0.1/deepdriver/test/test_image.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_intergration.py` & `deepdriver-1.0.1/deepdriver/test/test_intergration.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_log.py` & `deepdriver-1.0.1/deepdriver/test/test_log.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_multi_run.py` & `deepdriver-1.0.1/deepdriver/test/test_multi_run.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver/test/test_visualize.py` & `deepdriver-1.0.1/deepdriver/test/test_visualize.py`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/deepdriver.egg-info/PKG-INFO` & `deepdriver-1.0.1/deepdriver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdriver
-Version: 1.0.0
+Version: 1.0.1
 Summary: deepdriver experiments
 Home-page: https://bokchi.com
 Author: bokchi
 Author-email: molamola.bokchi@gmail.com
 Project-URL: bokchi git hub, https://github.com/molabokchi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepdriver-1.0.0/deepdriver.egg-info/SOURCES.txt` & `deepdriver-1.0.1/deepdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepdriver-1.0.0/setup.py` & `deepdriver-1.0.1/setup.py`

 * *Files identical despite different names*


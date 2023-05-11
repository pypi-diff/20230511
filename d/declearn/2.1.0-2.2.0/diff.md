# Comparing `tmp/declearn-2.1.0.tar.gz` & `tmp/declearn-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declearn-2.1.0.tar", last modified: Thu Mar  2 09:05:48 2023, max compression
+gzip compressed data, was "declearn-2.2.0.tar", last modified: Thu May 11 14:38:00 2023, max compression
```

## Comparing `declearn-2.1.0.tar` & `declearn-2.2.0.tar`

### file list

```diff
@@ -1,198 +1,267 @@
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.050454 declearn-2.1.0/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1231 2023-03-01 15:24:36.000000 declearn-2.1.0/.gitlab-ci.yml
--rw-r--r--   0 paandrey (670133) magnet    (5235)      560 2023-03-02 08:45:50.000000 declearn-2.1.0/AUTHORS
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11357 2023-02-13 09:41:03.000000 declearn-2.1.0/LICENSE
--rw-r--r--   0 paandrey (670133) magnet    (5235)    56831 2023-03-02 09:05:48.050454 declearn-2.1.0/PKG-INFO
--rw-r--r--   0 paandrey (670133) magnet    (5235)    42517 2023-03-01 15:24:36.000000 declearn-2.1.0/README.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.010455 declearn-2.1.0/declearn/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2290 2023-03-02 08:44:53.000000 declearn-2.1.0/declearn/__init__.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.014455 declearn-2.1.0/declearn/aggregator/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1363 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/aggregator/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4388 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/aggregator/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4372 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/aggregator/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4271 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/aggregator/_gma.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.014455 declearn-2.1.0/declearn/communication/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2497 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7050 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/_build.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.014455 declearn-2.1.0/declearn/communication/api/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      973 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/api/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8827 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/api/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13210 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/api/_server.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    16345 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/api/_service.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.018455 declearn-2.1.0/declearn/communication/grpc/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      804 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/grpc/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4811 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/grpc/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8877 2023-02-27 16:25:40.000000 declearn-2.1.0/declearn/communication/grpc/_server.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.018455 declearn-2.1.0/declearn/communication/grpc/protobufs/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1373 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/grpc/protobufs/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      263 2023-01-16 14:41:40.000000 declearn-2.1.0/declearn/communication/grpc/protobufs/message.proto
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1841 2023-01-16 14:41:40.000000 declearn-2.1.0/declearn/communication/grpc/protobufs/message_pb2.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5239 2023-01-16 14:41:40.000000 declearn-2.1.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.018455 declearn-2.1.0/declearn/communication/messaging/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1069 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/messaging/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6999 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/messaging/_messages.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1164 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/messaging/flags.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.018455 declearn-2.1.0/declearn/communication/websockets/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      798 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/websockets/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5973 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/websockets/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6469 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/websockets/_server.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3509 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/communication/websockets/_tools.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.022455 declearn-2.1.0/declearn/data_info/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2226 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/data_info/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8348 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/data_info/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4809 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/data_info/_fields.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.022455 declearn-2.1.0/declearn/dataset/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1310 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/dataset/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4930 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/dataset/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    23011 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/dataset/_inmemory.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5694 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/dataset/_sparse.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.022455 declearn-2.1.0/declearn/main/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1998 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    17567 2023-02-13 12:08:38.000000 declearn-2.1.0/declearn/main/_client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    28094 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/main/_server.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.022455 declearn-2.1.0/declearn/main/config/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1952 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/config/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7665 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/config/_dataclasses.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5572 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/config/_run_config.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7855 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/config/_strategy.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.022455 declearn-2.1.0/declearn/main/privacy/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      763 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/privacy/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9840 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/privacy/_dp_trainer.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.026455 declearn-2.1.0/declearn/main/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1006 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    21364 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/utils/_checkpoint.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5064 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/utils/_constraints.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7443 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/utils/_data_info.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3724 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/main/utils/_early_stop.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    14080 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/main/utils/_training.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.026455 declearn-2.1.0/declearn/metrics/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2465 2023-03-01 15:23:21.000000 declearn-2.1.0/declearn/metrics/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    12682 2023-03-01 15:24:08.000000 declearn-2.1.0/declearn/metrics/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8082 2023-02-17 11:09:43.000000 declearn-2.1.0/declearn/metrics/_classif.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5245 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/metrics/_mean.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11936 2023-03-01 08:51:06.000000 declearn-2.1.0/declearn/metrics/_roc_auc.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5036 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/metrics/_rsquared.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8191 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/metrics/_wrapper.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.026455 declearn-2.1.0/declearn/model/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1979 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/model/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1804 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/model/_utils.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.026455 declearn-2.1.0/declearn/model/api/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      847 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/model/api/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10467 2023-03-01 15:12:59.000000 declearn-2.1.0/declearn/model/api/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15357 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/api/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.030455 declearn-2.1.0/declearn/model/sklearn/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1103 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/model/sklearn/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3876 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/sklearn/_np_vec.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15073 2023-03-02 08:44:05.000000 declearn-2.1.0/declearn/model/sklearn/_sgd.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.030455 declearn-2.1.0/declearn/model/tensorflow/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1341 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/tensorflow/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15328 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/model/tensorflow/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10660 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/tensorflow/_optim.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10292 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/model/tensorflow/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.030455 declearn-2.1.0/declearn/model/tensorflow/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1482 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/model/tensorflow/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4424 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/tensorflow/utils/_gpu.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4016 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/tensorflow/utils/_loss.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5426 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/model/tensorflow/utils/_slices.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.030455 declearn-2.1.0/declearn/model/torch/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1294 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/torch/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    16768 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/torch/_model.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13030 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/torch/_optim.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6851 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/torch/_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.034455 declearn-2.1.0/declearn/model/torch/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      964 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/torch/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4608 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/model/torch/utils/_gpu.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.034455 declearn-2.1.0/declearn/optimizer/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1277 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/optimizer/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    19293 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/optimizer/_base.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.034455 declearn-2.1.0/declearn/optimizer/modules/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2056 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/optimizer/modules/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10910 2023-02-15 10:58:30.000000 declearn-2.1.0/declearn/optimizer/modules/_adaptive.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10878 2023-02-15 14:27:04.000000 declearn-2.1.0/declearn/optimizer/modules/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2317 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/optimizer/modules/_clipping.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6573 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/optimizer/modules/_momentum.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5970 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/optimizer/modules/_noise.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13022 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/optimizer/modules/_scaffold.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.034455 declearn-2.1.0/declearn/optimizer/regularizers/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1215 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/optimizer/regularizers/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6047 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/optimizer/regularizers/_api.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3385 2023-02-27 14:44:45.000000 declearn-2.1.0/declearn/optimizer/regularizers/_base.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)        0 2022-09-20 09:54:43.000000 declearn-2.1.0/declearn/py.typed
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.034455 declearn-2.1.0/declearn/test_utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1029 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/test_utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6688 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/test_utils/_assertions.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6040 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/test_utils/_gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2212 2023-02-28 13:10:59.000000 declearn-2.1.0/declearn/test_utils/_multiprocess.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6136 2023-03-01 15:24:36.000000 declearn-2.1.0/declearn/test_utils/_vectors.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1983 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/typing.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.038455 declearn-2.1.0/declearn/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3823 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/utils/__init__.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7741 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_dataclass.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4172 2023-03-01 15:13:00.000000 declearn-2.1.0/declearn/utils/_device_policy.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7024 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_json.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2656 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_logging.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1575 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_numpy.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10533 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_register.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6342 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_serialize.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    13623 2023-02-13 09:41:03.000000 declearn-2.1.0/declearn/utils/_toml_config.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.014455 declearn-2.1.0/declearn.egg-info/
--rw-r--r--   0 paandrey (670133) magnet    (5235)    56831 2023-03-02 09:05:47.000000 declearn-2.1.0/declearn.egg-info/PKG-INFO
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5012 2023-03-02 09:05:48.000000 declearn-2.1.0/declearn.egg-info/SOURCES.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)        1 2023-03-02 09:05:47.000000 declearn-2.1.0/declearn.egg-info/dependency_links.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)      525 2023-03-02 09:05:47.000000 declearn-2.1.0/declearn.egg-info/requires.txt
--rw-r--r--   0 paandrey (670133) magnet    (5235)        9 2023-03-02 09:05:47.000000 declearn-2.1.0/declearn.egg-info/top_level.txt
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.006455 declearn-2.1.0/examples/
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.038455 declearn-2.1.0/examples/adding_rmsprop/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4600 2023-02-13 09:41:03.000000 declearn-2.1.0/examples/adding_rmsprop/readme.md
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.042455 declearn-2.1.0/examples/heart-uci/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3538 2023-02-28 16:04:21.000000 declearn-2.1.0/examples/heart-uci/client.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3137 2023-02-13 09:41:03.000000 declearn-2.1.0/examples/heart-uci/data.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      916 2023-02-13 09:41:03.000000 declearn-2.1.0/examples/heart-uci/gen_ssl.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3135 2023-02-28 16:04:21.000000 declearn-2.1.0/examples/heart-uci/readme.md
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2029 2023-02-28 16:04:21.000000 declearn-2.1.0/examples/heart-uci/run.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4670 2023-02-28 16:04:21.000000 declearn-2.1.0/examples/heart-uci/server.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2810 2023-03-02 08:44:55.000000 declearn-2.1.0/pyproject.toml
--rw-r--r--   0 paandrey (670133) magnet    (5235)       38 2023-03-02 09:05:48.050454 declearn-2.1.0/setup.cfg
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.042455 declearn-2.1.0/test/
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.042455 declearn-2.1.0/test/communication/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1680 2023-02-13 09:41:03.000000 declearn-2.1.0/test/communication/conftest.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11813 2023-02-13 09:41:03.000000 declearn-2.1.0/test/communication/test_grpc.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6711 2023-02-28 13:10:59.000000 declearn-2.1.0/test/communication/test_routines.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     1213 2023-02-13 09:41:03.000000 declearn-2.1.0/test/conftest.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.042455 declearn-2.1.0/test/functional/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      975 2023-03-02 08:44:05.000000 declearn-2.1.0/test/functional/conftest.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11251 2023-03-02 08:44:05.000000 declearn-2.1.0/test/functional/test_main.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11968 2023-03-02 08:44:05.000000 declearn-2.1.0/test/functional/test_regression.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.042455 declearn-2.1.0/test/main/
--rw-r--r--   0 paandrey (670133) magnet    (5235)    19046 2023-02-13 09:41:03.000000 declearn-2.1.0/test/main/test_checkpoint.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    11884 2023-02-13 09:41:03.000000 declearn-2.1.0/test/main/test_train_manager.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6912 2023-02-13 09:41:03.000000 declearn-2.1.0/test/main/test_train_manager_dp.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.046455 declearn-2.1.0/test/metrics/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7320 2023-03-01 15:13:00.000000 declearn-2.1.0/test/metrics/metric_testing.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4532 2023-03-01 15:13:00.000000 declearn-2.1.0/test/metrics/test_binary_apr.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7386 2023-03-01 15:13:00.000000 declearn-2.1.0/test/metrics/test_binary_roc.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3936 2023-03-01 15:13:00.000000 declearn-2.1.0/test/metrics/test_mae_mse.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6907 2023-02-13 09:41:03.000000 declearn-2.1.0/test/metrics/test_metricset.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3328 2023-03-01 15:13:00.000000 declearn-2.1.0/test/metrics/test_multi_apr.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3503 2023-03-01 15:24:36.000000 declearn-2.1.0/test/metrics/test_rsquared.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.046455 declearn-2.1.0/test/model/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8764 2023-03-01 15:13:00.000000 declearn-2.1.0/test/model/model_testing.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6015 2023-03-01 15:13:00.000000 declearn-2.1.0/test/model/test_sksgd.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8260 2023-03-01 15:24:36.000000 declearn-2.1.0/test/model/test_tflow.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    10831 2023-03-01 15:13:00.000000 declearn-2.1.0/test/model/test_torch.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     7354 2023-03-01 15:13:00.000000 declearn-2.1.0/test/model/test_vector.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.046455 declearn-2.1.0/test/optimizer/
--rw-r--r--   0 paandrey (670133) magnet    (5235)      985 2023-02-13 09:41:03.000000 declearn-2.1.0/test/optimizer/conftest.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5234 2023-03-01 15:13:00.000000 declearn-2.1.0/test/optimizer/optim_testing.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     6356 2023-03-01 15:13:00.000000 declearn-2.1.0/test/optimizer/test_modules.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     3868 2023-02-13 09:41:03.000000 declearn-2.1.0/test/optimizer/test_noise.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)    15787 2023-03-01 15:13:00.000000 declearn-2.1.0/test/optimizer/test_optimizer.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     2189 2023-02-13 09:41:03.000000 declearn-2.1.0/test/optimizer/test_regularizers.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     4924 2023-03-01 15:24:36.000000 declearn-2.1.0/test/optimizer/test_scaffold.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     8569 2023-03-01 15:24:36.000000 declearn-2.1.0/test/optimizer/test_tflow_optim.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     9702 2023-03-01 15:13:00.000000 declearn-2.1.0/test/optimizer/test_torch_optim.py
-drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-03-02 09:05:48.050454 declearn-2.1.0/test/utils/
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5388 2023-02-13 09:41:03.000000 declearn-2.1.0/test/utils/test_json.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5454 2023-02-13 09:41:03.000000 declearn-2.1.0/test/utils/test_register.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)     5952 2023-02-13 09:41:03.000000 declearn-2.1.0/test/utils/test_serialize.py
--rw-r--r--   0 paandrey (670133) magnet    (5235)      817 2023-03-02 08:44:05.000000 declearn-2.1.0/tox.ini
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.838330 declearn-2.2.0/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1652 2023-05-04 10:01:14.000000 declearn-2.2.0/.gitlab-ci.yml
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      560 2023-04-26 13:33:08.000000 declearn-2.2.0/AUTHORS
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11357 2023-03-24 21:43:07.000000 declearn-2.2.0/LICENSE
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    19325 2023-05-11 14:38:00.838330 declearn-2.2.0/PKG-INFO
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4977 2023-05-04 10:01:14.000000 declearn-2.2.0/README.md
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2496 2023-05-10 13:11:18.000000 declearn-2.2.0/declearn/__init__.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/aggregator/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1705 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/aggregator/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5597 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/aggregator/_api.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4167 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/aggregator/_base.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4271 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/aggregator/_gma.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/communication/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3046 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8164 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/_build.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/communication/api/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1248 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     9146 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/_client.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    13310 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/_server.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    16342 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/api/_service.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn/communication/grpc/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1308 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/grpc/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4811 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/_client.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8877 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/communication/grpc/protobufs/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1398 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      263 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/message.proto
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1841 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5239 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/communication/messaging/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2409 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/messaging/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6999 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/messaging/_messages.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1410 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/messaging/flags.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/communication/websockets/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1143 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/websockets/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5973 2023-03-31 13:39:10.000000 declearn-2.2.0/declearn/communication/websockets/_client.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6514 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/communication/websockets/_server.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3509 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/communication/websockets/_tools.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/data_info/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2948 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/data_info/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8345 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/data_info/_base.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7274 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/data_info/_fields.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/dataset/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2119 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6510 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/dataset/_base.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    21645 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/_inmemory.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8307 2023-05-10 13:11:18.000000 declearn-2.2.0/declearn/dataset/_split_data.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.814331 declearn-2.2.0/declearn/dataset/examples/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1053 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/examples/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3532 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/examples/_heart_uci.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3770 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/examples/_mnist.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/dataset/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1693 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4866 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/_save_load.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6022 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/_sparse.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7065 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/dataset/utils/_split_classif.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2160 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    17375 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/_client.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    28091 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/_server.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/config/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1739 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/config/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7695 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/config/_dataclasses.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5589 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/config/_run_config.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7888 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/main/config/_strategy.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/privacy/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      904 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/privacy/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    10673 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/privacy/_dp_trainer.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/main/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2584 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    21365 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_checkpoint.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5064 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/main/utils/_constraints.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7442 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_data_info.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4007 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_early_stop.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    14134 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/main/utils/_training.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/metrics/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2861 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    12815 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_api.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8084 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_classif.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5249 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_mean.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11953 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_roc_auc.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5123 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_rsquared.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8185 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/metrics/_wrapper.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/model/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2949 2023-05-10 12:36:04.000000 declearn-2.2.0/declearn/model/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1803 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.818331 declearn-2.2.0/declearn/model/api/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1202 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/api/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11185 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/api/_model.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15988 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/api/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/haiku/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1062 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/haiku/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    20958 2023-05-11 13:44:56.000000 declearn-2.2.0/declearn/model/haiku/_model.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5742 2023-05-10 13:11:01.000000 declearn-2.2.0/declearn/model/haiku/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/haiku/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      857 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/haiku/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2751 2023-05-11 13:45:00.000000 declearn-2.2.0/declearn/model/haiku/utils/_gpu.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/sklearn/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1216 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/sklearn/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3957 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/sklearn/_np_vec.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15266 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/sklearn/_sgd.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/tensorflow/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1552 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15417 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/tensorflow/_model.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    10658 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/_optim.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    10302 2023-05-10 13:11:01.000000 declearn-2.2.0/declearn/model/tensorflow/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/tensorflow/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1881 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4455 2023-05-11 13:45:00.000000 declearn-2.2.0/declearn/model/tensorflow/utils/_gpu.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4016 2023-03-27 10:07:29.000000 declearn-2.2.0/declearn/model/tensorflow/utils/_loss.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5360 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/tensorflow/utils/_slices.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/torch/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1474 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/torch/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    16535 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/model/torch/_model.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    13026 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/torch/_optim.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6861 2023-05-10 13:11:01.000000 declearn-2.2.0/declearn/model/torch/_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/model/torch/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1094 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/model/torch/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4641 2023-05-11 13:45:00.000000 declearn-2.2.0/declearn/model/torch/utils/_gpu.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/optimizer/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1711 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    19710 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/_base.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3130 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/optimizer/modules/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2836 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11020 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_adaptive.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11323 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/modules/_api.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2318 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_clipping.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6600 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_momentum.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6031 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/modules/_noise.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15038 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/modules/_scaffold.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/optimizer/regularizers/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1453 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/regularizers/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6166 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/optimizer/regularizers/_api.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3405 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/optimizer/regularizers/_base.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)        0 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/py.typed
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.822331 declearn-2.2.0/declearn/quickrun/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1811 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/quickrun/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3938 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/quickrun/_config.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6652 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/quickrun/_parser.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     9386 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/quickrun/_run.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/declearn/test_utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1616 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/test_utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4704 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/test_utils/_argparse.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6683 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/test_utils/_assertions.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6040 2023-03-27 10:07:29.000000 declearn-2.2.0/declearn/test_utils/_gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1772 2023-04-26 13:33:08.000000 declearn-2.2.0/declearn/test_utils/_imports.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6524 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/test_utils/_vectors.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2096 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/typing.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/declearn/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5008 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/__init__.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7741 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/utils/_dataclass.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4174 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_device_policy.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7056 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_json.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2968 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_logging.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4938 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/utils/_multiprocess.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1575 2023-03-24 21:43:07.000000 declearn-2.2.0/declearn/utils/_numpy.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    10530 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_register.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6342 2023-05-04 10:01:14.000000 declearn-2.2.0/declearn/utils/_serialize.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15250 2023-05-10 12:05:04.000000 declearn-2.2.0/declearn/utils/_toml_config.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.810331 declearn-2.2.0/declearn.egg-info/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    19325 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/PKG-INFO
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6607 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/SOURCES.txt
+-rw-r--r--   0 paandrey (670133) magnet    (5235)        1 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/dependency_links.txt
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      117 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/entry_points.txt
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      641 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/requires.txt
+-rw-r--r--   0 paandrey (670133) magnet    (5235)        9 2023-05-11 14:38:00.000000 declearn-2.2.0/declearn.egg-info/top_level.txt
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/docs/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      181 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/SUMMARY.md
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/docs/api-reference/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      416 2023-05-10 13:10:41.000000 declearn-2.2.0/docs/api-reference/index.md
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.826331 declearn-2.2.0/docs/devs-guide/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      207 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3650 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/contribute.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2930 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/docs-build.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    10370 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/docs-style.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      746 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/index.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6994 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/devs-guide/tests.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3884 2023-05-10 13:09:13.000000 declearn-2.2.0/docs/index.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    12500 2023-05-10 13:11:18.000000 declearn-2.2.0/docs/quickstart.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4270 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/setup.md
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/docs/user-guide/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      230 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/SUMMARY.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4626 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/fl_process.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      799 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/index.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4989 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/local_dp.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5087 2023-05-04 10:01:14.000000 declearn-2.2.0/docs/user-guide/package.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     9739 2023-05-11 13:53:19.000000 declearn-2.2.0/docs/user-guide/usage.md
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.806331 declearn-2.2.0/examples/
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/adding_rmsprop/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4600 2023-03-24 21:43:07.000000 declearn-2.2.0/examples/adding_rmsprop/readme.md
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/heart-uci/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3698 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/heart-uci/client.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1642 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/heart-uci/data.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      916 2023-03-24 21:43:07.000000 declearn-2.2.0/examples/heart-uci/gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4214 2023-04-26 13:33:08.000000 declearn-2.2.0/examples/heart-uci/readme.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2191 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/heart-uci/run.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4801 2023-04-26 13:33:08.000000 declearn-2.2.0/examples/heart-uci/server.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/mnist/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3826 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/client.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      916 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/gen_ssl.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4882 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/readme.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2498 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/run.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5773 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist/server.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/examples/mnist_quickrun/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1628 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist_quickrun/config.toml
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    25127 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist_quickrun/mnist.ipynb
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      763 2023-05-11 14:00:17.000000 declearn-2.2.0/examples/mnist_quickrun/model.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1167 2023-05-04 10:01:14.000000 declearn-2.2.0/examples/mnist_quickrun/readme.md
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1046 2023-05-04 10:01:14.000000 declearn-2.2.0/mkdocs.yml
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3586 2023-05-11 13:57:25.000000 declearn-2.2.0/pyproject.toml
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/scripts/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5402 2023-05-04 10:01:14.000000 declearn-2.2.0/scripts/gen_docs.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)       38 2023-05-11 14:38:00.838330 declearn-2.2.0/setup.cfg
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/aggregator/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3011 2023-05-10 12:05:04.000000 declearn-2.2.0/test/aggregator/test_aggregator.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/communication/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1680 2023-03-24 21:43:07.000000 declearn-2.2.0/test/communication/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     9311 2023-05-04 10:01:14.000000 declearn-2.2.0/test/communication/test_exchanges.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11813 2023-03-24 21:43:07.000000 declearn-2.2.0/test/communication/test_grpc.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    16395 2023-05-04 10:01:14.000000 declearn-2.2.0/test/communication/test_server.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     1529 2023-05-04 10:01:14.000000 declearn-2.2.0/test/conftest.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/dataset/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2265 2023-05-04 10:01:14.000000 declearn-2.2.0/test/dataset/test_examples.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6439 2023-05-04 10:01:14.000000 declearn-2.2.0/test/dataset/test_utils.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.830330 declearn-2.2.0/test/functional/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      975 2023-04-26 13:33:08.000000 declearn-2.2.0/test/functional/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11484 2023-05-04 10:01:14.000000 declearn-2.2.0/test/functional/test_main.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2247 2023-05-10 12:05:04.000000 declearn-2.2.0/test/functional/test_quickrun.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    13698 2023-05-10 12:05:04.000000 declearn-2.2.0/test/functional/test_regression.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.834330 declearn-2.2.0/test/main/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    19053 2023-04-26 13:33:08.000000 declearn-2.2.0/test/main/test_checkpoint.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11884 2023-03-24 21:43:07.000000 declearn-2.2.0/test/main/test_train_manager.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6919 2023-04-26 13:33:08.000000 declearn-2.2.0/test/main/test_train_manager_dp.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.834330 declearn-2.2.0/test/metrics/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7320 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/metric_testing.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4532 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_binary_apr.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7386 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_binary_roc.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3936 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_mae_mse.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6907 2023-03-24 21:43:07.000000 declearn-2.2.0/test/metrics/test_metricset.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3328 2023-03-27 10:07:29.000000 declearn-2.2.0/test/metrics/test_multi_apr.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3503 2023-04-26 13:33:08.000000 declearn-2.2.0/test/metrics/test_rsquared.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.834330 declearn-2.2.0/test/model/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8764 2023-05-11 12:55:46.000000 declearn-2.2.0/test/model/model_testing.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    10752 2023-05-11 13:44:56.000000 declearn-2.2.0/test/model/test_haiku.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6022 2023-04-26 13:33:08.000000 declearn-2.2.0/test/model/test_sksgd.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8310 2023-05-11 07:58:34.000000 declearn-2.2.0/test/model/test_tflow.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    11226 2023-05-10 12:05:04.000000 declearn-2.2.0/test/model/test_torch.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     7354 2023-03-27 10:07:29.000000 declearn-2.2.0/test/model/test_vector.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.838330 declearn-2.2.0/test/optimizer/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      985 2023-03-24 21:43:07.000000 declearn-2.2.0/test/optimizer/conftest.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5234 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/optim_testing.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6356 2023-05-03 08:56:42.000000 declearn-2.2.0/test/optimizer/test_modules.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     3868 2023-03-24 21:43:07.000000 declearn-2.2.0/test/optimizer/test_noise.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15787 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/test_optimizer.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     2189 2023-03-24 21:43:07.000000 declearn-2.2.0/test/optimizer/test_regularizers.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     4924 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/test_scaffold.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     8569 2023-04-26 13:33:08.000000 declearn-2.2.0/test/optimizer/test_tflow_optim.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     9702 2023-03-27 10:07:29.000000 declearn-2.2.0/test/optimizer/test_torch_optim.py
+drwxr-xr-x   0 paandrey (670133) magnet    (5235)        0 2023-05-11 14:38:00.838330 declearn-2.2.0/test/utils/
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5388 2023-03-24 21:43:07.000000 declearn-2.2.0/test/utils/test_json.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     6623 2023-05-10 12:05:04.000000 declearn-2.2.0/test/utils/test_register.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)     5952 2023-03-24 21:43:07.000000 declearn-2.2.0/test/utils/test_serialize.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)    15940 2023-05-10 12:05:04.000000 declearn-2.2.0/test/utils/test_toml.py
+-rw-r--r--   0 paandrey (670133) magnet    (5235)      875 2023-05-10 12:05:04.000000 declearn-2.2.0/tox.ini
```

### Comparing `declearn-2.1.0/.gitlab-ci.yml` & `declearn-2.2.0/.gitlab-ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -8,33 +8,46 @@
 
 # Run the test suite using tox.
 # This job is called when commits are pushed to the main or a release branch.
 test:
   script:
     - pip install -U tox
     - tox -e py38
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: coverage.xml
+  coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
   rules:
     - if: ($CI_PIPELINE_SOURCE == "push") &&
           (($CI_COMMIT_BRANCH == "develop") || ($CI_COMMIT_BRANCH =~ "/^r\d\.\d+/"))
   tags:
     - ci.inria.fr
     - small
 
 # Run the test suite using tox, with --fulltest option.
 # This job is called on creation and pushes to non-Draft MRs.
 # It may also be launched manually upon pushes to Draft MRs or main/dev branch.
 test-full:
   script:
     - pip install -U tox
     - tox -e py38 -- --fulltest
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: coverage.xml
+  coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
   rules:
     - if: ($CI_PIPELINE_SOURCE == "merge_request_event") &&
           ($CI_MERGE_REQUEST_TITLE !~ /^Draft:.*/)
     - if: ($CI_PIPELINE_SOURCE == "merge_request_event") &&
           ($CI_MERGE_REQUEST_TITLE =~ /^Draft:.*/)
       when: manual
     - if: ($CI_PIPELINE_SOURCE == "push") &&
           (($CI_COMMIT_BRANCH == "develop") || ($CI_COMMIT_BRANCH =~ "/^r\d\.\d+/"))
       when: manual
+      allow_failure: true  # do not block the base "test" pipeline
   tags:
     - ci.inria.fr
     - small
```

### Comparing `declearn-2.1.0/AUTHORS` & `declearn-2.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/LICENSE` & `declearn-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/__init__.py` & `declearn-2.2.0/declearn/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,33 +25,34 @@
 
 Declearn provides with abstractions that enable algorithms to be written
 agnostic to the actual computation framework as well as with workable
 interfaces that cover some of the most popular frameworks, such as
 Scikit-Learn, TensorFlow and PyTorch.
 
 The package is organized into the following submodules:
-* aggregator:
+
+* [aggregator][declearn.aggregator]:
     Model updates aggregating API and implementations.
-* communication:
+* [communication][declearn.communication]:
     Client-Server network communications API and implementations.
-* data_info:
+* [data_info][declearn.data_info]:
     Tools to write and extend shareable metadata fields specifications.
-* dataset:
+* [dataset][declearn.dataset]:
     Data interfacing API and implementations.
-* main:
+* [main][declearn.main]:
     Main classes implementing a Federated Learning process.
-* metrics:
+* [metrics][declearn.metrics]:
     Iterative and federative evaluation metrics computation tools.
-* model:
+* [model][declearn.model]:
     Model interfacing API and implementations.
-* optimizer:
+* [optimizer][declearn.optimizer]:
     Framework-agnostic optimizer and algorithmic plug-ins API and tools.
-* typing:
+* [typing][declearn.typing]:
     Type hinting utils, defined and exposed for code readability purposes.
-* utils:
+* [utils][declearn.utils]:
     Shared utils used (extensively) across all of declearn.
 """
 
 from . import (
     aggregator,
     communication,
     data_info,
@@ -60,8 +61,8 @@
     metrics,
     model,
     optimizer,
     typing,
     utils,
 )
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

### Comparing `declearn-2.1.0/declearn/aggregator/__init__.py` & `declearn-2.2.0/declearn/aggregator/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,22 +13,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model updates aggregating API and implementations.
 
-An Aggregator is typically meant to be used on a round-wise basis by
+An `Aggregator` is typically meant to be used on a round-wise basis by
 the orchestrating server of a centralized federated learning process,
-to aggregate the client-wise model updated into a Vector that may then
-be used as "gradients" by the server's Optimizer to update the global
+to aggregate the client-wise model updated into a `Vector` that may then
+be used as "gradients" by the server's `Optimizer` to update the global
 model.
 
 This declearn submodule provides with:
-* Aggregator : abstract class defining an API for Vector aggregation
-* AveragingAggregator : average-based-aggregation Aggregator subclass
-* GradientMaskedAveraging : gradient Masked Averaging Aggregator subclass
+
+API tools
+---------
+
+* [Aggregator][declearn.aggregator.Aggregator]:
+    Abstract base class defining an API for Vector aggregation.
+* [list_aggregators][declearn.aggregator.list_aggregators]:
+    Return a mapping of registered Aggregator subclasses.
+
+
+Concrete classes
+----------------
+
+* [AveragingAggregator][declearn.aggregator.AveragingAggregator]:
+    Average-based-aggregation Aggregator subclass.
+* [GradientMaskedAveraging][declearn.aggregator.GradientMaskedAveraging]:
+    Gradient Masked Averaging Aggregator subclass.
 """
 
-from ._api import Aggregator
+from ._api import Aggregator, list_aggregators
 from ._base import AveragingAggregator
 from ._gma import GradientMaskedAveraging
```

### Comparing `declearn-2.1.0/declearn/aggregator/_api.py` & `declearn-2.2.0/declearn/aggregator/_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,26 +14,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model updates aggregation API."""
 
 from abc import ABCMeta, abstractmethod
-from typing import Any, ClassVar, Dict
+from typing import Any, ClassVar, Dict, Type, TypeVar
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Vector
-from declearn.utils import create_types_registry, register_type
+from declearn.utils import (
+    access_types_mapping,
+    create_types_registry,
+    register_type,
+)
 
 __all__ = [
     "Aggregator",
 ]
 
 
+T = TypeVar("T")
+
+
 @create_types_registry
 class Aggregator(metaclass=ABCMeta):
     """Abstract class defining an API for Vector aggregation.
 
     The aim of this abstraction (which itself operates on the Vector
     abstraction, so as to provide framework-agnostic algorithms) is
     to enable implementing arbitrary aggregation rules to turn local
@@ -46,56 +53,57 @@
     update the global model.
 
     Abstract
     --------
     The following attribute and method require to be overridden
     by any non-abstract child class of `Aggregator`:
 
-    name: str class attribute
+    - name: str class attribute
         Name identifier of the class (should be unique across existing
         Aggregator classes). Also used for automatic types-registration
         of the class (see `Inheritance` section below).
-    aggregate(updates: Dict[str, Vector], n_steps: Dict[str, int]) -> Vector:
+    - aggregate(updates: Dict[str, Vector], n_steps: Dict[str, int]) -> Vector:
         Aggregate input vectors into a single one.
         This is the main method for any `Aggregator`.
 
     Overridable
     -----------
-    get_config() -> Dict[str, Any]:
+    - get_config() -> Dict[str, Any]:
         Return a JSON-serializable configuration dict of an instance.
-    from_config(Dict[str, Any]) -> Aggregator:
+    - from_config(Dict[str, Any]) -> Aggregator:
         Classmethod to instantiate an Aggregator from a config dict.
 
     Inheritance
     -----------
     When a subclass inheriting from `Aggregator` is declared, it is
     automatically registered under the "Aggregator" group using its
     class-attribute `name`. This can be prevented by adding `register=False`
     to the inheritance specs (e.g. `class MyCls(Aggregator, register=False)`).
     See `declearn.utils.register_type` for details on types registration.
     """
 
     name: ClassVar[str] = NotImplemented
+    """Name identifier of the class, unique across Aggregator classes."""
 
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automatically type-register Aggregator subclasses."""
         super().__init_subclass__(**kwargs)
         if register:
             register_type(cls, cls.name, group="Aggregator")
 
     @abstractmethod
     def aggregate(
         self,
-        updates: Dict[str, Vector],
+        updates: Dict[str, Vector[T]],
         n_steps: Dict[str, int],  # revise: abstract~generalize kwargs use
-    ) -> Vector:
+    ) -> Vector[T]:
         """Aggregate input vectors into a single one.
 
         Parameters
         ----------
         updates: dict[str, Vector]
             Client-wise updates, as a dictionary with clients' names as
             string keys and updates as Vector values.
@@ -104,14 +112,19 @@
             the training round having produced the updates.
 
         Returns
         -------
         gradients: Vector
             Aggregated updates, as a Vector - treated as gradients by
             the server-side optimizer.
+
+        Raises
+        ------
+        TypeError
+            If the input `updates` are an empty dict.
         """
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
         """Return a JSON-serializable dict with this object's parameters."""
         return {}
@@ -119,7 +132,33 @@
     @classmethod
     def from_config(
         cls,
         config: Dict[str, Any],
     ) -> Self:
         """Instantiate an Aggregator from its configuration dict."""
         return cls(**config)
+
+
+def list_aggregators() -> Dict[str, Type[Aggregator]]:
+    """Return a mapping of registered Aggregator subclasses.
+
+    This function aims at making it easy for end-users to list and access
+    all available Aggregator classes at any given time. The returned dict
+    uses unique identifier keys, which may be used to specify the desired
+    algorithm as part of a federated learning process without going through
+    the fuss of importing and instantiating it manually.
+
+    Note that the mapping will include all declearn-provided plug-ins,
+    but also registered plug-ins provided by user or third-party code.
+
+    See also
+    --------
+    * [declearn.aggregator.Aggregator][]:
+        API-defining abstract base class for the aggregation algorithms.
+
+    Returns
+    -------
+    mapping:
+        Dictionary mapping unique str identifiers to `Aggregator` class
+        constructors.
+    """
+    return access_types_mapping("Aggregator")
```

### Comparing `declearn-2.1.0/declearn/aggregator/_base.py` & `declearn-2.2.0/declearn/aggregator/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """FedAvg-like mean-aggregation class."""
 
 from typing import Any, ClassVar, Dict, Optional
 
-from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.aggregator._api import Aggregator
 from declearn.model.api import Vector
 
 __all__ = [
     "AveragingAggregator",
 ]
@@ -72,21 +71,14 @@
         self,
     ) -> Dict[str, Any]:
         return {
             "steps_weighted": self.steps_weighted,
             "client_weights": self.client_weights,
         }
 
-    @classmethod
-    def from_config(
-        cls,
-        config: Dict[str, Any],
-    ) -> Self:
-        return cls(**config)
-
     def aggregate(
         self,
         updates: Dict[str, Vector],
         n_steps: Dict[str, int],
     ) -> Vector:
         if not updates:
             raise TypeError("Cannot aggregate an empty set of updates.")
```

### Comparing `declearn-2.1.0/declearn/aggregator/_gma.py` & `declearn-2.2.0/declearn/aggregator/_gma.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/__init__.py` & `declearn-2.2.0/declearn/communication/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,35 +18,43 @@
 """Submodule implementing client/server communications.
 
 This is done by  defining server-side and client-side network communication
 endpoints for federated learning processes, as well as suitable messages to
 be transmitted, and the available communication protocols.
 
 This module contains the following core submodules:
-* api:
+
+* [api][declearn.communication.api]:
     Base API to define client- and server-side communication endpoints.
-* messaging:
+* [messaging][declearn.communication.messaging]:
     Message dataclasses defining information containers to be exchanged
     between communication endpoints.
 
-It also exposes the following core utility functions:
-* build_client:
+It also exposes the following core utility functions and dataclasses:
+
+* [build_client][declearn.communication.build_client]:
     Instantiate a NetworkClient, selecting its subclass based on protocol name.
-* build_server:
+* [build_server][declearn.communication.build_server]:
     Instantiate a NetworkServer, selecting its subclass based on protocol name.
-* list_available_protocols:
+* [list_available_protocols][declearn.communication.list_available_protocols]:
     List the protocol names for which both a NetworkClient and NetworkServer
     classes are registered (hence available to `build_client`/`build_server`).
+* [NetworkClientConfig][declearn.communication.NetworkClientConfig]:
+    TOML-parsable dataclass for network clients' instantiation.
+* [NetworkServerConfig][declearn.communication.NetworkServerConfig]:
+    TOML-parsable dataclass for network servers' instantiation.
+
 
 Finally, it defines the following protocol-specific submodules, provided
 the associated third-party dependencies are available:
-* grpc:
+
+* [grpc][declearn.communication.grpc]:
     gRPC-based network communication endpoints.
     Requires the `grpcio` and `protobuf` third-party packages.
-* websockets:
+* [websockets][declearn.communication.websockets]:
     WebSockets-based network communication endpoints.
     Requires the `websockets` third-party package.
 """
 
 # Messaging and Communications API and base tools:
 from . import api, messaging
 from ._build import (
```

### Comparing `declearn-2.1.0/declearn/communication/_build.py` & `declearn-2.2.0/declearn/communication/_build.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,14 +82,19 @@
         communcations encryption.
     logger: logging.Logger or str or None, default=None,
         Logger to use, or name of a logger to set up using
         `declearn.utils.get_logger`. If None, use `type(client)-name`.
     **kwargs:
         Any valid additional keyword parameter may be passed as well.
         Refer to the target `NetworkClient` subclass for details.
+
+    Returns
+    -------
+    client: NetworkClient
+        NetworkClient communication endpoint instance.
     """
     protocol = protocol.strip().lower()
     try:
         cls = access_registered(name=protocol, group="NetworkClient")
     except KeyError as exc:
         raise_if_installable(protocol, exc)
         raise KeyError(
@@ -134,14 +139,19 @@
         If None but a password is needed, an input will be prompted.
     logger: logging.Logger or str or None, default=None,
         Logger to use, or name of a logger to set up with
         `declearn.utils.get_logger`. If None, use `type(server)`.
     **kwargs:
         Any valid additional keyword parameter may be passed as well.
         Refer to the target `NetworkServer` subclass for details.
+
+    Returns
+    -------
+    server: NetworkServer
+        NetworkServer communication endpoint instance.
     """
     # inherited signature; pylint: disable=too-many-arguments
     protocol = protocol.strip().lower()
     try:
         cls = access_registered(name=protocol, group="NetworkServer")
     except KeyError as exc:
         raise_if_installable(protocol, exc)
@@ -158,26 +168,52 @@
 BuildClientConfig = dataclass_from_func(build_client)
 
 
 BuildServerConfig = dataclass_from_func(build_server)
 
 
 class NetworkClientConfig(BuildClientConfig, TomlConfig):  # type: ignore
-    """TOML-parsable dataclass for network clients' instantiation."""
+    """TOML-parsable dataclass for network clients' instantiation.
+
+    This class enables parsing and bundling arguments to the
+    [build_client][declearn.communication.build_client] function
+    from a TOML config file (using the `from_toml` classmethod)
+    or from keyword arguments (using the `from_kwargs` one), and
+    calling that function using the `build_client` method.
+    """
 
     def build_client(self) -> NetworkClient:
-        """Build a NetworkClient from the wrapped parameters."""
+        """Build a NetworkClient from the wrapped parameters.
+
+        Returns
+        -------
+        client: NetworkClient
+            NetworkClient communication endpoint instance.
+        """
         return self.call()
 
 
 class NetworkServerConfig(BuildServerConfig, TomlConfig):  # type: ignore
-    """TOML-parsable dataclass for network servers' instantiation."""
+    """TOML-parsable dataclass for network servers' instantiation.
+
+    This class enables parsing and bundling arguments to the
+    [build_server][declearn.communication.build_server] function
+    from a TOML config file (using the `from_toml` classmethod)
+    or from keyword arguments (using the `from_kwargs` one), and
+    calling that function using the `build_server` method.
+    """
 
     def build_server(self) -> NetworkServer:
-        """Build a NetworkServer from the wrapped parameters."""
+        """Build a NetworkServer from the wrapped parameters.
+
+        Returns
+        -------
+        server: NetworkServer
+            NetworkServer communication endpoint instance.
+        """
         return self.call()
 
 
 def list_available_protocols() -> List[str]:
     """Return the list of available network protocols.
 
     List protocol names that are associated with both a registered
```

### Comparing `declearn-2.1.0/declearn/communication/api/__init__.py` & `declearn-2.2.0/declearn/communication/api/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,12 +15,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base API to define client- and server-side communication endpoints.
 
 This module provides `NetworkClient` and `NetworkServer`, two abstract
 base classes that are to be used as network communication endpoints for
-federated learning processes.
+federated learning processes:
+
+* [NetworkClient][declearn.communication.api.NetworkClient]:
+    Abstract class defining an API for client-side communication endpoints.
+* [NetworkServer][declearn.communication.api.NetworkServer]:
+    Abstract class defining an API for server-side communication endpoints.
 """
 
 from ._client import NetworkClient
 from ._server import NetworkServer
```

### Comparing `declearn-2.1.0/declearn/communication/api/_client.py` & `declearn-2.2.0/declearn/communication/api/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,36 +46,41 @@
     process, agnostic to the actual communication protocol in use.
 
     Instantiating a `NetworkClient` does not trigger a connection to
     the target server. To enable communicating with the server via a
     `NetworkClient` object, its `start` method must first be awaited
     and conversely, its `stop` method should be awaited to close the
     connection:
+    ```
     >>> client = ClientSubclass("example.domain.com:8765", "name", "cert_path")
     >>> await client.start()
     >>> try:
     >>>     client.register(data_info)
     >>>     ...
     >>> finally:
     >>>     await client.stop()
+    ```
 
     An alternative syntax to achieve the former is using the client
     object as an asynchronous context manager:
+    ```
     >>> async with ClientSubclass(...) as client:
     >>>     client.register(data_info)
     >>>     ...
+    ```
 
     Note that a declearn `NetworkServer` manages an allow-list of
     clients, which is defined during a registration phase of limited
     time, based on requests emitted through the `NetworkClient.register`
     method. Any message emitted using `NetworkClient.send_message` will
     probably be rejected by the server if the client has not registered.
     """
 
     protocol: ClassVar[str] = NotImplemented
+    """Protocol name identifier, unique across NetworkClient classes."""
 
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automate the type-registration of NetworkClient subclasses."""
@@ -176,15 +181,15 @@
         -------
         accepted: bool
             Whether the registration request was accepted by the server
             or not.
 
         Raises
         -------
-        TypeError:
+        TypeError
             If the server does not return a JoinReply message.
         """
         reply = await self._send_message(JoinRequest(self.name, data_info))
         # Case when a JoinReply was received.
         if isinstance(reply, JoinReply):
             self.logger.info(
                 "Registration was %saccepted: '%s'",
@@ -225,18 +230,18 @@
         Parameters
         ----------
         message: Message
             Message instance that is to be delivered to the server.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If the server emits an Error message in response to the
             message sent.
-        TypeError:
+        TypeError
             If the server returns a non-Empty message.
 
         Note
         ----
         The message sent here is designed to be received using the
         `NetworkServer.wait_for_messages` method.
         """
@@ -250,20 +255,25 @@
         raise TypeError(
             "Received an undue message type in response to the posted message."
         )
 
     async def check_message(self, timeout: Optional[int] = None) -> Message:
         """Retrieve the next message sent by the server.
 
+        Parameters
+        ----------
+        timeout: int or None, default=None
+            Optional timeout delay, after which the server will send an
+            Error message with `messaging.flags.CHECK_MESSAGE_TIMEOUT`
+            if no other message awaits collection by this client.
+
         Returns
         -------
-        action: str
-            Instruction for the client.
-        params: dict
-            Associated parameters, as a JSON-serializable dict.
+        message: Message
+            Message received from the server.
 
         Note
         ----
         The message received here is expected to have been sent
         using one of the following `NetorkServer` methods:
         `send_message`, `send_messages`, or `broadcast_message`.
         """
```

### Comparing `declearn-2.1.0/declearn/communication/api/_server.py` & `declearn-2.2.0/declearn/communication/api/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,37 +43,42 @@
     agnostic to the actual communication protocol in use.
 
     Instantiating a `NetworkServer` does not instantly serve the declearn
     messaging program on the selected host and port. To enable clients
     to connect to the server via a `NetworkServer` object, its `start`
     method must first be awaited, and conversely, its `stop` method
     should be awaited to close the connection:
+    ```
     >>> server = ServerSubclass(
     ...     "example.domain.com", 8765, "cert_path", "pkey_path"
     ... )
     >>> await server.start()
     >>> try:
     >>>     data_info = server.wait_for_clients(...)
     >>>     ...
     >>> finally:
     >>>     await server.stop()
+    ```
 
     An alternative syntax to achieve the former is using the server
     object as an asynchronous context manager:
+    ```
     >>> async with ServerSubclass(...) as server:
     >>>     data_info = server.wait_for_clients(...)
     >>>     ...
+    ```
 
     Note that a `NetworkServer` manages an allow-list of clients,
     which is defined based on `NetworkClient.register(...)`-emitted
     requests during a registration phase restricted to the context
     of the awaitable `wait_for_clients` method.
     """
 
     protocol: ClassVar[str] = NotImplemented
+    """Protocol name identifier, unique across NetworkServer classes."""
 
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automate the type-registration of NetworkServer subclasses."""
@@ -206,19 +211,18 @@
             Maximum number of clients authorized to register.
         timeout: int or None, default=None
             Optional maximum waiting time (in seconds) beyond which
             to close registration and either return or raise.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If the number of registered clients does not abide by the
             provided boundaries at the end of the process.
 
-
         Returns
         -------
         client_info: dict[str, dict[str, any]]
             A dictionary where the keys are the participants
             and the values are their information.
         """
         return await self.handler.wait_for_clients(
@@ -246,15 +250,15 @@
             has been collected by the client.
         timeout: int or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
-        asyncio.TimeoutError:
+        asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
             yet to be collected by at least one of the clients.
         """
         if clients is None:
             clients = self.client_names
         messages = {client: message for client in clients}
         await self.send_messages(messages, heartbeat, timeout)
@@ -277,15 +281,15 @@
             has been collected by the client.
         timeout: int or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
-        asyncio.TimeoutError:
+        asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
             yet to be collected by at least one of the clients.
         """
         routines = [
             self.send_message(message, client, heartbeat, timeout)
             for client, message in messages.items()
         ]
@@ -314,15 +318,15 @@
             has been collected by the client.
         timeout: int or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
-        asyncio.TimeoutError:
+        asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
             yet to be collected by the client.
         """
         await self.handler.send_message(message, client, heartbeat, timeout)
 
     async def wait_for_messages(
         self,
@@ -333,24 +337,24 @@
         """Wait for an ensemble of clients to have sent a message.
 
         Parameters
         ----------
         clients: set[str] or None, default=None
             Optional subset of registered clients, messages from
             whom to wait for. If None, set to `self.client_names`.
-        hearbeat: int, default=1
+        heartbeat: int, default=1
             Delay (in seconds) between verifications that a client
             has sent their message.
         timeout: int or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for messages and raise an asyncio.TimeoutError.
 
         Raises
         ------
-        asyncio.TimeoutError:
+        asyncio.TimeoutError
             If any of the clients has failed to deliver a message
             before `timeout` was reached.
 
         Returns
         -------
         messages: dict[str, Message]
             A dictionary where the keys are the clients' names and
```

### Comparing `declearn-2.1.0/declearn/communication/api/_service.py` & `declearn-2.2.0/declearn/communication/api/_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             has been collected by the client.
         timeout: int or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for collection and raise an asyncio.TimeoutError.
 
         Raises
         ------
-        asyncio.TimeoutError:
+        asyncio.TimeoutError
             If `timeout` is set and is reached while the message is
             yet to be collected by the client.
 
         Notes
         -----
         See the `post_message` method to synchronously post a message
         and move on without guarantees that it was collected.
@@ -332,15 +332,15 @@
             has been received from the client.
         timeout: int or None, default=None
             Optional maximum delay (in seconds) beyond which to stop
             waiting for a message and raise an asyncio.TimeoutError.
 
         Raises
         ------
-        asyncio.TimeoutError:
+        asyncio.TimeoutError
             If `timeout` is set and is reached while no message has
             been received from the client.
 
         Returns
         -------
         message: Message
             Collected message that was sent by `client`.
@@ -381,15 +381,15 @@
             Maximum number of clients authorized to register.
         timeout: int or None, default=None
             Optional maximum waiting time (in seconds) beyond which
             to close registration and either return or raise.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If the number of registered clients does not abide by the
             provided boundaries at the end of the process.
 
         Returns
         -------
         client_info: dict[str, dict[str, any]]
             A dictionary where the keys are the participants
```

### Comparing `declearn-2.1.0/declearn/communication/grpc/__init__.py` & `declearn-2.2.0/declearn/dataset/examples/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,12 +11,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""gRPC implementation of network communication endpoints."""
+"""Utils to fetch and prepare some open-source datasets.
 
-from . import protobufs
-from ._client import GrpcClient
-from ._server import GrpcServer
+Datasets
+--------
+* [load_heart_uci][declearn.dataset.examples.load_heart_uci]:
+    Load and/or download a pre-processed UCI heart disease dataset.
+* [load_mnist][declearn.dataset.examples.load_mnist]:
+    Load and/or download the MNIST digit-classification dataset.
+"""
+
+from ._heart_uci import load_heart_uci
+from ._mnist import load_mnist
```

### Comparing `declearn-2.1.0/declearn/communication/grpc/_client.py` & `declearn-2.2.0/declearn/communication/grpc/_client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/grpc/_server.py` & `declearn-2.2.0/declearn/communication/grpc/_server.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/grpc/protobufs/__init__.py` & `declearn-2.2.0/declearn/communication/grpc/protobufs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Load the gRPC backend code auto-generated from "message.proto".
 
 Instructions to re-generate the code:
+
 * From the commandline, with 'protobufs' as working directory, run:
-  python -m grpc_tools.protoc -I . --python_out=. \
-         --grpc_python_out=. ./message.proto
-  sed -i -E 's/^import.*_pb2/from . \0/' ./*_pb2*.py
+    - `python -m grpc_tools.protoc -I . --python_out=. \
+              --grpc_python_out=. ./message.proto`
+    - `sed -i -E 's/^import.*_pb2/from . \0/' ./*_pb2*.py`
+
 * On MAC OS, replace the second command with:
-  sed -i '' -E 's/^(import.*_pb2)/from . \1/' ./*_pb2*.py
+    - `sed -i '' -E 's/^(import.*_pb2)/from . \1/' ./*_pb2*.py`
 """
 
 try:
     from . import message_pb2
     from . import message_pb2_grpc
 except ImportError as err:
     raise ImportError(
```

### Comparing `declearn-2.1.0/declearn/communication/grpc/protobufs/message_pb2.py` & `declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py` & `declearn-2.2.0/declearn/communication/grpc/protobufs/message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/messaging/_messages.py` & `declearn-2.2.0/declearn/communication/messaging/_messages.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/messaging/flags.py` & `declearn-2.2.0/declearn/communication/messaging/flags.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Communication flags used in declearn communication backends."""
+"""Communication flags used in declearn communication backends.
+
+This module exposes the following flags, which are all str constants:
+
+- REGISTRATION_UNSTARTED
+- REGISTRATION_OPEN
+- REGISTRATION_CLOSED
+- REGISTERED_WELCOME
+- REGISTERED_ALREADY
+- CHECK_MESSAGE_TIMEOUT
+- INVALID_MESSAGE
+- REJECT_UNREGISTERED
+"""
 
 
 # Registration flags.
 REGISTRATION_UNSTARTED = "registration is not opened yet"
 REGISTRATION_OPEN = "registration is open"
 REGISTRATION_CLOSED = "registration is closed"
 REGISTERED_WELCOME = "welcome, you are now registered"
```

### Comparing `declearn-2.1.0/declearn/communication/websockets/__init__.py` & `declearn-2.2.0/declearn/model/haiku/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""WebSockets implementation of network communication endpoints."""
+"""Utils for jax backend support code.
 
-from ._client import WebsocketsClient
-from ._server import WebsocketsServer
+GPU/CPU backing device management utils:
+* select_device:
+    Select a backing device to use based on inputs and availability.
+"""
+
+from ._gpu import select_device
```

### Comparing `declearn-2.1.0/declearn/communication/websockets/_client.py` & `declearn-2.2.0/declearn/communication/websockets/_client.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/communication/websockets/_server.py` & `declearn-2.2.0/declearn/communication/websockets/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,9 +163,10 @@
 
     async def stop(
         self,
     ) -> None:
         """Stop the websockets server and purge information about clients."""
         if self._server is not None:
             self._server.close()
+            await self._server.wait_closed()
             self._server = None
         await self.handler.purge()
```

### Comparing `declearn-2.1.0/declearn/communication/websockets/_tools.py` & `declearn-2.2.0/declearn/communication/websockets/_tools.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/data_info/_base.py` & `declearn-2.2.0/declearn/data_info/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,24 +159,24 @@
         the individual dicts' fields.
         Values are the result of `DataInfoField.combine(...)` called
         on individual values, provided a `DataInfoField` subclass is
         associated with the field's name.
 
     Raises
     ------
-    KeyError:
+    KeyError
         If a field in `required_fields` is missing from at least one
         dict included in `clients_data_info`.
-    ValueError:
+    ValueError
         If any value of a shared field is invalid, or if values from
         a field are incompatible for combination.
 
     Warns
     -----
-    UserWarning:
+    UserWarning
         If one of the return fields has no corresponding registered
         `DataInfoField` specification class.
         In that case, return the list of individual values in lieu
         of aggregated value.
 
     Notes
     -----
```

### Comparing `declearn-2.1.0/declearn/dataset/_base.py` & `declearn-2.2.0/declearn/dataset/_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Dataset abstraction API."""
 
+import warnings
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
-from typing import Any, ClassVar, Iterator, Optional, Set
+from typing import Any, ClassVar, Iterator, List, Optional, Set, Tuple, Union
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.typing import Batch
 from declearn.utils import access_registered, create_types_registry, json_load
 
 __all__ = [
@@ -31,19 +32,54 @@
     "Dataset",
     "load_dataset_from_json",
 ]
 
 
 @dataclass
 class DataSpecs:
-    """Dataclass to wrap a dataset's metadata."""
+    """Dataclass to wrap a dataset's metadata.
+
+    Note
+    ----
+    The `n_features` attribute has been deprecated as of declearn 2.2
+    and will be removed in v2.4 and/or v3.0. It should therefore not
+    be used, whether at instantiation or afterwards. Please use the
+    `features_shape` attribute instead.
+    """
 
     n_samples: int
-    n_features: int
+    features_shape: Union[Tuple[Optional[int], ...], List[Optional[int]]]
     classes: Optional[Set[Any]] = None
+    data_type: Optional[str] = None
+    n_features: Optional[int] = None  # DEPRECATED as of declearn v2.2
+
+    def __post_init__(self):  # pragma: no cover
+        # future: remove this (declearn >=2.4)
+        if isinstance(self.features_shape, int):
+            self.features_shape = (self.features_shape,)
+            warnings.warn(
+                "'features_shape' has replaced now-deprecated 'n_features'"
+                " and should therefore be passed as a tuple or list.",
+                RuntimeWarning,
+                stacklevel=3,
+            )
+        if self.n_features is not None:
+            warnings.warn(
+                "'DataSepc.n_features' has been deprecated as of declearn v2.2"
+                " and should therefore no longer be used. It will be removed"
+                " in v2.4 and/or v3.0.",
+                RuntimeWarning,
+                stacklevel=3,
+            )
+            if self.features_shape[-1] != self.n_features:
+                raise ValueError(
+                    "Both 'features_shape' and deprecated 'n_features' were "
+                    "passed to 'DataSpecs.__init__', with incoherent values."
+                )
+        self.n_features = self.features_shape[-1]
 
 
 @create_types_registry
 class Dataset(metaclass=ABCMeta):
     """Abstract class defining an API to access training or testing data.
 
     A 'Dataset' is an interface towards data that exposes methods
```

### Comparing `declearn-2.1.0/declearn/dataset/_inmemory.py` & `declearn-2.2.0/declearn/dataset/_inmemory.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Dataset implementation to serve scikit-learn compatible in-memory data."""
 
-import functools
 import os
+import warnings
 from typing import Any, ClassVar, Dict, Iterator, List, Optional, Set, Union
 
 import numpy as np
-import pandas as pd  # type: ignore
+import pandas as pd
 from numpy.typing import ArrayLike
 from scipy.sparse import spmatrix  # type: ignore
 from sklearn.datasets import load_svmlight_file  # type: ignore
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.dataset._base import Dataset, DataSpecs
-from declearn.dataset._sparse import sparse_from_file, sparse_to_file
+from declearn.dataset.utils import load_data_array, save_data_array
 from declearn.typing import Batch
 from declearn.utils import json_dump, json_load, register_type
 
 __all__ = [
     "InMemoryDataset",
 ]
 
@@ -42,24 +42,24 @@
 
 
 @register_type(group="Dataset")
 class InMemoryDataset(Dataset):
     """Dataset subclass serving numpy(-like) memory-loaded data arrays.
 
     This subclass implements:
+
     * yielding (X, [y], [w]) batches matching the scikit-learn API,
       with data wrapped as numpy arrays, scipy sparse matrices,
       or pandas dataframes (or series for y and w)
     * loading the source data from which batches are derived
       fully in memory, with support for some standard file
       formats
 
     Note: future code refactoring may divide these functionalities
-          into two distinct base classes to articulate back into
-          this one.
+    into two distinct base classes to articulate back into this one.
 
     Attributes
     ----------
     data: data array
         Data array containing samples, with all input features
         (and optionally more columns).
     target: data array or None
@@ -76,23 +76,24 @@
     def __init__(
         self,
         data: Union[DataArray, str],
         target: Optional[Union[DataArray, str]] = None,
         s_wght: Optional[Union[DataArray, str]] = None,
         f_cols: Optional[Union[List[int], List[str]]] = None,
         expose_classes: bool = False,
+        expose_data_type: bool = False,
         seed: Optional[int] = None,
     ) -> None:
         """Instantiate the dataset interface.
 
         We thereafter use the term "data array" to designate
         an instance that is either a numpy ndarray, a pandas
         DataFrame or a scipy spmatrix.
 
-        See the `load_data_array` method for details
+        See the `load_data_array` function in dataset._utils for details
         on supported file formats.
 
         Parameters
         ----------
         data: data array or str
             Main data array which contains input features (and possibly
             more), or path to a dump file from which it is to be loaded.
@@ -112,25 +113,29 @@
             Optional list of columns in `data` to use as input features
             (other columns will not be included in the first array of
             the batches yielded by `self.generate_batches(...)`).
         expose_classes: bool, default=False
             Whether the dataset should be used for classification, in
             which case the unique values of `target` are exposed under
             `self.classes` and exported by `self.get_data_specs()`).
+        expose_data_type: bool, default=False
+            Whether the dataset should expose the data type , in
+            which case check if the type is unique and exposed it
+            under `self.data_type` and exported by `self.get_data_specs()`).
         seed: int or None, default=None
             Optional seed for the random number generator based on which
             the dataset is (optionally) shuffled when generating batches.
         """
         # arguments serve modularity; pylint: disable=too-many-arguments
         self._data_path = None  # type: Optional[str]
         self._trgt_path = None  # type: Optional[str]
         # Assign the main data array.
         if isinstance(data, str):
             self._data_path = data
-            data = self.load_data_array(data)
+            data = load_data_array(data)
         self.data = data
         # Assign the optional input features list.
         self.f_cols = f_cols
         # Assign the (optional) target data array.
         if isinstance(target, str):
             self._trgt_path = target
             if (
@@ -138,179 +143,126 @@
                 and target in self.data.columns
             ):
                 if f_cols is None:
                     self.f_cols = self.f_cols or list(self.data.columns)
                     self.f_cols.remove(target)  # type: ignore
                 target = self.data[target]
             else:
-                target = self.load_data_array(target)
+                target = load_data_array(target)
         self.target = target
         # Assign the (optional) sample weights data array.
         if isinstance(s_wght, str):
             self._wght_path = s_wght
             if isinstance(self.data, pd.DataFrame):
                 if s_wght in self.data.columns:
                     if f_cols is None:
                         self.f_cols = self.f_cols or list(self.data.columns)
                         self.f_cols.remove(s_wght)  # type: ignore
                     s_wght = self.data[s_wght]
             else:
-                s_wght = self.load_data_array(s_wght)
+                s_wght = load_data_array(s_wght)
         self.weights = s_wght
         # Assign the 'expose_classes' attribute.
         self.expose_classes = expose_classes
+        self.expose_data_type = expose_data_type
         # Assign a random number generator.
         self.seed = seed
         self._rng = np.random.default_rng(seed)
 
     @property
     def feats(
         self,
     ) -> DataArray:
         """Input features array."""
         if self.f_cols is None:
             return self.data
         if isinstance(self.data, pd.DataFrame):
             if isinstance(self.f_cols[-1], str):
-                return self.data.loc[:, self.f_cols]
-            return self.data.iloc[:, self.f_cols]
+                return self.data.loc[:, self.f_cols]  # type: ignore
+            return self.data.iloc[:, self.f_cols]  # type: ignore
         return self.data[:, self.f_cols]  # type: ignore
 
     @property
     def classes(self) -> Optional[Set[Any]]:
         """Unique target classes."""
         if (not self.expose_classes) or (self.target is None):
             return None
         if isinstance(self.target, pd.DataFrame):
-            return set(self.target.unstack().unique().tolist())
+            c_list = self.target.unstack().unique().tolist()  # type: ignore
+            return set(c_list)
         if isinstance(self.target, pd.Series):
             return set(self.target.unique().tolist())
         if isinstance(self.target, np.ndarray):
             return set(np.unique(self.target).tolist())
         if isinstance(self.target, spmatrix):
             return set(np.unique(self.target.tocsr().data).tolist())
         raise TypeError(
             f"Invalid 'target' attribute type: '{type(self.target)}'."
         )
 
+    @property
+    def data_type(self) -> Optional[str]:
+        """Unique data type."""
+        if not self.expose_data_type:
+            return None
+        if isinstance(self.data, pd.DataFrame):
+            dtypes = [str(t) for t in list(self.data.dtypes)]
+            if len(dtypes) > 1:
+                raise ValueError(
+                    "Cannot work with mixed data types:"
+                    "ensure the `data` attribute has unique dtype"
+                )
+            return dtypes[0]
+        if isinstance(self.data, (pd.Series, np.ndarray, spmatrix)):
+            return str(self.data.dtype)
+        raise TypeError(
+            f"Invalid 'data' attribute type: '{type(self.target)}'."
+        )
+
     @staticmethod
     def load_data_array(
         path: str,
         **kwargs: Any,
     ) -> DataArray:
         """Load a data array from a dump file.
 
-        Supported file extensions are:
-        .csv:
-            csv file, comma-delimited by default.
-            Any keyword arguments to `pandas.read_csv` may be passed.
-        .npy:
-            Non-pickle numpy array dump, created with `numpy.save`.
-        .sparse:
-            Scipy sparse matrix dump, created with the custom
-            `declearn.data.sparse.sparse_to_file` function.
-        .svmlight:
-            SVMlight sparse matrix and labels array dump.
-            Parse using `sklearn.load_svmlight_file`, and
-            return either features or labels based on the
-            `which` int keyword argument (default: 0, for
-            features).
-
-        Parameters
-        ----------
-        path: str
-            Path to the data array dump file.
-            Extension must be adequate to enable proper parsing;
-            see list of supported extensions above.
-        **kwargs:
-            Extension-type-based keyword parameters may be passed.
-            See above for details.
-
-        Returns
-        -------
-        data: numpy.ndarray or pandas.DataFrame or scipy.spmatrix
-            Reloaded data array.
+        As of declearn v2.2, this staticmethod is DEPRECATED in favor of
+        `declearn.dataset.utils.load_data_array`, which is now calls. It
+        will be removed in v2.4 and/or v3.0.
 
-        Raises
-        ------
-        TypeError:
-            If `path` is of unsupported extension.
-        Any exception raised by data-loading functions may also be
-        raised (e.g. if the file cannot be proprely parsed).
+        See [declearn.dataset.utils.load_data_array][] for more details.
         """
-        ext = os.path.splitext(path)[1]
-        if ext == ".csv":
-            return pd.read_csv(path, **kwargs)
-        if ext == ".npy":
-            return np.load(path, allow_pickle=False)
-        if ext == ".sparse":
-            return sparse_from_file(path)
-        if ext == ".svmlight":
-            which = kwargs.get("which", 0)
-            return load_svmlight_file(path)[which]
-        raise TypeError(f"Unsupported data array file extension: '{ext}'.")
+        warnings.warn(
+            "'InMemoryDataset.load_data_array' has been deprecated in favor"
+            " of `declearn.dataset.utils.load_data_array`. It will be removed"
+            " in version 2.4 and/or 3.0.",
+            category=DeprecationWarning,
+        )
+        return load_data_array(path, **kwargs)
 
     @staticmethod
     def save_data_array(
         path: str,
         array: Union[DataArray, pd.Series],
     ) -> str:
         """Save a data array to a dump file.
 
-        Supported types of data arrays are:
-        pandas.DataFrame or pandas.Series:
-            Dump to a comma-separated ".csv" file.
-        numpy.ndarray:
-            Dump to a non-pickle ".npy" file.
-        scipy.sparse.spmatrix:
-            Dump to a ".sparse" file, using a custom format
-            and `declearn.data.sparse.sparse_to_file`.
-
-        Parameters
-        ----------
-        path: str
-            Path to the file where to dump the array.
-            Appropriate file extension will be added when
-            not present (i.e. `path` may be a basename).
-        array: data array structure (see above)
-            Data array that needs dumping to file.
-            See above for supported types and associated
-            behaviours.
-
-        Returns
-        -------
-        path: str
-            Path to the created file dump, based on the input
-            `path` and the chosen file extension (see above).
+        As of declearn v2.2, this staticmethod is DEPRECATED in favor of
+        `declearn.dataset.utils.save_data_array`, which is now calls. It
+        will be removed in v2.4 and/or v3.0.
 
-        Raises
-        ------
-        TypeError:
-            If `array` is of unsupported type.
+        See [declearn.dataset.utils.save_data_array][] for more details.
         """
-        # Select a file extension and set up the array-dumping function.
-        if isinstance(array, (pd.DataFrame, pd.Series)):
-            ext = ".csv"
-            save = functools.partial(
-                array.to_csv, sep=",", encoding="utf-8", index=False
-            )
-        elif isinstance(array, np.ndarray):
-            ext = ".npy"
-            save = functools.partial(np.save, arr=array)
-        elif isinstance(array, spmatrix):
-            ext = ".sparse"
-            save = functools.partial(sparse_to_file, matrix=array)
-        else:
-            raise TypeError(f"Unsupported data array type: '{type(array)}'.")
-        # Ensure proper naming. Save the array. Return the path.
-        if not path.endswith(ext):
-            path += ext
-        os.makedirs(os.path.dirname(os.path.abspath(path)), exist_ok=True)
-        save(path)
-        return path
+        warnings.warn(
+            "'InMemoryDataset.save_data_array' has been deprecated in favor"
+            " of `declearn.dataset.utils.save_data_array`. It will be removed"
+            " in version 2.4 and/or 3.0.",
+            category=DeprecationWarning,
+        )
+        return save_data_array(path, array)
 
     @classmethod
     def from_svmlight(
         cls,
         path: str,
         f_cols: Optional[List[int]] = None,
         dtype: Union[str, np.dtype] = "float64",
@@ -356,23 +308,23 @@
         folder = os.path.dirname(path)
         info = {}  # type: Dict[str, Any]
         info["type"] = self._type_key
         # Optionally create data dumps. Record data dumps' paths.
         # fmt: off
         info["data"] = (
             self._data_path or
-            self.save_data_array(os.path.join(folder, "data"), self.data)
+            save_data_array(os.path.join(folder, "data"), self.data)
         )
         info["target"] = None if self.target is None else (
             self._trgt_path or
-            self.save_data_array(os.path.join(folder, "trgt"), self.target)
+            save_data_array(os.path.join(folder, "trgt"), self.target)
         )
         info["s_wght"] = None if self.weights is None else (
             self._wght_path or
-            self.save_data_array(os.path.join(folder, "wght"), self.weights)
+            save_data_array(os.path.join(folder, "wght"), self.weights)
         )
         # fmt: on
         info["f_cols"] = self.f_cols
         info["expose_classes"] = self.expose_classes
         info["seed"] = self.seed
         # Write the information to the JSON file.
         dump = {"name": self.__class__.__name__, "config": info}
@@ -411,16 +363,17 @@
 
     def get_data_specs(
         self,
     ) -> DataSpecs:
         """Return a DataSpecs object describing this dataset."""
         return DataSpecs(
             n_samples=self.feats.shape[0],
-            n_features=self.feats.shape[1],
+            features_shape=self.feats.shape[1:],
             classes=self.classes,
+            data_type=self.data_type,
         )
 
     def generate_batches(
         self,
         batch_size: int,
         shuffle: bool = False,
         drop_remainder: bool = True,
@@ -454,17 +407,19 @@
         inputs: data array
             Input features; scikit-learn's `X`.
         targets: data array or None
             Optional target labels or values; scikit-learn's `y`.
         weights: data array or None
             Optional sample weights; scikit-learn's `sample_weight`.
 
-        Note: in this context, a 'data array' is either a numpy array,
-              scipy sparse matrix, pandas dataframe or pandas series.
-        Note: batched arrays are aligned along their first axis.
+        Notes
+        -----
+        - In this context, a 'data array' is either a numpy array,
+          scipy sparse matrix, pandas dataframe or pandas series.
+        - Batched arrays are aligned along their first axis.
         """
         if poisson:
             order = self._poisson_sampling(batch_size, drop_remainder)
             # Enable slicing of the produced boolean mask in `_build_iterator`.
             batch_size = order.shape[1]  # n_samples
             order = order.flatten()
         else:
@@ -578,15 +533,18 @@
             If None, yield None as many times as `order` specifies it.
         batch_size: int
             Number of samples to include per batch.
         order: np.ndarray
             Array containing a pre-computed samples' ordering.
             Yield batches of samples drawn in that order from `data`.
 
-        Yield slices of `data`, or None values if `data` is None.
+        Yields
+        ------
+        batch: optional data array
+            Slice of `data`, or None if `data` is None.
         """
         if data is None:
             yield from (None for _ in range(0, len(order), batch_size))
         else:
             # Ensure slicing compatibility for pandas structures.
             if isinstance(data, (pd.DataFrame, pd.Series)):
                 data = data.values
```

### Comparing `declearn-2.1.0/declearn/dataset/_sparse.py` & `declearn-2.2.0/declearn/dataset/utils/_sparse.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Sparse matrix file dumping and loading utils, inspired by svmlight.
 
-The format used is mostly similar to the SVMlight one
-(see for example `sklearn.datasets.dump_svmlight_file`),
-but enables storing a single matrix rather than a (X, y)
-pair of arrays. It also records the input matrix's dtype
-and type of sparse format, which are thus restored when
-reloading - while the scikit-learn implementation always
-returns a CSR matrix and requires inputing the dtype.
-
-This implementation does not use any tricks (e.g. cython
-or interfacing an external c++ tool) to optimize dump or
-load runtimes, it may therefore be slower than using the
-scikit-learn functions or any third-party alternative.
+The format used is mostly similar to the SVMlight one (see for example
+`sklearn.datasets.dump_svmlight_file`), but enables storing a single
+matrix rather than a (X, y) pair of arrays. It also records the input
+matrix's dtype and type of sparse format, which are thus restored when
+reloading - while the scikit-learn implementation always returns a CSR
+matrix and requires inputing the dtype.
+
+This implementation does not use any tricks (e.g. cython or interfacing an
+external c++ tool) to optimize dump or load runtimes. It may therefore be
+slower than using the scikit-learn functions or any third-party alternative.
 """
 
 import json
 import os
 
 from scipy.sparse import (  # type: ignore
     bsr_matrix,
@@ -64,35 +62,39 @@
 
 def sparse_to_file(
     path: str,
     matrix: spmatrix,
 ) -> None:
     """Dump a scipy sparse matrix as a text file.
 
-    See function `sparse_from_file` to reload from the dump file.
+    See the [`sparse_from_file`][declearn.dataset.utils.sparse_from_file]
+    counterpart function to reload the dumped data from the created file.
 
     Parameters
     ----------
     path: str
         Path to the file where to store the sparse matrix.
         If the path does not end with a '.sparse' extension,
         one will be added automatically.
     matrix: scipy.sparse.spmatrix
         Sparse matrix that needs storing to file.
 
     Raises
     ------
-    TypeError if 'matrix' is of unsupported type, i.e. not
-    a BSR, CSC, CSR, COO, DIA, DOK or LIL sparse matrix.
-
-    Note: the format used is mostly similar to the SVMlight one
-    (see for example `sklearn.datasets.dump_svmlight_file`), but
-    enables storing a single matrix rather than a (X, y) pair of
-    arrays. It also records the input matrix's dtype and type of
-    sparse format, which are restored upon reloading.
+    TypeError
+        If 'matrix' is of unsupported type, i.e. not a BSR,
+        CSC, CSR, COO, DIA, DOK or LIL sparse matrix.
+
+    Note
+    ----
+    The format used is mostly similar to the SVMlight one (see for example
+    `sklearn.datasets.dump_svmlight_file`), but enables storing a single
+    matrix rather than a (X, y) pair of arrays. It also records the input
+    matrix's dtype and type of sparse format, which are restored when the
+    counterpart `sparse_from_file` function is used to reload it.
     """
     if os.path.splitext(path)[1] != ".sparse":
         path += ".sparse"
     # Identify the type of sparse matrix, and convert it to lil.
     name = SPARSE_TYPES.get(type(matrix))
     if name is None:
         raise TypeError(f"Unsupported sparse matrix type: '{type(matrix)}'.")
@@ -111,43 +113,45 @@
             row = " ".join(f"{i}:{v}" for i, v in zip(ind, val))
             file.write("\n" + row)
 
 
 def sparse_from_file(path: str) -> spmatrix:
     """Return a scipy sparse matrix loaded from a text file.
 
-    See function `sparse_to_file` to create reloadable dump files.
+    See the [`sparse_to_file`][declearn.dataset.utils.sparse_to_file]
+    counterpart function to create reloadable sparse data dump files.
 
     Parameters
     ----------
     path: str
         Path to the sparse matrix dump file.
 
     Returns
     -------
     matrix: scipy.sparse.spmatrix
         Sparse matrix restored from file, the exact type
         of which being defined by said file.
 
     Raises
     ------
-    KeyError:
+    KeyError
         If the file's header cannot be JSON-parsed or does not
         conform to the expected standard.
-    TypeError:
+    TypeError
         If the documented sparse matrix type is not supported,
         i.e. "bsr", "csv", "csc", "coo", "dia", "dok" or "lil".
 
 
-    Note: the format used is mostly similar to the SVMlight one
-    (see for example `sklearn.datasets.load_svmlight_file`), but
-    the file must store a single matrix rather than a (X, y) pair
-    of arrays. It must also record some metadata in its header,
-    which are notably used to restore the initial matrix's dtype
-    and type of sparse format.
+    Note
+    ----
+    The format used is mostly similar to the SVMlight one (see for example
+    `sklearn.datasets.load_svmlight_file`), but the file must store a single
+    matrix rather than a (X, y) pair of arrays. It must also record some
+    metadata in its header, which are notably used to restore the initial
+    matrix's dtype and type of sparse format.
     """
     with open(path, "r", encoding="utf-8") as file:
         # Read and parse the file's header.
         try:
             head = json.loads(file.readline())
         except json.JSONDecodeError as exc:
             raise KeyError("Invalid header for sparse matrix file.") from exc
@@ -156,12 +160,15 @@
         if head["stype"] not in SPARSE_TYPES.values():
             raise TypeError(f"Invalid sparse matrix type: '{head['stype']}'.")
         # Instantiate a lil_matrix abiding by the header's specs.
         lil = lil_matrix(tuple(head["shape"]), dtype=head["dtype"])
         cnv = int if lil.dtype.kind == "i" else float
         # Iteratively parse and fill-in row data.
         for rix, row in enumerate(file):
-            for field in row.strip(" \n").split(" "):
+            row = row.strip(" \n")
+            if not row:  # all-zeros row
+                continue
+            for field in row.split(" "):
                 ind, val = field.split(":")
                 lil[rix, int(ind)] = cnv(val)
     # Convert the matrix to its initial format and return.
     return getattr(lil, f"to{head['stype']}")()
```

### Comparing `declearn-2.1.0/declearn/main/__init__.py` & `declearn-2.2.0/declearn/main/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Main classes implementing a Federated Learning process.
 
 This module mainly implements the following two classes:
-* FederatedClient: Client-side main Federated Learning orchestrating class
-* FederatedServer: Server-side main Federated Learning orchestrating class
+
+* [FederatedClient][declearn.main.FederatedClient]:
+    Client-side main Federated Learning orchestrating class
+* [FederatedServer][declearn.main.FederatedServer]:
+    Server-side main Federated Learning orchestrating class
 
 This module also implements the following submodules, used by the former:
-* config:
+
+* [config][declearn.main.config]:
     Server-side dataclasses that specify a FL process's parameter.
-    The main class implemented here is `FLRunConfig`, that implements
-    parameters' parsing from python objets or from a TOML config file.
-* privacy:
+    The main classes implemented here are `FLRunConfig` and `FLOptimConfig`,
+    that implement parameters' parsing from python objets or from TOML files.
+* [privacy][declearn.main.privacy]:
     Differentially-Private training routine utils.
     The main class implemented here is `DPTrainingManager` that implements
     client-side DP-SGD training. This module is to be manually imported or
     lazy-imported by `FederatedClient`, and may trigger warnings or errors
     in the absence of the 'opacus' third-party dependency.
-* utils:
+* [utils][declearn.main.utils]:
     Various utils to the FL process.
     The main class of interest for end-users is `TrainingManager`, that
     implements client-side training and evaluation routines, and may
     therefore be leveraged in a non-FL setting or to implement other
     FL process routines than the centralized one defined here.
 """
```

### Comparing `declearn-2.1.0/declearn/main/_client.py` & `declearn-2.2.0/declearn/main/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         """Set up a Model and an Optimizer based on server instructions.
 
         Await server instructions (as an InitRequest message) and conduct
         initialization.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If initialization failed, either because the message was not
             received or was of incorrect type, or because instantiation
             of the objects it specifies failed.
 
         Returns
         -------
         model: Model
@@ -346,16 +346,14 @@
 
         If an exception is raised during the local process, wrap
         it as an Error message and send it to the server instead
         of raising it.
 
         Parameters
         ----------
-        manager: TrainingManager
-            Instance wrapping the model, optimizer and data to use.
         message: TrainRequest
             Instructions from the server regarding the training round.
         """
         assert self.trainmanager is not None
         # Run the training round.
         reply = self.trainmanager.training_round(message)
         # Send training results (or error message) to the server.
@@ -372,16 +370,14 @@
         of raising it.
 
         If a checkpointer is set, record the local loss, and the
         model weights received from the server.
 
         Parameters
         ----------
-        manager: TrainingManager
-            Instance wrapping the model and data to use.
         message: EvaluationRequest
             Instructions from the server regarding the evaluation round.
         """
         assert self.trainmanager is not None
         # Run the evaluation round.
         reply = self.trainmanager.evaluation_round(message)
         # Post-process the results.
```

### Comparing `declearn-2.1.0/declearn/main/_server.py` & `declearn-2.2.0/declearn/main/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         config: FLRunConfig
             Container instance wrapping hyper-parameters that specify
             the planned federated learning process, including clients
             registration ones as a RegisterConfig dataclass instance.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             In case any of the clients returned an Error message rather
             than an Empty ping-back message. Send CancelTraining to all
             clients before raising.
         """
         # Gather the RegisterConfig instance from the main FLRunConfig.
         regst_cfg = config.register
         # Wait for clients to register and process their data information.
@@ -277,15 +277,15 @@
         ----------
         clients_data_info: dict[str, dict[str, any]]
             Client-wise data-info dict, that are to be aggregated
             and passed to the global model for initialization.
 
         Raises
         ------
-        AggregationError:
+        AggregationError
             In case (some of) the clients' data info is invalid, or
             incompatible. Send CancelTraining to all clients before
             raising.
         """
         fields = self.model.required_data_info  # revise: add optimizer, etc.
         # Try aggregating the input data_info.
         try:
@@ -318,15 +318,15 @@
             Type of message that clients are expected to send.
         context: str
             Context of the results collection (e.g. "training" or
             "evaluation"), used in logging or error messages.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If any client sent an incorrect message or reported
             failure to conduct the evaluation step properly.
             Send CancelTraining to all clients before raising.
 
         Returns
         -------
         results: dict[str, `msgtype`]
```

### Comparing `declearn-2.1.0/declearn/main/config/__init__.py` & `declearn-2.2.0/declearn/main/config/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,30 +19,28 @@
 
 This submodule exposes dataclasses that group, document and facilitate
 parsing (from instances, config dicts and/or TOML files) elements that
 are required to specify a Federated Learning process from the server's
 side.
 
 The main classes implemented here are:
-* FLRunConfig   : federated learning orchestration hyper-parameters
-* FLOptimConfig : federated optimization strategy
-
-The following dataclasses are articulated by `FLRunConfig`:
-* EvaluateConfig : hyper-parameters for an evaluation round
-* RegisterConfig : hyper-parameters for clients registration
-* TrainingConfig : hyper-parameters for a training round
 
+* [FLRunConfig][declearn.main.config.FLRunConfig]:
+    Federated learning orchestration hyper-parameters.
+* [FLOptimConfig][declearn.main.config.FLOptimConfig]:
+    Federated optimization strategy.
 
-This submodule exposes dataclasses that group and document server-side
-hyper-parameters that specify a Federated Learning process, as well as
-a main class designed to act as a container and a parser for all these,
-that may be instantiated from python objects or from a TOML file.
+The following dataclasses are articulated by `FLRunConfig`:
 
-In other words, `FLRunConfig` in the key class implemented here, while
-the other exposed dataclasses are already articulated and used by it.
+* [EvaluateConfig][declearn.main.config.EvaluateConfig]:
+    Hyper-parameters for an evaluation round.
+* [RegisterConfig][declearn.main.config.RegisterConfig]:
+    Hyper-parameters for clients registration.
+* [TrainingConfig][declearn.main.config.TrainingConfig]:
+    Hyper-parameters for a training round.
 """
 
 from ._dataclasses import (
     EvaluateConfig,
     PrivacyConfig,
     RegisterConfig,
     TrainingConfig,
```

### Comparing `declearn-2.1.0/declearn/main/config/_dataclasses.py` & `declearn-2.2.0/declearn/main/config/_dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,20 @@
     """Dataclass wrapping parameters to set up local differential privacy.
 
     The parameters wrapped by this class specify the DP-SGD algorithm [1],
     providing with a budget, an accountant method, a sensitivity clipping
     threshold, and RNG-related parameters for the noise-addition module.
 
     Accountants supported by Opacus 1.2.0 include:
+
     * rdp : Renyi-DP accountant, see [1]
     * gdp : Gaussian-DP, see [2]
     * prv : Privacy loss Random Variables privacy accountant, see [3]
 
-    Note : for more details, refer to the Opacus source code and the
+    Note: for more details, refer to the Opacus source code and the
     doctrings of each accountant. See
     https://github.com/pytorch/opacus/tree/main/opacus/accountants
 
     Attributes
     ----------
     budget: (float, float)
         Target total privacy budget per client, expressed in terms of
@@ -174,21 +175,24 @@
         This is significantly slower than using the default numpy RNG.
     seed: int or None
         Optional seed to the noise-addition module's RNG.
         Unused if `safe_mode=True`.
 
     References
     ----------
-    [1] Abadi et al, 2016.
+    - [1]
+        Abadi et al, 2016.
         Deep Learning with Differential Privacy.
         https://arxiv.org/abs/1607.00133
-    [2] Dong et al, 2019.
+    - [2]
+        Dong et al, 2019.
         Gaussian Differential Privacy.
         https://arxiv.org/abs/1905.02383
-    [3] Gopi et al, 2021.
+    - [3]
+        Gopi et al, 2021.
         Numerical Composition of Differential Privacy.
         https://arxiv.org/abs/2106.02848
     """
 
     budget: Tuple[float, float]
     sclip_norm: float
     accountant: str = "rdp"
```

### Comparing `declearn-2.1.0/declearn/main/config/_run_config.py` & `declearn-2.2.0/declearn/main/config/_run_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,47 +52,47 @@
     This class is meant to be extendable through inheritance, so as
     to refine the expected fields or add some that might be used by
     children (or parallel) classes of `FederatedServer` that modify
     the default, centralized, federated learning process.
 
     Fields
     ------
-    rounds: int
+    - rounds: int
         Maximum number of training and validation rounds to perform.
-    register: RegisterConfig
+    - register: RegisterConfig
         Parameters for clients' registration (min and/or max number
         of clients to expect, optional max duration of the process).
-    training: TrainingConfig
+    - training: TrainingConfig
         Parameters for training rounds, including effort constraints
         and data-batching instructions.
-    evaluate: EvaluateConfig
+    - evaluate: EvaluateConfig
         Parameters for validation rounds, similar to training ones.
-    privacy: PrivacyConfig or None
+    - privacy: PrivacyConfig or None
         Optional parameters to set up local differential privacy,
         by having clients use the DP-SGD algorithm for training.
-    early_stop: EarlyStopConfig or None
+    - early_stop: EarlyStopConfig or None
         Optional parameters to set up an EarlyStopping criterion, to
         be leveraged so as to interrupt the federated learning process
         based on the tracking of a minimized quantity (e.g. model loss).
 
     Instantiation classmethods
     --------------------------
-    from_toml:
+    - from_toml:
         Instantiate by parsing a TOML configuration file.
-    from_params:
+    - from_params:
         Instantiate by parsing inputs dicts (or objects).
 
     Notes
     -----
-    * `register` may be defined as a single integer (in `from_params` or in
+    - `register` may be defined as a single integer (in `from_params` or in
       a TOML file), that will be used as the exact number of clients.
-    * If `evaluate` is not provided to `from_params` or in the parsed TOML
+    - If `evaluate` is not provided to `from_params` or in the parsed TOML
       file, default parameters will automatically be used and the training
       batch size will be used for evaluation as well.
-    * If `privacy` is provided and the 'poisson' parameter is unspecified
+    - If `privacy` is provided and the 'poisson' parameter is unspecified
       for `training`, it will be set to True by default rather than False.
     """
 
     rounds: int
     register: RegisterConfig
     training: TrainingConfig
     evaluate: EvaluateConfig
@@ -104,14 +104,15 @@
         cls,
         field: dataclasses.Field,  # future: dataclasses.Field[RegisterConfig]
         inputs: Any,
     ) -> RegisterConfig:
         """Field-specific parser to instantiate a RegisterConfig.
 
         This method supports specifying `register`:
+
         * as a single int, translated into {"min_clients": inputs}
         * as None (or missing kwarg), using default RegisterConfig()
 
         It otherwise routes inputs back to the `default_parser`.
         """
         if inputs is None:
             return RegisterConfig()
```

### Comparing `declearn-2.1.0/declearn/main/config/_strategy.py` & `declearn-2.2.0/declearn/main/config/_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """TOML-parsable container for a Federated Learning optimization strategy."""
 
 import dataclasses
 import functools
 from typing import Any, Dict, Union
 
 
-from declearn.aggregator import Aggregator
+from declearn.aggregator import Aggregator, AveragingAggregator
 from declearn.optimizer import Optimizer
 from declearn.utils import TomlConfig, access_registered, deserialize_object
 
 
 __all__ = [
     "FLOptimConfig",
 ]
@@ -45,76 +45,80 @@
     end-users.
 
     It is designed to be used by the orchestrating server in the
     case of a centralized federated learning process.
 
     Fields
     ------
-    client_opt: Optimizer
+    - client_opt: Optimizer
         Optimizer to be used by clients (that each hold a copy)
         so as to conduct the step-wise local model updates.
-    server_opt: Optimizer, default=Optimizer(lrate=1.0)
+    - server_opt: Optimizer, default=Optimizer(lrate=1.0)
         Optimizer to be used by the server so as to conduct a
         round-wise global model update based on the aggregated
         client updates.
-    aggregator: Aggregator, default=AverageAggregator()
+    - aggregator: Aggregator, default=AverageAggregator()
         Client weights aggregator to be used by the server so as
         to conduct the round-wise aggregation of client udpates.
 
     Notes
     -----
     The `aggregator` field may be specified in a variety of ways:
+
     - a single string may specify the registered name of the class
-      constructor to use.
-      In TOML, use `aggregator = "<name>"` outside of any section.
+    constructor to use.
+    In TOML, use `aggregator = "<name>"` outside of any section.
     - a serialization dict, that specifies the registration `name`,
-      and optionally a registration `group` and/or arguments to be
-      passed to the class constructor.
-      In TOML, use an `[aggregator]` section with a `name = "<name>"`
-      field and any other fields you wish to pass. Kwargs may either
-      be grouped into a dedicated `[aggregator.config]` sub-section
-      or provided as fields of the main aggregator section.
+    and optionally a registration `group` and/or arguments to be
+    passed to the class constructor.
+    In TOML, use an `[aggregator]` section with a `name = "<name>"`
+    field and any other fields you wish to pass. Kwargs may either
+    be grouped into a dedicated `[aggregator.config]` sub-section
+    or provided as fields of the main aggregator section.
 
     The `client_opt` and `server_opt` fields may be specified as:
+
     - a single float, specifying the learning rate for vanilla SGD.
-      In TOML, use `client_opt = 0.001` for `Optimizer(lrate=0.001)`.
+    In TOML, use `client_opt = 0.001` for `Optimizer(lrate=0.001)`.
     - a dict of keyword arguments for `declearn.optimizer.Optimizer`.
-      In TOML, use a `[client_opt]` section with fields specifying
-      the input parameters you wish to pass to the constructor.
+    In TOML, use a `[client_opt]` section with fields specifying
+    the input parameters you wish to pass to the constructor.
 
     Instantiation classmethods
     --------------------------
-    from_toml:
+    - from_toml:
         Instantiate by parsing a TOML configuration file.
-    from_params:
+    - from_params:
         Instantiate by parsing inputs dicts (or objects).
     """
 
     client_opt: Optimizer
     server_opt: Optimizer = dataclasses.field(
         default_factory=functools.partial(Optimizer, lrate=1.0)
     )
-    aggregator: Aggregator = dataclasses.field(default_factory=Aggregator)
+    aggregator: Aggregator = dataclasses.field(
+        default_factory=AveragingAggregator
+    )
 
     @classmethod
     def parse_client_opt(
         cls,
         field: dataclasses.Field,  # future: dataclasses.Field[Optimizer]
         inputs: Union[float, Dict[str, Any], Optimizer],
     ) -> Optimizer:
-        """ "Field-specific parser to instanciate the client-side Optimizer."""
+        """Field-specific parser to instantiate the client-side Optimizer."""
         return cls._parse_optimizer(field, inputs)
 
     @classmethod
     def parse_server_opt(
         cls,
         field: dataclasses.Field,  # future: dataclasses.Field[Optimizer]
         inputs: Union[float, Dict[str, Any], Optimizer, None],
     ) -> Optimizer:
-        """ "Field-specific parser to instanciate the server-side Optimizer."""
+        """Field-specific parser to instantiate the server-side Optimizer."""
         return cls._parse_optimizer(field, inputs)
 
     @classmethod
     def _parse_optimizer(
         cls,
         field: dataclasses.Field,  # future: dataclasses.Field[Optimizer]
         inputs: Union[float, Dict[str, Any], Optimizer, None],
@@ -134,21 +138,22 @@
         cls,
         field: dataclasses.Field,  # future: dataclasses.Field[Aggregator]
         inputs: Union[str, Dict[str, Any], Aggregator, None],
     ) -> Aggregator:
         """Field-specific parser to instantiate an Aggregator.
 
         This method supports specifying `aggregator`:
-        * as a str, used to retrieve a registered Aggregator class
-        * as a dict, parsed a serialized Aggregator configuration:
+
+        - as a str, used to retrieve a registered Aggregator class
+        - as a dict, parsed a serialized Aggregator configuration:
             - name: str used to retrieve a registered Aggregator class
             - (opt.) group: str used to retrieve the registered class
             - (opt.) config: dict specifying kwargs for the constructor
             - any other field will be added to the `config` kwargs dict
-        * as None (or missing kwarg), using default AverageAggregator()
+        - as None (or missing kwarg), using default AveragingAggregator()
         """
         # Case when using the default value: delegate to the default parser.
         if inputs is None:
             return cls.default_parser(field, inputs)
         # Case when the input is a valid instance: return it.
         if isinstance(inputs, Aggregator):
             return inputs
```

### Comparing `declearn-2.1.0/declearn/main/privacy/__init__.py` & `declearn-2.2.0/examples/heart-uci/gen_ssl.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,10 +11,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Submodule implementing Differential-Privacy-oriented tools."""
+"""Script to generate self-signed SSL certificates for the demo."""
 
-from ._dp_trainer import DPTrainingManager
+import os
+
+from declearn.test_utils import generate_ssl_certificates
+
+
+if __name__ == "__main__":
+    FILEDIR = os.path.dirname(os.path.abspath(__file__))
+    generate_ssl_certificates(FILEDIR)
```

### Comparing `declearn-2.1.0/declearn/main/privacy/_dp_trainer.py` & `declearn-2.2.0/declearn/main/privacy/_dp_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,27 +38,34 @@
 ]
 
 
 class DPTrainingManager(TrainingManager):
     """TrainingManager subclass adding Differential Privacy mechanisms.
 
     This class extends the base TrainingManager class in three key ways:
+
     * Perform per-sample gradients clipping (through the Model API),
       parametrized by the added, optional `sclip_norm` attribute.
     * Add noise to batch-averaged gradients at each step of training,
       calibrated from an (epsilon, delta) DP budget and the planned
       training computational effort (number of steps, sample rate...).
     * Keep track of the spent privacy budget during training, and block
       training once the monitored budget is fully spent (early-stop the
       training routine if the next step would result in over-spending).
 
     This TrainingManager therefore implements the differentially-private
     stochastic gradient descent algorithm (DP-SGD) [1] algorithm, in a
     modular fashion that enables using any kind of optimizer plug-in
     supported by its (non-DP) parent.
+
+    References
+    ----------
+    [1] Abadi et al, 2016.
+        Deep Learning with Differential Privacy.
+        https://arxiv.org/abs/1607.00133
     """
 
     def __init__(
         self,
         model: Model,
         optim: Optimizer,
         train_data: Dataset,
@@ -74,15 +81,22 @@
         self._dp_budget = (0.0, 0.0)
         self._dp_states = None  # type: Optional[Tuple[float, float]]
 
     def make_private(
         self,
         message: messaging.PrivacyRequest,
     ) -> None:
-        """Set up the use of DP-SGD based on a received PrivacyRequest."""
+        """Set up the use of DP-SGD based on a received PrivacyRequest.
+
+        Parameters
+        ----------
+        message: PrivacyRequest
+            PrivacyRequest message specifying the privacy budget, type
+            of accountant and expected use of the training data.
+        """
         # REVISE: add support for fixed requested noise multiplier
         # Compute the noise multiplier to use based on the budget
         # and the planned training duration and parameters.
         noise_multiplier = self._fit_noise_multiplier(
             budget=message.budget,
             n_samples=self.train_data.get_data_specs().n_samples,
             batch_size=message.batches["batch_size"],
@@ -145,22 +159,38 @@
             target_delta=budget[1],
             sample_rate=batch_size / n_samples,
             steps=steps,
             accountant=accountant,
         )
 
     def get_noise_multiplier(self) -> Optional[float]:
-        """Return the noise multiplier used for DP-SGD, if any."""
+        """Return the noise multiplier used for DP-SGD, if any.
+
+        Returns
+        -------
+        noise_multiplier: float or None
+            Standard deviation of the gaussian noise-addition module
+            placed at the start of the wrapped optimizer's pipeline,
+            if one is indeed present.
+        """
         if self.optim.modules:
             if isinstance(self.optim.modules[0], GaussianNoiseModule):
                 return self.optim.modules[0].std / (self.sclip_norm or 1.0)
         return None
 
     def get_privacy_spent(self) -> Tuple[float, float]:
-        """Return the (epsilon, delta) privacy budget used."""
+        """Return the (epsilon, delta) privacy budget spent so far.
+
+        Returns
+        -------
+        epsilon: float
+            epsilon component of the privacy budget spent.
+        delta: float
+            delta component of the privacy budget spent.
+        """
         if self.accountant is None:
             raise RuntimeError("Cannot return spent privacy: DP is not used.")
         delta = self._dp_budget[1]
         epsilon = self.accountant.get_epsilon(delta=delta)
         return epsilon, delta
 
     def _run_train_step(
```

### Comparing `declearn-2.1.0/declearn/main/utils/__init__.py` & `declearn-2.2.0/examples/mnist/gen_ssl.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utils for the main federated learning traning and evaluation processes."""
+"""Script to generate self-signed SSL certificates for the demo."""
 
-from ._checkpoint import Checkpointer
-from ._constraints import Constraint, ConstraintSet, TimeoutConstraint
-from ._data_info import AggregationError, aggregate_clients_data_info
-from ._early_stop import EarlyStopping, EarlyStopConfig
-from ._training import TrainingManager
+import os
+
+from declearn.test_utils import generate_ssl_certificates
+
+
+if __name__ == "__main__":
+    FILEDIR = os.path.dirname(os.path.abspath(__file__))
+    generate_ssl_certificates(FILEDIR)
```

### Comparing `declearn-2.1.0/declearn/main/utils/_checkpoint.py` & `declearn-2.2.0/declearn/main/utils/_checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,28 +92,29 @@
         """Type-check and/or transform inputs into a Checkpointer instance.
 
         This classmethod is merely implemented to avoid duplicate and
         boilerplate code from polluting FL orchestrating classes.
 
         Parameters
         ----------
-        specs: Checkpointer or dict[str, any] or str
+        inputs: Checkpointer or dict[str, any] or str
             Checkpointer instance to type-check, or instantiation kwargs
             to parse into one. If a single string is passed, treat it as
             the `folder` argument, and use default other parameters.
 
         Returns
         -------
         checkpointer: Checkpointer
             Checkpointer instance, type-checked or instantiated from inputs.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If `inputs` is of unproper type.
+
         Other exceptions may be raised when calling this class's `__init__`.
         """
         if isinstance(inputs, str):
             inputs = {"folder": inputs}
         if isinstance(inputs, dict):
             inputs = cls(**inputs)
         if not isinstance(inputs, cls):
```

### Comparing `declearn-2.1.0/declearn/main/utils/_constraints.py` & `declearn-2.2.0/declearn/main/utils/_constraints.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/main/utils/_data_info.py` & `declearn-2.2.0/declearn/main/utils/_data_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     required_fields: set[str]
         Optional set of fields to target among provided information.
         If set, raise if a field is missing from any client, and use
         only these fields in the returned dict.
 
     Raises
     ------
-    AggregationError:
+    AggregationError
         In case any error is raised when calling `aggregate_data_info`
         on the input arguments.
 
     Returns
     -------
     data_info: dict[str, any]
         Aggregated data specifications derived from individual ones,
```

### Comparing `declearn-2.1.0/declearn/main/utils/_early_stop.py` & `declearn-2.2.0/declearn/main/utils/_early_stop.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,7 +109,13 @@
             self._n_iter_stuck += 1
         else:
             self._n_iter_stuck = 0
         return self.keep_training
 
 
 EarlyStopConfig = dataclass_from_init(EarlyStopping, name="EarlyStopConfig")
+"""Auto-generated dataclass matching `EarlyStopping.__init__` signature.
+
+See [`declearn.main.utils.EarlyStopping.__init__`][] for details.
+You may also refer to the dynamically-generated docs, accessible using
+`help(EarlyStopConfig)` in a python terminal.
+"""  # for docs rendering
```

### Comparing `declearn-2.1.0/declearn/main/utils/_training.py` & `declearn-2.2.0/declearn/main/utils/_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ConstraintSet,
     TimeoutConstraint,
 )
 from declearn.metrics import MeanMetric, Metric, MetricInputType, MetricSet
 from declearn.model.api import Model
 from declearn.optimizer import Optimizer
 from declearn.typing import Batch
-from declearn.utils import get_logger
+from declearn.utils import LOGGING_LEVEL_MAJOR, get_logger
 
 __all__ = [
     "TrainingManager",
 ]
 
 
 class TrainingManager:
@@ -50,16 +50,16 @@
         train_data: Dataset,
         valid_data: Optional[Dataset] = None,
         metrics: Union[MetricSet, List[MetricInputType], None] = None,
         logger: Union[logging.Logger, str, None] = None,
     ) -> None:
         """Instantiate the client-side training and evaluation process.
 
-        Arguments
-        ---------
+        Parameters
+        ----------
         model: Model
             Model instance that needs training and/or evaluating.
         optim: Optimizer
             Optimizer instance that orchestrates training steps.
         train_data: Dataset
             Dataset instance wrapping the local training dataset.
         valid_data: Dataset or None, default=None
@@ -251,15 +251,15 @@
         Parameters
         ----------
         batch: Batch
             Batched data based on which to compute and apply model updates.
 
         Raises
         ------
-        StopIteration:
+        StopIteration
             If this step is being cancelled and the training routine
             in the context of which it is being called should stop.
         """
         self.optim.run_train_step(self.model, batch)
 
     def evaluation_round(
         self,
@@ -340,15 +340,16 @@
             constraints.increment()
             if constraints.saturated:
                 break
         # Gather the computed metrics and computational effort information.
         effort = constraints.get_values()
         result = self.metrics.get_result()
         states = self.metrics.get_states()
-        self.logger.info(
+        self.logger.log(
+            LOGGING_LEVEL_MAJOR,
             "Local scalar evaluation metrics: %s",
             {k: v for k, v in result.items() if isinstance(v, float)},
         )
         # Pack the result and computational effort information into a message.
         self.logger.info("Packing local results to be sent to the server.")
         return messaging.EvaluationReply(
             loss=float(result["loss"]),
```

### Comparing `declearn-2.1.0/declearn/metrics/__init__.py` & `declearn-2.2.0/declearn/metrics/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,48 +17,54 @@
 
 """Iterative and federative evaluation metrics computation tools.
 
 This module provides with Metric, an abstract base class that defines
 an API to iteratively and/or federatively compute evaluation metrics,
 as well as a number of concrete standard machine learning metrics.
 
-Abstractions:
-* Metric:
+Abstractions
+------------
+* [Metric][declearn.metrics.Metric]:
     Abstract base class defining an API for metrics' computation.
-* MeanMetric:
+* [MeanMetric][declearn.metrics.MeanMetric]:
     Abstract class that defines a template for simple scores' averaging.
 
-Utils:
-* MetricSet:
+Utils
+-----
+* [MetricSet][declearn.metrics.MetricSet]:
     Wrapper to bind together an ensemble of Metric instances.
 * MetricInputType:
     Type alias for valid inputs to specify a metric for `MetricSet`.
     Equivalent to `Union[Metric, str, Tuple[str, Dict[str, Any]]]`.
 
-Classification metrics:
-* BinaryAccuracyPrecisionRecall
+Classification metrics
+----------------------
+* [BinaryAccuracyPrecisionRecall]\
+[declearn.metrics.BinaryAccuracyPrecisionRecall]:
     Accuracy, precision, recall and confusion matrix for binary classif.
     Identifier name: "binary-classif".
-* MulticlassAccuracyPrecisionRecall
+* [MulticlassAccuracyPrecisionRecall]\
+[declearn.metrics.MulticlassAccuracyPrecisionRecall]:
     Accuracy, precision, recall and confusion matrix for multiclass classif.
     Identifier name: "multi-classif".
-* BinaryRocAuc:
+* [BinaryRocAUC][declearn.metrics.BinaryRocAUC]:
     Receiver Operator Curve and its Area Under the Curve for binary classif.
-    Identifier name: "binary-roc"
+    Identifier name: "binary-roc".
 
-Regression metrics:
-* MeanAbsoluteError:
+Regression metrics
+------------------
+* [MeanAbsoluteError][declearn.metrics.MeanAbsoluteError]:
     Mean absolute error, averaged across all samples (and channels).
-    Identifier name: "mae"
-* MeanSquaredError:
+    Identifier name: "mae".
+* [MeanSquaredError][declearn.metrics.MeanSquaredError]:
     Mean squared error, averaged across all samples (and channels).
-    Identifier name: "mse"
-* RSquared:
+    Identifier name: "mse".
+* [RSquared][declearn.metrics.RSquared]:
     R^2 (R-Squared, coefficient of determination) regression metric.
-    Identifier name: "r2"
+    Identifier name: "r2".
 
 """
 
 from ._api import Metric
 from ._classif import (
     BinaryAccuracyPrecisionRecall,
     MulticlassAccuracyPrecisionRecall,
```

### Comparing `declearn-2.1.0/declearn/metrics/_api.py` & `declearn-2.2.0/declearn/metrics/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,91 +41,98 @@
     """Abstract class defining an API to compute federative metrics.
 
     This class defines an API to instantiate stateful containers
     for one or multiple metrics, that enable computing the final
     results through iterative update steps that may additionally
     be run in a federative way.
 
+    Usage
+    -----
     Single-party usage:
+    ```
     >>> metric = MetricSubclass()
     >>> metric.update(y_true, y_pred)  # take one update state
     >>> metric.get_result()    # after one or multiple updates
     >>> metric.reset()  # reset before a next evaluation round
+    ```
 
     Multiple-parties usage:
+    ```
     >>> # Instantiate 2+ metrics and run local update steps.
     >>> metric_0 = MetricSubclass()
     >>> metric_1 = MetricSubclass()
     >>> metric_0.udpate(y_true_0, y_pred_0)
     >>> metric_1.update(y_true_1, y_pred_1)
     >>> # Gather and share metric states (aggregated information).
     >>> states_0 = metric_0.get_states()  # metrics_0 is unaltered
     >>> metric_1.agg_states(states_0)     # metrics_1 is updated
     >>> # Compute results that aggregate info from both clients.
     >>> metric_1.get_result()
+    ```
 
     Abstract
     --------
     To define a concrete Metric, one must subclass it and define:
 
-    name: str class attribute
+    - name: str class attribute
         Name identifier of the class (should be unique across existing
         Metric classes). Also used for automatic types-registration of
         the class (see `Inheritance` section below).
-    _build_states() -> dict[str, (float | np.ndarray)]:
+    - _build_states() -> dict[str, (float | np.ndarray)]:
         Build and return an ensemble of state variables.
         This method is called to initialize the `_states` attribute,
         that should be used and updated by other abstract methods.
-    update(y_true: np.ndarray, y_pred: np.ndarray, s_wght: (np.ndarray|None)):
+    - update(y_true: np.ndarray, y_pred: np.ndarray, s_wght: np.ndarray|None):
         Update the metric's internal state based on a data batch.
         This method should update `self._states` in-place.
-    get_result() -> dict[str, (float | np.ndarray)]:
+    - get_result() -> dict[str, (float | np.ndarray)]:
         Compute the metric(s), based on the current state variables.
         This method should make use of `self._states` and prevent
         side effects on its contents.
 
     Overridable
     -----------
     Some methods may be overridden based on the concrete Metric's needs.
     The most imporant one is the states-aggregation method:
 
-    agg_states(states: dict[str, (float | np.ndarray)]:
+    - agg_states(states: dict[str, (float | np.ndarray)]:
         Aggregate provided state variables into self ones.
         By default, it expects input and internal states to have
         similar specifications, and aggregates them by summation,
         which might no be proper depending on the actual metric.
 
     A pair of methods may be extended to cover non-`self._states`-contained
     variables:
 
-    reset():
+    - reset():
         Reset the metric to its initial state.
-    get_states() -> dict[str, (float | np.ndarray)]:
+    - get_states() -> dict[str, (float | np.ndarray)]:
         Return a copy of the current state variables.
 
 
     Finally, depending on the hyper-parameters defined by the subclass's
     `__init__`, one should adjust JSON-configuration-interfacing methods:
 
-    get_config() -> dict[str, any]:
+    - get_config() -> dict[str, any]:
         Return a JSON-serializable configuration dict for this Metric.
-    from_config(config: dict[str, any]) -> Self:
+    - from_config(config: dict[str, any]) -> Self:
         Instantiate a Metric from its configuration dict.
 
     Inheritance
     -----------
     When a subclass inheriting from `Metric` is declared, it is automatically
     registered under the "Metric" group using its class-attribute `name`.
     This can be prevented by adding `register=False` to the inheritance specs
     (e.g. `class MyCls(Metric, register=False)`).
 
     See `declearn.utils.register_type` for details on types registration.
     """
 
     name: ClassVar[str] = NotImplemented
+    """Name identifier of the class, unique across Metric classes."""
 
     def __init__(
         self,
     ) -> None:
         """Instantiate the metric object."""
         self._states = self._build_states()
 
@@ -219,19 +226,19 @@
         ----------
         states: dict[str, float or numpy.ndarray]
             Dict of states emitted by another instance of this class
             via its `get_states` method.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If any state variable is missing from `states`.
-        TypeError:
+        TypeError
             If any state variable is of unproper type.
-        ValueError:
+        ValueError
             If any array state variable is of unproper shape.
         """
         final = {}  # type: Dict[str, Union[float, np.ndarray]]
         # Iteratively compute sum-aggregated states, running sanity checks.
         for name, own in self._states.items():
             if name not in states:
                 raise KeyError(f"Missing required state variable: '{name}'.")
@@ -284,15 +291,15 @@
             Available as a class attribute.
         config: dict[str, any] or None
             Configuration dict of the metric, that is to be
             passed to its `from_config` class constructor.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If the provided `name` fails to be mapped to a registered
             Metric subclass.
         """
         try:
             cls = access_registered(name, group="Metric")
         except KeyError as exc:
             raise KeyError(
@@ -322,15 +329,15 @@
         -------
         s_wght: np.ndarray
             Input (opt. squeezed) `s_wght`, or `np.ones(n_samples)`
             if input was None.
 
         Raises
         ------
-        ValueError:
+        ValueError
             If the input array has improper shape or negative values.
         """
         if s_wght is None:
             return np.ones(shape=(n_samples,))
         s_wght = s_wght.squeeze()
         if s_wght.shape != (n_samples,) or np.any(s_wght < 0):
             raise ValueError(
```

### Comparing `declearn-2.1.0/declearn/metrics/_classif.py` & `declearn-2.2.0/declearn/metrics/_classif.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     This metric applies to binary classifier, and computes the (opt.
     weighted) amount of true positives (TP), true negatives (TN),
     false positives (FP) and false negatives (FN) predictions over
     time, from which basic evaluation metrics may be derived.
 
     Computed metrics are the following:
+
     * accuracy: float
         Accuracy of the classifier, i.e. P(pred==true).
         Formula: (TP + TN) / (TP + TN + FP + FN)
     * precision: float
         Precision score, i.e. P(true=1|pred=1).
         Formula: TP / (TP + FP)
     * recall: float
@@ -128,14 +129,15 @@
 
     This metric assumes that the evaluated classifier emits a score for
     each and every predictable label, and that the predicted label is
     that with the highest score. Alternatively, pre-selected labels (or
     one-hot encodings) may be passed as predictions.
 
     Computed metrics are the following:
+
     * accuracy: float
         Overall accuracy of the classifier, i.e. P(pred==true).
     * precision: 1-d numpy.ndarray
         Label-wise precision score, i.e. P(true=k|pred=k).
     * recall: 1-d numpy.ndarray
         Label-wise recall score, i.e. P(pred=k|true=k).
     * f-score: 1-d numpy.ndarray
```

### Comparing `declearn-2.1.0/declearn/metrics/_mean.py` & `declearn-2.2.0/declearn/metrics/_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     that rely on computing a sample-wise score and its average
     across iterative inputs.
 
     Abstract
     --------
     To implement such an actual Metric, inherit `MeanMetric` and define:
 
-    name: str class attribute:
+    - name: str class attribute:
         Name identifier of the Metric (should be unique across existing
         Metric classes). Used for automated type-registration and name-
         based retrieval. Also used to label output results.
-    metric_func(y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
+    - metric_func(y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
         Method that computes a score from the predictions and labels
         associated with a given batch, that is to be aggregated into
         an average metric across all input batches.
     """
 
     @abstractmethod
     def metric_func(
@@ -110,15 +110,16 @@
     """Mean Absolute Error (MAE) metric.
 
     This metric applies to a regression model, and computes the (opt.
     weighted) mean sample-wise absolute error. Note that for inputs
     with multiple channels, the sum of absolute channel-wise errors
     is computed for each sample, and averaged across samples.
 
-    Computed metrics is the following:
+    Computed metric is the following:
+
     * mae: float
         Mean absolute error, averaged across samples (possibly
         summed over channels for (>=2)-dimensional inputs).
     """
 
     name: ClassVar[str] = "mae"
 
@@ -138,15 +139,16 @@
     """Mean Squared Error (MSE) metric.
 
     This metric applies to a regression model, and computes the (opt.
     weighted) mean sample-wise squared error. Note that for inputs
     with multiple channels, the sum of squared channel-wise errors
     is computed for each sample, and averaged across samples.
 
-    Computed metrics is the following:
+    Computed metric is the following:
+
     * mse: float
         Mean squared error, averaged across samples (possibly
         summed over channels for (>=2)-dimensional inputs).
     """
 
     name: ClassVar[str] = "mse"
```

### Comparing `declearn-2.1.0/declearn/metrics/_roc_auc.py` & `declearn-2.2.0/declearn/metrics/_roc_auc.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     This metric applies to a binary classifier, and computes the (opt.
     weighted) amount of true positives (TP), true negatives (TN), false
     positives (FP) and false negatives (FN) predictions over time around
     a variety of thresholds; from which TP rate, FP rate and finally ROC
     AUC metrics are eventually derived.
 
     Computed metrics are the following:
+
     * fpr: 1-d numpy.ndarray
         True-positive rate values for a variety of thresholds.
         Formula: TP / (TP + FN), i.e. P(pred=1|true=1)
     * tpr: 1-d numpy.ndarray
         False-positive rate values for a variety of thresholds.
         Formula: FP / (FP + TN), i.e. P(pred=1|true=0)
     * thresh: 1-d numpy.ndarray
@@ -79,22 +80,22 @@
             Optional lower and upper bounds for threshold values. If
             set, disable adjusting the scale based on input values.
             If None, start with (0, 1) and extend the scale on both
             ends when input values exceed them.
 
         Notes
         -----
-        Using the default `bound=None` enables the thresholds at which
-        the ROC curve points are compute to vary dynamically based on
-        inputs, but also based on input states to the `agg_states`
-        method, that may come from a metric with different parameters.
-        Setting up explicit boundaries prevents thresholds from being
-        adjusted at update time, and a ValueError will be raise by the
-        `agg_states` method if inputs are adjusted to a distinct set
-        of thresholds.
+        - Using the default `bound=None` enables the thresholds at which
+          the ROC curve points are compute to vary dynamically based on
+          inputs, but also based on input states to the `agg_states`
+          method, that may come from a metric with different parameters.
+        - Setting up explicit boundaries prevents thresholds from being
+          adjusted at update time, and a ValueError will be raise by the
+          `agg_states` method if inputs are adjusted to a distinct set
+          of thresholds.
         """
         self.scale = scale
         self.label = label
         self.bound = bound
         super().__init__()
 
     def get_config(self) -> Dict[str, Any]:
```

### Comparing `declearn-2.1.0/declearn/metrics/_rsquared.py` & `declearn-2.2.0/declearn/metrics/_rsquared.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,49 +31,52 @@
 class RSquared(Metric):
     """R^2 (R-Squared, coefficient of determination) regression metric.
 
     This metric applies to a regression model, and computes the (opt.
     weighted) R^2 score, also known as coefficient of determination.
 
     Computed metric is the following:
+
     * r2: float
         R^2 score, or coefficient of determination, averaged across samples.
         It is defined as the proportion of total sample variance explained
         by the regression model:
         * SSr = Sum((true - pred)^2)  # Residual sum of squares
         * SSt = Sum((true - mean(true))^2)  # Total sum of squares
         * R^2 = 1 - (SSr / SSt)
 
-    Notes:
+    Notes
+    -----
     - This metric expects 1d-arrays, or arrays than can be reduced to 1-d
     - If the true variance is zero, we by convention return a perfect score
       if the expected variance is also zero, else return a score of 0.0.
     - The R^2 score is not well-defined with less than two samples.
 
-    Implementation details:
+    Implementation details
+    ----------------------
     - Since this metric is to be computed iteratively and with a single pass
       over a batched dataset, we use the König-Huygens formula to decompose
       the total sum of squares into a sum of terms that can be updated with
       summation for each batch received (as opposed to using an estimate of
       the mean of true values that would vary with each batch). This gives:
-        wSST = Sum(weight * (true - mean(true))^2)  # initial definition
-        wSST = Sum(weight * true^2) - (Sum(weight * true))^2 / Sum(weight)
+        - wSST = Sum(weight * (true - mean(true))^2)  # initial definition
+        - wSST = Sum(weight * true^2) - (Sum(weight * true))^2 / Sum(weight)
 
-    LaTeX formulas (with weights):
-    - Canonical formula:
-        $$R^2(y, \\hat{y})= 1 - \\frac{
-            \\sum_{i=1}^n w_i \\left(y_i-\\hat{y}_i\\right)^2
-        }{
-            \\sum_{i=1}^n w_i \\left(y_i-\\bar{y}\\right)^2
-        }$$
-    - Decomposed weighted total sum of squares:
-        $$\\sum_{i=1}^n w_i \\left(y_i-\\bar{y}\\right)^2 =
-            \\sum_i w_i y_i^2
-            - \\frac{\\left(\\sum_i w_i y_i\\right)^2}{\\sum_i w_i}
-        $$
+    - LaTeX formulas (with weights):
+        - Canonical formula:
+            $$R^2(y, \\hat{y})= 1 - \\dfrac{
+                \\sum_{i=1}^n w_i \\left(y_i-\\hat{y}_i\\right)^2
+            }{
+                \\sum_{i=1}^n w_i \\left(y_i-\\bar{y}\\right)^2
+            }$$
+        - Decomposed weighted total sum of squares:
+            $$\\sum_{i=1}^n w_i \\left(y_i-\\bar{y}\\right)^2 =
+                \\sum_i w_i y_i^2
+                - \\frac{\\left(\\sum_i w_i y_i\\right)^2}{\\sum_i w_i}
+            $$
     """
 
     name: ClassVar[str] = "r2"
 
     def _build_states(
         self,
     ) -> Dict[str, Union[float, np.ndarray]]:
```

### Comparing `declearn-2.1.0/declearn/metrics/_wrapper.py` & `declearn-2.2.0/declearn/metrics/_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
         metrics: list[Metric, str, tuple(str, dict[str, any])]
             List of metrics to bind together. The metrics may be provided
             either as a Metric instance, a name identifier string, or a
             tuple with both a name identifier and a configuration dict.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If one of the input `metrics` elements is of improper type.
-        KeyError:
+        KeyError
             If a metric name identifier fails to be mapped to a Metric class.
-        RuntimeError:
+        RuntimeError
             If multiple metrics are of the same final type.
         """
         # REVISE: store metrics into a Dict and adjust labels when needed
         self.metrics = []  # type: List[Metric]
         for metric in metrics:
             if isinstance(metric, str):
                 metric = Metric.from_specs(metric)
@@ -113,16 +113,17 @@
         Returns
         -------
         metricset: MetricSet
             MetricSet instance, type-checked or instantiated from inputs.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If `metrics` is of unproper type.
+
         Other exceptions may be raised when calling this class's `__init__`.
         """
         if metrics is None:
             metrics = cls([])
         if isinstance(metrics, list):
             metrics = cls(metrics)
         if not isinstance(metrics, cls):
@@ -206,19 +207,19 @@
         ----------
         states: dict[str, float or numpy.ndarray]
             Dict of states emitted by another instance of this class
             via its `get_states` method.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If any state variable is missing from `states`.
-        TypeError:
+        TypeError
             If any state variable is of unproper type.
-        ValueError:
+        ValueError
             If any array state variable is of unproper shape.
         """
         for metric in self.metrics:
             if metric.name in states:
                 metric.agg_states(states[metric.name])
 
     def get_config(
```

### Comparing `declearn-2.1.0/declearn/model/__init__.py` & `declearn-2.2.0/declearn/model/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,36 +14,64 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model interfacing submodule, defining an API an derived applications.
 
 This declearn submodule provides with:
-* Model and Vector abstractions, used as an API to design FL algorithms
-* Submodules implementing interfaces to various frameworks and models.
 
+- Model and Vector abstractions, used as an API to design FL algorithms.
+- Submodules implementing interfaces to various frameworks and models.
+
+Default Submodules
+------------------
 The automatically-imported submodules implemented here are:
-* api: Model and Vector abstractions' defining module.
-    - Model: abstract API to interface framework-specific models.
-    - Vector: abstract API for data tensors containers.
-* sklearn: scikit-learn based or oriented tools
-    - NumpyVector: Vector for numpy array data structures.
-    - SklearnSGDModel: Model for scikit-learn's SGDClassifier and SGDRegressor.
 
+* [api][declearn.model.api]:
+    Model and Vector abstractions' defining module.
+    - [Model][declearn.model.api.Model]:
+        abstract API to interface framework-specific models.
+    - [Vector][declearn.model.api.Vector]:
+        abstract API for data tensors containers.
+* [sklearn][declearn.model.sklearn]:
+    Scikit-Learn based or oriented tools
+    - [NumpyVector][declearn.model.sklearn.NumpyVector]
+        Vector for numpy array data structures.
+    - [SklearnSGDModel][declearn.model.sklearn.SklearnSGDModel]
+        Model for scikit-learn's SGDClassifier and SGDRegressor.
+
+Optional Submodules
+-------------------
 The optional-dependency-based submodules that may be manually imported are:
-* tensorflow: tensorflow-interfacing tools
-    - TensorflowModel: Model to wrap any tensorflow-keras Layer model.
-    - TensorflowOptiModule: Hacky OptiModule to wrap a keras Optimizer.
-    - TensorflowVector: Vector for tensorflow Tensor and IndexedSlices.
-* torch: pytorch-interfacing tools
-    - TorchModel: Model to wrap any torch Module model.
-    - TorchOptiModule: Hacky OptiModule to wrap a torch Optimizer.
-    - TorchVector: Vector for torch Tensor objects.
+
+* [haiku][declearn.model.haiku]:
+    Jax- and Haiku-interfacing tools.
+    - [HaikuModel][declearn.model.haiku.HaikuModel]:
+        Model to wrap a haiku-transformable model function.
+    - [JaxNumpyVector][declearn.model.haiku.JaxNumpyVector]:
+        Vector for jax array data structures.
+* [tensorflow][declearn.model.tensorflow]:
+    TensorFlow-interfacing tools
+    - [TensorflowModel][declearn.model.tensorflow.TensorflowModel]:
+        Model to wrap any tensorflow-keras Layer model.
+    - [TensorflowOptiModule][declearn.model.tensorflow.TensorflowOptiModule]:
+        Hacky OptiModule to wrap a keras Optimizer.
+    - [TensorflowVector][declearn.model.tensorflow.TensorflowVector]:
+        Vector for tensorflow Tensor and IndexedSlices.
+* [torch][declearn.model.torch]:
+    PyTorch-interfacing tools
+    - [TorchModel][declearn.model.torch.TorchModel]:
+        Model to wrap any torch Module model.
+    - [TorchOptiModule][declearn.model.torch.TorchOptiModule]:
+        Hacky OptiModule to wrap a torch Optimizer.
+    - [TorchVector][declearn.model.torch.TorchVector]:
+        Vector for torch Tensor objects.
 """
 
 from . import api
 from . import sklearn
 
 OPTIONAL_MODULES = [
+    "haiku",
     "tensorflow",
     "torch",
 ]
```

### Comparing `declearn-2.1.0/declearn/model/_utils.py` & `declearn-2.2.0/declearn/model/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Expected set of string values.
     context: str, default="expected"
         String piece used in the raised exception's description to
         designate the `expected` names.
 
     Raises
     ------
-    KeyError:
+    KeyError
         In case `received != expected`.
         Verbose about the missing and/or unexpected `received` keys.
     """
     if received != expected:
         missing = expected.difference(received)
         unexpct = received.difference(expected)
         raise KeyError(
```

### Comparing `declearn-2.1.0/declearn/model/api/_model.py` & `declearn-2.2.0/declearn/model/api/_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,31 +14,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model abstraction API."""
 
 from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Optional, Set, Tuple
+from typing import Any, Dict, Generic, Optional, Set, Tuple, TypeVar
 
 import numpy as np
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api._vector import Vector
 from declearn.typing import Batch
 from declearn.utils import DevicePolicy, create_types_registry
 
 
 __all__ = [
     "Model",
 ]
 
 
+VectorT = TypeVar("VectorT", bound=Vector)
+"""Type-annotation for the Vector subclass proper to a given Model."""
+
+
 @create_types_registry
-class Model(metaclass=ABCMeta):
+class Model(Generic[VectorT], metaclass=ABCMeta):
     """Abstract class defining an API to manipulate a ML model.
 
     A 'Model' is an abstraction that defines a generic interface
     to access a model's parameters and perform operations (such
     as computing gradients or metrics over some data), enabling
     writing algorithms and operations agnostic to the framework
     in which the underlying model is implemented (e.g. PyTorch,
@@ -55,30 +59,45 @@
     def __init__(
         self,
         model: Any,
     ) -> None:
         """Instantiate a Model interface wrapping a 'model' object."""
         self._model = model
 
+    def get_wrapped_model(self) -> Any:
+        """Getter to access the wrapped framework-specific model object.
+
+        This getter should be used sparingly, so as to avoid undesirable
+        side effects. In particular, it should not be used in declearn
+        backend code (but may be in examples or tests), as it is merely
+        a way for end-users to access the wrapped model after training.
+
+        Returns
+        -------
+        model:
+            Wrapped model, of (framework/Model-subclass)-specific type.
+        """
+        return self._model
+
     @property
     @abstractmethod
     def device_policy(
         self,
     ) -> DevicePolicy:
         """Return the device-placement policy currently used by this model."""
 
     @property
     @abstractmethod
     def required_data_info(
         self,
     ) -> Set[str]:
         """List of 'data_info' fields required to initialize this model.
 
-        Note: these fields should match a registered specification
-              (see `declearn.data_info` submodule)
+        Note: These fields should match a registered specification
+        (see the [`declearn.data_info`][] submodule).
         """
 
     @abstractmethod
     def initialize(
         self,
         data_info: Dict[str, Any],
     ) -> None:
@@ -88,15 +107,15 @@
         ----------
         data_info: dict[str, any]
             Data specifications, presenting values for all fields
             listed under `self.required_data_info`
 
         Raises
         ------
-        KeyError:
+        KeyError
             If some fields in `required_data_info` are missing.
 
         Notes
         -----
         See the `aggregate_data_info` method to derive `data_info`
         from client-wise dict.
         """
@@ -115,15 +134,15 @@
     ) -> Self:
         """Instantiate a model from a configuration dict."""
 
     @abstractmethod
     def get_weights(
         self,
         trainable: bool = False,
-    ) -> Vector:
+    ) -> VectorT:
         """Return the model's weights, optionally excluding frozen ones.
 
         Parameters
         ----------
         trainable: bool, default=False
             Whether to restrict the returned weights to the trainable ones,
             or include those that are frozen, i.e. are not updates as part
@@ -136,15 +155,15 @@
             The concrete type of the returned Vector depends on the concrete
             `Model`, and is the same as with `compute_batch_gradients`.
         """
 
     @abstractmethod
     def set_weights(
         self,
-        weights: Vector,
+        weights: VectorT,
         trainable: bool = False,
     ) -> None:
         """Assign values to the model's weights.
 
         This method can only be used to update the values of *all*
         model weights, with the optional exception of frozen (i.e.
         non-trainable) ones. It cannot be used to alter the values
@@ -160,27 +179,27 @@
         trainable: bool, default=False
             Whether the assigned weights only cover the trainable ones,
             or include those that are frozen, i.e. are not updated as
             part of the training process.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If the input weights do not match the expected number and
             names of weight tensors.
-        TypeError:
+        TypeError
             If the input weights are of unproper concrete Vector type.
         """
 
     @abstractmethod
     def compute_batch_gradients(
         self,
         batch: Batch,
         max_norm: Optional[float] = None,
-    ) -> Vector:
+    ) -> VectorT:
         """Compute and return gradients computed over a given data batch.
 
         Compute the average gradients of the model's loss with respect
         to its trainable parameters for the given data batch.
         Optionally clip sample-wise gradients before batch-averaging.
 
         Parameters
@@ -200,15 +219,15 @@
             Batch-averaged gradients, wrapped into a Vector (using
             a suited Vector subclass depending on the Model class).
         """
 
     @abstractmethod
     def apply_updates(
         self,
-        updates: Vector,
+        updates: VectorT,
     ) -> None:
         """Apply updates to the model's weights."""
 
     @abstractmethod
     def compute_batch_predictions(
         self,
         batch: Batch,
```

### Comparing `declearn-2.1.0/declearn/model/api/_vector.py` & `declearn-2.2.0/declearn/model/api/_vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Vector abstraction API."""
 
 import operator
 from abc import ABCMeta, abstractmethod
-from typing import Any, Callable, Dict, Optional, Set, Tuple, Type, Union
+from typing import (
+    # fmt: off
+    Any, Callable, Dict, Generic, Optional, Set, Tuple, Type, TypeVar, Union
+)
 
 from numpy.typing import ArrayLike
 from typing_extensions import Self  # future: import from typing (Py>=3.11)
 
 from declearn.utils import (
     add_json_support,
     create_types_registry,
@@ -33,109 +36,119 @@
 __all__ = [
     "Vector",
     "register_vector_type",
 ]
 
 
 VECTOR_TYPES = {}  # type: Dict[Type[Any], Type[Vector]]
+"""Private constant holding registered Vector types."""
+
+
+T = TypeVar("T")
+"""Type-annotation for the data structures proper to a given Vector class."""
 
 
 @create_types_registry
-class Vector(metaclass=ABCMeta):
+class Vector(Generic[T], metaclass=ABCMeta):
     """Abstract class defining an API to manipulate (sets of) data arrays.
 
     A Vector is an abstraction used to wrap a collection of data
     structures (numpy arrays, tensorflow or torch tensors, etc.).
     It enables writing algorithms and operations on such structures,
     agnostic of their actual implementation support.
 
     Use `vector.coefs` to access the stored coefficients.
 
     Any concrete Vector subclass should:
+
     - add type checks to `__init__` to control wrapped coefficients' type
     - opt. override `_op_...` properties to define compatible operators
     - implement the abstract operators (`sign`, `maximum`, `minimum`...)
     - opt. override `pack` and `unpack` to enable their serialization
     - opt. extend `compatible_vector_types` to specify their compatibility
       with other Vector subclasses
     - opt. override the `dtypes` and `shapes` methods
     """
 
     @property
-    def _op_add(self) -> Callable[[Any, Any], Any]:
+    def _op_add(self) -> Callable[[Any, Any], T]:
         """Framework-compatible addition operator."""
         return operator.add
 
     @property
-    def _op_sub(self) -> Callable[[Any, Any], Any]:
+    def _op_sub(self) -> Callable[[Any, Any], T]:
         """Framework-compatible substraction operator."""
         return operator.sub
 
     @property
-    def _op_mul(self) -> Callable[[Any, Any], Any]:
+    def _op_mul(self) -> Callable[[Any, Any], T]:
         """Framework-compatible multiplication operator."""
         return operator.mul
 
     @property
-    def _op_div(self) -> Callable[[Any, Any], Any]:
+    def _op_div(self) -> Callable[[Any, Any], T]:
         """Framework-compatible true division operator."""
         return operator.truediv
 
     @property
-    def _op_pow(self) -> Callable[[Any, Any], Any]:
+    def _op_pow(self) -> Callable[[Any, Any], T]:
         """Framework-compatible power operator."""
         return operator.pow
 
     @property
     def compatible_vector_types(self) -> Set[Type["Vector"]]:
         """Compatible Vector types, that may be combined into this.
 
-        Note that VectorTypeA may be compatible with VectorTypeB
-        while the opposite is False. It means that, for example,
-            (VectorTypeB + VectorTypeA) -> VectorTypeB
-        while
-            (VectorTypeA + VectorTypeB) -> TypeError
+        If VectorTypeA is listed as compatible with VectorTypeB,
+        then `(VectorTypeB + VectorTypeA) -> VectorTypeB` (both
+        for addition and any basic operator). In general, such
+        compatibility should be declared in one way only, hence
+        `(VectorTypeA + VectorTypeB) -> VectorTypeB` as well.
 
         This is for example the case is VectorTypeB stores numpy
         arrays while VectorTypeA stores tensorflow tensors since
         tf.add(tensor, array) returns a tensor, not an array.
+
+        If two vector types were inter-compatible, the above
+        operations would result in a vector of the left-hand
+        type.
         """
         return {type(self)}
 
     def __init__(
         self,
-        coefs: Dict[str, Any],
+        coefs: Dict[str, T],
     ) -> None:
         """Instantiate the Vector to wrap a collection of data arrays.
 
         Parameters
         ----------
-        coefs: dict[str, any]
+        coefs: dict[str, <T>]
             Dict grouping a named collection of data arrays.
             The supported types of that dict's values depends
             on the concrete `Vector` subclass being used.
         """
         self.coefs = coefs
 
     @staticmethod
     def build(
-        coefs: Dict[str, Any],
+        coefs: Dict[str, T],
     ) -> "Vector":
         """Instantiate a Vector, inferring its exact subtype from coefs'.
 
         'Vector' is an abstract class. Its subclasses, however, are
         expected to be designed for wrapping specific types of data
         structures. Using the `register_vector_type` decorator, the
         implemented Vector subclasses can be made buildable through
         this staticmethod, which relies on input coefficients' type
         analysis to infer the Vector type to instantiate and return.
 
         Parameters
         ----------
-        coefs: dict[str, any]
+        coefs: dict[str, <T>]
             Dict grouping a named collection of data arrays, that
             all belong to the same framework.
 
         Returns
         -------
         vector: Vector
             Vector instance, the concrete class of which depends
@@ -180,15 +193,18 @@
         Returns
         -------
         shapes: dict[str, tuple(int, ...)]
             Dict containing the shape of each of the wrapped data array,
             indexed by the coefficient's name.
         """
         try:
-            return {key: coef.shape for key, coef in self.coefs.items()}
+            return {
+                key: coef.shape  # type: ignore  # exception caught
+                for key, coef in self.coefs.items()
+            }
         except AttributeError as exc:
             raise NotImplementedError(
                 "Wrapped coefficients appear not to implement `.shape`.\n"
                 f"`{type(self).__name__}.shapes` probably needs overriding."
             ) from exc
 
     def dtypes(
@@ -201,15 +217,18 @@
         dtypes: dict[str, tuple(int, ...)]
             Dict containing the dtype of each of the wrapped data array,
             indexed by the coefficient's name. The dtypes are parsed as
             a string, the values of which may vary depending on the
             concrete framework of the Vector.
         """
         try:
-            return {key: str(coef.dtype) for key, coef in self.coefs.items()}
+            return {
+                key: str(coef.dtype)  # type: ignore  # exception caught
+                for key, coef in self.coefs.items()
+            }
         except AttributeError as exc:
             raise NotImplementedError(
                 "Wrapped coefficients appear not to implement `.dtype`.\n"
                 f"`{type(self).__name__}.dtypes` probably needs overriding."
             ) from exc
 
     def pack(
@@ -252,27 +271,28 @@
         vector: Self
             Instance of this Vector subclass, (re-)created from the inputs.
         """
         return cls(data)
 
     def apply_func(
         self,
-        func: Callable[..., Any],
+        func: Callable[..., T],
         *args: Any,
         **kwargs: Any,
     ) -> Self:
         """Apply a given function to the wrapped coefficients.
 
         Parameters
         ----------
         func: function(<T>, *args, **kwargs) -> <T>
             Function to be applied to each and every coefficient (data
             array) wrapped by this Vector, that must return a similar
             array (same type, shape and dtype).
-        *args and **kwargs to `func` may also be passed.
+
+        Any `*args` and `**kwargs` to `func` may also be passed.
 
         Returns
         -------
         vector: Self
             Vector similar to the present one, wrapping the resulting data.
         """
         coefs = {
@@ -280,22 +300,23 @@
             for key, coef in self.coefs.items()
         }
         return type(self)(coefs)
 
     def _apply_operation(
         self,
         other: Any,
-        func: Callable[[Any, Any], Any],
+        func: Callable[[Any, Any], T],
     ) -> Self:
         """Apply an operation to combine this vector with another.
 
         Parameters
         ----------
-        other: Vector
-            Vector with the same names, shapes and dtypes as this one.
+        other:
+            Vector with the same names, shapes and dtypes as this one;
+            or scalar object on which to operate (e.g. a float value).
         func: function(<T>, <T>) -> <T>
             Function to be applied to combine the data arrays stored
             in this vector and the `other` one.
 
         Returns
         -------
         vector: Self
@@ -422,17 +443,18 @@
 
 
 def register_vector_type(
     v_type: Type[Any],
     *types: Type[Any],
     name: Optional[str] = None,
 ) -> Callable[[Type[Vector]], Type[Vector]]:
-    """Decorate a Vector subclass to make it buildable with `Vector(...)`.
+    """Decorate a Vector subclass to make it buildable with `Vector.build`.
 
     Decorating a Vector subclass with this has three effects:
+
     * Add the class to registered type (in the "Vector" group).
       See `declearn.utils.register_type` for details.
     * Make instances of that class JSON-serializable, embarking
       the wrapped data by using the `pack` and `unpack` methods
       of the class. See `declearn.utils.add_json_support`.
     * Make the subclass buildable through `Vector.build(coefs)`,
       based on the analysis of wrapped coefficients' type.
```

### Comparing `declearn-2.1.0/declearn/model/sklearn/__init__.py` & `declearn-2.2.0/declearn/model/sklearn/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Scikit-Learn models interfacing tools.
 
-Due to the variety of model classes provided by scikit-learn
-and to the way their learning process is implemented, model-
-specific interfaces are required for declearn compatibility.
+Due to the variety of model classes provided by scikit-learn and to the way
+their learning process is implemented, model-specific interfaces are required
+for declearn compatibility.
 
-This module currently implements:
-* NumpyVector: Vector subclass to wrap numpy.ndarray objects
-* SklearnSGDModel: interface to SGD-based linear models
+This module exposes the following classes:
+
+* [NumpyVector][declearn.model.sklearn.NumpyVector]:
+    Vector subclass to wrap numpy.ndarray objects.
+* [SklearnSGDModel][declearn.model.sklearn.SklearnSGDModel]:
+    Model subclass interfacing SGD-based linear models.
 """
 
 from ._np_vec import NumpyVector
 from ._sgd import SklearnSGDModel
```

### Comparing `declearn-2.1.0/declearn/model/sklearn/_np_vec.py` & `declearn-2.2.0/declearn/model/sklearn/_np_vec.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,37 +54,43 @@
       notably the case with `TensorflowVector` and `TorchVector`.
     - There is currently no support for GPU-acceleration with the
       `NumpyVector` class, that only handles arrays and operations
       placed on a CPU device.
     """
 
     @property
-    def _op_add(self) -> Callable[[Any, Any], Any]:
+    def _op_add(self) -> Callable[[Any, Any], np.ndarray]:
         return np.add
 
     @property
-    def _op_sub(self) -> Callable[[Any, Any], Any]:
+    def _op_sub(self) -> Callable[[Any, Any], np.ndarray]:
         return np.subtract
 
     @property
-    def _op_mul(self) -> Callable[[Any, Any], Any]:
+    def _op_mul(self) -> Callable[[Any, Any], np.ndarray]:
         return np.multiply
 
     @property
-    def _op_div(self) -> Callable[[Any, Any], Any]:
+    def _op_div(self) -> Callable[[Any, Any], np.ndarray]:
         return np.divide
 
     @property
-    def _op_pow(self) -> Callable[[Any, Any], Any]:
+    def _op_pow(self) -> Callable[[Any, Any], np.ndarray]:
         return np.power
 
-    def __init__(self, coefs: Dict[str, np.ndarray]) -> None:
+    def __init__(
+        self,
+        coefs: Dict[str, np.ndarray],
+    ) -> None:
         super().__init__(coefs)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(
+        self,
+        other: Any,
+    ) -> bool:
         valid = isinstance(other, NumpyVector)
         if valid:
             valid = self.coefs.keys() == other.coefs.keys()
         if valid:
             valid = all(
                 np.array_equal(self.coefs[k], other.coefs[k])
                 for k in self.coefs
```

### Comparing `declearn-2.1.0/declearn/model/sklearn/_sgd.py` & `declearn-2.2.0/declearn/model/sklearn/_sgd.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 from declearn.data_info import aggregate_data_info
 from declearn.model.api import Model
 from declearn.model.sklearn._np_vec import NumpyVector
 from declearn.typing import Batch
 from declearn.utils import DevicePolicy, register_type
 
-
 __all__ = [
     "SklearnSGDModel",
 ]
 
 
 LossesLiteral = Literal[
     "hinge",
@@ -62,17 +61,18 @@
     """Model wrapper for Scikit-Learn SGDClassifier and SGDRegressor.
 
     This `Model` subclass is designed to wrap a `SGDClassifier`
     or `SGDRegressor` instance (from `sklearn.linear_model`) to
     be learned federatively.
 
     Notes regarding device management (CPU, GPU, etc.):
-    * This Model may only run on CPU, and is unaffected by device-
+
+    - This Model may only run on CPU, and is unaffected by device-
       management policies.
-    * Calling the `update_device_policy` method has no effect, and
+    - Calling the `update_device_policy` method has no effect, and
       raises a UserWarning if a GPU-targetting policy is passed to
       it directly.
     """
 
     def __init__(
         self,
         model: Union[SGDClassifier, SGDRegressor],
@@ -92,15 +92,15 @@
         """
         if not isinstance(model, (SGDClassifier, SGDRegressor)):
             raise TypeError(
                 "'model' should be a scikit-learn SGDClassifier"
                 " or SGDRegressor instance."
             )
         model = model.set_params(
-            eta0=0.1,
+            eta0=1.0,
             learning_rate="constant",
             warm_start=False,
             average=False,
         )
         super().__init__(model)
         self._initialized = False
         self._predict = (
@@ -119,33 +119,41 @@
         return DevicePolicy(gpu=False, idx=None)
 
     @property
     def required_data_info(
         self,
     ) -> Set[str]:
         if isinstance(self._model, SGDRegressor):
-            return {"n_features"}
-        return {"n_features", "classes"}
+            return {"features_shape"}
+        return {"features_shape", "classes"}
 
     def initialize(
         self,
         data_info: Dict[str, Any],
     ) -> None:
         # Check that required fields are available and of valid type.
         data_info = aggregate_data_info([data_info], self.required_data_info)
+        if not (
+            len(data_info["features_shape"]) == 1
+            and isinstance(data_info["features_shape"][0], int)
+        ):
+            raise ValueError(
+                "SklearnSGDModel requires fixed-size 1-d input features."
+            )
+        feat = data_info["features_shape"][0]
         # SGDClassifier case.
         if isinstance(self._model, SGDClassifier):
             self._model.classes_ = np.array(list(data_info["classes"]))
             n_classes = len(self._model.classes_)
             dim = n_classes if (n_classes > 2) else 1
-            self._model.coef_ = np.zeros((dim, data_info["n_features"]))
+            self._model.coef_ = np.zeros((dim, feat))
             self._model.intercept_ = np.zeros((dim,))
         # SGDRegressor case.
         else:
-            self._model.coef_ = np.zeros((data_info["n_features"],))
+            self._model.coef_ = np.zeros((feat,))
             self._model.intercept_ = np.zeros((1,))
         # Mark the SklearnSGDModel as initialized.
         self._initialized = True
 
     @classmethod
     def from_parameters(
         cls,
@@ -189,19 +197,19 @@
         n_jobs: int or None, default=None
             Number of CPUs to use when to compute one-versus-all.
             Only used for multi-class classifiers.
             `None` means 1, while -1 means all available CPUs.
 
         Notes
         -----
-        Save for `kind`, all parameters are strictly equivalent to those
-        of `sklearn.linear_modelSGDClassifier` and `SGDRegressor`. Refer
-        to the latter' documentation for additional details.
-        Note that unexposed parameters from those classes are simply not
-        used and/or overwritten when wrapped by `SklearnSGDModel`.
+        - Save for `kind`, all parameters are strictly equivalent to those
+          of `sklearn.linear_modelSGDClassifier` and `SGDRegressor`. Refer
+          to the latter' documentation for additional details.
+        - Note that unexposed parameters from those classes are simply not
+          used and/or overwritten when wrapped by `SklearnSGDModel`.
 
         Returns
         -------
         model: SklearnSGDModel
             A declearn Model wrapping an instantiated scikit-learn one.
         """
         # partially-inherited signature; pylint: disable=too-many-arguments
@@ -234,15 +242,15 @@
     def get_config(
         self,
     ) -> Dict[str, Any]:
         is_clf = isinstance(self._model, SGDClassifier)
         data_info = None  # type: Optional[Dict[str, Any]]
         if self._initialized:
             data_info = {
-                "n_features": self._model.coef_.shape[-1],
+                "features_shape": (self._model.coef_.shape[-1],),
                 "classes": self._model.classes_.tolist() if is_clf else None,
             }
         return {
             "kind": "classifier" if is_clf else "regressor",
             "params": self._model.get_params(),
             "data_info": data_info,
         }
@@ -270,15 +278,15 @@
     ) -> NumpyVector:
         weights = {
             "intercept": self._model.intercept_.copy(),
             "coef": self._model.coef_.copy(),
         }
         return NumpyVector(weights)
 
-    def set_weights(  # type: ignore  # Vector subtype specification
+    def set_weights(
         self,
         weights: NumpyVector,
         trainable: bool = False,
     ) -> None:
         if not isinstance(weights, NumpyVector):
             raise TypeError("SklearnSGDModel requires NumpyVector weights.")
         for key in ("coef", "intercept"):
@@ -342,17 +350,17 @@
         # Perform SGD step and gather weights.
         x_smp = x_smp.reshape((1, -1))  # type: ignore
         self._model.partial_fit(x_smp, [y_smp])
         w_end = self.get_weights()
         # Restore the model's weights.
         self.set_weights(w_srt)
         # Compute gradients based on weights' update.
-        return (w_srt - w_end) / self._model.eta0
+        return w_srt - w_end
 
-    def apply_updates(  # type: ignore  # Vector subtype specification
+    def apply_updates(
         self,
         updates: NumpyVector,
     ) -> None:
         if not isinstance(updates, NumpyVector):
             raise TypeError("SklearnSGDModel requires NumpyVector updates.")
         self._model.coef_ += updates.coefs["coef"]
         self._model.intercept_ += updates.coefs["intercept"]
@@ -375,15 +383,15 @@
         return self._loss_fn(y_true, y_pred)
 
     def _setup_loss_fn(
         self,
     ) -> Callable[[np.ndarray, np.ndarray], np.ndarray]:
         """Return a function to compute point-wise loss for a given batch."""
         # fmt: off
-        # Gather or instantiate a loss function from the wrapped model's specs.
+        # Gather / instantiate a loss function from the wrapped model's specs.
         if hasattr(self._model, "loss_function_"):
             loss_smp = self._model.loss_function_.py_loss
         else:
             loss_cls, *args = self._model.loss_functions[self._model.loss]
             loss_smp = loss_cls(*args).py_loss
         # Wrap it to support batched inputs.
         def loss_1d(y_true: np.ndarray, y_pred: np.ndarray) -> np.ndarray:
@@ -394,14 +402,15 @@
                 return np.sum([
                     loss_1d(y_true == val, y_pred[:, i])
                     for i, val in enumerate(self._model.classes_)
                 ], axis=0)
         else:
             loss_fn = loss_1d
         return loss_fn
+        # fmt: on
 
     def update_device_policy(
         self,
         policy: Optional[DevicePolicy] = None,
     ) -> None:
         if policy is not None and policy.gpu:
             warnings.warn("'SklearnSGDModel' only runs on a CPU backend.")
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/__init__.py` & `declearn-2.2.0/declearn/model/tensorflow/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,24 +13,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tensorflow models interfacing tools.
 
-This submodule provides with a generic interface to wrap up
-any TensorFlow `keras.Model` instance that is to be trained
-through gradient descent.
-
-This module exposes:
-* TensorflowModel: Model subclass to wrap tensorflow.keras.Model objects
-* TensorflowOptiModule: OptiModule subclass to wrap keras Optimizer objects
-* TensorflowVector: Vector subclass to wrap tensorflow.Tensor objects
+This submodule provides with a generic interface to wrap up any TensorFlow
+`tensorflow.keras.Model` instance that is to be trained with gradient descent.
 
-It also exposes the `utils` submodule, which mainly aims at
-providing tools used in the backend of the former objects.
+It exposes the following classes:
+
+* [TensorflowModel][declearn.model.tensorflow.TensorflowModel]:
+    Model subclass to wrap tensorflow.keras.Model objects.
+* [TensorflowOptiModule][declearn.model.tensorflow.TensorflowOptiModule]:
+    OptiModule subclass to wrap keras Optimizer objects.
+* [TensorflowVector][declearn.model.tensorflow.TensorflowVector]:
+    Vector subclass to wrap tensorflow.Tensor objects.
+
+It also exposes the [utils][declearn.model.tensorflow.utils] submodule, which
+mainly aims at providing tools used in the backend of the former objects.
 """
 
 from . import utils
 from ._vector import TensorflowVector
 from ._optim import TensorflowOptiModule
 from ._model import TensorflowModel
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/_model.py` & `declearn-2.2.0/declearn/model/tensorflow/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,52 +22,52 @@
 
 import numpy as np
 import tensorflow as tf  # type: ignore
 from numpy.typing import ArrayLike
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.data_info import aggregate_data_info
+from declearn.model._utils import raise_on_stringsets_mismatch
 from declearn.model.api import Model
+from declearn.model.tensorflow._vector import TensorflowVector
 from declearn.model.tensorflow.utils import (
     build_keras_loss,
     move_layer_to_device,
     select_device,
 )
-from declearn.model.tensorflow._vector import TensorflowVector
-from declearn.model._utils import raise_on_stringsets_mismatch
 from declearn.typing import Batch
 from declearn.utils import DevicePolicy, get_device_policy, register_type
 
-
 __all__ = [
     "TensorflowModel",
 ]
 
 
 @register_type(name="TensorflowModel", group="Model")
 class TensorflowModel(Model):
     """Model wrapper for TensorFlow Model instances.
 
     This `Model` subclass is designed to wrap a `tf.keras.Model` instance
     to be trained federatively.
 
     Notes regarding device management (CPU, GPU, etc.):
-    * By default, tensorflow places data and operations on GPU whenever one
+
+    - By default, tensorflow places data and operations on GPU whenever one
       is available.
-    * Our `TensorflowModel` instead consults the device-placement policy (via
+    - Our `TensorflowModel` instead consults the device-placement policy (via
       `declearn.utils.get_device_policy`), places the wrapped keras model's
       weights there, and runs computations defined under public methods in
       a `tensorflow.device` context, to enforce that policy.
-    * Note that there is no guarantee that calling a private method directly
+    - Note that there is no guarantee that calling a private method directly
       will result in abiding by that policy. Hence, be careful when writing
       custom code, and use your own context managers to get guarantees.
-    * Note that if the global device-placement policy is updated, this will
+    - Note that if the global device-placement policy is updated, this will
       only be propagated to existing instances by manually calling their
       `update_device_policy` method.
-    * You may consult the device policy currently enforced by a TensorflowModel
+    - You may consult the device policy enforced by a TensorflowModel
       instance by accessing its `device_policy` property.
     """
 
     def __init__(
         self,
         model: tf.keras.layers.Layer,
         loss: Union[str, tf.keras.losses.Loss],
@@ -128,24 +128,28 @@
             idx = None
         return DevicePolicy(gpu=(device.device_type == "GPU"), idx=idx)
 
     @property
     def required_data_info(
         self,
     ) -> Set[str]:
-        return set() if self._model.built else {"input_shape"}
+        return set() if self._model.built else {"features_shape"}
 
     def initialize(
         self,
         data_info: Dict[str, Any],
     ) -> None:
         if not self._model.built:
-            data_info = aggregate_data_info([data_info], {"input_shape"})
+            # Type- and value-check the provided information.
+            data_info = aggregate_data_info(
+                [data_info], self.required_data_info
+            )
+            # Build the model using the specified input shape.
             with tf.device(self._device):
-                self._model.build(data_info["input_shape"])
+                self._model.build((None, *data_info["features_shape"]))
 
     def get_config(
         self,
     ) -> Dict[str, Any]:
         config = tf.keras.layers.serialize(self._model)  # type: Dict[str, Any]
         kwargs = deepcopy(self._kwargs)
         loss = tf.keras.losses.serialize(kwargs.pop("loss"))
@@ -175,15 +179,15 @@
         trainable: bool = False,
     ) -> TensorflowVector:
         variables = (
             self._model.trainable_weights if trainable else self._model.weights
         )
         return TensorflowVector({var.name: var.value() for var in variables})
 
-    def set_weights(  # type: ignore  # Vector subtype specification
+    def set_weights(
         self,
         weights: TensorflowVector,
         trainable: bool = False,
     ) -> None:
         if not isinstance(weights, TensorflowVector):
             raise TypeError(
                 "TensorflowModel requires TensorflowVector weights."
@@ -208,15 +212,15 @@
             values or gradient-based updates).
         trainable: bool, default=False
             Whether to restrict the comparision to the model's trainable
             weights rather than to all of its weights.
 
         Raises
         ------
-        KeyError:
+        KeyError
             In case some expected keys are missing, or additional keys
             are present. Be verbose about the identified mismatch(es).
         """
         variables = (
             self._model.trainable_weights if trainable else self._model.weights
         )
         raise_on_stringsets_mismatch(
@@ -251,14 +255,15 @@
         # Define an array-to-tensor conversion routine.
         def convert(data: Optional[ArrayLike]) -> Optional[tf.Tensor]:
             if (data is None) or tf.is_tensor(data):
                 return data
             return tf.convert_to_tensor(data)
         # Apply it to the the batched elements.
         return tf.nest.map_structure(convert, batch)
+        # fmt: on
 
     @tf.function  # optimize tensorflow runtime
     def _compute_batch_gradients(
         self,
         inputs: tf.Tensor,
         y_true: Optional[tf.Tensor],
         s_wght: Optional[tf.Tensor],
@@ -310,15 +315,15 @@
         outp = []  # type: List[tf.Tensor]
         for grad in gradients:
             dims = list(range(1, grad.shape.rank))
             grad = tf.clip_by_norm(grad, max_norm, axes=dims)
             outp.append(tf.reduce_mean(grad * s_wght, axis=0))
         return outp
 
-    def apply_updates(  # type: ignore  # Vector subtype specification
+    def apply_updates(
         self,
         updates: TensorflowVector,
     ) -> None:
         self._verify_weights_compatibility(updates, trainable=True)
         with tf.device(self._device):
             for var in self._model.trainable_weights:
                 updt = updates.coefs[var.name]
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/_optim.py` & `declearn-2.2.0/declearn/model/tensorflow/_optim.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,21 @@
     and computations. `reset` also drops internal states' values.
 
     Please note that this relies on a hack that may have unforeseen side
     effects on the optimization algorithm if used carelessly and will at
     any rate cause some memory overhead. Thus it should be used sparingly,
     taking into account the following constraints and limitations:
 
-    * The wrapped optimizer's learning rate will be forced to 1.0, so that
+    - The wrapped optimizer's learning rate will be forced to 1.0, so that
       updates' scaling remains the responsibility of the wrapping declearn
       Optimizer.
-    * The wrapped optimizer should not make use of the updated variables'
+    - The wrapped optimizer should not make use of the updated variables'
       values, only of their gradients, because it will in fact operate on
       artificial, zero-valued variables at each step.
-    * If the module is to be used by the clients, the wrapped optimizer
+    - If the module is to be used by the clients, the wrapped optimizer
       class must have been imported from a third-party package that is
       also available to the clients (e.g. tensorflow).
 
     This class is mostly provided for experimental use of algorithms that
     are not natively available in declearn, for users that do not want to
     put in (or reserve for later) the effort of writing a custom, dedicated,
     framework-agnostic OptiModule subclass implementing that algorithm.
@@ -126,18 +126,18 @@
         Parameters
         ----------
         gradients: TensorflowVector
             Input gradients that are to be processed and updated.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If `gradients` are not a TensorflowVector (this module is
             a framework-specific hack).
-        KeyError:
+        KeyError
             If `gradients` have an inconsistent spec with the first
             ones ever processed by this module. Use `reset` if you
             wish to start back from the beginning.
 
         Returns
         -------
         gradients: TensorflowVector
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/_vector.py` & `declearn-2.2.0/declearn/model/tensorflow/_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,18 +92,18 @@
     such as SparseTensor or RaggedTensor.
 
     Use `vector.coefs` to access the stored coefficients.
 
     Notes
     -----
     - A `TensorflowVector` can be operated with either a:
-      - scalar value
-      - `NumpyVector` that has similar specifications
-      - `TensorflowVector` that has similar specifications
-      => resulting in a `TensorflowVector` in each of these cases.
+        - scalar value
+        - `NumpyVector` that has similar specifications
+        - `TensorflowVector` that has similar specifications
+        - => resulting in a `TensorflowVector` in each of these cases.
     - The wrapped tensors may be placed on any device (CPU, GPU...)
       and may not be all on the same device.
     - The device-placement of the initial `TensorflowVector`'s data
       is preserved by operations, including with `NumpyVector`.
     - When combining two `TensorflowVector`, the device-placement
       of the left-most one is used; in that case, one ends up with
       `gpu + cpu = gpu` while `cpu + gpu = cpu`. In both cases, a
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/utils/__init__.py` & `declearn-2.2.0/declearn/test_utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utils for tensorflow backend support code.
+"""Collection of utils for running tests and examples around declearn.
 
-GPU/CPU backing device management utils:
-* move_layer_to_device:
-    Create a copy of an input keras layer placed on a given device.
-* preserve_tensor_device:
-    Wrap a tensor-processing function to have it run on its inputs' device.
-* select_device:
-    Select a backing device to use based on inputs and availability.
+This submodule is not imported with declearn by default - it requires
+being explicitly imported, and should not be so by end-users, unless
+they accept the risk of using unstable features.
 
-Loss function management utils:
-* build_keras_loss:
-    Type-check, deserialize and/or wrap a keras loss into a Loss object.
-
-Better support for sparse tensor structures:
-* add_indexed_slices_support:
-    Run a function on a pair of tensors, adding support for IndexedSlices.
+This submodule is *not* considered part of the stable declearn API,
+meaning that its contents may change without warnings. Its features
+are not designed to be used outside of the scope of declearn-shipped
+tests and examples. It may also serve to introduce experimental new
+features that may be ported to the stable API in the future.
 """
 
-from ._gpu import (
-    move_layer_to_device,
-    preserve_tensor_device,
-    select_device,
+from ._argparse import setup_client_argparse, setup_server_argparse
+from ._assertions import (
+    assert_dict_equal,
+    assert_list_equal,
+    assert_json_serializable_dict,
+)
+from ._gen_ssl import generate_ssl_certificates
+from ._imports import make_importable
+from ._vectors import (
+    FrameworkType,
+    GradientsTestCase,
+    list_available_frameworks,
 )
-from ._loss import build_keras_loss
-from ._slices import add_indexed_slices_support
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/utils/_gpu.py` & `declearn-2.2.0/declearn/model/tensorflow/utils/_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     idx: int or None, default=None
         Optional pre-selected device index. Only used when `gpu=True`.
         If `idx is None` or exceeds the number of available GPU devices,
         use the first available one.
 
     Warns
     -----
-    UserWarning:
+    RuntimeWarning
         If `gpu=True` but no GPU is available.
         If `idx` exceeds the number of available GPU devices.
 
     Returns
     -------
     device: tf.config.LogicalDevice
         Selected device, usable as `tf.device` argument.
@@ -69,15 +69,16 @@
         )
         device_type, idx = "CPU", 0
         devices = tf.config.list_logical_devices("CPU")
     # Case when the desired device index is invalid: select another one.
     if idx >= len(devices):
         warnings.warn(
             f"Cannot use {device_type} device n°{idx}: index is out-of-range."
-            f"\nUsing {device_type} device n°0 instead."
+            f"\nUsing {device_type} device n°0 instead.",
+            RuntimeWarning,
         )
         idx = 0
     # Return the selected device.
     return devices[idx]
 
 
 def move_layer_to_device(
```

### Comparing `declearn-2.1.0/declearn/model/tensorflow/utils/_loss.py` & `declearn-2.2.0/declearn/model/tensorflow/utils/_loss.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/model/tensorflow/utils/_slices.py` & `declearn-2.2.0/declearn/model/tensorflow/utils/_slices.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         or from re-wrapping `tf_op(first.values, other[.values])` into a
         tf.IndexedSlices structure if first is such a structure. The only
         exception is when operating on IndexedSlices and a full-rank array
         or tensor: then a full-rank output is returned, with a warning.
 
     Raises
     ------
-    TypeError:
+    TypeError
         If `first` and `other` are two tf.IndexedSlices with different
         shapes or non-zero indices.
         If `first` is a tf.IndexedSlices and `func` failed on its values.
     """
     slice_inp = isinstance(first, tf.IndexedSlices)
     # Case when combining two IndexedSlices objects.
     if slice_inp and isinstance(other, tf.IndexedSlices):
@@ -120,15 +120,15 @@
     inplc: bool, default=False
         Whether to replace the second argument of `tf_op` with None.
         Use this to transform tensor-processing functions (wich, in
         general, have a `name=None` argument) rather than operations.
 
     Returns
     -------
-    func: function(<T>, any) -> <T>, with <T>:(tf.Tensor|tf.IndexedSlices)
+    func:
         Tensor-processing operation that wraps `tf_op` but supports and
         preserves tf.IndexedSlices inputs as first (and opt. second)
         argument.
         Note that in the rare case when func(slices, dense) is called,
         the output will be dense, and a RuntimeWarning will be raised.
     """
     func = functools.partial(apply_func_to_tensor_or_slices, tf_op=tf_op)
```

### Comparing `declearn-2.1.0/declearn/model/torch/__init__.py` & `declearn-2.2.0/declearn/model/torch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tensorflow models interfacing tools.
+"""Pytorch models interfacing tools.
 
-This submodule provides with a generic interface to wrap up
-any PyTorch `nn.Module` instance that is to be trained with
-gradient descent.
-
-This module exposes:
-* TorchModel: Model subclass to wrap torch.nn.Module objects
-* TorchOptiModule: OptiModule subclass to wrap torch.nn.Optimizer objects
-* TorchVector: Vector subclass to wrap torch.Tensor objects
+This submodule provides with a generic interface to wrap up any PyTorch
+`torch.nn.Module` instance that is to be trained with gradient descent.
 
-It also exposes the `utils` submodule, which mainly aims at
-providing tools used in the backend of the former objects.
+This module exposes the following classes:
+
+* [TorchModel][declearn.model.torch.TorchModel]:
+    Model subclass to wrap torch.nn.Module objects.
+* [TorchOptiModule][declearn.model.torch.TorchOptiModule]:
+    OptiModule subclass to wrap torch.nn.Optimizer objects.
+* [TorchVector][declearn.model.torch.TorchVector]:
+    Vector subclass to wrap torch.Tensor objects.
+
+It also exposes the [utils][declearn.model.torch.utils] submodule, which
+mainly aims at providing tools used in the backend of the former objects.
 """
 
 from . import utils
 from ._vector import TorchVector
 from ._optim import TorchOptiModule
 from ._model import TorchModel
```

### Comparing `declearn-2.1.0/declearn/model/torch/_model.py` & `declearn-2.2.0/declearn/model/torch/_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Model subclass to wrap PyTorch models."""
 
+import functools
 import io
 import warnings
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple
 
 import functorch  # type: ignore
+
+try:
+    import functorch.compile  # type: ignore
+except ModuleNotFoundError:
+    COMPILE_AVAILABLE = False
+else:
+    COMPILE_AVAILABLE = True
 import numpy as np
 import torch
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Model
 from declearn.model.torch.utils import AutoDeviceModule, select_device
 from declearn.model.torch._vector import TorchVector
@@ -49,26 +57,27 @@
 class TorchModel(Model):
     """Model wrapper for PyTorch Model instances.
 
     This `Model` subclass is designed to wrap a `torch.nn.Module` instance
     to be trained federatively.
 
     Notes regarding device management (CPU, GPU, etc.):
-    * By default torch operates on CPU, and it does not automatically move
+
+    - By default torch operates on CPU, and it does not automatically move
       tensors between devices. This means users have to be careful where
       tensors are placed to avoid operations between tensors on different
       devices, leading to runtime errors.
-    * Our `TorchModel` instead consults the global device-placement policy
+    - Our `TorchModel` instead consults the global device-placement policy
       (via `declearn.utils.get_device_policy`), places the wrapped torch
       modules' weights there, and automates the placement of input data on
       the same device as the wrapped model.
-    * Note that if the global device-placement policy is updated, this will
+    - Note that if the global device-placement policy is updated, this will
       only be propagated to existing instances by manually calling their
       `update_device_policy` method.
-    * You may consult the device policy currently enforced by a TorchModel
+    - You may consult the device policy currently enforced by a TorchModel
       instance by accessing its `device_policy` property.
     """
 
     def __init__(
         self,
         model: torch.nn.Module,
         loss: torch.nn.Module,
@@ -78,15 +87,17 @@
         Parameters
         ----------
         model: torch.nn.Module
             Torch Module instance that defines the model's architecture.
         loss: torch.nn.Module
             Torch Module instance that defines the model's loss, that
             is to be minimized through training. Note that it will be
-            altered when wrapped.
+            altered when wrapped. It must expect `y_pred` and `y_true`
+            as input arguments (in that order) and will be used to get
+            sample-wise loss values (by removing any reduction scheme).
         """
         # Type-check the input model.
         if not isinstance(model, torch.nn.Module):
             raise TypeError("'model' should be a torch.nn.Module instance.")
         # Select the device where to place computations, and wrap the model.
         policy = get_device_policy()
         device = select_device(gpu=policy.gpu, idx=policy.idx)
@@ -94,15 +105,15 @@
         super().__init__(model)
         # Assign loss module and set it not to reduce sample-wise values.
         if not isinstance(loss, torch.nn.Module):
             raise TypeError("'loss' should be a torch.nn.Module instance.")
         loss.reduction = "none"  # type: ignore
         self._loss_fn = AutoDeviceModule(loss, device=device)
         # Compute and assign a functional version of the model.
-        self._func_model = functorch.make_functional(self._model)[0]
+        self._func_model, _ = functorch.make_functional(self._model)
 
     @property
     def device_policy(
         self,
     ) -> DevicePolicy:
         device = self._model.device
         return DevicePolicy(gpu=(device.type == "cuda"), idx=device.index)
@@ -153,15 +164,15 @@
         if trainable:
             weights = {k: p.data for k, p in params if p.requires_grad}
         else:
             weights = {k: p.data for k, p in params}
         # Note: calling `tensor.clone()` to return a copy rather than a view.
         return TorchVector({k: t.detach().clone() for k, t in weights.items()})
 
-    def set_weights(  # type: ignore  # Vector subtype specification
+    def set_weights(
         self,
         weights: TorchVector,
         trainable: bool = False,
     ) -> None:
         if not isinstance(weights, TorchVector):
             raise TypeError("TorchModel requires TorchVector weights.")
         self._verify_weights_compatibility(weights, trainable=trainable)
@@ -187,15 +198,15 @@
             values or gradient-based updates).
         trainable: bool, default=False
             Whether to restrict the comparision to the model's trainable
             weights rather than to all of its weights.
 
         Raises
         ------
-        KeyError:
+        KeyError
             In case some expected keys are missing, or additional keys
             are present. Be verbose about the identified mismatch(es).
         """
         received = set(vector.coefs)
         expected = {
             name
             for name, param in self._model.named_parameters()
@@ -260,127 +271,118 @@
     ) -> torch.Tensor:
         """Compute the average (opt. weighted) loss over given predictions."""
         loss = self._loss_fn(y_pred, y_true)
         if s_wght is not None:
             loss.mul_(s_wght.to(loss.device))
         return loss.mean()
 
-    def _compute_samplewise_gradients(
+    def _compute_clipped_gradients(
         self,
         batch: Batch,
+        max_norm: float,
     ) -> TorchVector:
-        """Compute and return stacked sample-wise gradients from a batch."""
-        # Delegate preparation of the gradients-computing function.
-        # fmt: off
-        grads_fn, data, params, pnames, in_axes = (
-            self._prepare_samplewise_gradients_computations(batch)
+        """Compute and return batch-averaged sample-wise-clipped gradients."""
+        # Compute sample-wise clipped gradients, using functorch.
+        grads = self._compute_samplewise_gradients(batch, max_norm)
+        # Batch-average the resulting sample-wise gradients.
+        return TorchVector(
+            {name: tensor.mean(dim=0) for name, tensor in grads.coefs.items()}
         )
-        # Vectorize the function to compute sample-wise gradients.
-        with torch.no_grad():
-            grads = functorch.vmap(grads_fn, in_axes)(*data, *params)
-        # Wrap the results into a TorchVector and return it.
-        return TorchVector(dict(zip(pnames, grads)))
 
-    def _compute_clipped_gradients(
+    def _compute_samplewise_gradients(
         self,
         batch: Batch,
-        max_norm: float,
+        max_norm: Optional[float],
     ) -> TorchVector:
-        """Compute and return batch-averaged sample-wise-clipped gradients."""
-        # Delegate preparation of the gradients-computing function.
-        # fmt: off
-        grads_fn, data, params, pnames, in_axes = (
-            self._prepare_samplewise_gradients_computations(batch)
+        """Compute and return stacked sample-wise gradients over a batch."""
+        # Unpack the inputs, gather parameters and list gradients to compute.
+        inputs, y_true, s_wght = self._unpack_batch(batch)
+        params = []  # type: List[torch.nn.Parameter]
+        idxgrd = []  # type: List[int]
+        pnames = []  # type: List[str]
+        for index, (name, param) in enumerate(self._model.named_parameters()):
+            params.append(param)
+            if param.requires_grad:
+                idxgrd.append(index + 3)
+                pnames.append(name)
+        # Gather or build the sample-wise clipped gradients computing function.
+        grads_fn = self._build_samplewise_grads_fn(
+            idxgrd=tuple(idxgrd),
+            inputs=len(inputs),
+            y_true=(y_true is not None),
+            s_wght=(s_wght is not None),
         )
-        # Compose it to clip output gradients on the way.
-        def clipped_grads_fn(inputs, y_true, s_wght, *params):
-            grads = grads_fn(inputs, y_true, None, *params)
-            for grad in grads:
-                # future: use torch.linalg.norm when supported by functorch
-                norm = torch.norm(grad, p=2, keepdim=True)
-                # false-positive; pylint: disable=no-member
-                grad.mul_(torch.clamp(max_norm / norm, max=1))
-                if s_wght is not None:
-                    grad.mul_(s_wght.to(grad.device))
-            return grads
-        # Vectorize the function to compute sample-wise clipped gradients.
+        # Call it on the current inputs, with optional clipping.
         with torch.no_grad():
-            grads = functorch.vmap(clipped_grads_fn, in_axes)(*data, *params)
-        # Wrap batch-averaged results into a TorchVector and return it.
-        return TorchVector(
-            {name: grad.mean(dim=0) for name, grad in zip(pnames, grads)}
-        )
+            grads = grads_fn(inputs, y_true, s_wght, *params, clip=max_norm)
+        # Wrap the results into a TorchVector and return it.
+        return TorchVector(dict(zip(pnames, grads)))
 
-    def _prepare_samplewise_gradients_computations(
+    @functools.lru_cache
+    def _build_samplewise_grads_fn(
         self,
-        batch: Batch,
-    ) -> Tuple[
-        Callable[..., List[torch.Tensor]],
-        TensorBatch,
-        List[torch.nn.Parameter],
-        List[str],
-        Tuple[Any, ...],
-    ]:
-        """Prepare a function an parameters to compute sample-wise gradients.
-
-        Note: this method is merely implemented as a way to avoid code
-        redundancies between the `_compute_samplewise_gradients` method
-        and the `_compute_clipped_gradients` ones.
+        idxgrd: Tuple[int, ...],
+        inputs: int,
+        y_true: bool,
+        s_wght: bool,
+    ) -> Callable[..., List[torch.Tensor]]:
+        """Build a functorch-based sample-wise gradients-computation function.
+
+        This function is cached, i.e. repeated calls with the same parameters
+        will return the same object - enabling to reduce runtime costs due to
+        building and (when available) compiling the output function.
 
         Parameters
         ----------
-        batch: declearn.typing.Batch
-            Batch structure wrapping the input data, target labels and
-            optional sample weights based on which to compute gradients.
+        idxgrd: tuple of int
+            Pre-incremented indices of the parameters that require gradients.
+        inputs: int
+            Number of input tensors.
+        y_true: bool
+            Whether a true labels tensor is provided.
+        s_wght: bool
+            Whether a sample weights tensor is provided.
 
         Returns
         -------
-        grads_fn: function(*data, *params) -> List[torch.Tensor]
-            Functorch-issued gradients computation function.
-        data: tuple([torch.Tensor], torch.Tensor, torch.Tensor or None)
-            Tensor-converted data unpacked from `batch`.
-        params: list[torch.nn.Parameter]
-            Input parameters of the model, some of which require grads.
-        pnames: list[str]
-            Names of the parameters that require gradients.
-        in_axes: tuple(...)
-            Prepared `in_axes` parameter to `functorch.vmap`, suitable
-            to distribute `grads_fn` (or any compose that shares its
-            input signature) over a batch so as to compute sample-wise
-            gradients in a computationally-efficient manner.
+        grads_fn: callable[inputs, y_true, s_wght, *params, /, clip]
+            Functorch-optimized function to efficiently compute sample-
+            wise gradients based on batched inputs, and optionally clip
+            them based on a maximum l2-norm value `clip`.
         """
-        # fmt: off
-        # Unpack and validate inputs.
-        data = (inputs, y_true, s_wght) = self._unpack_batch(batch)
-        # Gather parameters and list those that require gradients.
-        idxgrd = []  # type: List[int]
-        pnames = []  # type: List[str]
-        params = []  # type: List[torch.nn.Parameter]
-        for idx, (name, param) in enumerate(self._model.named_parameters()):
-            params.append(param)
-            if param.requires_grad:
-                pnames.append(name)
-                idxgrd.append(idx)
-        # Define a differentiable function wrapping the forward pass.
+
         def forward(inputs, y_true, s_wght, *params):
+            """Conduct the forward pass in a functional way."""
             y_pred = self._func_model(params, *inputs)
             return self._compute_loss(y_pred, y_true, s_wght)
-        # Transform it into a sample-wise-gradients-computing function.
-        grads_fn = functorch.grad(forward, argnums=tuple(i+3 for i in idxgrd))
-        # Prepare `functools.vmap` parameter to slice through data and params.
-        in_axes = [
-            [0] * len(inputs),
-            None if y_true is None else 0,
-            None if s_wght is None else 0,
-        ]
-        in_axes.extend([None] * len(params))
-        # Return all this prepared material.
-        return grads_fn, data, params, pnames, tuple(in_axes)
 
-    def apply_updates(  # type: ignore  # Vector subtype specification
+        def grads_fn(inputs, y_true, s_wght, *params, clip=None):
+            """Compute gradients and optionally clip them."""
+            gfunc = functorch.grad(forward, argnums=idxgrd)
+            grads = gfunc(inputs, y_true, None, *params)
+            if clip:
+                for grad in grads:
+                    # future: use torch.linalg.norm when supported by functorch
+                    norm = torch.norm(grad, p=2, keepdim=True)
+                    # false-positive; pylint: disable=no-member
+                    grad.mul_(torch.clamp(clip / norm, max=1))
+                    if s_wght is not None:
+                        grad.mul_(s_wght.to(grad.device))
+            return grads
+
+        # Wrap the former function to compute and clip sample-wise gradients.
+        in_axes = [[0] * inputs, 0 if y_true else None, 0 if s_wght else None]
+        in_axes.extend([None] * sum(1 for _ in self._model.parameters()))
+        grads_fn = functorch.vmap(grads_fn, tuple(in_axes))
+        # Compile the resulting function to decrease runtime costs.
+        if not COMPILE_AVAILABLE:
+            return grads_fn
+        return functorch.compile.aot_function(grads_fn, functorch.compile.nop)
+
+    def apply_updates(
         self,
         updates: TorchVector,
     ) -> None:
         if not isinstance(updates, TorchVector):
             raise TypeError("TorchModel requires TorchVector updates.")
         self._verify_weights_compatibility(updates, trainable=True)
         with torch.no_grad():
```

### Comparing `declearn-2.1.0/declearn/model/torch/_optim.py` & `declearn-2.2.0/declearn/model/torch/_optim.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,21 @@
     and device-placement choices at once.
 
     Please note that this relies on a hack that may have unforeseen side
     effects on the optimization algorithm if used carelessly and will at
     any rate cause some memory overhead. Thus it should be used sparingly,
     taking into account the following constraints and limitations:
 
-    * The wrapped optimizer class should have a "lr" (learning-rate)
+    - The wrapped optimizer class should have a "lr" (learning-rate)
       parameter, that will be forced to 1.0, so that updates' scaling
       remains the responsibility of the wrapping declearn Optimizer.
-    * The wrapped optimizer class should not make use of the watched
+    - The wrapped optimizer class should not make use of the watched
       parameters' values, only of their gradients, because it will in
       fact monitor artificial, zero-valued parameters at each step.
-    * If the module is to be used by the clients, the wrapped optimizer
+    - If the module is to be used by the clients, the wrapped optimizer
       class must have been imported from a third-party package that is
       also available to the clients (e.g. torch).
 
     Also note that passing a string input as `optim_cls` (as is always done
     when deserializing the module from its auto-generated config) may raise
     security concerns due to its resulting in importing external code. As a
     consequence, users will be asked to validate any non-torch import before
@@ -126,18 +126,18 @@
         validate: bool, default=True
             Whether the user should be prompted to validate the module-
             import action triggered in case `optim_cls` is a string and
             targets another package than 'torch'.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If `optim_cls` is a string and the target class cannot be loaded.
             If `optim_cls` is a string and the user denies the import command.
-        TypeError:
+        TypeError
             If `optim_cls` (or the object loaded in case it is a string)
             is not a `torch.nn.Optimizer` subclass.
 
         Returns
         -------
         optim_cls: Type[torch.optim.Optimizer]
             Torch Optimizer class constructor.
@@ -177,18 +177,18 @@
         Parameters
         ----------
         gradients: TorchVector
             Input gradients that are to be processed and updated.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If `gradients` are not a TorchVector (this module is
             a framework-specific hack).
-        KeyError:
+        KeyError
             If `gradients` have an inconsistent spec with the first
             ones ever processed by this module. Use `reset` if you
             wish to start back from the beginning.
 
         Returns
         -------
         gradients: TorchVector
```

### Comparing `declearn-2.1.0/declearn/model/torch/_vector.py` & `declearn-2.2.0/declearn/model/torch/_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,18 +44,18 @@
     (i.e. two TorchVector with similar specifications).
 
     Use `vector.coefs` to access the stored coefficients.
 
     Notes
     -----
     - A `TorchVector` can be operated with either a:
-      - scalar value
-      - `NumpyVector` that has similar specifications
-      - `TorchVector` that has similar specifications
-      => resulting in a `TorchVector` in each of these cases.
+        - scalar value
+        - `NumpyVector` that has similar specifications
+        - `TorchVector` that has similar specifications
+        - => resulting in a `TorchVector` in each of these cases.
     - The wrapped tensors may be placed on any device (CPU, GPU...)
       and may not be all on the same device.
     - The device-placement of the initial `TorchVector`'s data
       is preserved by operations, including with `NumpyVector`.
     - When combining two `TorchVector`, the device-placement
       of the left-most one is used; in that case, one ends up with
       `gpu + cpu = gpu` while `cpu + gpu = cpu`. In both cases, a
```

### Comparing `declearn-2.1.0/declearn/model/torch/utils/__init__.py` & `declearn-2.2.0/declearn/model/haiku/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utils for torch backend support code.
+"""Haiku models interfacing tools.
 
-GPU/CPU backing device management utils:
-* AutoDeviceModule:
-    Wrapper for a `torch.nn.Module`, automating device-management.
-* select_device:
-    Select a backing device to use based on inputs and availability.
+This submodule provides with a generic interface to wrap up
+any Haiku module instance that is to be trained
+through gradient descent.
+
+This module exposes:
+* HaikuModel: Model subclass to wrap haiku.Model objects
+* JaxNumpyVector: Vector subclass to wrap jax.numpy.ndarray objects
 """
 
-from ._gpu import AutoDeviceModule, select_device
+from . import utils
+from ._vector import JaxNumpyVector
+from ._model import HaikuModel
```

### Comparing `declearn-2.1.0/declearn/model/torch/utils/_gpu.py` & `declearn-2.2.0/declearn/model/torch/utils/_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     idx: int or None, default=None
         Optional pre-selected GPU device index. Only used when `gpu=True`.
         If `idx is None` or exceeds the number of available GPU devices,
         use `torch.cuda.current_device()`.
 
     Warns
     -----
-    UserWarning:
+    RuntimeWarning
         If `gpu=True` but no GPU is available.
         If `idx` exceeds the number of available GPU devices.
 
     Returns
     -------
     device: torch.device
         Selected torch device, with type "cpu" or "cuda".
@@ -65,33 +65,35 @@
             "or no GPU is visible to torch."
         )
         return torch.device("cpu")  # pylint: disable=no-member
     # Case when the desired GPU is invalid: select another one.
     if (idx or 0) >= torch.cuda.device_count():
         warnings.warn(
             f"Cannot use GPU device n°{idx}: index is out-of-range.\n"
-            f"Using GPU device n°{torch.cuda.current_device()} instead."
+            f"Using GPU device n°{torch.cuda.current_device()} instead.",
+            RuntimeWarning,
         )
         idx = None
     # Return the selected or auto-selected GPU device index.
     if idx is None:
         idx = torch.cuda.current_device()
     return torch.device("cuda", index=idx)  # pylint: disable=no-member
 
 
 class AutoDeviceModule(torch.nn.Module):
     """Wrapper for a `torch.nn.Module`, automating device-management.
 
     This `torch.nn.Module` subclass enables wrapping another one, and
     provides:
-    * a `device` attribute (and instantiation parameter) indicating
+
+    - a `device` attribute (and instantiation parameter) indicating
       where the wrapped module is placed
-    * automatic placement of input tensors on that device as part of
+    - automatic placement of input tensors on that device as part of
       `forward` calls to the module
-    * a `set_device` method to change the device and move the wrapped
+    - a `set_device` method to change the device and move the wrapped
       module to it
 
     This aims at internalizing device-management boilerplate code.
     The wrapped module is assigned to the `module` attribute and thus
     can be accessed directly.
     """
 
@@ -130,11 +132,11 @@
         device: torch.device,  # pylint: disable=no-member
     ) -> None:
         """Move the wrapped module to a pre-selected torch device.
 
         Parameters
         ----------
         device: torch.device
-           Torch device where to place the wrapped module and computations.
+            Torch device where to place the wrapped module and computations.
         """
         self.device = device
         self.module.to(device)
```

### Comparing `declearn-2.1.0/declearn/optimizer/__init__.py` & `declearn-2.2.0/declearn/optimizer/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,18 +18,30 @@
 """Framework-agnostic optimizer tools, both generic or FL-specific.
 
 In more details, we here define an `Optimizer` class that wraps together a set
 of plug-in modules, used to implement various optimization and regularization
 techniques.
 
 Main class:
-* Optimizer: Base class to define gradient-descent-based optimizers.
 
-This module also implements the following submodules, used by the former:
-* modules: gradients-alteration algorithms, implemented as plug-in modules.
-* regularizers: loss-regularization algorithms, implemented as plug-in modules.
+* [Optimizer][declearn.optimizer.Optimizer]:
+    Base class to define gradient-descent-based optimizers.
 
- """
+Submodules providing with plug-in algorithms:
+
+* [modules][declearn.optimizer.modules]:
+    Gradients-alteration algorithms, implemented as plug-in modules.
+* [regularizers][declearn.optimizer.regularizers]:
+    Loss-regularization algorithms, implemented as plug-in modules.
+
+Utils to list available plug-ins:
+
+* [list_optim_modules][declearn.optimizer.list_optim_modules]:
+    Return a mapping of registered OptiModule subclasses.
+* [list_optim_regularizers][declearn.optimizer.list_optim_regularizers]:
+    Return a mapping of registered Regularizer subclasses.
+"""
 
 
 from . import modules, regularizers
 from ._base import Optimizer
+from ._utils import list_optim_modules, list_optim_regularizers
```

### Comparing `declearn-2.1.0/declearn/optimizer/_base.py` & `declearn-2.2.0/declearn/optimizer/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,47 +13,55 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base class to define gradient-descent-based optimizers."""
 
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    # fmt: off
+    Any, Dict, List, Optional, Sequence, Tuple, Type, TypeVar, Union
+)
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Model, Vector
 from declearn.optimizer.modules import OptiModule
 from declearn.optimizer.regularizers import Regularizer
 from declearn.typing import Batch
 
 __all__ = [
     "Optimizer",
 ]
 
 
+T = TypeVar("T")
+
+
 class Optimizer:
     """Base class to define gradient-descent-based optimizers.
 
     The `Optimizer` class defines an API that is required by other
     declearn components for federated learning processes to run.
     It is also fully-workable and is designed to be customizable
     through the use of "plug-in modules" rather than subclassing
     (which might be used for advanced algorithm modifications):
-    see `declearn.optimizer.modules.OptiModule` for API details.
+    see the base classes [declearn.optimizer.modules.OptiModule][]
+    and [declearn.optimizer.regularizers.Regularizer][] for details.
 
     The process implemented here is the following:
-    * Compute or receive the (pseudo-)gradients of a model.
-    * Compute loss-regularization terms and add them to the
+
+    - Compute or receive the (pseudo-)gradients of a model.
+    - Compute loss-regularization terms and add them to the
       gradients, based on a list of plug-in regularizers.
-    * Refine gradients by running them through plug-in modules,
+    - Refine gradients by running them through plug-in modules,
       which are thus composed by sequential application.
-    * Optionally compute a decoupled weight decay term (see [1])
+    - Optionally compute a decoupled weight decay term (see [1])
       and add it to the updates (i.e. refined gradients).
-    * Apply the learning rate and perform the weights' udpate.
+    - Apply the learning rate and perform the weights' udpate.
 
     Most plug-in modules are self-contained, in the sense that they
     do not require any information flow between the server and its
     clients in a federated process, and may be used solely by the
     server, by clients or even by a subset of clients - at least
     formally (their might be correctness or convergence issues with
     clients not adopting similar local optimization strategies).
@@ -66,46 +74,52 @@
     mechanisms are to be implemented at the level of the modules
     themselves, but are wrapped at optimizer level, which collects
     plugged-in-modules' variables and maps back received variables
     to them.
 
     Attributes
     ----------
-
     lrate: float
         Base learning rate applied to computed updates.
     w_decay: float
         Decoupled weight decay parameter.
     modules: list[OptiModule]
         List of plug-in modules composed into the optimizer's
         gradients-to-updates computation algorithm.
     regularizers: list[Regularizer]
         List of plug-in loss regularization modules composed into
         the optimizer's gradients-to-updates computation algorithm.
 
-    API methods:
+    API methods
     -----------
-    apply_gradients(Model, Vector) -> None:
+    - apply_gradients(Model, Vector) -> None:
         Update a Model based on a pre-computed Vector of gradients.
-    collect_aux_var() -> Dict[str, Dict[str, Any]]:
+    - collect_aux_var() -> Dict[str, Dict[str, Any]]:
         Collect and package plug-in modules' auxiliary variables.
-    compute_updates_from_gradients(Model, Vector) -> Vector:
+    - compute_updates_from_gradients(Model, Vector) -> Vector:
         Compute and return model updates based on pre-computed gradients.
-    process_aux_var(Dict[str, Dict[str, Any]]) -> None:
+    - process_aux_var(Dict[str, Dict[str, Any]]) -> None:
         Pass auxiliary variables to plug-in modules for processing.
-    run_train_step(Model, batch) -> None:
+    - run_train_step(Model, batch) -> None:
         Compute gradients of a Model over a Batch and apply updates.
-    start_round() -> None:
+    - start_round() -> None:
         Signal that a new training round is starting to wrapped regularizers.
 
     References
     ----------
     [1] Loshchilov & Hutter, 2019.
         Decoupled Weight Decay Regularization.
         https://arxiv.org/abs/1711.05101
+
+    See also
+    --------
+    - [declearn.optimizer.list_optim_modules][]:
+        Return a mapping of registered OptiModule subclasses.
+    - [declearn.optimizer.list_optim_regularizers][]:
+        Return a mapping of registered Regularizer subclasses.
     """
 
     def __init__(
         self,
         lrate: float,  # future: add scheduling tools
         w_decay: float = 0.0,  # future: add scheduling tools
         regularizers: Optional[
@@ -242,25 +256,25 @@
         Parameters
         ----------
         config: dict[str, Any]
             Dict storing the optimizer's instantiation configuration.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If the provided `config` lacks some required parameters
             and/or contains some unused ones.
         """
         return cls(**config)
 
     def compute_updates_from_gradients(
         self,
-        model: Model,
-        gradients: Vector,
-    ) -> Vector:
+        model: Model[Vector[T]],
+        gradients: Vector[T],
+    ) -> Vector[T]:
         """Compute and return model updates based on pre-computed gradients.
 
         Parameters
         ----------
         model: Model
             Model instance that is to be trained using gradient-descent.
             This parameter is only used to access current weights in case
@@ -388,16 +402,16 @@
             This method does not return, as `model` is updated in-place.
         """
         gradients = model.compute_batch_gradients(batch, max_norm=sclip)
         self.apply_gradients(model, gradients)
 
     def apply_gradients(
         self,
-        model: Model,
-        gradients: Vector,
+        model: Model[Vector[T]],
+        gradients: Vector[T],
     ) -> None:
         """Compute and apply model updates based on pre-computed gradients.
 
         Parameters
         ----------
         model: Model
             Model instance that is to be trained using gradient-descent.
@@ -436,27 +450,27 @@
     ) -> None:
         """Load a saved state dict into an optimizer instance.
 
         The counterpart to this method is the `get_state` one.
 
         Parameters
         ----------
-        state: dict[str, any]
+        states: dict[str, any]
             Dict storing values to assign to this optimizer's inner
             state variables (i.e. those from its modules).
 
         Raises
         ------
-        KeyError:
+        KeyError
             If the received states do not match the expected config,
             whether because a module is missing or one of its states
             is missing.
             In both cases, the Optimizer's states will be reverted
             to their values prior to the failed call to this method.
-        RuntimeError:
+        RuntimeError
             If a KeyError was raised both when trying to apply the
             input `state` and when trying to revert the states to
             their initial values after that first error was raised.
             This should never happen and indicates a source code
             error in a wrapped module, or even in this class.
         """
         if "modules" not in states:
```

### Comparing `declearn-2.1.0/declearn/optimizer/modules/_adaptive.py` & `declearn-2.2.0/declearn/optimizer/modules/_adaptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,27 @@
 ]
 
 
 class AdaGradModule(OptiModule):
     """Adaptative Gradient Algorithm (AdaGrad) module.
 
     This module implements the following algorithm:
+
         Init(eps):
             state = 0
         Step(grads):
             state += (grads ** 2)
             grads /= (sqrt(state) + eps)
 
     In other words, gradients (i.e. indirectly the learning rate)
     are scaled down by the square-root of the sum of the past
     squared gradients. See reference [1].
 
-    References:
+    References
+    ----------
     [1] Duchi et al., 2012.
         Adaptive Subgradient Methods for Online Learning
         and Stochastic Optimization.
         https://jmlr.org/papers/v12/duchi11a.html
     """
 
     name: ClassVar[str] = "adagrad"
@@ -96,25 +98,27 @@
         self.state = state["state"]
 
 
 class RMSPropModule(OptiModule):
     """Root Mean Square Propagation (RMSProp) module.
 
     This module implements the following algorithm:
+
         Init(beta, eps):
             state = 0
         Step(grads, step):
             state = beta*state + (1-beta)*(grads**2)
             grads /= (sqrt(state) + eps)
 
     In other words, gradients (i.e. indirectly the learning rate)
     are scaled down by the square-root of the momentum-corrected
     sum of the past squared gradients. See reference [1].
 
-    References:
+    References
+    ----------
     [1] Tieleman and Hinton, 2012.
         Lecture 6.5-rmsprop: Divide the Gradient by a Running
         Average of its Recent Magnitude.
     """
 
     name: ClassVar[str] = "rmsprop"
 
@@ -162,14 +166,15 @@
         self.ewma.set_state(state)
 
 
 class AdamModule(OptiModule):
     """Adaptive Moment Estimation (Adam) module.
 
     This module implements the following algorithm:
+
         Init(beta_1, beta_2, eps):
             state_m = 0
             state_v = 0
         Step(grads, step):
             state_m = beta_1*state_m + (1-beta_1)*grads
             state_v = beta_2*state_v + (1-beta_2)*(grads**2)
             m_hat = state_m / (1 - beta_1**step)
@@ -185,19 +190,22 @@
     Optionally, the AMSGrad [2] algorithm may be implemented,
     with a similar formula but using the element-wise maximum
     of present-and-past v_hat values as a scaling factor. This
     guarantees that the learning rate is shrinked across time,
     at least from the point of view of this module (a warm-up
     schedule might for example counteract this).
 
-    References:
-    [1] Kingma and Ba, 2014.
+    References
+    ----------
+    - [1]
+        Kingma and Ba, 2014.
         Adam: A Method for Stochastic Optimization.
         https://arxiv.org/abs/1412.6980
-    [2] Reddi et al., 2018.
+    - [2]
+        Reddi et al., 2018.
         On the Convergence of Adam and Beyond.
         https://arxiv.org/abs/1904.09237
     """
 
     name: ClassVar[str] = "adam"
 
     def __init__(
@@ -285,14 +293,15 @@
         self.vmax = state["vmax"]
 
 
 class YogiModule(AdamModule):
     """Yogi additive adaptive moment estimation module.
 
     This module implements the following algorithm:
+
         Init(beta_1, beta_2, eps):
             state_m = 0
             state_v = 0
         Step(grads, step):
             state_m = beta_1*state_m + (1-beta_1)*grads
             sign_uv = sign(state_v - grads**2)
             state_v = state_v + sign_uv*(1-beta_2)*(grads**2)
@@ -303,21 +312,25 @@
     In other words, Yogi [1] implements the Adam [2] algorithm,
     but modifies the update rule of the 'v' state variable that
     is used to scale the learning rate.
 
     Note that this implementation allows combining the Yogi
     modification of Adam with the AMSGrad [3] one.
 
-    References:
-    [1] Zaheer and Reddi et al., 2018.
+    References
+    ----------
+    - [1]
+        Zaheer and Reddi et al., 2018.
         Adaptive Methods for Nonconvex Optimization.
-    [2] Kingma and Ba, 2014.
+    - [2]
+        Kingma and Ba, 2014.
         Adam: A Method for Stochastic Optimization.
         https://arxiv.org/abs/1412.6980
-    [3] Reddi et al., 2018.
+    - [3]
+        Reddi et al., 2018.
         On the Convergence of Adam and Beyond.
         https://arxiv.org/abs/1904.09237
     """
 
     name: ClassVar[str] = "yogi"
 
     def __init__(
```

### Comparing `declearn-2.1.0/declearn/optimizer/modules/_api.py` & `declearn-2.2.0/declearn/optimizer/modules/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base API for plug-in gradients-alteration algorithms."""
 
 from abc import ABCMeta, abstractmethod
-from typing import Any, ClassVar, Dict, Optional
+from typing import Any, ClassVar, Dict, Optional, TypeVar
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Vector
 from declearn.utils import (
     access_registered,
     create_types_registry,
@@ -30,14 +30,17 @@
 )
 
 __all__ = [
     "OptiModule",
 ]
 
 
+T = TypeVar("T")
+
+
 @create_types_registry
 class OptiModule(metaclass=ABCMeta):
     """Abstract class defining an API to implement gradients adaptation tools.
 
     The aim of this abstraction (which itself operates on the Vector
     abstraction, so as to provide framework-agnostic algorithms) is
     to enable implementing unitary gradients-adaptation bricks that
@@ -52,69 +55,77 @@
     weight-decay mechanisms are implemented at `Optimizer` level.
 
     Abstract
     --------
     The following attribute and method require to be overridden
     by any non-abstract child class of `OptiModule`:
 
-    name: str class attribute
+    - name: str class attribute
         Name identifier of the class (should be unique across existing
         OptiModule classes). Also used for automatic types-registration
         of the class (see `Inheritance` section below).
-    run(gradients: Vector) -> Vector:
+    - run(gradients: Vector) -> Vector:
         Apply an adaptation algorithm to input gradients and return
         them. This is the main method for any `OptiModule`.
 
     Overridable
     -----------
     The following methods may be overridden to implement information-
     passing and parallel behaviors between client/server module pairs.
     As defined at `OptiModule` level, they have no effect and may thus
     be safely ignored when implementing self-contained algorithms.
 
-    collect_aux_var() -> Optional[Dict[str, Any]]:
+    - collect_aux_var() -> Optional[Dict[str, Any]]:
         Emit a JSON-serializable dict of auxiliary variables,
         to be received by a counterpart of this module on the
         other side of the client/server relationship.
-    process_aux_var(Dict[str, Any]) -> None:
+    - process_aux_var(Dict[str, Any]) -> None:
         Process a dict of auxiliary variables, received from
         a counterpart to this module on the other side of the
         client/server relationship.
-    aux_name: optional[str] class attribute, default=None
+    - aux_name: optional[str] class attribute, default=None
         Name to use when sending or receiving auxiliary variables
         between synchronous client/server modules, that therefore
         need to share the *same* `aux_name`.
 
     Inheritance
     -----------
     When a subclass inheriting from `OptiModule` is declared, it is
     automatically registered under the "OptiModule" group using its
     class-attribute `name`. This can be prevented by adding `register=False`
     to the inheritance specs (e.g. `class MyCls(OptiModule, register=False)`).
     See `declearn.utils.register_type` for details on types registration.
     """
 
     name: ClassVar[str] = NotImplemented
+    """Name identifier of the class, unique across OptiModule classes."""
+
     aux_name: ClassVar[Optional[str]] = None
+    """Optional aux-var-sharing identifier of the class.
+
+    This name may be shared by a pair of OptiModule classes, designed
+    to operate on the client and server side respectively. It should
+    be unique to that pair of classes across all OptiModule classes.
+    """
 
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automatically type-register OptiModule subclasses."""
         super().__init_subclass__(**kwargs)
         if register:
             register_type(cls, cls.name, group="OptiModule")
 
     @abstractmethod
     def run(
         self,
-        gradients: Vector,
-    ) -> Vector:
+        gradients: Vector[T],
+    ) -> Vector[T]:
         """Apply the module's algorithm to input gradients.
 
         Please refer to the module's main docstring for details
         on the implemented algorithm and the way it transforms
         input gradients.
 
         Parameters
@@ -133,37 +144,38 @@
     def collect_aux_var(
         self,
     ) -> Optional[Dict[str, Any]]:
         """Return auxiliary variables that need to be shared between nodes.
 
         Returns
         -------
-        aux_var: dict[str, any] or None
+        aux_var: Optional[Dict[str, Any]]
             Optional JSON-serializable dict of auxiliary variables that
             are to be shared with a similarly-named OptiModule on the
             other side of the client-server relationship.
 
         Notes
         -----
         Specfications for the output and calling context depend on whether
         the module is part of a client's optimizer or of the server's one:
-        * Client:
-          - aux_var is dict[str, any] or None.
-          - `collect_aux_var` is expected to happen after taking a series
-            of local optimization steps, before sending the local updates
-            to the server for aggregation and further processing.
-        * Server:
-          - aux_var may be None ; dict[str, any] (to send the same values
-            to each and every client) ; or dict[str, dict[str, any]] with
-            clients' names as keys and client-wise new aux_var as values
-            so as to send distinct values to the clients.
-          - `collect_aux_var` is expected to happen when the global model
-            weights are ready to be shared with clients, i.e. at the very
-            end of a training round or at the beginning of the training
-            process.
+
+        - Client:
+            - `aux_var` is dict[str, any] or None.
+            - `collect_aux_var` is expected to happen after taking a series
+              of local optimization steps, before sending the local updates
+              to the server for aggregation and further processing.
+        - Server:
+            - `aux_var` may be None ; dict[str, any] (to send the same values
+              to each and every client) ; or dict[str, dict[str, any]] with
+              clients' names as keys and client-wise new aux_var as values
+              so as to send distinct values to the clients.
+            - `collect_aux_var` is expected to happen when the global model
+              weights are ready to be shared with clients, i.e. at the very
+              end of a training round or at the beginning of the training
+              process.
         """
         return None
 
     def process_aux_var(
         self,
         aux_var: Dict[str, Any],
     ) -> None:
@@ -177,32 +189,33 @@
             the client side) or before processing global updates (on the
             server side).
 
         Notes
         -----
         Specfications for the inputs and calling context depend on whether
         the module is part of a client's optimizer or of the server's one:
-        * Client:
-          - aux_var is dict[str, any] and may be client-specific.
-          - `process_aux_var` is expected to happen at the beginning of
-            a training round to define gradients' processing during the
-            local optimization steps taken through that round.
-        * Server:
-          - aux_var is dict[str, dict[str, any]] with clients' names as
-            primary keys and client-wise collected aux_var as values.
-          - `process_aux_var` is expected to happen upon receiving local
-            updates (and, thus, aux_var), before the aggregated updates
-            are computed and passed through the server optimizer (which
-            comprises this module).
+
+        - Client:
+            - `aux_var` is dict[str, any] and may be client-specific.
+            - `process_aux_var` is expected to happen at the beginning of
+              a training round to define gradients' processing during the
+              local optimization steps taken through that round.
+        - Server:
+            - `aux_var` is dict[str, dict[str, any]] with clients' names as
+              primary keys and client-wise collected aux_var as values.
+            - `process_aux_var` is expected to happen upon receiving local
+              updates (and, thus, aux_var), before the aggregated updates
+              are computed and passed through the server optimizer (which
+              comprises this module).
 
         Raises
         ------
-        KeyError:
+        KeyError
             If an expected auxiliary variable is missing.
-        TypeError:
+        TypeError
             If a variable is of unproper type, or if aux_var
             is not formatted as it should be.
         """
         # API-defining method; pylint: disable=unused-argument
 
     def get_config(
         self,
@@ -210,15 +223,15 @@
         """Return a JSON-serializable dict with this module's parameters.
 
         The counterpart to this method is the `from_config` classmethod.
         To access the module's inner states, see the `get_state` method.
 
         Returns
         -------
-        config: dict[str, any]
+        config: Dict[str, Any]
             JSON-serializable dict storing this module's instantiation
             configuration.
         """
         return {}
 
     @classmethod
     def from_config(
@@ -234,15 +247,15 @@
         ----------
         config: dict[str, Any]
             Dict storing the module's instantiation configuration.
             This must match the target subclass's requirements.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If the provided `config` lacks some required parameters
             and/or contains some unused ones.
         """
         return cls(**config)
 
     @staticmethod
     def from_specs(
@@ -269,15 +282,15 @@
     ) -> Dict[str, Any]:
         """Return a JSON-serializable dict with this module's state(s).
 
         The counterpart to this method is the `set_state` one.
 
         Returns
         -------
-        state: dict[str, any]
+        state: Dict[str, Any]
             JSON-serializable dict storing this module's inner state
             variables.
         """
         return {}
 
     def set_state(
         self,
@@ -291,11 +304,11 @@
         ----------
         state: dict[str, any]
             Dict storing values to assign to this module's inner
             state variables.
 
         Raises
         ------
-        KeyError:
+        KeyError
             If an expected state variable is missing from `state`.
         """
         # API-defining method; pylint: disable=unused-argument
```

### Comparing `declearn-2.1.0/declearn/optimizer/modules/_clipping.py` & `declearn-2.2.0/declearn/optimizer/modules/_clipping.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 __all__ = ["L2Clipping"]
 
 
 class L2Clipping(OptiModule):
     """Fixed-threshold L2-norm gradient clipping module.
 
     This module implements the following algorithm:
+
         Init(max_norm):
         Step(max_norm):
             norm = euclidean_norm(grads)
             clip = min(norm, max_norm)
             grads *= clip / max_norm
 
     In other words, (batch-averaged) gradients are clipped
```

### Comparing `declearn-2.1.0/declearn/optimizer/modules/_momentum.py` & `declearn-2.2.0/declearn/optimizer/modules/_momentum.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,36 +29,39 @@
 ]
 
 
 class MomentumModule(OptiModule):
     """Momentum gradient-acceleration module.
 
     This module impements the following algorithm:
+
         Init(beta):
             velocity = 0
         Step(grads):
             velocity = beta * velocity + grads
             if nesterov:
                 grads = beta * velocity + grads
             else:
                 grads = velocity
 
     Note that this contrasts with the canonical implementation of momentum
     by Sutskever et. al. [1]. The learning rate is applied to the whole output
     of the algorithm above, in the Optmizer class, rather than only to the
-    gradient part of it, following the [pytorch implementation]\
-    (https://pytorch.org/docs/stable/generated/torch.optim.SGD.html).
+    gradient part of it, following the [pytorch implementation](\
+    https://pytorch.org/docs/stable/generated/torch.optim.SGD.html).
     The nesterov variant's implementation is equivalently adapted.
 
-    This formaluation is equivalent to the canonical one for constant learning
+    This formulation is equivalent to the canonical one for constant learning
     rare (eta), with both approaches outputting:
-    $$ w_{t+1} = w_t - \\eta \\sum_{k=1}^t \\beta^{t-k} \nabla_k $$
+        $$ w_{t+1} = w_t - \\eta \\sum_{k=1}^t \\beta^{t-k} \\nabla_k $$
+
     It may however yield differences when $\\eta$ changes through training:
-    (can.) $$ w_{t+1} = w_t - \\sum_{k=1}^t \\eta_k \\beta^{t-k} \\nabla_k $$
-    (ours) $$ w_{t+1} = w_t - \\eta_t \\sum_{k=1}^t \\beta^{t-k} \\nabla_k $$
+
+    - (can.) $$ w_{t+1} = w_t - \\sum_{k=1}^t \\eta_k \\beta^{t-k} \\nabla_k $$
+    - (ours) $$ w_{t+1} = w_t - \\eta_t \\sum_{k=1}^t \\beta^{t-k} \\nabla_k $$
 
     References
     ----------
     [1] Sutskever et. al., 2013.
         On the importance of initialization and momentum in deep learning
         https://proceedings.mlr.press/v28/sutskever13.pdf
     """
@@ -115,14 +118,15 @@
         self.velocity = state["velocity"]
 
 
 class EWMAModule(OptiModule):
     """Exponentially Weighted Moving Average module.
 
     This module impements the following algorithm:
+
         Init(beta):
             state = 0
         Step(grads):
             state = beta*state + (1-beta)*grads
             grads = state
 
     In other words, gradients are corrected by an exponentially-
@@ -176,29 +180,31 @@
         self.state = state["state"]
 
 
 class YogiMomentumModule(EWMAModule):
     """Yogi-specific momentum gradient-acceleration module.
 
     This module impements the following algorithm:
+
         Init(beta):
             state = 0
         Step(grads):
             state = state + sign(state-grads)*(1-beta)*grads
             grads = state
 
     In other words, gradients are corrected in a somewhat-simlar
     fashion as in the base momentum formula, but so that the
     magnitude of the state update is merely a function of inputs
     rather than of both the inputs and the previous state [1].
 
     Note that this module is actually meant to be used to compute
     a learning-rate adaptation term based on squared gradients.
 
-    References:
+    References
+    ----------
     [1] Zaheer and Reddi et al., 2018.
         Adaptive Methods for Nonconvex Optimization.
     """
 
     name: ClassVar[str] = "yogi-momentum"
 
     def run(
```

### Comparing `declearn-2.1.0/declearn/optimizer/modules/_noise.py` & `declearn-2.2.0/declearn/optimizer/modules/_noise.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,29 @@
         return {"safe_mode": self.safe_mode, "seed": self.seed}
 
     def run(
         self,
         gradients: Vector,
     ) -> Vector:
         if not NumpyVector in gradients.compatible_vector_types:
-            raise TypeError(
+            raise TypeError(  # pragma: no cover
                 f"{self.__class__.__name__} requires input gradients to "
                 "be compatible with NumpyVector, which is not the case "
                 f"of {type(gradients).__name__}."
             )
         # Gather gradients' specs.
         shapes = gradients.shapes()
         dtypes = gradients.dtypes()
         # Conduct noise sampling for each and every gradient coordinate.
         noise = {
             key: self._sample_noise(shapes[key], dtypes[key])
             for key in gradients.coefs
         }
         # Add the sampled noise to the gradients and return them.
-        # Silence warnings about sparse gradients getting sparsified.
+        # Silence warnings about sparse gradients getting densified.
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", ".*densifying.*", RuntimeWarning)
             return gradients + NumpyVector(noise)
 
     @abstractmethod
     def _sample_noise(
         self,
@@ -162,8 +162,10 @@
             array = np.array(value).reshape(shape).astype(dtype)
             return scipy.stats.norm.ppf(array, scale=self.std)
         # Case when using numpy RNG, that provides with gaussian sampling.
         if isinstance(self._rng, np.random.Generator):
             # false-positive; pylint: disable=no-member
             return self._rng.normal(scale=self.std, size=shape).astype(dtype)
         # Theoretically-unreachable case.
-        raise RuntimeError("Unexpected `GaussianeNoiseModule._rng` type.")
+        raise RuntimeError(  # pragma: no cover
+            "Unexpected `GaussianeNoiseModule._rng` type."
+        )
```

### Comparing `declearn-2.1.0/declearn/optimizer/modules/_scaffold.py` & `declearn-2.2.0/declearn/optimizer/modules/_scaffold.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 the SCAFFOLD (Stochastic Averaging for Federated Learning) algorithm
 as a plug-in option to optimizer processes.
 
 They only implement Option-II of the paper regarding client-specific
 state variables' update, and implementing Option-I would require the
 use of a specific Optimizer sub-class.
 
-References:
+References
+----------
 [1] Karimireddy et al., 2019.
     SCAFFOLD: Stochastic Controlled Averaging for Federated Learning.
     https://arxiv.org/abs/1910.06378
 """
 
 import warnings
 from typing import Any, ClassVar, Dict, List, Optional, Union
@@ -44,17 +45,19 @@
 
 
 class ScaffoldClientModule(OptiModule):
     """Client-side Stochastic Controlled Averaging (SCAFFOLD) module.
 
     This module is to be added to the optimizer used by a federated-
     learning client, and expects that the server's optimizer use its
-    counterpart module: `ScaffoldServerModule`.
+    counterpart module:
+    [`ScaffoldServerModule`][declearn.optimizer.modules.ScaffoldServerModule].
 
     This module implements the following algorithm:
+
         Init:
             delta = 0
             _past = 0
             _step = 0
         Step(grads):
             _past += grads
             _step += 1
@@ -84,15 +87,16 @@
     corresponds to the "Option-II" in the paper.
     Implementing Option-I would require holding a copy of the shared
     model and computing its gradients in addition to those of the
     local model, effectively doubling computations. This can be done
     in `declearn`, but requires implementing an alternative training
     procedure rather than an optimizer plug-in.
 
-    References:
+    References
+    ----------
     [1] Karimireddy et al., 2019.
         SCAFFOLD: Stochastic Controlled Averaging for Federated Learning.
         https://arxiv.org/abs/1910.06378
     """
 
     name: ClassVar[str] = "scaffold-client"
     aux_name: ClassVar[str] = "scaffold"
@@ -113,20 +117,34 @@
         self._grads = self._grads + gradients
         self._steps += 1
         # Apply state-based correction to outputs.
         return gradients - self.delta
 
     def collect_aux_var(
         self,
-    ) -> Optional[Dict[str, Any]]:
+    ) -> Dict[str, Any]:
         """Return auxiliary variables that need to be shared between nodes.
 
         Compute and package (without applying it) the updated value
         of the local state variable, so that the server may compute
         the updated shared state variable.
+
+        Returns
+        -------
+        aux_var: dict[str, any]
+            JSON-serializable dict of auxiliary variables that
+            are to be shared with a ScaffoldServerModule held
+            by the orchestrating server.
+
+        Warns
+        -----
+        RuntimeWarning
+            If called on an instance that has not processed any gradients
+            (via a call to `run`) since the last call to `process_aux_var`
+            (or its instantiation).
         """
         state = self._compute_updated_state()
         return {"state": state}
 
     def _compute_updated_state(
         self,
     ) -> Union[Vector, float]:
@@ -166,14 +184,30 @@
         self,
         aux_var: Dict[str, Any],
     ) -> None:
         """Update this module based on received shared auxiliary variables.
 
         Collect the (local_state - shared_state) variable sent by server.
         Reset hidden variables used to compute the local state's updates.
+
+        Parameters
+        ----------
+        aux_var: dict[str, any]
+            JSON-serializable dict of auxiliary variables that are to be
+            processed by this module at the start of a training round (on
+            the client side).
+            Expected keys for this class: {"delta"}.
+
+        Raises
+        ------
+        KeyError
+            If an expected auxiliary variable is missing.
+        TypeError
+            If a variable is of unproper type, or if aux_var
+            is not formatted as it should be.
         """
         # Expect a state variable and apply it.
         delta = aux_var.get("delta", None)
         if delta is None:
             raise KeyError(
                 "Missing 'delta' key in ScaffoldClientModule's "
                 "received auxiliary variables."
@@ -191,17 +225,19 @@
 
 
 class ScaffoldServerModule(OptiModule):
     """Server-side Stochastic Controlled Averaging (SCAFFOLD) module.
 
     This module is to be added to the optimizer used by a federated-
     learning server, and expects that the clients' optimizer use its
-    counterpart module: `ScaffoldClientModule`.
+    counterpart module:
+    [`ScaffoldClientModule`][declearn.optimizer.modules.ScaffoldClientModule].
 
     This module implements the following algorithm:
+
         Init(clients):
             state = 0
             s_loc = {client: 0 for client in clients}
         Step(grads):
             grads
         Send:
             delta = {client: (s_loc[client] - state); client in s_loc}
@@ -222,15 +258,16 @@
     that new delta values can be sent to clients as the next round
     of training starts.
 
     The SCAFFOLD algorithm is described in reference [1].
     The client-side correction of gradients and the computation of
     updated local states are deferred to `ScaffoldClientModule`.
 
-    References:
+    References
+    ----------
     [1] Karimireddy et al., 2019.
         SCAFFOLD: Stochastic Controlled Averaging for Federated Learning.
         https://arxiv.org/abs/1910.06378
     """
 
     name: ClassVar[str] = "scaffold-server"
     aux_name: ClassVar[str] = "scaffold"
@@ -242,22 +279,24 @@
         """Instantiate the server-side SCAFFOLD gradients-correction module.
 
         Parameters
         ----------
         clients: list[str] or None, default=None
             Optional list of known clients' id strings.
 
-        If this module is used under a training strategy that has
-        participating clients vary across epochs, leaving `clients`
-        to None will affect the update rule for the shared state,
-        as it uses a (n_participating / n_total_clients) term, the
-        divisor of which will be incorrect (at least on the first
-        step, potentially on following ones as well).
-        Similarly, listing clients that in fact do not participate
-        in training will have side effects on computations.
+        Notes
+        -----
+        - If this module is used under a training strategy that has
+          participating clients vary across epochs, leaving `clients`
+          to None will affect the update rule for the shared state,
+          as it uses a (n_participating / n_total_clients) term, the
+          divisor of which will be incorrect (at least on the first
+          step, potentially on following ones as well).
+        - Similarly, listing clients that in fact do not participate
+          in training will have side effects on computations.
         """
         self.state = 0.0  # type: Union[Vector, float]
         self.s_loc = {}  # type: Dict[str, Union[Vector, float]]
         if clients:
             self.s_loc = {client: 0.0 for client in clients}
 
     def get_config(
@@ -270,34 +309,57 @@
         gradients: Vector,
     ) -> Vector:
         # Note: ScaffoldServer only manages auxiliary variables.
         return gradients
 
     def collect_aux_var(
         self,
-    ) -> Optional[Dict[str, Any]]:
+    ) -> Dict[str, Dict[str, Any]]:
         """Return auxiliary variables that need to be shared between nodes.
 
-        Package client-wise (local_state - shared_state) variables.
+        Package client-wise `delta = (local_state - shared_state)` variables.
+
+        Returns
+        -------
+        aux_var:
+            JSON-serializable dict of auxiliary variables that are to
+            be shared with the client-wise ScaffoldClientModule. This
+            dict has a `{client-name: {"delta": value}}` structure.
         """
         # Compute clients' delta variable, package them and return.
         aux_var = {}  # type: Dict[str, Dict[str, Any]]
         for client, state in self.s_loc.items():
             delta = state - self.state
             aux_var[client] = {"delta": delta}
         return aux_var
 
     def process_aux_var(
         self,
-        aux_var: Dict[str, Any],
+        aux_var: Dict[str, Dict[str, Any]],
     ) -> None:
         """Update this module based on received shared auxiliary variables.
 
         Collect updated local state variables sent by clients.
         Update the global state variable based on the latter.
+
+        Parameters
+        ----------
+        aux_var: dict[str, dict[str, any]]
+            JSON-serializable dict of auxiliary variables that are to be
+            processed by this module before processing global updates.
+            This dict should have a `{client-name: {"state": value}}`
+            structure.
+
+        Raises
+        ------
+        KeyError:
+            If an expected auxiliary variable is missing.
+        TypeError:
+            If a variable is of unproper type, or if aux_var
+            is not formatted as it should be.
         """
         # Collect updated local states received from Scaffold client modules.
         s_new = {}  # type: Dict[str, Union[Vector, float]]
         for client, c_dict in aux_var.items():
             if not isinstance(c_dict, dict):
                 raise TypeError(
                     "ScaffoldServerModule requires auxiliary variables "
```

### Comparing `declearn-2.1.0/declearn/optimizer/regularizers/__init__.py` & `declearn-2.2.0/declearn/optimizer/regularizers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,23 +13,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Optimizer loss-regularization algorithms, implemented as plug-in modules.
 
-Base class implemented here:
+API base class
+--------------
 * Regularizer: base API for loss-regularization plug-ins
 
-Common regularization terms:
-* LassoRegularizer : L1 regularization, aka Lasso penalization
-* RidgeRegularizer : L2 regularization, aka Ridge penalization
+Common regularization terms
+---------------------------
+* [LassoRegularizer][declearn.optimizer.regularizers.LassoRegularizer]:
+    L1 regularization, aka Lasso penalization.
+* [RidgeRegularizer][declearn.optimizer.regularizers.RidgeRegularizer]:
+    L2 regularization, aka Ridge penalization.
 
-Federated-Learning-specific regularizers:
-* FedProxRegularizer : FedProx algorithm, as a proximal term regularizer
+Federated-Learning-specific regularizers
+----------------------------------------
+* [FedProxRegularizer][declearn.optimizer.regularizers.FedProxRegularizer]:
+    FedProx algorithm, as a proximal term regularizer.
 """
 
 from ._api import Regularizer
 from ._base import (
     FedProxRegularizer,
     LassoRegularizer,
     RidgeRegularizer,
```

### Comparing `declearn-2.1.0/declearn/optimizer/regularizers/_api.py` & `declearn-2.2.0/declearn/optimizer/regularizers/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base API for loss regularization optimizer plug-ins."""
 
 from abc import ABCMeta, abstractmethod
-from typing import Any, ClassVar, Dict
+from typing import Any, ClassVar, Dict, TypeVar
 
 from typing_extensions import Self  # future: import from typing (py >=3.11)
 
 from declearn.model.api import Vector
 from declearn.utils import (
     access_registered,
     create_types_registry,
@@ -30,23 +30,27 @@
 )
 
 __all__ = [
     "Regularizer",
 ]
 
 
+T = TypeVar("T")
+
+
 @create_types_registry
 class Regularizer(metaclass=ABCMeta):
     """Abstract class defining an API to implement loss-regularizers.
 
     The `Regularizer` API is close to the `OptiModule` one, with the
     following differences:
-    * Regularizers are meant to be applied prior to Modules, as a way
+
+    - Regularizers are meant to be applied prior to Modules, as a way
       to complete the computation of "raw" gradients.
-    * Regularizers do not provide an API to share stateful variables
+    - Regularizers do not provide an API to share stateful variables
       between a server and its clients.
 
     The aim of this abstraction (which itself operates on the Vector
     abstraction, so as to provide framework-agnostic algorithms) is
     to enable implementing loss-regularization terms, rewritten as
     gradients-correction bricks, that can easily and modularly be
     plugged into optimization algorithms.
@@ -55,40 +59,41 @@
     and routines for computing and applying gradients-based updates.
     `Regularizer` instances are designed to be "plugged in" such an
     `Optimizer` instance, to be applied to the raw gradients prior
     to any further processing (e.g. adaptative scaling algorithms).
 
     Abstract
     --------
-    name: str class attribute
+    - name: str class attribute
         Name identifier of the class (should be unique across existing
         Regularizer classes). Also used for automatic types-registration
         of the class (see `Inheritance` section below).
-    run(gradients: Vector, weights: Vector) -> Vector:
+    - run(gradients: Vector, weights: Vector) -> Vector:
         Compute the regularization term's derivative from weights,
         and add it to the input gradients. This is the main method
         for any `Regularizer`.
 
     Overridable
     -----------
-    on_round_start() -> None:
+    - on_round_start() -> None:
         Perform any required operation (e.g. resetting a state variable)
         at the start of a training round. By default, this method has no
         effect and mey thus be safely ignored when no behavior is needed.
 
     Inheritance
     -----------
     When a subclass inheriting from `Regularizer` is declared, it is
     automatically registered under the "Regularizer" group using its
     class-attribute `name`. This can be prevented by adding `register=False`
     to the inheritance specs (e.g. `class MyCls(Regularizer, register=False)`).
     See `declearn.utils.register_type` for details on types registration.
     """
 
     name: ClassVar[str] = NotImplemented
+    """Name identifier of the class, unique across Regularizer classes."""
 
     def __init_subclass__(
         cls,
         register: bool = True,
         **kwargs: Any,
     ) -> None:
         """Automatically type-register Regularizer subclasses."""
@@ -109,17 +114,17 @@
             regularized loss function's formulation.
         """
         self.alpha = alpha
 
     @abstractmethod
     def run(
         self,
-        gradients: Vector,
-        weights: Vector,
-    ) -> Vector:
+        gradients: Vector[T],
+        weights: Vector[T],
+    ) -> Vector[T]:
         """Compute and add the regularization term's derivative to gradients.
 
         Parameters
         ----------
         gradients: Vector
             Input gradients to which the correction term is to be added.
         weights: Vector
```

### Comparing `declearn-2.1.0/declearn/optimizer/regularizers/_base.py` & `declearn-2.2.0/declearn/optimizer/regularizers/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,25 +34,28 @@
 
     The FedProx algorithm is implemented through this regularizer,
     that adds a proximal term to the loss function so as to handle
     heterogeneity across clients in a federated learning context.
     See paper [1].
 
     This regularizer implements the following term:
+
         loss += alpha / 2 * (weights - ref_wgt)^2
         w/ ref_wgt := weights at the 1st step of the round
 
     To do so, it applies the following correction to gradients:
+
         grads += alpha * (weights - ref_wgt)
 
     In other words, this regularizer penalizes weights' departure
     (as a result from local optimization steps) from their initial
     (shared) values.
 
-    References:
+    References
+    ----------
     [1] Li et al., 2020.
         Federated Optimization in Heterogeneous Networks.
         https://arxiv.org/abs/1812.06127
     """
 
     name: ClassVar[str] = "fedprox"
 
@@ -80,17 +83,19 @@
         return gradients + correct
 
 
 class LassoRegularizer(Regularizer):
     """L1 (Lasso) loss-regularization plug-in.
 
     This regularizer implements the following term:
+
         loss += alpha * l1_norm(weights)
 
     To do so, it applies the following correction to gradients:
+
         grads += alpha * sign(weights)
     """
 
     name: ClassVar[str] = "lasso"
 
     def run(
         self,
@@ -101,17 +106,19 @@
         return gradients + correct
 
 
 class RidgeRegularizer(Regularizer):
     """L2 (Ridge) loss-regularization plug-in.
 
     This regularizer implements the following term:
+
         loss += alpha * l2_norm(weights)
 
     To do so, it applies the following correction to gradients:
+
         grads += alpha * 2 * weights
     """
 
     name: ClassVar[str] = "ridge"
 
     def run(
         self,
```

### Comparing `declearn-2.1.0/declearn/test_utils/__init__.py` & `declearn-2.2.0/declearn/model/api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Collection of utils for running tests and examples around declearn."""
+"""Model and Vector abstractions submodule.
 
-from ._assertions import (
-    assert_dict_equal,
-    assert_list_equal,
-    assert_json_serializable_dict,
-)
-from ._gen_ssl import generate_ssl_certificates
-from ._multiprocess import run_as_processes
-from ._vectors import (
-    FrameworkType,
-    GradientsTestCase,
-    list_available_frameworks,
-)
+This submodules exports the building blocks of the Model and Vector APIs:
+
+* [Model][declearn.model.api.Model]:
+    Abstract class defining an API to interface a ML model.
+* [Vector][declearn.model.api.Vector]:
+    Abstract class defining an API to manipulate (sets of) data arrays.
+* [register_vector_type][declearn.model.api.register_vector_type]:
+    Decorate a Vector subclass to make it buildable with `Vector.build`.
+"""
+
+from ._vector import Vector, register_vector_type
+from ._model import Model
```

### Comparing `declearn-2.1.0/declearn/test_utils/_assertions.py` & `declearn-2.2.0/declearn/test_utils/_assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     Parameters
     ----------
     sdict: Dict[str, Any]
         Dictionary, the JSON-serializability of which to assert.
 
     Raises
     ------
-    AssertionError:
+    AssertionError
         If `sdict` or the JSON-reloaded object is not a dict, or
         if the latter has different keys and/or values compared
         to the former.
-    Exception:
+    Exception
         Other exceptions may be raised if the JSON encoding (or
         decoding) operation goes wrong.
     """
     assert isinstance(sdict, dict)
     dump = json.dumps(sdict, default=json_pack)
     load = json.loads(dump, object_hook=json_unpack)
     assert isinstance(load, dict)
@@ -89,15 +89,15 @@
         two compared dicts).
     np_tolerance: float or none, default=None
         Optional absolute tolerance to numpy arrays or float values'
         differences (use `np.allclose(a, b, rtol=0, atol=np_tolerance)`).
 
     Raises
     ------
-    AssertionError:
+    AssertionError
         If the two dicts are not equal.
     """
     assert dict_a.keys() == dict_b.keys()
     for key, val_a in dict_a.items():
         val_b = dict_b[key]
         assert_values_equal(val_a, val_b, strict_tuple, np_tolerance)
 
@@ -113,29 +113,29 @@
     This function is a more complex equivalent of `assert list_a == list_b`
     that enables comparing numpy array values, and optionally accepting to
     cast tuples as lists rather than assert that a tuple and a list are not
     equal in any case (even when their contents are the same).
 
     Parameters
     ----------
-    dict_a: list
+    list_a: list
         First list to compare.
-    dict_b: list
+    list_b: list
         Second list to compare.
     strict_tuple: bool, default=False
         Whether to cast tuples to list prior to comparing them
         (enabling some tuple-list type differences between the
         two compared lists).
     np_tolerance: float or none, default=None
         Optional absolute tolerance to numpy arrays or float values'
         differences (use `np.allclose(a, b, rtol=0, atol=np_tolerance)`).
 
     Raises
     ------
-    AssertionError:
+    AssertionError
         If the two lists are not equal.
     """
     assert len(list_a) == len(list_b)
     for val_a, val_b in zip(list_a, list_b):
         assert_values_equal(val_a, val_b, strict_tuple, np_tolerance)
 
 
@@ -165,15 +165,15 @@
         two compared values).
     np_tolerance: float or none, default=None
         Optional absolute tolerance to numpy arrays or float values'
         differences (use `np.allclose(a, b, rtol=0, atol=np_tolerance)`).
 
     Raises
     ------
-    AssertionError:
+    AssertionError
         If the two lists are not equal.
     """
     if isinstance(val_a, dict):
         assert isinstance(val_b, dict)
         assert_dict_equal(val_a, val_b, strict_tuple)
     elif isinstance(val_a, np.ndarray):
         assert isinstance(val_b, np.ndarray)
```

### Comparing `declearn-2.1.0/declearn/test_utils/_gen_ssl.py` & `declearn-2.2.0/declearn/test_utils/_gen_ssl.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/test_utils/_multiprocess.py` & `declearn-2.2.0/declearn/model/haiku/utils/_gpu.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,53 +11,72 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utils to run concurrent routines parallelly using multiprocessing."""
+"""Utils for GPU support and device management in jax."""
 
-import multiprocessing as mp
-from typing import Any, Callable, List, Optional, Tuple
+import warnings
+from typing import Optional
 
+import jax
 
-__all__ = [
-    "run_as_processes",
-]
+__all__ = ["select_device"]
 
 
-def run_as_processes(
-    *routines: Tuple[Callable[..., Any], Tuple[Any, ...]]
-) -> List[Optional[int]]:
-    """Run coroutines concurrently within individual processes.
+def select_device(
+    gpu: bool,
+    idx: Optional[int] = None,
+) -> jax.Device:
+    """Select a backing device to use based on inputs and availability.
 
     Parameters
     ----------
-    *routines: tuple(function, tuple(any, ...))
-        Sequence of routines that need running concurrently,
-        each formatted as a 2-elements tuple containing the
-        function to run, and a tuple storing its arguments.
+    gpu: bool
+        Whether to select a GPU device rather than the CPU one.
+    idx: int or None, default=None
+        Optional pre-selected device index. Only used when `gpu=True`.
+        If `idx is None` or exceeds the number of available GPU devices,
+        use the first available one.
+
+    Warns
+    -----
+    RuntimeWarning:
+        If `gpu=True` but no GPU is available.
+        If `idx` exceeds the number of available GPU devices.
 
     Returns
     -------
-    exitcodes: list[int]
-        List of exitcodes of the processes wrapping the routines.
-        If all codes are zero, then all functions ran properly.
+    device: jaxlib.xla_extension.Device
+        Selected device.
     """
-    # Wrap routines as individual processes and run them concurrently.
-    processes = [mp.Process(target=func, args=args) for func, args in routines]
+    idx = 0 if idx is None else idx
+    device_type = "gpu" if gpu else "cpu"
+    # List devices, handling errors related to the lack of GPU (or CPU error).
     try:
-        # Start all processes.
-        for process in processes:
-            process.start()
-        # Regularly check for any failed process and exit if so.
-        while any(process.is_alive() for process in processes):
-            if any(process.exitcode for process in processes):
-                break
-            processes[0].join(timeout=1)
-    # Ensure not to leave processes running in the background.
-    finally:
-        for process in processes:
-            process.terminate()
-    # Return processes' exitcodes.
-    return [process.exitcode for process in processes]
+        devices = jax.devices(device_type)
+    except RuntimeError as exc:
+        # Warn about the lack of GPU (support?), and fall back to CPU.
+        if gpu:
+            warnings.warn(
+                "Cannot use a GPU device: either CUDA is unavailable "
+                f"or no GPU is visible to jax: raised {repr(exc)}.",
+                RuntimeWarning,
+            )
+            return select_device(gpu=False, idx=0)
+        # Case when no CPU is found: this should never be reached.
+        raise RuntimeError(  # pragma: no cover
+            "Failed to have jax select a CPU device."
+        ) from exc
+    # similar code to tensorflow util; pylint: disable=duplicate-code
+    # Case when the desired device index is invalid: select another one.
+    if idx >= len(devices):
+        warnings.warn(
+            f"Cannot use {device_type} device n°{idx}: index is out-of-range."
+            f"\nUsing {device_type} device n°0 instead.",
+            RuntimeWarning,
+        )
+        idx = 0
+    # Return the selected device.
+    return devices[idx]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `declearn-2.1.0/declearn/test_utils/_vectors.py` & `declearn-2.2.0/declearn/test_utils/_vectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 """Shared objects for testing purposes."""
 
 import importlib
 import typing
 from typing import List, Literal, Optional, Type
 
 import numpy as np
-import pkg_resources
+import pkg_resources  # type: ignore
 from numpy.typing import ArrayLike
 
 from declearn.model.api import Vector
 from declearn.model.sklearn import NumpyVector
 
 __all__ = [
     "FrameworkType",
     "GradientsTestCase",
     "list_available_frameworks",
 ]
 
 
-FrameworkType = Literal["numpy", "tensorflow", "torch"]
+FrameworkType = Literal["numpy", "tensorflow", "torch", "jax"]
 
 
 def list_available_frameworks() -> List[FrameworkType]:
     """List available Vector backend frameworks."""
     available = []
     for framework in typing.get_args(FrameworkType):
         try:
@@ -56,15 +56,17 @@
 
     This class aims at providing with seeded random or zero-valued Vector
     instances (with deterministic specifications) that may be used in the
     context of unit tests.
     """
 
     def __init__(
-        self, framework: FrameworkType, seed: Optional[int] = 0
+        self,
+        framework: FrameworkType,
+        seed: Optional[int] = 0,
     ) -> None:
         """Instantiate the parametrized test-case."""
         if framework not in list_available_frameworks():
             raise RuntimeError(f"Framework '{framework}' is unavailable.")
         self.framework = framework
         self.seed = seed
 
@@ -75,33 +77,41 @@
             return NumpyVector
         if self.framework == "tensorflow":
             module = importlib.import_module("declearn.model.tensorflow")
             return module.TensorflowVector
         if self.framework == "torch":
             module = importlib.import_module("declearn.model.torch")
             return module.TorchVector
+        if self.framework == "jax":
+            module = importlib.import_module("declearn.model.haiku")
+            return module.JaxNumpyVector
         raise ValueError(f"Invalid framework '{self.framework}'")
 
     def convert(self, array: np.ndarray) -> ArrayLike:
         """Convert an input numpy array to a framework-based structure."""
         if self.framework == "numpy":
             return array
         if self.framework == "tensorflow":
             tensorflow = importlib.import_module("tensorflow")
             with tensorflow.device("CPU"):
                 return tensorflow.convert_to_tensor(array)
         if self.framework == "torch":
             torch = importlib.import_module("torch")
             return torch.from_numpy(array)
+        if self.framework == "jax":
+            jnp = importlib.import_module("jax.numpy")
+            return jnp.asarray(array)
         raise ValueError(f"Invalid framework '{self.framework}'")
 
     def to_numpy(self, array: ArrayLike) -> np.ndarray:
         """Convert an input framework-based structure to a numpy array."""
         if isinstance(array, np.ndarray):
             return array
+        if self.framework == "jax":
+            return np.asarray(array)
         if self.framework == "tensorflow":  # add support for IndexedSlices
             tensorflow = importlib.import_module("tensorflow")
             if isinstance(array, tensorflow.IndexedSlices):
                 with tensorflow.device(array.device):
                     return tensorflow.convert_to_tensor(array).numpy()
         return array.numpy()  # type: ignore
```

### Comparing `declearn-2.1.0/declearn/typing.py` & `declearn-2.2.0/declearn/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,22 +25,27 @@
 
 
 __all__ = [
     "Batch",
     "SupportsConfig",
 ]
 
-# Data batches specification: (inputs, labels, weights), where:
-# - inputs and labels may be an array or a list of arrays:
-# - labels and/or weights may ne None
+
 Batch = Tuple[
     Union[ArrayLike, List[ArrayLike]],
     Optional[Union[ArrayLike, List[ArrayLike]]],
     Optional[ArrayLike],
 ]
+"""Data batches specification type-annotation.
+
+This type-hint designates (inputs, labels, weights) inputs, where:
+
+- inputs and labels may be an array or a list of arrays;
+- labels and/or weights may be None;
+"""  # this is rendered as a docstring for `Batch` in the docs
 
 
 class SupportsConfig(Protocol, metaclass=ABCMeta):
     """Protocol for type annotation of objects with get/from_config methods.
 
     This class is primarily designed to be used for type annotation,
     but may also be used to implement `get_config` and `from_config`
```

### Comparing `declearn-2.1.0/declearn/utils/_dataclass.py` & `declearn-2.2.0/declearn/utils/_dataclass.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/utils/_device_policy.py` & `declearn-2.2.0/declearn/utils/_device_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utils to define a computation device policy.
 
 This private submodule defines:
-* A dataclass defining a standard to hold a device-selection policy.
-* A private global variable holding the current package-wise device policy.
-* A public pair of functions acting as a getter and a setter for that variable.
+
+- A dataclass defining a standard to hold a device-selection policy.
+- A private global variable holding the current package-wise device policy.
+- A public pair of functions acting as a getter and a setter for that variable.
 """
 
 import dataclasses
 from typing import Optional
 
 
 __all__ = [
@@ -79,14 +80,15 @@
 DEVICE_POLICY = DevicePolicy(gpu=True, idx=None)
 
 
 def get_device_policy() -> DevicePolicy:
     """Return a copy of the current global device policy.
 
     This method is meant to be used:
+
     - By end-users that wish to check the current device policy.
     - By the backend code of framework-specific objects so as to
       take the required steps towards implementing that policy.
 
     To update the current policy, use `declearn.utils.set_device_policy`.
 
     Returns
```

### Comparing `declearn-2.1.0/declearn/utils/_json.py` & `declearn-2.2.0/declearn/utils/_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,16 +154,18 @@
     path: str,
     encoding: str = "utf-8",
     indent: Optional[int] = None,
 ) -> None:
     """Dump a given object to a JSON file, using extended types support.
 
     This function is merely a shortcut to run the following code:
+    ```
     >>> with open(path, "w", encoding=encoding) as file:
     >>>     json.dump(obj, file, default=declearn.utils.json_pack)
+    ```
 
     See `declearn.utils.add_json_support` to extend the behaviour
     of JSON (de)serialization to non-standard types, that will be
     used as part of this function.
 
     See `declearn.utils.json_load` for the counterpart method.
     """
@@ -174,16 +176,18 @@
 def json_load(
     path: str,
     encoding: str = "utf-8",
 ) -> Any:
     """Load data from a JSON file, using extended types support.
 
     This function is merely a shortcut to run the following code:
+    ```
     >>> with open(path, "r", encoding=encoding) as file:
     >>>     return json.load(file, object_hook=declearn.utils.json_unpack)
+    ```
 
     See `declearn.utils.add_json_support` to extend the behaviour
     of JSON (de)serialization to non-standard types, that will be
     used as part of this function.
 
     See `declearn.utils.json_dump` for the counterpart method.
     """
```

### Comparing `declearn-2.1.0/declearn/utils/_numpy.py` & `declearn-2.2.0/declearn/utils/_numpy.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/declearn/utils/_register.py` & `declearn-2.2.0/declearn/utils/_register.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     Returns
     -------
     cls: type
         Type retrieved from a types registry.
 
     Raises
     ------
-    KeyError:
+    KeyError
         If no registered type matching the input parameters is found.
     """
     # If group is unspecified, look the name up in each and every registry.
     if group is None:
         for reg in REGISTRIES.values():
             try:
                 return reg.access(name)
@@ -285,15 +285,15 @@
     name: str
         Name under which the type is registered.
     group: str
         Name of the TypesRegistry in which the type is registered.
 
     Raises
     ------
-    KeyError:
+    KeyError
         If the provided information does not match a registered type.
     """
     # If group is unspecified, look the type up in each and every registry.
     if group is None:
         for grp, reg in REGISTRIES.items():
             try:
                 return reg.get_name(cls), grp
@@ -322,13 +322,13 @@
     -------
     mapping: Dict[str, type]
         `{name: type}` dict mapping of registered types.
         Note that this is a copy of the actual registry.
 
     Raises
     ------
-    KeyError:
+    KeyError
         If the `group` types registry does not exist.
     """
     if group not in REGISTRIES:
         raise KeyError(f"Type registry '{group}' does not exist.")
     return REGISTRIES[group].get_mapping()
```

### Comparing `declearn-2.1.0/declearn/utils/_serialize.py` & `declearn-2.2.0/declearn/utils/_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
 
     This function is the counterpart to `declearn.utils.deserialize_object`.
 
     Parameters
     ----------
     obj: object
         Object that needs serialization. To be valid, the object must:
-        * implement the `get_config` and `from_config` (class)methods
-        * belong to a registered type, unless `allow_unregistered=True`
+        - implement the `get_config` and `from_config` (class)methods
+        - belong to a registered type, unless `allow_unregistered=True`
           (i.e. a type that has been passed to or decorated with the
           `declearn.utils.register_type` function)
     group: str or None, default=None
         Optional name of the group under which the object's type was
         registered. If None, the type will be looked for in each and
         every exiting group, and the first match will be used.
     allow_unregistered: bool, default=False
```

### Comparing `declearn-2.1.0/declearn/utils/_toml_config.py` & `declearn-2.2.0/declearn/utils/_toml_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Base class to define TOML-parsable configuration containers."""
 
 import dataclasses
+import os
 import typing
 import warnings
 
 try:
     import tomllib  # type: ignore
 except ModuleNotFoundError:
     import tomli as tomllib
@@ -63,15 +64,15 @@
     is_instance: bool
         Whether `inputs` abides by the type specified by `typevar`.
         For composed type generics, recursive type-checks may be
         conducted (e.g. to type-check elements of an iterable).
 
     Raises
     ------
-    TypeError:
+    TypeError
         If an unsupported `typevar` is provided.
     """
     origin = typing.get_origin(typevar)
     # Case of a raw, unit type.
     if origin is None:
         return (typevar is Any) or isinstance(inputs, typevar)
     # Case of a typing generic.
@@ -95,47 +96,59 @@
     if origin is tuple:
         return (
             isinstance(inputs, tuple)
             and len(inputs) == len(args)
             and all(_isinstance_generic(e, t) for e, t in zip(inputs, args))
         )
     # Unsupported cases.
-    raise TypeError(
+    raise TypeError(  # pragma: no cover
         "Unsupported subscripted generic for instance check: "
         f"'{typevar}' with origin '{origin}'."
     )
 
 
 def _parse_float(src: str) -> Optional[float]:
     """Custom float parser that replaces nan values with None."""
     return None if src == "nan" else float(src)
 
 
 def _instantiate_field(
     field: dataclasses.Field,  # future: dataclasses.Field[T] (Py >=3.9)
-    *args: Any,
     **kwargs: Any,
 ) -> Any:  # future: T
     """Instantiate a dataclass field from input args and kwargs.
 
-    This functions is meant to enable automatically building dataclass
-    fields that are annotated to be a union of types, notably optional
-    fields (i.e. Union[T, None]).
+    This function is meant to enable building dataclass object fields,
+    that requring instantiating from a received value or dict of kwargs.
+
+    It supports doing so even when for fields that are annotated to be a
+    union of types (notably optional ones: Union[T, None]), and/or are a
+    `TomlConfig` subclass that should be instantiated via `from_params`
+    rather than `cls(*args, **kwargs)`.
 
     It will raise a TypeError if instantiation fails or if `field.type`
     has and unsupported typing origin. It may also raise any exception
     coming from the target type's `__init__` method.
     """
+
+    def _instantiate(cls: Type[Any]) -> Any:
+        """Try instantiating a given class from the kwargs."""
+        if issubclass(cls, TomlConfig):
+            return cls.from_params(**kwargs)
+        return cls(**kwargs)
+
     origin = typing.get_origin(field.type)
-    if origin is None:  # raw type
-        return field.type(*args, **kwargs)
-    if origin is Union:  # union of types, including optional
+    # Case of a raw type.
+    if origin is None:
+        return _instantiate(field.type)
+    # Case of a union of types (including optional).
+    if origin is Union:
         for cls in typing.get_args(field.type):
             try:
-                return cls(*args, **kwargs)
+                return _instantiate(cls)
             except TypeError:
                 pass
         raise TypeError(
             f"Failed to instantiate {field.name} using type constructors "
             f"{typing.get_args(field.type)}."
         )
     raise TypeError(
@@ -170,17 +183,18 @@
         cls,
         **kwargs: Any,
     ) -> Self:
         """Instantiate a structured configuration from input keyword arguments.
 
         The input keyword arguments should match this class's fields' names.
         For each and every dataclass field of this class:
-            - If unprovided, set the argument to None.
-            - If a `parse_{field.name}` method exists, use that method.
-            - Else, use the `default_parser` method.
+
+        - If unprovided, set the argument to None.
+        - If a `parse_{field.name}` method exists, use that method.
+        - Else, use the `default_parser` method.
 
         Notes
         -----
         - If a field supports being None, not passing a kwarg for it will
           by default result in setting it to None.
         - If a field has a default value and does not support being None,
           not passing a kwarg for it will by default result in using its
@@ -189,21 +203,21 @@
           may be preferrable to pass an empty dict kwarg so as to use the
           field's default value rather than a non-default None value.
         - The former remarks hold up when the field does not benefit from
           a specific parser (that may implement arbitrary processing).
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             In case a field failed to be instantiated using the input key-
             word argument (or None value resulting from the lack thereof).
 
         Warns
         -----
-        UserWarning:
+        UserWarning
             In case some keyword arguments are unused due to the lack of a
             corresponding dataclass field.
         """
         fields = {}  # type: Dict[str, Any]
         # Look up expected kwargs and parse them.
         for field in dataclasses.fields(cls):
             parser = getattr(cls, f"parse_{field.name}", cls.default_parser)
@@ -214,20 +228,22 @@
                 raise RuntimeError(
                     f"Failed to parse '{field.name}' field: {exc}"
                 ) from exc
         # Warn about unused keyword arguments.
         for key in kwargs:
             warnings.warn(
                 f"Unsupported keyword argument in {cls.__name__}.from_params: "
-                f"'{key}'. This argument was ignored."
+                f"'{key}'. This argument was ignored.",
+                category=RuntimeWarning,
             )
         return cls(**fields)
 
-    @staticmethod
+    @classmethod
     def default_parser(
+        cls,
         field: dataclasses.Field,  # future: dataclasses.Field[T] (Py >=3.9)
         inputs: Union[str, Dict[str, Any], T, None],
     ) -> Any:
         """Default method to instantiate a field from python inputs.
 
         Parameters
         ----------
@@ -240,21 +256,22 @@
             - If dict, treat them as kwargs to the field's type constructor.
             - If str, treat as the path to a TOML file specifying the object.
 
         Notes
         -----
         If `inputs` is str and treated as the path to a TOML file,
         it will be parsed in one of the following ways:
+
         - Call `field.type.from_toml` if `field.type` is a TomlConfig.
         - Use the file's `field.name` section as kwargs, if it exists.
         - Use the entire file's contents as kwargs otherwise.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If instantiation failed, for any reason.
 
         Returns
         -------
         object: <T>
             Instantiated object that matches the field's specifications.
         """
@@ -266,38 +283,40 @@
             if field.default is not dataclasses.MISSING:
                 return field.default
             if field.default_factory is not dataclasses.MISSING:
                 return field.default_factory()
             raise TypeError(
                 f"Field '{field.name}' does not provide a default value."
             )
-        # Case of str inputs: treat as the path to a TOML file to parse.
-        if isinstance(inputs, str):
-            # If the field implements TOML parsing, call it.
-            if issubclass(field.type, TomlConfig):
-                return field.type.from_toml(inputs)
-            # Otherwise, conduct minimal parsing.
-            with open(inputs, "rb") as file:
-                config = tomllib.load(file, parse_float=_parse_float)
-            section = config.get(field.name, config)  # subsection or full file
-            return (
-                _instantiate_field(field, **section)
-                if isinstance(section, dict)
-                else _instantiate_field(field, section)
-            )
+        # Case of str inputs poiting to a file: try parsing it.
+        if isinstance(inputs, str) and os.path.isfile(inputs):
+            try:
+                with open(inputs, "rb") as file:
+                    config = tomllib.load(file, parse_float=_parse_float)
+            except tomllib.TOMLDecodeError as exc:
+                raise TypeError(
+                    f"Field {field.name}: could not parse secondary TOML file."
+                ) from exc
+            # Look for a subsection, otherwise keep the entire file.
+            section = config.get(field.name, config)
+            # Recursively call this parser.
+            return cls.default_parser(field, section)
         # Case of dict inputs: try instantiating the target type.
         if isinstance(inputs, dict):
             return _instantiate_field(field, **inputs)
         # Otherwise, raise a TypeError.
         raise TypeError(f"Failed to parse inputs for field {field.name}.")
 
     @classmethod
     def from_toml(
         cls,
         path: str,
+        warn_user: bool = True,
+        use_section: Optional[str] = None,
+        section_fail_ok: bool = False,
     ) -> Self:
         """Parse a structured configuration from a TOML file.
 
         The parsed TOML configuration file should be organized into sections
         that are named after this class's fields, and provide parameters to
         be parsed by the field's associated dataclass.
 
@@ -309,37 +328,54 @@
           not have a null data type.
 
         Parameters
         ----------
         path: str
             Path to a TOML configuration file, that provides with the
             hyper-parameters making up for the FL "run" configuration.
+        warn_user: bool, default=True
+            Boolean indicating whether to raise a warning when some
+            fields are unused. Useful for cases where unused fields are
+            expected, e.g. in declearn-quickrun mode.
+        use_section: optional(str), default=None
+            If not None, points to a specific section of the TOML that
+            should be used, rather than the whole file. Useful to parse
+            orchestrating TOML files, e.g. in declearn-quickrun mode.
+        section_fail_ok: bool, default=False
+            If True, allow the section specified in use_section to be
+            missing from the TOML file without raising an Error.
 
         Raises
         ------
-        RuntimeError:
+        RuntimeError
             If parsing fails, whether due to misformatting of the TOML
             file, presence of undue parameters, or absence of required
             ones.
 
         Warns
         -----
-        UserWarning:
+        UserWarning
             In case some sections of the TOML file are unused due to the
             lack of a corresponding dataclass field.
         """
         # Parse the TOML configuration file.
         try:
             with open(path, "rb") as file:
                 config = tomllib.load(file, parse_float=_parse_float)
         except tomllib.TOMLDecodeError as exc:
             raise RuntimeError(
                 "Failed to parse the TOML configuration file."
             ) from exc
         # Look for expected config sections in the parsed TOML file.
+        if isinstance(use_section, str):
+            try:
+                config = config[use_section]
+            except KeyError as exc:
+                if not section_fail_ok:
+                    raise KeyError("Specified section not found") from exc
         params = {}  # type: Dict[str, Any]
         for field in dataclasses.fields(cls):
             # Case when the section is provided: set it up for parsing.
             if field.name in config:
                 params[field.name] = config.pop(field.name)
             # Case when the section is missing: raise if it is required.
             elif (
@@ -347,14 +383,16 @@
                 and field.default_factory is dataclasses.MISSING
             ):
                 raise RuntimeError(
                     "Missing required section in the TOML configuration "
                     f"file: '{field.name}'."
                 )
         # Warn about remaining (unused) config sections.
-        for name in config:
-            warnings.warn(
-                f"Unsupported section encountered in {path} TOML file: "
-                f"'{name}'. This section will be ignored."
-            )
+        if warn_user:
+            for name in config:
+                warnings.warn(
+                    f"Unsupported section encountered in {path} TOML file: "
+                    f"'{name}'. This section will be ignored.",
+                    category=RuntimeWarning,
+                )
         # Finally, instantiate the FLConfig container.
         return cls.from_params(**params)
```

### Comparing `declearn-2.1.0/examples/adding_rmsprop/readme.md` & `declearn-2.2.0/examples/adding_rmsprop/readme.md`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/examples/heart-uci/client.py` & `declearn-2.2.0/examples/heart-uci/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,72 +13,74 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Script to run a federated client on the heart-disease example."""
 
-import argparse
 import os
-import sys
+from typing import Literal
 
 import numpy as np
-import pandas as pd  # type: ignore
+
 from declearn.communication import NetworkClientConfig
 from declearn.dataset import InMemoryDataset
+from declearn.dataset.examples import load_heart_uci
 from declearn.main import FederatedClient
+from declearn.test_utils import make_importable, setup_client_argparse
+
 
-FILEDIR = os.path.dirname(os.path.abspath(__file__))
-# Perform local imports.
-sys.path.append(FILEDIR)
-from data import get_data  # pylint: disable=wrong-import-order
+FILEDIR = os.path.dirname(__file__)
 
 
 def run_client(
-    name: str,
+    name: Literal["cleveland", "hungarian", "switzerland", "va"],
     ca_cert: str,
+    protocol: str = "websockets",
+    serv_uri: str = "wss://localhost:8765",
 ) -> None:
     """Instantiate and run a given client.
 
     Arguments
     ---------
     name: str
         Name of the client (i.e. center data from which to use).
     ca_cert: str
         Path to the certificate authority file that was used to
         sign the server's SSL certificate.
+    protocol: str, default="websockets"
+        Name of the communication protocol to use.
+    serv_uri: str, default="wss://localhost:8765"
+        URI of the server to which to connect.
     """
 
     # (1-2) Interface training and optional validation data.
 
-    # Load and randomly split the dataset.
-    path = os.path.join(FILEDIR, f"data/{name}.csv")
-    if not os.path.isfile(path):
-        get_data(os.path.join(FILEDIR, "data"), [name])
-    data = pd.read_csv(path)
+    # Load and randomly split the dataset. Note: target is a str (column name).
+    data, target = load_heart_uci(name, folder=os.path.join(FILEDIR, "data"))
     data = data.loc[np.random.permutation(data.index)]
     n_tr = round(len(data) * 0.8)  # 80% train, 20% valid
 
     # Wrap train and validation data as Dataset objects.
     train = InMemoryDataset(
         data=data.iloc[:n_tr],
-        target="num",
+        target=target,
         expose_classes=True,  # share unique target labels with server
     )
     valid = InMemoryDataset(
         data=data.iloc[n_tr:],
-        target="num",
+        target=target,
     )
 
     # (3) Define network communication parameters.
 
     # Here, use websockets protocol on localhost:8765, with SSL encryption.
     network = NetworkClientConfig(
-        protocol="websockets",
-        server_uri="wss://localhost:8765",
+        protocol=protocol,
+        server_uri=serv_uri,
         name=name,
         certificate=ca_cert,
     )
 
     # (4) Run any necessary import statement.
     #  => None are required in this example.
 
@@ -92,24 +94,20 @@
     )
     client.run()
 
 
 # Called when the script is called directly (using `python client.py`).
 if __name__ == "__main__":
     # Parse command-line arguments.
-    parser = argparse.ArgumentParser()
+    parser = setup_client_argparse(
+        usage="Start a client providing a UCI Heart-Disease Dataset shard.",
+        default_cert=os.path.join(FILEDIR, "ca-cert.pem"),
+    )
     parser.add_argument(
         "name",
         type=str,
         help="name of your client",
         choices=["cleveland", "hungarian", "switzerland", "va"],
     )
-    parser.add_argument(
-        "--cert_path",
-        dest="cert_path",
-        type=str,
-        help="path to the client-side ssl certification",
-        default=os.path.join(FILEDIR, "ca-cert.pem"),
-    )
     args = parser.parse_args()
     # Run the client routine.
-    run_client(args.name, args.cert_path)
+    run_client(args.name, args.certificate, args.protocol, args.uri)
```

### Comparing `declearn-2.1.0/examples/heart-uci/gen_ssl.py` & `declearn-2.2.0/declearn/model/torch/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Script to generate self-signed SSL certificates for the demo."""
+"""Utils for torch backend support code.
 
-import os
+GPU/CPU backing device management utils
+---------------------------------------
+* [AutoDeviceModule][declearn.model.torch.utils.AutoDeviceModule]:
+    Wrapper for a `torch.nn.Module`, automating device-management.
+* [select_device][declearn.model.torch.utils.select_device]:
+    Select a backing device to use based on inputs and availability.
+"""
 
-from declearn.test_utils import generate_ssl_certificates
-
-
-if __name__ == "__main__":
-    FILEDIR = os.path.dirname(os.path.abspath(__file__))
-    generate_ssl_certificates(FILEDIR)
+from ._gpu import AutoDeviceModule, select_device
```

### Comparing `declearn-2.1.0/examples/heart-uci/run.py` & `declearn-2.2.0/examples/heart-uci/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Demonstration script using the UCI Heart Disease Dataset."""
 
 import os
-import sys
 import tempfile
 
+from declearn.test_utils import generate_ssl_certificates, make_importable
+from declearn.utils import run_as_processes
+
 # Perform local imports.
-sys.path.append(os.path.dirname(os.path.abspath(__file__)))
-from client import run_client  # pylint: disable=wrong-import-position
-from server import run_server  # pylint: disable=wrong-import-position
-
-from declearn.test_utils import (
-    generate_ssl_certificates,
-    run_as_processes,
-)
+# pylint: disable=wrong-import-position, wrong-import-order
+with make_importable(os.path.dirname(__file__)):
+    from client import run_client
+    from server import run_server
+# pylint: enable=wrong-import-position, wrong-import-order
 
 
 NAMES = ["cleveland", "hungarian", "switzerland", "va"]
 
 
 def run_demo(
     nb_clients: int = 4,
@@ -45,14 +44,17 @@
         ca_cert, sv_cert, sv_pkey = generate_ssl_certificates(folder)
         # Specify the server and client routines that need executing.
         server = (run_server, (nb_clients, sv_cert, sv_pkey))
         clients = [
             (run_client, (name, ca_cert)) for name in NAMES[:nb_clients]
         ]
         # Run routines in isolated processes. Raise if any failed.
-        exitcodes = run_as_processes(server, *clients)
-        if any(code != 0 for code in exitcodes):
-            raise RuntimeError("Something went wrong during the demo.")
+        success, outp = run_as_processes(server, *clients)
+        if not success:
+            raise RuntimeError(
+                "Something went wrong during the demo. Exceptions caught:\n"
+                "\n".join(str(e) for e in outp if isinstance(e, RuntimeError))
+            )
 
 
 if __name__ == "__main__":
     run_demo()
```

### Comparing `declearn-2.1.0/examples/heart-uci/server.py` & `declearn-2.2.0/examples/heart-uci/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Script to run a federated server on the heart-disease example."""
 
-import argparse
 import os
 
 from declearn.communication import NetworkServerConfig
 from declearn.main import FederatedServer
 from declearn.main.config import FLOptimConfig, FLRunConfig
 from declearn.model.sklearn import SklearnSGDModel
+from declearn.test_utils import setup_server_argparse
+
 
 FILEDIR = os.path.dirname(os.path.abspath(__file__))
 
 
 def run_server(
     nb_clients: int,
-    sv_cert: str,
-    sv_priv: str,
+    certificate: str,
+    private_key: str,
+    protocol: str = "websockets",
+    host: str = "localhost",
+    port: int = 8765,
 ) -> None:
     """Instantiate and run the orchestrating server.
 
     Arguments
     ---------
     nb_clients: int
         Exact number of clients used in this example.
-    sv_cert: str
+    certificate: str
         Path to the (self-signed) SSL certificate to use.
-    sv_priv: str
+    private_key: str
         Path to the associated private-key to use.
+    protocol: str, default="websockets"
+        Name of the communication protocol to use.
+    host: str, default="localhost"
+        Hostname or IP address on which to serve.
+    port: int, default=8765
+        Communication port on which to serve.
     """
 
     # (1) Define a model
 
     # Here we use a scikit-learn SGD classifier and parametrize it
     # into a L2-penalized binary logistic regression.
     model = SklearnSGDModel.from_parameters(
@@ -84,19 +94,19 @@
         server_opt=server_opt,
     )
 
     # (3) Define network communication parameters.
 
     # Here, use websockets protocol on localhost:8765, with SSL encryption.
     network = NetworkServerConfig(
-        protocol="websockets",
-        host="localhost",
-        port=8765,
-        certificate=sv_cert,
-        private_key=sv_priv,
+        protocol=protocol,
+        host=host,
+        port=port,
+        certificate=certificate,
+        private_key=private_key,
     )
 
     # (4) Instantiate and run a FederatedServer.
 
     # Here, we add instructions to compute accuracy, precision, recall,
     # f1-score and roc auc (with plot-enabling fpr/tpr curves) during
     # evaluation rounds.
@@ -119,31 +129,21 @@
     )
     server.run(run_cfg)
 
 
 # Called when the script is called directly (using `python server.py`).
 if __name__ == "__main__":
     # Parse command-line arguments.
-    parser = argparse.ArgumentParser()
+    parser = setup_server_argparse(
+        usage="Start a server to train a logistic regression model.",
+        default_cert=os.path.join(FILEDIR, "server-cert.pem"),
+        default_pkey=os.path.join(FILEDIR, "server-pkey.pem"),
+    )
     parser.add_argument(
         "nb_clients",
         type=int,
         help="number of clients",
         choices=[1, 2, 3, 4],
     )
-    parser.add_argument(
-        "--cert_path",
-        dest="cert_path",
-        type=str,
-        help="path to the server-side ssl certification",
-        default=os.path.join(FILEDIR, "server-cert.pem"),
-    )
-    parser.add_argument(
-        "--key_path",
-        dest="key_path",
-        type=str,
-        help="path to the server-side ssl private key",
-        default=os.path.join(FILEDIR, "server-pkey.pem"),
-    )
     args = parser.parse_args()
     # Run the server routine.
-    run_server(args.nb_clients, args.cert_path, args.key_path)
+    run_server(**args.__dict__)
```

### Comparing `declearn-2.1.0/test/communication/conftest.py` & `declearn-2.2.0/test/communication/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/communication/test_grpc.py` & `declearn-2.2.0/test/communication/test_grpc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/conftest.py` & `declearn-2.2.0/test/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,21 +16,33 @@
 # limitations under the License.
 
 """Shared pytest configuration code for the test suite."""
 
 import pytest
 
 
-def pytest_addoption(parser) -> None:  # type: ignore
-    """Add a '--fulltest' option to the pytest commandline."""
+def pytest_addoption(parser) -> None:
+    """Add some custom options to the pytest commandline."""
     parser.addoption(
         "--fulltest",
         action="store_true",
         default=False,
         help="--fulltest: run all test scenarios in 'test_main.py'",
     )
+    parser.addoption(
+        "--cpu-only",
+        action="store_true",
+        default=False,
+        help="--cpu-only: disable the use of GPU devices in tests",
+    )
 
 
 @pytest.fixture(name="fulltest")
-def fulltest_fixture(request) -> bool:  # type: ignore
+def fulltest_fixture(request) -> bool:
     """Gather the '--fulltest' option's value."""
     return bool(request.config.getoption("--fulltest"))
+
+
+@pytest.fixture(name="cpu_only")
+def cpu_only_fixture(request) -> bool:
+    """Gather the '--cpu-only' option's value."""
+    return bool(request.config.getoption("--cpu-only"))
```

### Comparing `declearn-2.1.0/test/functional/conftest.py` & `declearn-2.2.0/test/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/functional/test_main.py` & `declearn-2.2.0/test/functional/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     list_available_protocols,
 )
 from declearn.communication.api import NetworkClient, NetworkServer
 from declearn.dataset import InMemoryDataset
 from declearn.model.api import Model
 from declearn.model.sklearn import SklearnSGDModel
 from declearn.main import FederatedClient, FederatedServer
-from declearn.test_utils import run_as_processes
+from declearn.utils import run_as_processes
+from declearn.utils import set_device_policy
 
 # Select the subset of tests to run, based on framework availability.
 # Note: TensorFlow and Torch (-related) imports are delayed due to this.
 # pylint: disable=ungrouped-imports
 FRAMEWORKS = ["Sksgd", "Tflow", "Torch"]
 try:
     import tensorflow as tf  # type: ignore
@@ -210,14 +211,15 @@
             "server_opt": {"lrate": 1.0, "modules": server_modules},
         }
 
     def run_federated_server(
         self,
     ) -> None:
         """Set up and run a FederatedServer."""
+        set_device_policy(gpu=False)  # disable GPU use to avoid concurrence
         model = self.build_model()
         netwk = self.build_netwk_server()
         optim = self.build_optim_config()
         with tempfile.TemporaryDirectory() as folder:
             server = FederatedServer(model, netwk, optim, checkpoint=folder)
             config = {
                 "rounds": self.rounds,
@@ -227,14 +229,15 @@
             server.run(config)
 
     def run_federated_client(
         self,
         name: str = "client",
     ) -> None:
         """Set up and run a FederatedClient."""
+        set_device_policy(gpu=False)  # disable GPU use to avoid concurrence
         netwk = self.build_netwk_client(name)
         train = self.build_dataset(size=1000)
         valid = self.build_dataset(size=250)
         with tempfile.TemporaryDirectory() as folder:
             client = FederatedClient(netwk, train, valid, folder)
             client.run()
 
@@ -260,18 +263,19 @@
     # fmt: on
     # Prepare the server and clients routines.
     server = (test_case.run_federated_server, tuple())  # type: ignore
     clients = [
         (test_case.run_federated_client, (f"cli_{i}",))
         for i in range(nb_clients)
     ]
-    # Run them concurrently using multiprocessing.
-    exitcodes = run_as_processes(server, *clients)
-    # Verify that all processes ended without error nor interruption.
-    assert all(code == 0 for code in exitcodes)
+    # Run them concurrently using multiprocessing. Assert none failed.
+    success, outputs = run_as_processes(server, *clients)
+    assert success, "Test case failed:\n" + "\n".join(
+        str(exc) for exc in outputs if isinstance(exc, RuntimeError)
+    )
 
 
 @pytest.mark.parametrize("strategy", ["FedAvg", "FedAvgM", "Scaffold"])
 @pytest.mark.parametrize("framework", FRAMEWORKS)
 @pytest.mark.parametrize("kind", ["Reg", "Bin", "Clf"])
 @pytest.mark.filterwarnings("ignore: PyTorch JSON serialization")
 def test_declearn(
@@ -282,15 +286,15 @@
 ) -> None:
     """Pytest-collected functional test of declearn's main classes.
 
     Note: Run 2 training rounds with 2 clients.
     Note: Use unsecured websockets communication, which are less
           costful to establish than gRPC and/or SSL-secured ones
           (the latter due to the certificates-generation costs).
-    Note: if websockets is unavailable, use gRPC (warn) or fail.
+    Note: If websockets is unavailable, use gRPC (warn) or fail.
     """
     if not fulltest:
         if (kind != "Reg") or (strategy == "FedAvgM"):
             pytest.skip("skip scenario (no --fulltest option)")
     protocol = "websockets"  # type: Literal["grpc", "websockets"]
     if "websockets" not in list_available_protocols():
         if "grpc" not in list_available_protocols():
```

### Comparing `declearn-2.1.0/test/functional/test_regression.py` & `declearn-2.2.0/test/functional/test_regression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # coding: utf-8
 
+# Copyright 2023 Inria (Institut National de Recherche en Informatique
+# et Automatique)
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 """Script to run convergence tests on a toy regression problem.
 
 This script sets up a toy problem, and three experiments based on it.
 
 * Problem description:
   - Toy dataset, generated using (seeded) `make_regression` from scikit-learn.
   - Dimensions: 100 features, 10 of which are informative, and 1 target.
@@ -28,39 +43,71 @@
 """
 
 import json
 import tempfile
 from typing import List, Tuple
 
 import numpy as np
-import tensorflow as tf  # type: ignore
-import torch
 from sklearn.datasets import make_regression  # type: ignore
 from sklearn.linear_model import SGDRegressor  # type: ignore
 
 from declearn.communication import NetworkClientConfig, NetworkServerConfig
 from declearn.dataset import InMemoryDataset
 from declearn.main import FederatedClient, FederatedServer
 from declearn.main.config import FLOptimConfig, FLRunConfig
 from declearn.metrics import RSquared
 from declearn.model.api import Model
 from declearn.model.sklearn import SklearnSGDModel
-from declearn.model.tensorflow import TensorflowModel
-from declearn.model.torch import TorchModel
 from declearn.optimizer import Optimizer
-from declearn.test_utils import FrameworkType, run_as_processes
+from declearn.test_utils import FrameworkType
+from declearn.utils import run_as_processes
+from declearn.utils import set_device_policy
+
+# optional frameworks' dependencies pylint: disable=ungrouped-imports
+# pylint: disable=duplicate-code
+# tensorflow imports
+try:
+    import tensorflow as tf  # type: ignore
+except ModuleNotFoundError:
+    pass
+else:
+    from declearn.model.tensorflow import TensorflowModel
+# torch imports
+try:
+    import torch
+except ModuleNotFoundError:
+    pass
+else:
+    from declearn.model.torch import TorchModel
+# pylint: enable=duplicate-code
+# haiku and jax imports
+try:
+    import haiku as hk
+    import jax
+except ModuleNotFoundError:
+    pass
+else:
+    from declearn.model.haiku import HaikuModel
+
+    def haiku_model_fn(inputs: jax.Array) -> jax.Array:
+        """Simple linear model implemented with Haiku."""
+        return hk.Linear(1)(inputs)
+
+    def haiku_loss_fn(y_pred: jax.Array, y_true: jax.Array) -> jax.Array:
+        """Sample-wise squared error loss function."""
+        return (y_pred - y_true) ** 2
+
 
 SEED = 0
 R2_THRESHOLD = 0.999
 
-# pylint: disable=too-many-function-args
-
 
 def get_model(framework: FrameworkType) -> Model:
     """Set up a simple toy regression model."""
+    set_device_policy(gpu=False)  # disable GPU use to avoid concurrence
     if framework == "numpy":
         np.random.seed(SEED)  # set seed
         model = SklearnSGDModel.from_parameters(
             kind="regressor", loss="squared_error", penalty="none"
         )  # type: Model
     elif framework == "tensorflow":
         tf.random.set_seed(SEED)  # set seed
@@ -70,14 +117,16 @@
     elif framework == "torch":
         torch.manual_seed(SEED)  # set seed
         torchmod = torch.nn.Sequential(
             torch.nn.Linear(100, 1, bias=True),
             torch.nn.Flatten(0),
         )
         model = TorchModel(torchmod, loss=torch.nn.MSELoss())
+    elif framework == "jax":
+        model = HaikuModel(haiku_model_fn, loss=haiku_loss_fn)
     else:
         raise ValueError("unrecognised framework")
     return model
 
 
 def prep_client_datasets(
     clients: int = 3,
@@ -190,47 +239,49 @@
         # Set up the (func, args) tuples specifying client-wise processes.
         datasets = prep_client_datasets(clients)
         p_client = []
         for i, data in enumerate(datasets):
             client = (_client_routine, (data[0], data[1], f"client_{i}"))
             p_client.append(client)
         # Run each and every process in parallel.
-        exitcodes = run_as_processes(p_server, *p_client)
-        if not all(code == 0 for code in exitcodes):
-            raise RuntimeError("The FL experiment failed.")
+        success, outputs = run_as_processes(p_server, *p_client)
+        assert success, "The FL process failed:\n" + "\n".join(
+            str(exc) for exc in outputs if isinstance(exc, RuntimeError)
+        )
         # Assert convergence
         with open(f"{folder}/metrics.json", encoding="utf-8") as file:
             r2_dict = json.load(file)
             last_r2_dict = r2_dict.get(max(r2_dict.keys()))
             final_r2 = float(last_r2_dict.get("r2"))
-            assert final_r2 > R2_THRESHOLD
+            assert final_r2 > R2_THRESHOLD, "The FL training did not converge"
 
 
 def _server_routine(
     folder: str,
     framework: FrameworkType,
     lrate: float = 0.01,
     rounds: int = 10,
     b_size: int = 10,
     clients: int = 3,
 ) -> None:
     """Routine to run a FL server, called by `run_declearn_experiment`."""
     # pylint: disable=too-many-arguments
     # Set up the FederatedServer.
     model = get_model(framework)
-    netwk = NetworkServerConfig("websockets", "127.0.0.1", 8765)
+    netwk = NetworkServerConfig.from_params(
+        protocol="websockets", host="127.0.0.1", port=8765
+    )
     optim = FLOptimConfig.from_params(
         aggregator="averaging",
         client_opt={
             "lrate": lrate,
             "regularizers": [("lasso", {"alpha": 0.1})],
         },
         server_opt=1.0,
     )
-
     server = FederatedServer(
         model,
         netwk,
         optim,
         metrics=["r2"],
         checkpoint=folder,
     )
@@ -249,16 +300,17 @@
 
 def _client_routine(
     train: InMemoryDataset,
     valid: InMemoryDataset,
     name: str = "client",
 ) -> None:
     """Routine to run a FL client, called by `run_declearn_experiment`."""
-    # Run the declearn FL client routine.
-    netwk = NetworkClientConfig("websockets", "ws://localhost:8765", name)
+    netwk = NetworkClientConfig.from_params(
+        protocol="websockets", server_uri="ws://localhost:8765", name=name
+    )
     client = FederatedClient(netwk, train, valid)
     client.run()
 
 
 def test_declearn_baseline(
     lrate: float = 0.01,
     rounds: int = 10,
@@ -281,15 +333,15 @@
         and the final batch may be smaller than the others (no drop).
     """
     # Generate the client datasets, then centralize them into numpy arrays.
     train, valid = prep_full_dataset()
     d_train = InMemoryDataset(train[0], train[1])
     # Set up a declearn model and a vanilla SGD optimizer.
     model = get_model("numpy")
-    model.initialize({"n_features": d_train.data.shape[1]})
+    model.initialize({"features_shape": (d_train.data.shape[1],)})
     opt = Optimizer(lrate=lrate, regularizers=[("lasso", {"alpha": 0.1})])
     # Iteratively train the model, evaluating it after each epoch.
     for _ in range(rounds):
         # Run the training round.
         for batch in d_train.generate_batches(batch_size=b_size):
             grads = model.compute_batch_gradients(batch)
             opt.apply_gradients(model, grads)
```

### Comparing `declearn-2.1.0/test/main/test_checkpoint.py` & `declearn-2.2.0/test/main/test_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     yield Checkpointer(tmp_path, 2)
 
 
 @pytest.fixture(name="model")
 def fixture_model() -> SklearnSGDModel:
     """Crete a toy binary-classification model."""
     model = SklearnSGDModel(SGDClassifier())
-    model.initialize({"n_features": 8, "classes": np.arange(2)})
+    model.initialize({"features_shape": (8,), "classes": np.arange(2)})
     return model
 
 
 @pytest.fixture(name="optimizer")
 def fixture_optimizer() -> Optimizer:
     """Create a toy optimizer"""
     testopt = Optimizer(lrate=1.0, modules=[("momentum", {"beta": 0.95})])
```

### Comparing `declearn-2.1.0/test/main/test_train_manager.py` & `declearn-2.2.0/test/main/test_train_manager.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/main/test_train_manager_dp.py` & `declearn-2.2.0/test/main/test_train_manager_dp.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 def build_dp_manager(n_batch: int) -> Any:  # DPTrainingManager with Mock attrs
     """Return a DPTrainingManager instance with Mock attributes."""
     base = build_manager(n_batch)
     # Enable accessing the (emulated) number of samples in the mock dataset.
     base.train_data.get_data_specs.return_value = DataSpecs(
         n_samples=n_batch * BATCHES["batch_size"],
-        n_features=8,  # unused
+        features_shape=(8,),  # unused
     )
     # Enable accessing the `modules` attribute of the mock Optimizer.
     base.optim.modules = []
     # Replace the base TrainingManager with a DPTrainingManager.
     return DPTrainingManager(
         base.model, base.optim, base.train_data, base.valid_data
     )
```

### Comparing `declearn-2.1.0/test/metrics/metric_testing.py` & `declearn-2.2.0/test/metrics/metric_testing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/metrics/test_binary_apr.py` & `declearn-2.2.0/test/metrics/test_binary_apr.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/metrics/test_binary_roc.py` & `declearn-2.2.0/test/metrics/test_binary_roc.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/metrics/test_mae_mse.py` & `declearn-2.2.0/test/metrics/test_mae_mse.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/metrics/test_metricset.py` & `declearn-2.2.0/test/metrics/test_metricset.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/metrics/test_multi_apr.py` & `declearn-2.2.0/test/metrics/test_multi_apr.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/metrics/test_rsquared.py` & `declearn-2.2.0/test/metrics/test_rsquared.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/model/model_testing.py` & `declearn-2.2.0/test/model/model_testing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/model/test_sksgd.py` & `declearn-2.2.0/test/model/test_sksgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     @property
     def model(
         self,
     ) -> SklearnSGDModel:
         """Suited toy binary-classification model."""
         skmod = (SGDClassifier if self.n_classes else SGDRegressor)()
         model = SklearnSGDModel(skmod)
-        data_info = {"n_features": 8}  # type: Dict[str, Any]
+        data_info = {"features_shape": (8,)}  # type: Dict[str, Any]
         if self.n_classes:
             data_info["classes"] = np.arange(self.n_classes)
         model.initialize(data_info)
         return model
 
     def assert_correct_device(
         self,
```

### Comparing `declearn-2.1.0/test/model/test_tflow.py` & `declearn-2.2.0/test/model/test_tflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for TensorflowModel."""
 
-import warnings
 import sys
+import warnings
 from typing import Any, List, Literal
 
 import numpy as np
 import pytest
 
 try:
     with warnings.catch_warnings():  # silence tensorflow import-time warnings
@@ -34,28 +34,28 @@
 from declearn.model.tensorflow import TensorflowModel, TensorflowVector
 from declearn.typing import Batch
 from declearn.utils import set_device_policy
 
 # dirty trick to import from `model_testing.py`;
 # pylint: disable=wrong-import-order, wrong-import-position
 sys.path.append(".")
-from model_testing import ModelTestSuite, ModelTestCase
+from model_testing import ModelTestCase, ModelTestSuite
 
 
 class TensorflowTestCase(ModelTestCase):
     """Tensorflow Keras test-case-provider fixture.
 
     Implemented architectures are:
     * "MLP":
         - input: 64-dimensional features vectors
         - stack: 32-neurons fully-connected layer with ReLU
                  16-neurons fully-connected layer with ReLU
                  1 output neuron with sigmoid activation
     * "MLP-tune":
-        - same as NLP, but freeze the first layer of the stack
+        - same as MLP, but freeze the first layer of the stack
     * "RNN":
         - input: 128-tokens-sequence in a 100-tokens-vocabulary
         - stack: 32-dimensional embedding matrix
                  16-neurons LSTM layer with tanh activation
                  1 output neuron with sigmoid activation
     * "CNN":
         - input: 64x64 image with 3 channels (normalized values)
@@ -155,16 +155,19 @@
         )
 
 
 @pytest.fixture(name="test_case")
 def fixture_test_case(
     kind: Literal["MLP", "MLP-tune", "RNN", "CNN"],
     device: Literal["CPU", "GPU"],
+    cpu_only: bool,
 ) -> TensorflowTestCase:
     """Fixture to access a TensorflowTestCase."""
+    if cpu_only and (device == "GPU"):
+        pytest.skip(reason="--cpu-only mode")
     return TensorflowTestCase(kind, device)
 
 
 DEVICES = ["CPU"]
 if tf.config.list_logical_devices("GPU"):
     DEVICES.append("GPU")
 
@@ -176,30 +179,30 @@
 
     def test_get_frozen_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
         """Check that `get_weights` behaves properly with frozen weights."""
         model = test_case.model
-        tfmod = getattr(model, "_model")  # type: tf.keras.Sequential
+        tfmod = model.get_wrapped_model()
         tfmod.layers[0].trainable = False  # freeze the first layer's weights
         w_all = model.get_weights()
         w_trn = model.get_weights(trainable=True)
         assert set(w_trn.coefs).issubset(w_all.coefs)  # check on keys
         assert w_trn.coefs.keys() == {v.name for v in tfmod.trainable_weights}
         assert w_all.coefs.keys() == {v.name for v in tfmod.weights}
 
     def test_set_frozen_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
         """Check that `set_weights` behaves properly with frozen weights."""
         # Setup a model with some frozen weights, and gather trainable ones.
         model = test_case.model
-        tfmod = getattr(model, "_model")  # type: tf.keras.Sequential
+        tfmod = model.get_wrapped_model()
         tfmod.layers[0].trainable = False  # freeze the first layer's weights
         w_trn = model.get_weights(trainable=True)
         # Test that `set_weights` works if and only if properly parametrized.
         with pytest.raises(KeyError):
             model.set_weights(w_trn)
         model.set_weights(w_trn, trainable=True)
         with pytest.raises(KeyError):
@@ -210,11 +213,11 @@
         test_case: TensorflowTestCase,
     ) -> None:
         """Check that at instantiation, model weights are properly placed."""
         model = test_case.model
         policy = model.device_policy
         assert policy.gpu == (test_case.device == "GPU")
         assert policy.idx == 0
-        tfmod = getattr(model, "_model")
+        tfmod = model.get_wrapped_model()
         device = f"{test_case.device}:0"
         for var in tfmod.weights:
             assert var.device.endswith(device)
```

### Comparing `declearn-2.1.0/test/model/test_torch.py` & `declearn-2.2.0/test/model/test_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,32 @@
 # dirty trick to import from `model_testing.py`;
 # pylint: disable=wrong-import-order, wrong-import-position
 sys.path.append(".")
 from model_testing import ModelTestSuite, ModelTestCase
 
 
 class ExtractLSTMFinalOutput(torch.nn.Module):
-    """Custom torch Module to gather only the desired output from a LSTM."""
+    """Custom torch Module to gather only the desired output from a LSTM.
+
+    A `torch.nn.LSTM` layer outputs:
+
+    - `output`: output tensor of shape (batch, l_seq, d_rnn)
+    - `(h_n), (c_n)`: tuple of (d_rnn, ...) final cell state tensors
+
+    This layer expects to receive these outputs as inputs, and returns
+    only the last-time-step outputs, i.e. `output[:, -1]`, with shape
+    (batch, d_rnn).
+    """
 
     def forward(
         self,
         inputs: Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]],
     ) -> torch.Tensor:
         """Extract the desired Tensor from a LSTM's outputs."""
-        return inputs[1][0][0]
+        return inputs[0][:, -1]
 
 
 class FlattenCNNOutput(torch.nn.Module):
     """Custom torch Module to reshape the output of the CNN conv layers."""
 
     def forward(self, inputs: torch.Tensor) -> torch.Tensor:
         """Reshape the Tensor to the desired shape."""
@@ -172,16 +182,19 @@
         )
 
 
 @pytest.fixture(name="test_case")
 def fixture_test_case(
     kind: Literal["MLP", "MLP-tune", "RNN", "CNN"],
     device: Literal["CPU", "GPU"],
+    cpu_only: bool,
 ) -> TorchTestCase:
     """Fixture to access a TorchTestCase."""
+    if cpu_only and device == "GPU":
+        pytest.skip(reason="--cpu-only mode")
     return TorchTestCase(kind, device)
 
 
 DEVICES = ["CPU"]
 if torch.cuda.device_count():
     DEVICES.append("GPU")
 
@@ -219,16 +232,16 @@
         # Same setup as in parent test: a model and a config-based other.
         model = test_case.model
         config = json.dumps(model.get_config())
         other = model.from_config(json.loads(config))
         # Verify that both models have the same device policy.
         assert model.device_policy == other.device_policy
         # Verify that both models have a similar structure of modules.
-        mod_a = list(getattr(model, "_model").modules())
-        mod_b = list(getattr(other, "_model").modules())
+        mod_a = list(model.get_wrapped_model().modules())
+        mod_b = list(other.get_wrapped_model().modules())
         assert len(mod_a) == len(mod_b)
         assert all(isinstance(a, type(b)) for a, b in zip(mod_a, mod_b))
         assert all(repr(a) == repr(b) for a, b in zip(mod_a, mod_b))
 
     def test_compute_batch_gradients_clipped(
         self,
         test_case: ModelTestCase,
@@ -245,15 +258,15 @@
 
     def test_get_frozen_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
         """Check that `get_weights` behaves properly with frozen weights."""
         model = test_case.model
-        ptmod = getattr(model, "_model")  # type: torch.nn.Module
+        ptmod = model.get_wrapped_model()
         next(ptmod.parameters()).requires_grad = False  # freeze some weights
         w_all = model.get_weights()
         w_trn = model.get_weights(trainable=True)
         assert set(w_trn.coefs).issubset(w_all.coefs)  # check on keys
         n_params = sum(1 for _ in ptmod.parameters())
         n_frozen = sum(not p.requires_grad for p in ptmod.parameters())
         assert n_frozen >= 1  # at least the one frozen for this test
@@ -263,15 +276,15 @@
     def test_set_frozen_weights(
         self,
         test_case: ModelTestCase,
     ) -> None:
         """Check that `set_weights` behaves properly with frozen weights."""
         # Setup a model with some frozen weights, and gather trainable ones.
         model = test_case.model
-        ptmod = getattr(model, "_model")  # type: torch.nn.Module
+        ptmod = model.get_wrapped_model()
         next(ptmod.parameters()).requires_grad = False  # freeze some weights
         w_trn = model.get_weights(trainable=True)
         # Test that `set_weights` works if and only if properly parametrized.
         with pytest.raises(KeyError):
             model.set_weights(w_trn)
         with pytest.raises(KeyError):
             model.set_weights(model.get_weights(), trainable=True)
@@ -282,11 +295,11 @@
         test_case: TorchTestCase,
     ) -> None:
         """Check that at instantiation, model weights are properly placed."""
         model = test_case.model
         policy = model.device_policy
         assert policy.gpu == (test_case.device == "GPU")
         assert (policy.idx == 0) if policy.gpu else (policy.idx is None)
-        ptmod = getattr(model, "_model").module
+        ptmod = model.get_wrapped_model().module
         device_type = "cpu" if test_case.device == "CPU" else "cuda"
         for param in ptmod.parameters():
             assert param.device.type == device_type
```

### Comparing `declearn-2.1.0/test/model/test_vector.py` & `declearn-2.2.0/test/model/test_vector.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/conftest.py` & `declearn-2.2.0/test/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/optim_testing.py` & `declearn-2.2.0/test/optimizer/optim_testing.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_modules.py` & `declearn-2.2.0/test/optimizer/test_modules.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_noise.py` & `declearn-2.2.0/test/optimizer/test_noise.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_optimizer.py` & `declearn-2.2.0/test/optimizer/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_regularizers.py` & `declearn-2.2.0/test/optimizer/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_scaffold.py` & `declearn-2.2.0/test/optimizer/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_tflow_optim.py` & `declearn-2.2.0/test/optimizer/test_tflow_optim.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/optimizer/test_torch_optim.py` & `declearn-2.2.0/test/optimizer/test_torch_optim.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/utils/test_json.py` & `declearn-2.2.0/test/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `declearn-2.1.0/test/utils/test_register.py` & `declearn-2.2.0/test/utils/test_register.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,17 +29,21 @@
     register_type,
 )
 
 
 def test_create_types_registry() -> None:
     """Unit tests for 'create_types_registry'."""
     group = f"test_{time.time_ns()}"
-    assert create_types_registry(object, group) is object
+
+    class AnyClass:  # pylint: disable=all
+        pass
+
+    assert create_types_registry(AnyClass, group) is AnyClass
     with pytest.raises(KeyError):
-        create_types_registry(object, group)
+        create_types_registry(AnyClass, group)
 
 
 def test_register_type() -> None:
     """Unit tests for 'register_type' using valid instructions."""
 
     # Define mock custom classes.
     class BaseClass:  # pylint: disable=all
@@ -71,14 +75,17 @@
     class OtherClass:  # pylint: disable=all
         pass
 
     # Try registering in a group that does not exist.
     group = f"test_{time.time_ns()}"
     with pytest.raises(KeyError):
         register_type(BaseClass, name="base", group=group)
+    # Try registering in any group, with no valid parent group.
+    with pytest.raises(TypeError):
+        register_type(BaseClass, name="base", group=None)
     # Try registering in a group with wrong class constraints.
     create_types_registry(BaseClass, group)
     with pytest.raises(TypeError):
         register_type(OtherClass, name="other", group=group)
     # Try registering the same name twice.
     register_type(BaseClass, name="base", group=group)
     with pytest.raises(KeyError):
@@ -100,17 +107,38 @@
     assert access_registered(name, group=name) is Class
     assert access_registered(name, group=None) is Class
     # Test that invalid instructions fail.
     name_2 = f"test_{time.time_ns()}"
     with pytest.raises(KeyError):
         access_registered(name_2, group=name)  # invalid name under group
     with pytest.raises(KeyError):
+        access_registered(name_2, group=None)  # invalid name under any group
+    with pytest.raises(KeyError):
         access_registered(name, group=name_2)  # non-existing group
 
 
+def test_register_unspecified_group() -> None:
+    """Unit tests for type-registration with implicit group membership."""
+    group = f"test_{time.time_ns()}"
+
+    # Define a parent class and an associted type registry.
+    @create_types_registry(name=group)
+    class Parent:  # pylint: disable=all
+        pass
+
+    # Define a child class, and register it without specifying the group.
+    @register_type(name="new-child")
+    class Child(Parent):  # pylint: disable=all
+        pass
+
+    # Verify that the class was put into the proper group.
+    assert access_registered("new-child") is Child
+    assert access_registration_info(Child) == ("new-child", group)
+
+
 def test_access_registeration_info() -> None:
     """Unit tests for 'access_registration_info'."""
 
     # Define a pair of mock custom class.
     class Class_1:  # pylint: disable=all
         pass
 
@@ -153,7 +181,11 @@
 
     # Test that the accessed mapping is a copy, with no side effect on the
     # true underlying mapping (editable through registration functions).
     mapping["renamed"] = mapping.pop("child")
     assert mapping != access_types_mapping(group=group)
     with pytest.raises(KeyError):
         access_registered("renamed", group=group)
+
+    # Test that the expected exception is raised for non-existing groups.
+    with pytest.raises(KeyError):
+        access_types_mapping(group=f"test_{time.time_ns()}")
```

### Comparing `declearn-2.1.0/test/utils/test_serialize.py` & `declearn-2.2.0/test/utils/test_serialize.py`

 * *Files identical despite different names*


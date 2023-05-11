# Comparing `tmp/aws_fortuna-0.1.8.tar.gz` & `tmp/aws_fortuna-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_fortuna-0.1.8.tar", max compression
+gzip compressed data, was "aws_fortuna-0.1.9.tar", max compression
```

## Comparing `aws_fortuna-0.1.8.tar` & `aws_fortuna-0.1.9.tar`

### file list

```diff
@@ -1,315 +1,316 @@
--rw-r--r--   0        0        0    10142 2022-12-29 11:49:13.235292 aws_fortuna-0.1.8/LICENSE
--rw-r--r--   0        0        0     9064 2022-12-29 11:49:13.235549 aws_fortuna-0.1.8/README.rst
--rw-r--r--   0        0        0    10244 2022-12-29 11:49:13.246233 aws_fortuna-0.1.8/fortuna/.DS_Store
--rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.246278 aws_fortuna-0.1.8/fortuna/__init__.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.246433 aws_fortuna-0.1.8/fortuna/calib_model/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.246482 aws_fortuna-0.1.8/fortuna/calib_model/__init__.py
--rw-r--r--   0        0        0      149 2023-01-06 00:21:59.676546 aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4883 2023-01-06 00:22:03.291320 aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    17293 2023-01-06 00:22:04.472027 aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/calib_model_calibrator.cpython-39.pyc
--rw-r--r--   0        0        0     4107 2023-01-06 00:21:59.677259 aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     4177 2023-01-06 00:22:24.516419 aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/regression.cpython-39.pyc
--rw-r--r--   0        0        0     6017 2022-12-29 11:49:13.246648 aws_fortuna-0.1.8/fortuna/calib_model/base.py
--rw-r--r--   0        0        0      344 2022-12-29 11:49:13.246792 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__init__.py
--rw-r--r--   0        0        0      561 2023-01-06 00:22:03.291927 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1418 2023-01-06 00:22:03.292437 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1662 2023-01-06 00:22:03.292836 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/checkpointer.cpython-39.pyc
--rw-r--r--   0        0        0     3555 2023-01-06 00:22:04.468958 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/monitor.cpython-39.pyc
--rw-r--r--   0        0        0      950 2023-01-06 00:22:04.469413 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/optimizer.cpython-39.pyc
--rw-r--r--   0        0        0      959 2023-01-06 00:22:04.469742 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/processor.cpython-39.pyc
--rw-r--r--   0        0        0     1203 2022-12-29 11:49:13.246869 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/base.py
--rw-r--r--   0        0        0     1491 2022-12-29 11:49:13.246956 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/checkpointer.py
--rw-r--r--   0        0        0     3789 2022-12-29 11:49:13.247060 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/monitor.py
--rw-r--r--   0        0        0      573 2022-12-29 11:49:13.247141 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/optimizer.py
--rw-r--r--   0        0        0      614 2022-12-29 11:49:13.247233 aws_fortuna-0.1.8/fortuna/calib_model/calib_config/processor.py
--rw-r--r--   0        0        0    22252 2022-12-29 11:49:13.247396 aws_fortuna-0.1.8/fortuna/calib_model/calib_model_calibrator.py
--rw-r--r--   0        0        0     4152 2022-12-29 11:49:13.247572 aws_fortuna-0.1.8/fortuna/calib_model/classification.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.247706 aws_fortuna-0.1.8/fortuna/calib_model/predictive/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.247745 aws_fortuna-0.1.8/fortuna/calib_model/predictive/__init__.py
--rw-r--r--   0        0        0      160 2023-01-06 00:22:24.461596 aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9084 2023-01-06 00:22:24.463139 aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     4122 2023-01-06 00:22:24.462174 aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     3949 2023-01-06 00:22:24.516932 aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/regression.cpython-39.pyc
--rw-r--r--   0        0        0    10735 2022-12-29 11:49:13.247872 aws_fortuna-0.1.8/fortuna/calib_model/predictive/base.py
--rw-r--r--   0        0        0     3671 2022-12-29 11:49:13.247970 aws_fortuna-0.1.8/fortuna/calib_model/predictive/classification.py
--rw-r--r--   0        0        0     3962 2022-12-29 11:49:13.248072 aws_fortuna-0.1.8/fortuna/calib_model/predictive/regression.py
--rw-r--r--   0        0        0     4192 2022-12-29 11:49:13.248176 aws_fortuna-0.1.8/fortuna/calib_model/regression.py
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.248264 aws_fortuna-0.1.8/fortuna/calibration/__init__.py
--rw-r--r--   0        0        0      149 2022-12-29 17:05:22.433467 aws_fortuna-0.1.8/fortuna/calibration/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    19616 2022-12-29 17:05:22.447152 aws_fortuna-0.1.8/fortuna/calibration/__pycache__/calibrator.cpython-39.pyc
--rw-r--r--   0        0        0     2871 2022-12-29 17:05:22.433967 aws_fortuna-0.1.8/fortuna/calibration/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0    24432 2022-12-29 11:49:13.248510 aws_fortuna-0.1.8/fortuna/calibration/calibrator.py
--rw-r--r--   0        0        0     2644 2022-12-29 11:49:13.248709 aws_fortuna-0.1.8/fortuna/calibration/state.py
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.248833 aws_fortuna-0.1.8/fortuna/conformal/__init__.py
--rw-r--r--   0        0        0      147 2023-01-05 18:38:21.670711 aws_fortuna-0.1.8/fortuna/conformal/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      202 2023-01-05 11:56:17.889869 aws_fortuna-0.1.8/fortuna/conformal/classification/__init__.py
--rw-r--r--   0        0        0      386 2023-01-05 18:38:21.671204 aws_fortuna-0.1.8/fortuna/conformal/classification/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4729 2023-01-06 14:43:51.700495 aws_fortuna-0.1.8/fortuna/conformal/classification/__pycache__/adaptive_prediction.cpython-39.pyc
--rw-r--r--   0        0        0     4259 2023-01-06 14:43:51.341741 aws_fortuna-0.1.8/fortuna/conformal/classification/__pycache__/simple_prediction.cpython-39.pyc
--rw-r--r--   0        0        0     4338 2023-01-06 11:07:50.484620 aws_fortuna-0.1.8/fortuna/conformal/classification/adaptive_prediction.py
--rw-r--r--   0        0        0     3708 2023-01-06 11:07:18.735462 aws_fortuna-0.1.8/fortuna/conformal/classification/simple_prediction.py
--rw-r--r--   0        0        0      433 2023-01-06 13:43:42.427204 aws_fortuna-0.1.8/fortuna/conformal/regression/__init__.py
--rw-r--r--   0        0        0      646 2023-01-06 13:48:51.901248 aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4784 2023-01-06 13:48:52.222142 aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/cvplus.cpython-39.pyc
--rw-r--r--   0        0        0     3694 2023-01-06 15:12:30.932486 aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/jackknife_minmax.cpython-39.pyc
--rw-r--r--   0        0        0     3650 2023-01-06 15:12:30.931980 aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/jackknifeplus.cpython-39.pyc
--rw-r--r--   0        0        0     5669 2023-01-06 12:07:51.377618 aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/onedim_uncertainty.cpython-39.pyc
--rw-r--r--   0        0        0     5817 2023-01-06 12:07:51.374132 aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/quantile.cpython-39.pyc
--rw-r--r--   0        0        0     4764 2023-01-06 12:53:06.387459 aws_fortuna-0.1.8/fortuna/conformal/regression/cvplus.py
--rw-r--r--   0        0        0     3845 2023-01-06 15:12:04.746670 aws_fortuna-0.1.8/fortuna/conformal/regression/jackknife_minmax.py
--rw-r--r--   0        0        0     3837 2023-01-06 15:12:14.777330 aws_fortuna-0.1.8/fortuna/conformal/regression/jackknifeplus.py
--rw-r--r--   0        0        0     5993 2023-01-06 11:06:28.077332 aws_fortuna-0.1.8/fortuna/conformal/regression/onedim_uncertainty.py
--rw-r--r--   0        0        0     7050 2023-01-06 11:05:55.570666 aws_fortuna-0.1.8/fortuna/conformal/regression/quantile.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.249293 aws_fortuna-0.1.8/fortuna/data/.DS_Store
--rwxr-xr-x   0        0        0       72 2022-12-29 11:49:13.249391 aws_fortuna-0.1.8/fortuna/data/__init__.py
--rw-r--r--   0        0        0      287 2022-12-29 15:35:29.052348 aws_fortuna-0.1.8/fortuna/data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      243 2022-12-29 17:04:53.881537 aws_fortuna-0.1.8/fortuna/data/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    43692 2022-12-29 15:35:29.055163 aws_fortuna-0.1.8/fortuna/data/__pycache__/loader.cpython-311.pyc
--rw-r--r--   0        0        0    30898 2023-01-06 00:22:04.483083 aws_fortuna-0.1.8/fortuna/data/__pycache__/loader.cpython-39.pyc
--rwxr-xr-x   0        0        0    26663 2022-12-31 17:01:08.623545 aws_fortuna-0.1.8/fortuna/data/loader.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.249773 aws_fortuna-0.1.8/fortuna/distribution/.DS_Store
--rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.249826 aws_fortuna-0.1.8/fortuna/distribution/__init__.py
--rw-r--r--   0        0        0      150 2022-12-29 17:05:22.485269 aws_fortuna-0.1.8/fortuna/distribution/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      687 2022-12-29 17:05:22.486024 aws_fortuna-0.1.8/fortuna/distribution/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     3672 2022-12-29 17:05:22.485783 aws_fortuna-0.1.8/fortuna/distribution/__pycache__/gaussian.cpython-39.pyc
--rw-r--r--   0        0        0      244 2022-12-29 11:49:13.249945 aws_fortuna-0.1.8/fortuna/distribution/base.py
--rwxr-xr-x   0        0        0     2992 2022-12-29 11:49:13.250065 aws_fortuna-0.1.8/fortuna/distribution/gaussian.py
--rwxr-xr-x   0        0        0     4735 2022-12-29 11:49:13.250172 aws_fortuna-0.1.8/fortuna/make_data.py
--rw-r--r--   0        0        0      392 2022-12-29 11:49:13.250284 aws_fortuna-0.1.8/fortuna/make_model.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.250444 aws_fortuna-0.1.8/fortuna/metric/.DS_Store
--rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.250499 aws_fortuna-0.1.8/fortuna/metric/__init__.py
--rw-r--r--   0        0        0      162 2022-12-29 15:35:22.220782 aws_fortuna-0.1.8/fortuna/metric/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-12-29 17:04:47.090878 aws_fortuna-0.1.8/fortuna/metric/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9818 2022-12-29 15:35:22.223376 aws_fortuna-0.1.8/fortuna/metric/__pycache__/classification.cpython-311.pyc
--rw-r--r--   0        0        0     6776 2022-12-29 17:04:47.093271 aws_fortuna-0.1.8/fortuna/metric/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     4962 2023-01-06 17:12:51.554831 aws_fortuna-0.1.8/fortuna/metric/__pycache__/regression.cpython-39.pyc
--rwxr-xr-x   0        0        0     6597 2022-12-29 11:49:13.250634 aws_fortuna-0.1.8/fortuna/metric/classification.py
--rwxr-xr-x   0        0        0     4892 2023-01-06 17:10:57.806574 aws_fortuna-0.1.8/fortuna/metric/regression.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.250918 aws_fortuna-0.1.8/fortuna/model/.DS_Store
--rwxr-xr-x   0        0        0      297 2023-01-05 10:41:10.292067 aws_fortuna-0.1.8/fortuna/model/__init__.py
--rw-r--r--   0        0        0      504 2023-01-05 10:47:43.750184 aws_fortuna-0.1.8/fortuna/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2136 2023-01-05 10:47:44.213413 aws_fortuna-0.1.8/fortuna/model/__pycache__/cnn.cpython-39.pyc
--rw-r--r--   0        0        0     3439 2022-12-29 17:05:02.932265 aws_fortuna-0.1.8/fortuna/model/__pycache__/lenet.cpython-39.pyc
--rw-r--r--   0        0        0      842 2023-01-05 10:54:45.647452 aws_fortuna-0.1.8/fortuna/model/__pycache__/linear.cpython-39.pyc
--rw-r--r--   0        0        0     3370 2022-12-29 17:05:02.933507 aws_fortuna-0.1.8/fortuna/model/__pycache__/mlp.cpython-39.pyc
--rw-r--r--   0        0        0     7815 2022-12-29 17:05:02.935372 aws_fortuna-0.1.8/fortuna/model/__pycache__/resnet.cpython-39.pyc
--rw-r--r--   0        0        0     7877 2022-12-29 17:05:02.937540 aws_fortuna-0.1.8/fortuna/model/__pycache__/wideresnet.cpython-39.pyc
--rwxr-xr-x   0        0        0     1973 2022-12-29 11:49:13.251161 aws_fortuna-0.1.8/fortuna/model/cnn.py
--rwxr-xr-x   0        0        0     2910 2022-12-29 11:49:13.251271 aws_fortuna-0.1.8/fortuna/model/lenet.py
--rw-r--r--   0        0        0      400 2023-01-05 10:54:40.447740 aws_fortuna-0.1.8/fortuna/model/linear.py
--rwxr-xr-x   0        0        0     3173 2022-12-29 11:49:13.251381 aws_fortuna-0.1.8/fortuna/model/mlp.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.251532 aws_fortuna-0.1.8/fortuna/model/model_manager/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.251582 aws_fortuna-0.1.8/fortuna/model/model_manager/__init__.py
--rw-r--r--   0        0        0      157 2022-12-29 17:05:02.939181 aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2697 2022-12-29 17:05:22.429207 aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     2819 2022-12-29 17:05:02.939774 aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     4060 2022-12-29 17:05:22.524196 aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/regression.cpython-39.pyc
--rw-r--r--   0        0        0     2423 2022-12-29 17:05:22.454991 aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/state.cpython-39.pyc
--rwxr-xr-x   0        0        0     2183 2022-12-29 11:49:13.251709 aws_fortuna-0.1.8/fortuna/model/model_manager/base.py
--rw-r--r--   0        0        0     2669 2022-12-29 11:49:13.251857 aws_fortuna-0.1.8/fortuna/model/model_manager/classification.py
--rw-r--r--   0        0        0     5561 2022-12-29 11:49:13.251957 aws_fortuna-0.1.8/fortuna/model/model_manager/regression.py
--rw-r--r--   0        0        0     1739 2022-12-29 11:49:13.252072 aws_fortuna-0.1.8/fortuna/model/model_manager/state.py
--rw-r--r--   0        0        0     7821 2022-12-29 11:49:13.252194 aws_fortuna-0.1.8/fortuna/model/resnet.py
--rw-r--r--   0        0        0     7897 2022-12-29 11:49:13.252298 aws_fortuna-0.1.8/fortuna/model/wideresnet.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.252455 aws_fortuna-0.1.8/fortuna/output_calibrator/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.252508 aws_fortuna-0.1.8/fortuna/output_calibrator/__init__.py
--rw-r--r--   0        0        0      155 2022-12-29 17:05:22.430421 aws_fortuna-0.1.8/fortuna/output_calibrator/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1049 2022-12-29 17:05:22.430838 aws_fortuna-0.1.8/fortuna/output_calibrator/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     1130 2022-12-29 17:05:22.524568 aws_fortuna-0.1.8/fortuna/output_calibrator/__pycache__/regression.cpython-39.pyc
--rw-r--r--   0        0        0      582 2022-12-29 11:49:13.252617 aws_fortuna-0.1.8/fortuna/output_calibrator/classification.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.252753 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.252798 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/__init__.py
--rw-r--r--   0        0        0      176 2022-12-29 17:05:22.431357 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3341 2022-12-29 17:05:22.432014 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     2360 2022-12-29 17:05:22.455438 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     3415 2022-12-29 11:49:13.252900 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/base.py
--rw-r--r--   0        0        0     1804 2022-12-29 11:49:13.252998 aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/state.py
--rw-r--r--   0        0        0      682 2022-12-29 11:49:13.253100 aws_fortuna-0.1.8/fortuna/output_calibrator/regression.py
--rwxr-xr-x   0        0        0    14387 2022-12-29 11:49:13.253245 aws_fortuna-0.1.8/fortuna/plot.py
--rw-r--r--   0        0        0     8196 2022-12-29 11:49:13.253384 aws_fortuna-0.1.8/fortuna/prob_model/.DS_Store
--rw-r--r--   0        0        0      117 2022-12-29 11:49:13.253473 aws_fortuna-0.1.8/fortuna/prob_model/__init__.py
--rw-r--r--   0        0        0      287 2022-12-29 17:05:02.930302 aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7837 2022-12-29 17:05:22.433143 aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     7780 2022-12-29 17:05:02.931217 aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     4486 2022-12-29 17:05:22.444291 aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/prob_model_calibrator.cpython-39.pyc
--rw-r--r--   0        0        0     8332 2022-12-29 17:05:22.523509 aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/regression.cpython-39.pyc
--rw-r--r--   0        0        0    10434 2022-12-29 11:49:13.253559 aws_fortuna-0.1.8/fortuna/prob_model/base.py
--rw-r--r--   0        0        0      339 2022-12-29 11:49:13.253687 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__init__.py
--rw-r--r--   0        0        0      555 2022-12-29 17:05:22.439617 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1408 2022-12-29 17:05:22.439998 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1661 2022-12-29 17:05:22.440332 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/checkpointer.cpython-39.pyc
--rw-r--r--   0        0        0     3608 2022-12-29 17:05:22.440781 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/monitor.cpython-39.pyc
--rw-r--r--   0        0        0      949 2022-12-29 17:05:22.441208 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/optimizer.cpython-39.pyc
--rw-r--r--   0        0        0     1154 2022-12-29 17:05:22.441533 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/processor.cpython-39.pyc
--rw-r--r--   0        0        0     1194 2022-12-29 11:49:13.253761 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/base.py
--rw-r--r--   0        0        0     1491 2022-12-29 11:49:13.253833 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/checkpointer.py
--rw-r--r--   0        0        0     3843 2022-12-29 11:49:13.253905 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/monitor.py
--rw-r--r--   0        0        0      573 2022-12-29 11:49:13.253987 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/optimizer.py
--rw-r--r--   0        0        0      866 2022-12-29 11:49:13.254083 aws_fortuna-0.1.8/fortuna/prob_model/calib_config/processor.py
--rw-r--r--   0        0        0     8324 2022-12-29 11:49:13.254193 aws_fortuna-0.1.8/fortuna/prob_model/classification.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.254327 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/.DS_Store
--rw-r--r--   0        0        0      319 2022-12-29 11:49:13.254499 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__init__.py
--rw-r--r--   0        0        0      533 2022-12-29 17:05:22.441879 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1377 2022-12-29 17:05:22.442203 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1651 2022-12-29 17:05:22.442488 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/checkpointer.cpython-39.pyc
--rw-r--r--   0        0        0     2679 2022-12-29 17:05:22.442915 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/monitor.cpython-39.pyc
--rw-r--r--   0        0        0      938 2022-12-29 17:05:22.443284 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/optimizer.cpython-39.pyc
--rw-r--r--   0        0        0      947 2022-12-29 17:05:22.443592 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/processor.cpython-39.pyc
--rw-r--r--   0        0        0     1151 2022-12-29 11:49:13.254582 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/base.py
--rw-r--r--   0        0        0     1485 2022-12-29 11:49:13.254667 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/checkpointer.py
--rw-r--r--   0        0        0     2708 2022-12-29 11:49:13.254757 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/monitor.py
--rw-r--r--   0        0        0      566 2022-12-29 11:49:13.254845 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/optimizer.py
--rw-r--r--   0        0        0      607 2022-12-29 11:49:13.254938 aws_fortuna-0.1.8/fortuna/prob_model/fit_config/processor.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.255080 aws_fortuna-0.1.8/fortuna/prob_model/joint/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.255128 aws_fortuna-0.1.8/fortuna/prob_model/joint/__init__.py
--rw-r--r--   0        0        0      154 2022-12-29 17:05:22.453933 aws_fortuna-0.1.8/fortuna/prob_model/joint/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5092 2022-12-29 17:05:22.454564 aws_fortuna-0.1.8/fortuna/prob_model/joint/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     2538 2022-12-29 17:05:22.455841 aws_fortuna-0.1.8/fortuna/prob_model/joint/__pycache__/state.cpython-39.pyc
--rwxr-xr-x   0        0        0     5159 2022-12-29 11:49:13.255259 aws_fortuna-0.1.8/fortuna/prob_model/joint/base.py
--rw-r--r--   0        0        0     2375 2022-12-29 11:49:13.255395 aws_fortuna-0.1.8/fortuna/prob_model/joint/state.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.255542 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.255589 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__init__.py
--rw-r--r--   0        0        0      159 2022-12-29 17:05:22.456135 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    23738 2022-12-29 17:05:22.458177 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     7140 2022-12-29 17:05:22.461587 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     6484 2022-12-29 17:05:22.525488 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/regression.cpython-39.pyc
--rw-r--r--   0        0        0    29103 2022-12-29 11:49:13.255830 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/base.py
--rw-r--r--   0        0        0     7717 2022-12-29 11:49:13.255963 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/classification.py
--rw-r--r--   0        0        0     7184 2022-12-29 11:49:13.256053 aws_fortuna-0.1.8/fortuna/prob_model/likelihood/regression.py
--rw-r--r--   0        0        0     8196 2022-12-29 11:49:13.256190 aws_fortuna-0.1.8/fortuna/prob_model/posterior/.DS_Store
--rwxr-xr-x   0        0        0      526 2022-12-29 11:49:13.256314 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__init__.py
--rw-r--r--   0        0        0      709 2022-12-29 17:05:22.462696 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5188 2022-12-29 17:05:22.464085 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0      952 2022-12-29 17:05:22.464786 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/name_to_posterior_state.cpython-39.pyc
--rw-r--r--   0        0        0     1413 2022-12-29 17:05:22.481125 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_approximations.cpython-39.pyc
--rw-r--r--   0        0        0     1120 2022-12-29 17:05:22.464441 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_mixin.cpython-39.pyc
--rw-r--r--   0        0        0     1013 2022-12-29 17:05:22.474309 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_state_repository.cpython-39.pyc
--rw-r--r--   0        0        0      496 2022-12-29 17:05:22.477274 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_trainer.cpython-39.pyc
--rw-r--r--   0        0        0     3717 2022-12-29 17:05:22.466860 aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/state.cpython-39.pyc
--rwxr-xr-x   0        0        0     4792 2022-12-29 11:49:13.256428 aws_fortuna-0.1.8/fortuna/prob_model/posterior/base.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.256561 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/.DS_Store
--rw-r--r--   0        0        0       37 2022-12-29 11:49:13.256651 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__init__.py
--rw-r--r--   0        0        0      208 2022-12-29 17:05:22.463070 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1120 2022-12-29 17:05:22.463445 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_approximator.cpython-39.pyc
--rw-r--r--   0        0        0     5472 2022-12-29 17:05:22.481848 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_posterior.cpython-39.pyc
--rw-r--r--   0        0        0     4544 2022-12-29 17:05:22.482540 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_repositories.cpython-39.pyc
--rw-r--r--   0        0        0      322 2022-12-29 17:05:22.482798 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_state.cpython-39.pyc
--rw-r--r--   0        0        0      616 2022-12-29 11:49:13.256755 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_approximator.py
--rwxr-xr-x   0        0        0     7127 2022-12-29 11:49:13.256879 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_posterior.py
--rw-r--r--   0        0        0     4113 2022-12-29 11:49:13.256990 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_repositories.py
--rw-r--r--   0        0        0      125 2022-12-29 11:49:13.257095 aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_state.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.257248 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/.DS_Store
--rw-r--r--   0        0        0       25 2022-12-29 11:49:13.257345 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__init__.py
--rw-r--r--   0        0        0      190 2022-12-29 17:05:22.465107 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1561 2022-12-29 17:05:22.475490 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/laplace_approximator.cpython-39.pyc
--rw-r--r--   0        0        0     9981 2022-12-29 17:05:22.484116 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/laplace_posterior.cpython-39.pyc
--rw-r--r--   0        0        0     2146 2022-12-29 17:05:22.465591 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/laplace_state.cpython-39.pyc
--rw-r--r--   0        0        0     1172 2022-12-29 11:49:13.257439 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/laplace_approximator.py
--rwxr-xr-x   0        0        0    11255 2022-12-29 11:49:13.257547 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/laplace_posterior.py
--rw-r--r--   0        0        0     1958 2022-12-29 11:49:13.257658 aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/laplace_state.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.257805 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/.DS_Store
--rw-r--r--   0        0        0       17 2022-12-29 11:49:13.257904 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__init__.py
--rw-r--r--   0        0        0      178 2022-12-29 17:05:22.465976 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      760 2022-12-29 17:05:22.476433 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_approximator.cpython-39.pyc
--rw-r--r--   0        0        0     4029 2022-12-29 17:05:22.476147 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_posterior.cpython-39.pyc
--rw-r--r--   0        0        0      747 2022-12-29 17:05:22.466350 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_state.cpython-39.pyc
--rw-r--r--   0        0        0     3146 2022-12-29 17:05:22.477011 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_trainer.cpython-39.pyc
--rw-r--r--   0        0        0      362 2022-12-29 11:49:13.258005 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/map_approximator.py
--rwxr-xr-x   0        0        0     4941 2022-12-29 11:49:13.258107 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/map_posterior.py
--rw-r--r--   0        0        0      412 2022-12-29 11:49:13.258211 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/map_state.py
--rw-r--r--   0        0        0     3089 2022-12-29 11:49:13.258368 aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/map_trainer.py
--rw-r--r--   0        0        0      736 2022-12-29 11:49:13.258513 aws_fortuna-0.1.8/fortuna/prob_model/posterior/name_to_posterior_state.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.258655 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/.DS_Store
--rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.258702 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/__init__.py
--rw-r--r--   0        0        0      175 2022-12-29 17:05:22.470657 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8683 2022-12-29 17:05:22.487690 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/__pycache__/normalizing_flow_trainer.cpython-39.pyc
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.258839 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/.DS_Store
--rw-r--r--   0        0        0       19 2022-12-29 11:49:13.258925 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__init__.py
--rw-r--r--   0        0        0      198 2022-12-29 17:05:22.471022 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1687 2022-12-29 17:05:22.480443 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_approximator.cpython-39.pyc
--rw-r--r--   0        0        0     3628 2022-12-29 17:05:22.486494 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_architecture.cpython-39.pyc
--rw-r--r--   0        0        0     6825 2022-12-29 17:05:22.484993 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_posterior.cpython-39.pyc
--rw-r--r--   0        0        0     1690 2022-12-29 17:05:22.471438 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_state.cpython-39.pyc
--rw-r--r--   0        0        0      664 2022-12-29 17:05:22.486785 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_trainer.cpython-39.pyc
--rw-r--r--   0        0        0     1265 2022-12-29 11:49:13.259017 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_approximator.py
--rw-r--r--   0        0        0     3146 2022-12-29 11:49:13.259115 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_architecture.py
--rwxr-xr-x   0        0        0     8809 2022-12-29 11:49:13.259224 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_posterior.py
--rw-r--r--   0        0        0     1391 2022-12-29 11:49:13.259323 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_state.py
--rw-r--r--   0        0        0      278 2022-12-29 11:49:13.259415 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_trainer.py
--rw-r--r--   0        0        0     8825 2022-12-29 11:49:13.259498 aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/normalizing_flow_trainer.py
--rw-r--r--   0        0        0     1100 2022-12-29 11:49:13.259593 aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_approximations.py
--rw-r--r--   0        0        0      828 2022-12-29 11:49:13.259675 aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_mixin.py
--rw-r--r--   0        0        0      606 2022-12-29 11:49:13.259775 aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_state_repository.py
--rw-r--r--   0        0        0      226 2022-12-29 11:49:13.259858 aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_trainer.py
--rw-r--r--   0        0        0     3885 2022-12-29 11:49:13.259949 aws_fortuna-0.1.8/fortuna/prob_model/posterior/state.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.260077 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/.DS_Store
--rw-r--r--   0        0        0       19 2022-12-29 11:49:13.260167 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__init__.py
--rw-r--r--   0        0        0      181 2022-12-29 17:05:22.472621 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1298 2022-12-29 17:05:22.480781 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_approximator.cpython-39.pyc
--rw-r--r--   0        0        0     6964 2022-12-29 17:05:22.488644 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_posterior.cpython-39.pyc
--rw-r--r--   0        0        0     2637 2022-12-29 17:05:22.473074 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_state.cpython-39.pyc
--rw-r--r--   0        0        0     3549 2022-12-29 17:05:22.489197 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_trainer.cpython-39.pyc
--rw-r--r--   0        0        0      798 2022-12-29 11:49:13.260252 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_approximator.py
--rwxr-xr-x   0        0        0     9315 2022-12-29 11:49:13.260357 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_posterior.py
--rw-r--r--   0        0        0     2132 2022-12-29 11:49:13.260452 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_state.py
--rw-r--r--   0        0        0     3541 2022-12-29 11:49:13.260553 aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_trainer.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.260679 aws_fortuna-0.1.8/fortuna/prob_model/predictive/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.260718 aws_fortuna-0.1.8/fortuna/prob_model/predictive/__init__.py
--rw-r--r--   0        0        0      159 2022-12-29 17:05:22.489634 aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    25190 2022-12-29 17:05:22.492739 aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    14391 2022-12-29 17:05:22.490509 aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0    11724 2022-12-29 17:05:22.527278 aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/regression.cpython-39.pyc
--rwxr-xr-x   0        0        0    30099 2022-12-29 11:49:13.260827 aws_fortuna-0.1.8/fortuna/prob_model/predictive/base.py
--rw-r--r--   0        0        0    14989 2022-12-29 11:49:13.260978 aws_fortuna-0.1.8/fortuna/prob_model/predictive/classification.py
--rw-r--r--   0        0        0    13019 2022-12-29 11:49:13.261065 aws_fortuna-0.1.8/fortuna/prob_model/predictive/regression.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.261196 aws_fortuna-0.1.8/fortuna/prob_model/prior/.DS_Store
--rw-r--r--   0        0        0      148 2022-12-29 11:49:13.261289 aws_fortuna-0.1.8/fortuna/prob_model/prior/__init__.py
--rw-r--r--   0        0        0      282 2022-12-29 17:05:22.459757 aws_fortuna-0.1.8/fortuna/prob_model/prior/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1724 2022-12-29 17:05:22.460733 aws_fortuna-0.1.8/fortuna/prob_model/prior/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     3126 2022-12-29 17:05:22.460389 aws_fortuna-0.1.8/fortuna/prob_model/prior/__pycache__/gaussian.cpython-39.pyc
--rwxr-xr-x   0        0        0     1249 2022-12-29 11:49:13.261374 aws_fortuna-0.1.8/fortuna/prob_model/prior/base.py
--rw-r--r--   0        0        0     2369 2022-12-29 11:49:13.261470 aws_fortuna-0.1.8/fortuna/prob_model/prior/gaussian.py
--rw-r--r--   0        0        0     3741 2022-12-29 11:49:13.261577 aws_fortuna-0.1.8/fortuna/prob_model/prob_model_calibrator.py
--rwxr-xr-x   0        0        0     8945 2022-12-29 11:49:13.261659 aws_fortuna-0.1.8/fortuna/prob_model/regression.py
--rwxr-xr-x   0        0        0     1739 2022-12-29 11:49:13.261739 aws_fortuna-0.1.8/fortuna/prob_model/state.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.261871 aws_fortuna-0.1.8/fortuna/prob_output_layer/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.261912 aws_fortuna-0.1.8/fortuna/prob_output_layer/__init__.py
--rw-r--r--   0        0        0      155 2022-12-29 17:05:22.458735 aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5335 2022-12-29 17:05:22.459268 aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     5585 2022-12-29 17:05:22.462261 aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/classification.cpython-39.pyc
--rw-r--r--   0        0        0     5376 2022-12-29 17:05:22.526195 aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/regression.cpython-39.pyc
--rwxr-xr-x   0        0        0     4667 2022-12-29 11:49:13.262040 aws_fortuna-0.1.8/fortuna/prob_output_layer/base.py
--rw-r--r--   0        0        0     4516 2022-12-29 11:49:13.262125 aws_fortuna-0.1.8/fortuna/prob_output_layer/classification.py
--rw-r--r--   0        0        0     4877 2022-12-29 11:49:13.262236 aws_fortuna-0.1.8/fortuna/prob_output_layer/regression.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.262371 aws_fortuna-0.1.8/fortuna/training/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-29 11:49:13.262415 aws_fortuna-0.1.8/fortuna/training/__init__.py
--rw-r--r--   0        0        0      146 2022-12-29 17:05:22.434292 aws_fortuna-0.1.8/fortuna/training/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4913 2022-12-29 17:05:22.449874 aws_fortuna-0.1.8/fortuna/training/__pycache__/mixin.cpython-39.pyc
--rw-r--r--   0        0        0      511 2022-12-29 17:05:22.451614 aws_fortuna-0.1.8/fortuna/training/__pycache__/name_to_train_state.cpython-39.pyc
--rw-r--r--   0        0        0      933 2022-12-29 17:05:22.434805 aws_fortuna-0.1.8/fortuna/training/__pycache__/train_state.cpython-39.pyc
--rw-r--r--   0        0        0     2940 2022-12-29 17:05:22.474918 aws_fortuna-0.1.8/fortuna/training/__pycache__/train_state_repository.cpython-39.pyc
--rw-r--r--   0        0        0    16612 2022-12-29 17:05:22.479591 aws_fortuna-0.1.8/fortuna/training/__pycache__/trainer.cpython-39.pyc
--rwxr-xr-x   0        0        0     5190 2022-12-29 11:49:13.262520 aws_fortuna-0.1.8/fortuna/training/mixin.py
--rw-r--r--   0        0        0      241 2022-12-29 11:49:13.262609 aws_fortuna-0.1.8/fortuna/training/name_to_train_state.py
--rw-r--r--   0        0        0      468 2022-12-29 11:49:13.262695 aws_fortuna-0.1.8/fortuna/training/train_state.py
--rw-r--r--   0        0        0     3085 2022-12-29 11:49:13.262784 aws_fortuna-0.1.8/fortuna/training/train_state_repository.py
--rwxr-xr-x   0        0        0    21748 2022-12-29 11:49:13.262935 aws_fortuna-0.1.8/fortuna/training/trainer.py
--rwxr-xr-x   0        0        0      533 2022-12-29 11:49:13.263036 aws_fortuna-0.1.8/fortuna/typing.py
--rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.263177 aws_fortuna-0.1.8/fortuna/utils/.DS_Store
--rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.263224 aws_fortuna-0.1.8/fortuna/utils/__init__.py
--rw-r--r--   0        0        0      143 2022-12-29 17:05:22.429504 aws_fortuna-0.1.8/fortuna/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1432 2022-12-29 17:05:22.452158 aws_fortuna-0.1.8/fortuna/utils/__pycache__/builtins.cpython-39.pyc
--rw-r--r--   0        0        0      704 2022-12-29 17:05:22.453189 aws_fortuna-0.1.8/fortuna/utils/__pycache__/data.cpython-39.pyc
--rw-r--r--   0        0        0     1157 2022-12-29 17:05:22.453569 aws_fortuna-0.1.8/fortuna/utils/__pycache__/device.cpython-39.pyc
--rw-r--r--   0        0        0     4933 2022-12-29 17:05:22.469437 aws_fortuna-0.1.8/fortuna/utils/__pycache__/nested_dicts.cpython-39.pyc
--rw-r--r--   0        0        0     2575 2022-12-29 17:05:22.430050 aws_fortuna-0.1.8/fortuna/utils/__pycache__/random.cpython-39.pyc
--rw-r--r--   0        0        0      521 2022-12-29 17:05:22.435202 aws_fortuna-0.1.8/fortuna/utils/__pycache__/strings.cpython-39.pyc
--rw-r--r--   0        0        0      759 2022-12-29 11:49:13.263326 aws_fortuna-0.1.8/fortuna/utils/builtins.py
--rwxr-xr-x   0        0        0      569 2022-12-29 11:49:13.263412 aws_fortuna-0.1.8/fortuna/utils/data.py
--rw-r--r--   0        0        0     1032 2022-12-29 11:49:13.263502 aws_fortuna-0.1.8/fortuna/utils/device.py
--rw-r--r--   0        0        0     5583 2022-12-29 11:49:13.263595 aws_fortuna-0.1.8/fortuna/utils/nested_dicts.py
--rw-r--r--   0        0        0     1692 2022-12-29 11:49:13.263687 aws_fortuna-0.1.8/fortuna/utils/random.py
--rw-r--r--   0        0        0      124 2022-12-29 11:49:13.263775 aws_fortuna-0.1.8/fortuna/utils/strings.py
--rw-r--r--   0        0        0     1448 2023-01-06 19:35:08.766153 aws_fortuna-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    11507 1970-01-01 00:00:00.000000 aws_fortuna-0.1.8/setup.py
--rw-r--r--   0        0        0    10575 1970-01-01 00:00:00.000000 aws_fortuna-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-12-29 11:49:13.235292 aws_fortuna-0.1.9/LICENSE
+-rw-r--r--   0        0        0     9064 2022-12-29 11:49:13.235549 aws_fortuna-0.1.9/README.rst
+-rw-r--r--   0        0        0    10244 2023-01-31 14:49:18.679816 aws_fortuna-0.1.9/fortuna/.DS_Store
+-rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.246278 aws_fortuna-0.1.9/fortuna/__init__.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.246433 aws_fortuna-0.1.9/fortuna/calib_model/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.246482 aws_fortuna-0.1.9/fortuna/calib_model/__init__.py
+-rw-r--r--   0        0        0      149 2023-01-06 00:21:59.676546 aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4883 2023-01-06 00:22:03.291320 aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    17293 2023-01-06 00:22:04.472027 aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/calib_model_calibrator.cpython-39.pyc
+-rw-r--r--   0        0        0     4107 2023-01-06 00:21:59.677259 aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     4177 2023-01-06 00:22:24.516419 aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/regression.cpython-39.pyc
+-rw-r--r--   0        0        0     6017 2022-12-29 11:49:13.246648 aws_fortuna-0.1.9/fortuna/calib_model/base.py
+-rw-r--r--   0        0        0      344 2022-12-29 11:49:13.246792 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__init__.py
+-rw-r--r--   0        0        0      561 2023-01-06 00:22:03.291927 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1418 2023-01-06 00:22:03.292437 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1662 2023-01-06 00:22:03.292836 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/checkpointer.cpython-39.pyc
+-rw-r--r--   0        0        0     3555 2023-01-06 00:22:04.468958 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/monitor.cpython-39.pyc
+-rw-r--r--   0        0        0      950 2023-01-06 00:22:04.469413 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/optimizer.cpython-39.pyc
+-rw-r--r--   0        0        0      959 2023-01-06 00:22:04.469742 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/processor.cpython-39.pyc
+-rw-r--r--   0        0        0     1203 2022-12-29 11:49:13.246869 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/base.py
+-rw-r--r--   0        0        0     1491 2022-12-29 11:49:13.246956 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/checkpointer.py
+-rw-r--r--   0        0        0     3789 2022-12-29 11:49:13.247060 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/monitor.py
+-rw-r--r--   0        0        0      573 2022-12-29 11:49:13.247141 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/optimizer.py
+-rw-r--r--   0        0        0      614 2022-12-29 11:49:13.247233 aws_fortuna-0.1.9/fortuna/calib_model/calib_config/processor.py
+-rw-r--r--   0        0        0    22252 2022-12-29 11:49:13.247396 aws_fortuna-0.1.9/fortuna/calib_model/calib_model_calibrator.py
+-rw-r--r--   0        0        0     4152 2022-12-29 11:49:13.247572 aws_fortuna-0.1.9/fortuna/calib_model/classification.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.247706 aws_fortuna-0.1.9/fortuna/calib_model/predictive/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.247745 aws_fortuna-0.1.9/fortuna/calib_model/predictive/__init__.py
+-rw-r--r--   0        0        0      160 2023-01-06 00:22:24.461596 aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9084 2023-01-06 00:22:24.463139 aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     4122 2023-01-06 00:22:24.462174 aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     3949 2023-01-06 00:22:24.516932 aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/regression.cpython-39.pyc
+-rw-r--r--   0        0        0    10735 2022-12-29 11:49:13.247872 aws_fortuna-0.1.9/fortuna/calib_model/predictive/base.py
+-rw-r--r--   0        0        0     3671 2022-12-29 11:49:13.247970 aws_fortuna-0.1.9/fortuna/calib_model/predictive/classification.py
+-rw-r--r--   0        0        0     3962 2022-12-29 11:49:13.248072 aws_fortuna-0.1.9/fortuna/calib_model/predictive/regression.py
+-rw-r--r--   0        0        0     4192 2022-12-29 11:49:13.248176 aws_fortuna-0.1.9/fortuna/calib_model/regression.py
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.248264 aws_fortuna-0.1.9/fortuna/calibration/__init__.py
+-rw-r--r--   0        0        0      149 2022-12-29 17:05:22.433467 aws_fortuna-0.1.9/fortuna/calibration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    19616 2022-12-29 17:05:22.447152 aws_fortuna-0.1.9/fortuna/calibration/__pycache__/calibrator.cpython-39.pyc
+-rw-r--r--   0        0        0     2871 2022-12-29 17:05:22.433967 aws_fortuna-0.1.9/fortuna/calibration/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0    24432 2022-12-29 11:49:13.248510 aws_fortuna-0.1.9/fortuna/calibration/calibrator.py
+-rw-r--r--   0        0        0     2644 2022-12-29 11:49:13.248709 aws_fortuna-0.1.9/fortuna/calibration/state.py
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.248833 aws_fortuna-0.1.9/fortuna/conformal/__init__.py
+-rw-r--r--   0        0        0      147 2023-01-05 18:38:21.670711 aws_fortuna-0.1.9/fortuna/conformal/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      202 2023-01-17 15:23:37.591852 aws_fortuna-0.1.9/fortuna/conformal/classification/__init__.py
+-rw-r--r--   0        0        0      386 2023-01-31 14:46:01.270622 aws_fortuna-0.1.9/fortuna/conformal/classification/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4729 2023-01-31 14:46:01.659931 aws_fortuna-0.1.9/fortuna/conformal/classification/__pycache__/adaptive_prediction.cpython-39.pyc
+-rw-r--r--   0        0        0     4259 2023-01-31 14:46:01.272056 aws_fortuna-0.1.9/fortuna/conformal/classification/__pycache__/simple_prediction.cpython-39.pyc
+-rw-r--r--   0        0        0     4338 2023-01-17 15:23:37.592009 aws_fortuna-0.1.9/fortuna/conformal/classification/adaptive_prediction.py
+-rw-r--r--   0        0        0     3708 2023-01-17 15:23:37.592168 aws_fortuna-0.1.9/fortuna/conformal/classification/simple_prediction.py
+-rw-r--r--   0        0        0      433 2023-01-17 15:23:37.592325 aws_fortuna-0.1.9/fortuna/conformal/regression/__init__.py
+-rw-r--r--   0        0        0      646 2023-01-18 13:41:24.757948 aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4786 2023-01-31 14:46:01.661271 aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/cvplus.cpython-39.pyc
+-rw-r--r--   0        0        0     3694 2023-01-18 13:41:24.764287 aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/jackknife_minmax.cpython-39.pyc
+-rw-r--r--   0        0        0     3650 2023-01-18 13:41:24.762841 aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/jackknifeplus.cpython-39.pyc
+-rw-r--r--   0        0        0     5669 2023-01-18 13:41:24.760691 aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/onedim_uncertainty.cpython-39.pyc
+-rw-r--r--   0        0        0     5817 2023-01-18 13:41:24.759545 aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/quantile.cpython-39.pyc
+-rw-r--r--   0        0        0     4767 2023-01-31 14:14:10.033276 aws_fortuna-0.1.9/fortuna/conformal/regression/cvplus.py
+-rw-r--r--   0        0        0     1003 2023-01-31 14:15:31.799626 aws_fortuna-0.1.9/fortuna/conformal/regression/enbpi.py
+-rw-r--r--   0        0        0     3845 2023-01-17 15:23:37.592692 aws_fortuna-0.1.9/fortuna/conformal/regression/jackknife_minmax.py
+-rw-r--r--   0        0        0     3837 2023-01-17 15:23:37.592945 aws_fortuna-0.1.9/fortuna/conformal/regression/jackknifeplus.py
+-rw-r--r--   0        0        0     5993 2023-01-17 15:23:37.593187 aws_fortuna-0.1.9/fortuna/conformal/regression/onedim_uncertainty.py
+-rw-r--r--   0        0        0     7050 2023-01-17 15:23:37.593378 aws_fortuna-0.1.9/fortuna/conformal/regression/quantile.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.249293 aws_fortuna-0.1.9/fortuna/data/.DS_Store
+-rwxr-xr-x   0        0        0       72 2022-12-29 11:49:13.249391 aws_fortuna-0.1.9/fortuna/data/__init__.py
+-rw-r--r--   0        0        0      287 2022-12-29 15:35:29.052348 aws_fortuna-0.1.9/fortuna/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      243 2022-12-29 17:04:53.881537 aws_fortuna-0.1.9/fortuna/data/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    43692 2022-12-29 15:35:29.055163 aws_fortuna-0.1.9/fortuna/data/__pycache__/loader.cpython-311.pyc
+-rw-r--r--   0        0        0    30898 2023-01-18 13:28:43.038564 aws_fortuna-0.1.9/fortuna/data/__pycache__/loader.cpython-39.pyc
+-rwxr-xr-x   0        0        0    26663 2023-01-17 15:23:37.568773 aws_fortuna-0.1.9/fortuna/data/loader.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.249773 aws_fortuna-0.1.9/fortuna/distribution/.DS_Store
+-rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.249826 aws_fortuna-0.1.9/fortuna/distribution/__init__.py
+-rw-r--r--   0        0        0      150 2022-12-29 17:05:22.485269 aws_fortuna-0.1.9/fortuna/distribution/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      687 2022-12-29 17:05:22.486024 aws_fortuna-0.1.9/fortuna/distribution/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     3672 2022-12-29 17:05:22.485783 aws_fortuna-0.1.9/fortuna/distribution/__pycache__/gaussian.cpython-39.pyc
+-rw-r--r--   0        0        0      244 2022-12-29 11:49:13.249945 aws_fortuna-0.1.9/fortuna/distribution/base.py
+-rwxr-xr-x   0        0        0     2992 2022-12-29 11:49:13.250065 aws_fortuna-0.1.9/fortuna/distribution/gaussian.py
+-rwxr-xr-x   0        0        0     4735 2022-12-29 11:49:13.250172 aws_fortuna-0.1.9/fortuna/make_data.py
+-rw-r--r--   0        0        0      392 2022-12-29 11:49:13.250284 aws_fortuna-0.1.9/fortuna/make_model.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.250444 aws_fortuna-0.1.9/fortuna/metric/.DS_Store
+-rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.250499 aws_fortuna-0.1.9/fortuna/metric/__init__.py
+-rw-r--r--   0        0        0      162 2022-12-29 15:35:22.220782 aws_fortuna-0.1.9/fortuna/metric/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-12-29 17:04:47.090878 aws_fortuna-0.1.9/fortuna/metric/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9818 2022-12-29 15:35:22.223376 aws_fortuna-0.1.9/fortuna/metric/__pycache__/classification.cpython-311.pyc
+-rw-r--r--   0        0        0     6789 2023-01-31 14:46:01.672204 aws_fortuna-0.1.9/fortuna/metric/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     4962 2023-01-18 13:31:29.326030 aws_fortuna-0.1.9/fortuna/metric/__pycache__/regression.cpython-39.pyc
+-rwxr-xr-x   0        0        0     6637 2023-01-31 14:46:59.815700 aws_fortuna-0.1.9/fortuna/metric/classification.py
+-rwxr-xr-x   0        0        0     4892 2023-01-17 15:23:37.600823 aws_fortuna-0.1.9/fortuna/metric/regression.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.250918 aws_fortuna-0.1.9/fortuna/model/.DS_Store
+-rwxr-xr-x   0        0        0      297 2023-01-17 15:23:37.582327 aws_fortuna-0.1.9/fortuna/model/__init__.py
+-rw-r--r--   0        0        0      504 2023-01-18 13:30:09.657201 aws_fortuna-0.1.9/fortuna/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2136 2023-01-05 10:47:44.213413 aws_fortuna-0.1.9/fortuna/model/__pycache__/cnn.cpython-39.pyc
+-rw-r--r--   0        0        0     3439 2022-12-29 17:05:02.932265 aws_fortuna-0.1.9/fortuna/model/__pycache__/lenet.cpython-39.pyc
+-rw-r--r--   0        0        0      842 2023-01-18 13:30:09.662058 aws_fortuna-0.1.9/fortuna/model/__pycache__/linear.cpython-39.pyc
+-rw-r--r--   0        0        0     3370 2022-12-29 17:05:02.933507 aws_fortuna-0.1.9/fortuna/model/__pycache__/mlp.cpython-39.pyc
+-rw-r--r--   0        0        0     7815 2022-12-29 17:05:02.935372 aws_fortuna-0.1.9/fortuna/model/__pycache__/resnet.cpython-39.pyc
+-rw-r--r--   0        0        0     7877 2022-12-29 17:05:02.937540 aws_fortuna-0.1.9/fortuna/model/__pycache__/wideresnet.cpython-39.pyc
+-rwxr-xr-x   0        0        0     1973 2022-12-29 11:49:13.251161 aws_fortuna-0.1.9/fortuna/model/cnn.py
+-rwxr-xr-x   0        0        0     2910 2022-12-29 11:49:13.251271 aws_fortuna-0.1.9/fortuna/model/lenet.py
+-rw-r--r--   0        0        0      400 2023-01-17 15:23:37.582513 aws_fortuna-0.1.9/fortuna/model/linear.py
+-rwxr-xr-x   0        0        0     3173 2022-12-29 11:49:13.251381 aws_fortuna-0.1.9/fortuna/model/mlp.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.251532 aws_fortuna-0.1.9/fortuna/model/model_manager/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.251582 aws_fortuna-0.1.9/fortuna/model/model_manager/__init__.py
+-rw-r--r--   0        0        0      157 2022-12-29 17:05:02.939181 aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2697 2022-12-29 17:05:22.429207 aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2819 2022-12-29 17:05:02.939774 aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     4060 2022-12-29 17:05:22.524196 aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/regression.cpython-39.pyc
+-rw-r--r--   0        0        0     2423 2022-12-29 17:05:22.454991 aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/state.cpython-39.pyc
+-rwxr-xr-x   0        0        0     2183 2022-12-29 11:49:13.251709 aws_fortuna-0.1.9/fortuna/model/model_manager/base.py
+-rw-r--r--   0        0        0     2669 2022-12-29 11:49:13.251857 aws_fortuna-0.1.9/fortuna/model/model_manager/classification.py
+-rw-r--r--   0        0        0     5561 2022-12-29 11:49:13.251957 aws_fortuna-0.1.9/fortuna/model/model_manager/regression.py
+-rw-r--r--   0        0        0     1739 2022-12-29 11:49:13.252072 aws_fortuna-0.1.9/fortuna/model/model_manager/state.py
+-rw-r--r--   0        0        0     7821 2022-12-29 11:49:13.252194 aws_fortuna-0.1.9/fortuna/model/resnet.py
+-rw-r--r--   0        0        0     7897 2022-12-29 11:49:13.252298 aws_fortuna-0.1.9/fortuna/model/wideresnet.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.252455 aws_fortuna-0.1.9/fortuna/output_calibrator/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.252508 aws_fortuna-0.1.9/fortuna/output_calibrator/__init__.py
+-rw-r--r--   0        0        0      155 2022-12-29 17:05:22.430421 aws_fortuna-0.1.9/fortuna/output_calibrator/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1049 2022-12-29 17:05:22.430838 aws_fortuna-0.1.9/fortuna/output_calibrator/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     1130 2022-12-29 17:05:22.524568 aws_fortuna-0.1.9/fortuna/output_calibrator/__pycache__/regression.cpython-39.pyc
+-rw-r--r--   0        0        0      582 2022-12-29 11:49:13.252617 aws_fortuna-0.1.9/fortuna/output_calibrator/classification.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.252753 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.252798 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/__init__.py
+-rw-r--r--   0        0        0      176 2022-12-29 17:05:22.431357 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3341 2022-12-29 17:05:22.432014 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2360 2022-12-29 17:05:22.455438 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0     3415 2022-12-29 11:49:13.252900 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/base.py
+-rw-r--r--   0        0        0     1804 2022-12-29 11:49:13.252998 aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/state.py
+-rw-r--r--   0        0        0      682 2022-12-29 11:49:13.253100 aws_fortuna-0.1.9/fortuna/output_calibrator/regression.py
+-rwxr-xr-x   0        0        0    14387 2022-12-29 11:49:13.253245 aws_fortuna-0.1.9/fortuna/plot.py
+-rw-r--r--   0        0        0     8196 2022-12-29 11:49:13.253384 aws_fortuna-0.1.9/fortuna/prob_model/.DS_Store
+-rw-r--r--   0        0        0      117 2022-12-29 11:49:13.253473 aws_fortuna-0.1.9/fortuna/prob_model/__init__.py
+-rw-r--r--   0        0        0      287 2022-12-29 17:05:02.930302 aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7837 2022-12-29 17:05:22.433143 aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     7780 2022-12-29 17:05:02.931217 aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     4486 2022-12-29 17:05:22.444291 aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/prob_model_calibrator.cpython-39.pyc
+-rw-r--r--   0        0        0     8332 2022-12-29 17:05:22.523509 aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/regression.cpython-39.pyc
+-rw-r--r--   0        0        0    10434 2022-12-29 11:49:13.253559 aws_fortuna-0.1.9/fortuna/prob_model/base.py
+-rw-r--r--   0        0        0      339 2022-12-29 11:49:13.253687 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__init__.py
+-rw-r--r--   0        0        0      555 2022-12-29 17:05:22.439617 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1408 2022-12-29 17:05:22.439998 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1661 2022-12-29 17:05:22.440332 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/checkpointer.cpython-39.pyc
+-rw-r--r--   0        0        0     3608 2022-12-29 17:05:22.440781 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/monitor.cpython-39.pyc
+-rw-r--r--   0        0        0      949 2022-12-29 17:05:22.441208 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/optimizer.cpython-39.pyc
+-rw-r--r--   0        0        0     1154 2022-12-29 17:05:22.441533 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/processor.cpython-39.pyc
+-rw-r--r--   0        0        0     1194 2022-12-29 11:49:13.253761 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/base.py
+-rw-r--r--   0        0        0     1491 2022-12-29 11:49:13.253833 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/checkpointer.py
+-rw-r--r--   0        0        0     3843 2022-12-29 11:49:13.253905 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/monitor.py
+-rw-r--r--   0        0        0      573 2022-12-29 11:49:13.253987 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/optimizer.py
+-rw-r--r--   0        0        0      866 2022-12-29 11:49:13.254083 aws_fortuna-0.1.9/fortuna/prob_model/calib_config/processor.py
+-rw-r--r--   0        0        0     8324 2022-12-29 11:49:13.254193 aws_fortuna-0.1.9/fortuna/prob_model/classification.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.254327 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/.DS_Store
+-rw-r--r--   0        0        0      319 2022-12-29 11:49:13.254499 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__init__.py
+-rw-r--r--   0        0        0      533 2022-12-29 17:05:22.441879 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1377 2022-12-29 17:05:22.442203 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1651 2022-12-29 17:05:22.442488 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/checkpointer.cpython-39.pyc
+-rw-r--r--   0        0        0     2679 2022-12-29 17:05:22.442915 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/monitor.cpython-39.pyc
+-rw-r--r--   0        0        0      938 2022-12-29 17:05:22.443284 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/optimizer.cpython-39.pyc
+-rw-r--r--   0        0        0      947 2022-12-29 17:05:22.443592 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/processor.cpython-39.pyc
+-rw-r--r--   0        0        0     1151 2022-12-29 11:49:13.254582 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/base.py
+-rw-r--r--   0        0        0     1485 2022-12-29 11:49:13.254667 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/checkpointer.py
+-rw-r--r--   0        0        0     2708 2022-12-29 11:49:13.254757 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/monitor.py
+-rw-r--r--   0        0        0      566 2022-12-29 11:49:13.254845 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/optimizer.py
+-rw-r--r--   0        0        0      607 2022-12-29 11:49:13.254938 aws_fortuna-0.1.9/fortuna/prob_model/fit_config/processor.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.255080 aws_fortuna-0.1.9/fortuna/prob_model/joint/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.255128 aws_fortuna-0.1.9/fortuna/prob_model/joint/__init__.py
+-rw-r--r--   0        0        0      154 2022-12-29 17:05:22.453933 aws_fortuna-0.1.9/fortuna/prob_model/joint/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5092 2022-12-29 17:05:22.454564 aws_fortuna-0.1.9/fortuna/prob_model/joint/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2538 2022-12-29 17:05:22.455841 aws_fortuna-0.1.9/fortuna/prob_model/joint/__pycache__/state.cpython-39.pyc
+-rwxr-xr-x   0        0        0     5159 2022-12-29 11:49:13.255259 aws_fortuna-0.1.9/fortuna/prob_model/joint/base.py
+-rw-r--r--   0        0        0     2375 2022-12-29 11:49:13.255395 aws_fortuna-0.1.9/fortuna/prob_model/joint/state.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.255542 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.255589 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__init__.py
+-rw-r--r--   0        0        0      159 2022-12-29 17:05:22.456135 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    23738 2022-12-29 17:05:22.458177 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     7140 2022-12-29 17:05:22.461587 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     6484 2022-12-29 17:05:22.525488 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/regression.cpython-39.pyc
+-rw-r--r--   0        0        0    29103 2022-12-29 11:49:13.255830 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/base.py
+-rw-r--r--   0        0        0     7717 2022-12-29 11:49:13.255963 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/classification.py
+-rw-r--r--   0        0        0     7184 2022-12-29 11:49:13.256053 aws_fortuna-0.1.9/fortuna/prob_model/likelihood/regression.py
+-rw-r--r--   0        0        0     8196 2022-12-29 11:49:13.256190 aws_fortuna-0.1.9/fortuna/prob_model/posterior/.DS_Store
+-rwxr-xr-x   0        0        0      526 2022-12-29 11:49:13.256314 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__init__.py
+-rw-r--r--   0        0        0      709 2022-12-29 17:05:22.462696 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5188 2022-12-29 17:05:22.464085 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0      952 2022-12-29 17:05:22.464786 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/name_to_posterior_state.cpython-39.pyc
+-rw-r--r--   0        0        0     1413 2022-12-29 17:05:22.481125 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_approximations.cpython-39.pyc
+-rw-r--r--   0        0        0     1120 2022-12-29 17:05:22.464441 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_mixin.cpython-39.pyc
+-rw-r--r--   0        0        0     1013 2022-12-29 17:05:22.474309 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_state_repository.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2022-12-29 17:05:22.477274 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_trainer.cpython-39.pyc
+-rw-r--r--   0        0        0     3717 2022-12-29 17:05:22.466860 aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/state.cpython-39.pyc
+-rwxr-xr-x   0        0        0     4792 2022-12-29 11:49:13.256428 aws_fortuna-0.1.9/fortuna/prob_model/posterior/base.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.256561 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/.DS_Store
+-rw-r--r--   0        0        0       37 2022-12-29 11:49:13.256651 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__init__.py
+-rw-r--r--   0        0        0      208 2022-12-29 17:05:22.463070 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1120 2022-12-29 17:05:22.463445 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_approximator.cpython-39.pyc
+-rw-r--r--   0        0        0     5472 2022-12-29 17:05:22.481848 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_posterior.cpython-39.pyc
+-rw-r--r--   0        0        0     4544 2022-12-29 17:05:22.482540 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_repositories.cpython-39.pyc
+-rw-r--r--   0        0        0      322 2022-12-29 17:05:22.482798 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_state.cpython-39.pyc
+-rw-r--r--   0        0        0      616 2022-12-29 11:49:13.256755 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_approximator.py
+-rwxr-xr-x   0        0        0     7127 2022-12-29 11:49:13.256879 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_posterior.py
+-rw-r--r--   0        0        0     4113 2022-12-29 11:49:13.256990 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_repositories.py
+-rw-r--r--   0        0        0      125 2022-12-29 11:49:13.257095 aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_state.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.257248 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/.DS_Store
+-rw-r--r--   0        0        0       25 2022-12-29 11:49:13.257345 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__init__.py
+-rw-r--r--   0        0        0      190 2022-12-29 17:05:22.465107 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1561 2022-12-29 17:05:22.475490 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/laplace_approximator.cpython-39.pyc
+-rw-r--r--   0        0        0     9981 2022-12-29 17:05:22.484116 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/laplace_posterior.cpython-39.pyc
+-rw-r--r--   0        0        0     2146 2022-12-29 17:05:22.465591 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/laplace_state.cpython-39.pyc
+-rw-r--r--   0        0        0     1172 2022-12-29 11:49:13.257439 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/laplace_approximator.py
+-rwxr-xr-x   0        0        0    11255 2022-12-29 11:49:13.257547 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/laplace_posterior.py
+-rw-r--r--   0        0        0     1958 2022-12-29 11:49:13.257658 aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/laplace_state.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.257805 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/.DS_Store
+-rw-r--r--   0        0        0       17 2022-12-29 11:49:13.257904 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__init__.py
+-rw-r--r--   0        0        0      178 2022-12-29 17:05:22.465976 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      760 2022-12-29 17:05:22.476433 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_approximator.cpython-39.pyc
+-rw-r--r--   0        0        0     4029 2022-12-29 17:05:22.476147 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_posterior.cpython-39.pyc
+-rw-r--r--   0        0        0      747 2022-12-29 17:05:22.466350 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_state.cpython-39.pyc
+-rw-r--r--   0        0        0     3146 2022-12-29 17:05:22.477011 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_trainer.cpython-39.pyc
+-rw-r--r--   0        0        0      362 2022-12-29 11:49:13.258005 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/map_approximator.py
+-rwxr-xr-x   0        0        0     4941 2022-12-29 11:49:13.258107 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/map_posterior.py
+-rw-r--r--   0        0        0      412 2022-12-29 11:49:13.258211 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/map_state.py
+-rw-r--r--   0        0        0     3089 2022-12-29 11:49:13.258368 aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/map_trainer.py
+-rw-r--r--   0        0        0      736 2022-12-29 11:49:13.258513 aws_fortuna-0.1.9/fortuna/prob_model/posterior/name_to_posterior_state.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.258655 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/.DS_Store
+-rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.258702 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/__init__.py
+-rw-r--r--   0        0        0      175 2022-12-29 17:05:22.470657 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8683 2022-12-29 17:05:22.487690 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/__pycache__/normalizing_flow_trainer.cpython-39.pyc
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.258839 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/.DS_Store
+-rw-r--r--   0        0        0       19 2022-12-29 11:49:13.258925 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__init__.py
+-rw-r--r--   0        0        0      198 2022-12-29 17:05:22.471022 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1687 2022-12-29 17:05:22.480443 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_approximator.cpython-39.pyc
+-rw-r--r--   0        0        0     3628 2022-12-29 17:05:22.486494 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_architecture.cpython-39.pyc
+-rw-r--r--   0        0        0     6825 2022-12-29 17:05:22.484993 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_posterior.cpython-39.pyc
+-rw-r--r--   0        0        0     1690 2022-12-29 17:05:22.471438 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_state.cpython-39.pyc
+-rw-r--r--   0        0        0      664 2022-12-29 17:05:22.486785 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_trainer.cpython-39.pyc
+-rw-r--r--   0        0        0     1265 2022-12-29 11:49:13.259017 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_approximator.py
+-rw-r--r--   0        0        0     3146 2022-12-29 11:49:13.259115 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_architecture.py
+-rwxr-xr-x   0        0        0     8809 2022-12-29 11:49:13.259224 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_posterior.py
+-rw-r--r--   0        0        0     1391 2022-12-29 11:49:13.259323 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_state.py
+-rw-r--r--   0        0        0      278 2022-12-29 11:49:13.259415 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_trainer.py
+-rw-r--r--   0        0        0     8825 2022-12-29 11:49:13.259498 aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/normalizing_flow_trainer.py
+-rw-r--r--   0        0        0     1100 2022-12-29 11:49:13.259593 aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_approximations.py
+-rw-r--r--   0        0        0      828 2022-12-29 11:49:13.259675 aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_mixin.py
+-rw-r--r--   0        0        0      606 2022-12-29 11:49:13.259775 aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_state_repository.py
+-rw-r--r--   0        0        0      226 2022-12-29 11:49:13.259858 aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_trainer.py
+-rw-r--r--   0        0        0     3885 2022-12-29 11:49:13.259949 aws_fortuna-0.1.9/fortuna/prob_model/posterior/state.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.260077 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/.DS_Store
+-rw-r--r--   0        0        0       19 2022-12-29 11:49:13.260167 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__init__.py
+-rw-r--r--   0        0        0      181 2022-12-29 17:05:22.472621 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1298 2022-12-29 17:05:22.480781 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_approximator.cpython-39.pyc
+-rw-r--r--   0        0        0     6964 2022-12-29 17:05:22.488644 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_posterior.cpython-39.pyc
+-rw-r--r--   0        0        0     2637 2022-12-29 17:05:22.473074 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_state.cpython-39.pyc
+-rw-r--r--   0        0        0     3549 2022-12-29 17:05:22.489197 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_trainer.cpython-39.pyc
+-rw-r--r--   0        0        0      798 2022-12-29 11:49:13.260252 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_approximator.py
+-rwxr-xr-x   0        0        0     9315 2022-12-29 11:49:13.260357 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_posterior.py
+-rw-r--r--   0        0        0     2132 2022-12-29 11:49:13.260452 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_state.py
+-rw-r--r--   0        0        0     3541 2022-12-29 11:49:13.260553 aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_trainer.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.260679 aws_fortuna-0.1.9/fortuna/prob_model/predictive/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.260718 aws_fortuna-0.1.9/fortuna/prob_model/predictive/__init__.py
+-rw-r--r--   0        0        0      159 2022-12-29 17:05:22.489634 aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    25190 2022-12-29 17:05:22.492739 aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    14391 2022-12-29 17:05:22.490509 aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0    11724 2022-12-29 17:05:22.527278 aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/regression.cpython-39.pyc
+-rwxr-xr-x   0        0        0    30099 2022-12-29 11:49:13.260827 aws_fortuna-0.1.9/fortuna/prob_model/predictive/base.py
+-rw-r--r--   0        0        0    14989 2022-12-29 11:49:13.260978 aws_fortuna-0.1.9/fortuna/prob_model/predictive/classification.py
+-rw-r--r--   0        0        0    13019 2022-12-29 11:49:13.261065 aws_fortuna-0.1.9/fortuna/prob_model/predictive/regression.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.261196 aws_fortuna-0.1.9/fortuna/prob_model/prior/.DS_Store
+-rw-r--r--   0        0        0      148 2022-12-29 11:49:13.261289 aws_fortuna-0.1.9/fortuna/prob_model/prior/__init__.py
+-rw-r--r--   0        0        0      282 2022-12-29 17:05:22.459757 aws_fortuna-0.1.9/fortuna/prob_model/prior/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1724 2022-12-29 17:05:22.460733 aws_fortuna-0.1.9/fortuna/prob_model/prior/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     3126 2022-12-29 17:05:22.460389 aws_fortuna-0.1.9/fortuna/prob_model/prior/__pycache__/gaussian.cpython-39.pyc
+-rwxr-xr-x   0        0        0     1249 2022-12-29 11:49:13.261374 aws_fortuna-0.1.9/fortuna/prob_model/prior/base.py
+-rw-r--r--   0        0        0     2369 2022-12-29 11:49:13.261470 aws_fortuna-0.1.9/fortuna/prob_model/prior/gaussian.py
+-rw-r--r--   0        0        0     3741 2022-12-29 11:49:13.261577 aws_fortuna-0.1.9/fortuna/prob_model/prob_model_calibrator.py
+-rwxr-xr-x   0        0        0     8945 2022-12-29 11:49:13.261659 aws_fortuna-0.1.9/fortuna/prob_model/regression.py
+-rwxr-xr-x   0        0        0     1739 2022-12-29 11:49:13.261739 aws_fortuna-0.1.9/fortuna/prob_model/state.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.261871 aws_fortuna-0.1.9/fortuna/prob_output_layer/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.261912 aws_fortuna-0.1.9/fortuna/prob_output_layer/__init__.py
+-rw-r--r--   0        0        0      155 2022-12-29 17:05:22.458735 aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5335 2022-12-29 17:05:22.459268 aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     5585 2022-12-29 17:05:22.462261 aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/classification.cpython-39.pyc
+-rw-r--r--   0        0        0     5376 2022-12-29 17:05:22.526195 aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/regression.cpython-39.pyc
+-rwxr-xr-x   0        0        0     4667 2022-12-29 11:49:13.262040 aws_fortuna-0.1.9/fortuna/prob_output_layer/base.py
+-rw-r--r--   0        0        0     4516 2022-12-29 11:49:13.262125 aws_fortuna-0.1.9/fortuna/prob_output_layer/classification.py
+-rw-r--r--   0        0        0     4877 2022-12-29 11:49:13.262236 aws_fortuna-0.1.9/fortuna/prob_output_layer/regression.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.262371 aws_fortuna-0.1.9/fortuna/training/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-29 11:49:13.262415 aws_fortuna-0.1.9/fortuna/training/__init__.py
+-rw-r--r--   0        0        0      146 2022-12-29 17:05:22.434292 aws_fortuna-0.1.9/fortuna/training/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4913 2022-12-29 17:05:22.449874 aws_fortuna-0.1.9/fortuna/training/__pycache__/mixin.cpython-39.pyc
+-rw-r--r--   0        0        0      511 2022-12-29 17:05:22.451614 aws_fortuna-0.1.9/fortuna/training/__pycache__/name_to_train_state.cpython-39.pyc
+-rw-r--r--   0        0        0      933 2022-12-29 17:05:22.434805 aws_fortuna-0.1.9/fortuna/training/__pycache__/train_state.cpython-39.pyc
+-rw-r--r--   0        0        0     2940 2022-12-29 17:05:22.474918 aws_fortuna-0.1.9/fortuna/training/__pycache__/train_state_repository.cpython-39.pyc
+-rw-r--r--   0        0        0    16612 2022-12-29 17:05:22.479591 aws_fortuna-0.1.9/fortuna/training/__pycache__/trainer.cpython-39.pyc
+-rwxr-xr-x   0        0        0     5190 2022-12-29 11:49:13.262520 aws_fortuna-0.1.9/fortuna/training/mixin.py
+-rw-r--r--   0        0        0      241 2022-12-29 11:49:13.262609 aws_fortuna-0.1.9/fortuna/training/name_to_train_state.py
+-rw-r--r--   0        0        0      468 2022-12-29 11:49:13.262695 aws_fortuna-0.1.9/fortuna/training/train_state.py
+-rw-r--r--   0        0        0     3085 2022-12-29 11:49:13.262784 aws_fortuna-0.1.9/fortuna/training/train_state_repository.py
+-rwxr-xr-x   0        0        0    21748 2022-12-29 11:49:13.262935 aws_fortuna-0.1.9/fortuna/training/trainer.py
+-rwxr-xr-x   0        0        0      533 2022-12-29 11:49:13.263036 aws_fortuna-0.1.9/fortuna/typing.py
+-rw-r--r--   0        0        0     6148 2022-12-29 11:49:13.263177 aws_fortuna-0.1.9/fortuna/utils/.DS_Store
+-rwxr-xr-x   0        0        0        0 2022-12-29 11:49:13.263224 aws_fortuna-0.1.9/fortuna/utils/__init__.py
+-rw-r--r--   0        0        0      143 2022-12-29 17:05:22.429504 aws_fortuna-0.1.9/fortuna/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1432 2022-12-29 17:05:22.452158 aws_fortuna-0.1.9/fortuna/utils/__pycache__/builtins.cpython-39.pyc
+-rw-r--r--   0        0        0      704 2022-12-29 17:05:22.453189 aws_fortuna-0.1.9/fortuna/utils/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0        0        0     1157 2022-12-29 17:05:22.453569 aws_fortuna-0.1.9/fortuna/utils/__pycache__/device.cpython-39.pyc
+-rw-r--r--   0        0        0     4933 2022-12-29 17:05:22.469437 aws_fortuna-0.1.9/fortuna/utils/__pycache__/nested_dicts.cpython-39.pyc
+-rw-r--r--   0        0        0     2575 2022-12-29 17:05:22.430050 aws_fortuna-0.1.9/fortuna/utils/__pycache__/random.cpython-39.pyc
+-rw-r--r--   0        0        0      521 2022-12-29 17:05:22.435202 aws_fortuna-0.1.9/fortuna/utils/__pycache__/strings.cpython-39.pyc
+-rw-r--r--   0        0        0      759 2022-12-29 11:49:13.263326 aws_fortuna-0.1.9/fortuna/utils/builtins.py
+-rwxr-xr-x   0        0        0      569 2022-12-29 11:49:13.263412 aws_fortuna-0.1.9/fortuna/utils/data.py
+-rw-r--r--   0        0        0     1032 2022-12-29 11:49:13.263502 aws_fortuna-0.1.9/fortuna/utils/device.py
+-rw-r--r--   0        0        0     5583 2022-12-29 11:49:13.263595 aws_fortuna-0.1.9/fortuna/utils/nested_dicts.py
+-rw-r--r--   0        0        0     1692 2022-12-29 11:49:13.263687 aws_fortuna-0.1.9/fortuna/utils/random.py
+-rw-r--r--   0        0        0      124 2022-12-29 11:49:13.263775 aws_fortuna-0.1.9/fortuna/utils/strings.py
+-rw-r--r--   0        0        0     1448 2023-01-31 14:48:49.369207 aws_fortuna-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    11507 1970-01-01 00:00:00.000000 aws_fortuna-0.1.9/setup.py
+-rw-r--r--   0        0        0    10575 1970-01-01 00:00:00.000000 aws_fortuna-0.1.9/PKG-INFO
```

### Comparing `aws_fortuna-0.1.8/LICENSE` & `aws_fortuna-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/README.rst` & `aws_fortuna-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/.DS_Store` & `aws_fortuna-0.1.9/fortuna/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/.DS_Store` & `aws_fortuna-0.1.9/fortuna/calib_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/calib_model_calibrator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/calib_model_calibrator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/base.py` & `aws_fortuna-0.1.9/fortuna/calib_model/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/__init__.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/checkpointer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/checkpointer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/monitor.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/monitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/optimizer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/optimizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/__pycache__/processor.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/__pycache__/processor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/base.py` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/checkpointer.py` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/checkpointer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/monitor.py` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/monitor.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/optimizer.py` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/optimizer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_config/processor.py` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_config/processor.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/calib_model_calibrator.py` & `aws_fortuna-0.1.9/fortuna/calib_model/calib_model_calibrator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/classification.py` & `aws_fortuna-0.1.9/fortuna/calib_model/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/.DS_Store` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/base.py` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/classification.py` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/predictive/regression.py` & `aws_fortuna-0.1.9/fortuna/calib_model/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calib_model/regression.py` & `aws_fortuna-0.1.9/fortuna/calib_model/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calibration/__pycache__/calibrator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calibration/__pycache__/calibrator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calibration/__pycache__/state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/calibration/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calibration/calibrator.py` & `aws_fortuna-0.1.9/fortuna/calibration/calibrator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/calibration/state.py` & `aws_fortuna-0.1.9/fortuna/calibration/state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/classification/__pycache__/adaptive_prediction.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/classification/__pycache__/adaptive_prediction.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 11:07:50 2023 UTC, .py size: 4338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0601 b863 f210 0000  a..........c....
+00000000: 610d 0d0a 0000 0000 79bd c663 f210 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a05 0100 6400 6402 6c04  d.l.m.Z...d.d.l.
 00000050: 5a06 6400 6403 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 8302 5a0b 6402 5300 2907 e900  ..d...Z.d.S.)...
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/classification/__pycache__/simple_prediction.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/classification/__pycache__/simple_prediction.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 11:07:18 2023 UTC, .py size: 3708 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 e600 b863 7c0e 0000  a..........c|...
+00000000: 610d 0d0a 0000 0000 79bd c663 7c0e 0000  a.......y..c|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a0a  ..G.d.d...d...Z.
 00000070: 6402 5300 2907 e900 0000 0029 02da 084f  d.S.)......)...O
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/classification/adaptive_prediction.py` & `aws_fortuna-0.1.9/fortuna/conformal/classification/adaptive_prediction.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/classification/simple_prediction.py` & `aws_fortuna-0.1.9/fortuna/conformal/classification/simple_prediction.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/__init__.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 13:43:42 2023 UTC, .py size: 433 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8e25 b863 b101 0000  a........%.c....
+00000000: 610d 0d0a 0000 0000 79bd c663 b101 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6406 5300 2907  d.l.m.Z...d.S.).
 00000070: e900 0000 0029 01da 1a51 7561 6e74 696c  .....)...Quantil
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/cvplus.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/cvplus.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 12:53:06 2023 UTC, .py size: 4764 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b219 b863 9c12 0000  a..........c....
+00000000: 610d 0d0a 0000 0000 3222 d963 9f12 0000  a.......2".c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a07  ..G.d.d...d...Z.
 00000060: 6401 5300 2906 e900 0000 004e 2901 da05  d.S.)......N)...
 00000070: 4172 7261 7929 01da 044c 6973 7463 0000  Array)...Listc..
@@ -39,15 +39,15 @@
 00000260: 6365 7320 746f 206a 6163 6b6b 6e69 6665  ces to jackknife
 00000270: 2b2e 0a20 2020 2029 05da 1163 726f 7373  +..    )...cross
 00000280: 5f76 616c 5f6f 7574 7075 7473 da11 6372  _val_outputs..cr
 00000290: 6f73 735f 7661 6c5f 7461 7267 6574 73da  oss_val_targets.
 000002a0: 1263 726f 7373 5f74 6573 745f 6f75 7470  .cross_test_outp
 000002b0: 7574 73da 0565 7272 6f72 da06 7265 7475  uts..error..retu
 000002c0: 726e 6305 0000 0000 0000 0000 0000 000e  rnc.............
-000002d0: 0000 0006 0000 0043 0000 0073 a401 0000  .......C...s....
+000002d0: 0000 0006 0000 0043 0000 0073 a601 0000  .......C...s....
 000002e0: 7400 7c01 8301 7401 6b03 7214 7402 6401  t.|...t.k.r.t.d.
 000002f0: 8301 8201 7400 7c02 8301 7401 6b03 7228  ....t.|...t.k.r(
 00000300: 7402 6402 8301 8201 7400 7c03 8301 7401  t.d.....t.|...t.
 00000310: 6b03 723c 7402 6403 8301 8201 7403 7404  k.r<t.d.....t.t.
 00000320: 7c01 7c02 7c03 8303 8301 4400 5dce 5c02  |.|.|.....D.].\.
 00000330: 7d05 5c03 7d06 7d07 7d08 7c06 6a05 6404  }.\.}.}.}.|.j.d.
 00000340: 1900 7c07 6a05 6404 1900 6b03 7276 7406  ..|.j.d...k.rvt.
@@ -62,238 +62,239 @@
 000003d0: 6407 6407 8502 6407 6602 1900 7c03 7c05  d.d...d.f...|.|.
 000003e0: 3c00 714c 7c08 6a05 6406 1900 6406 6b03  <.qL|.j.d...d.k.
 000003f0: 724c 7406 640a 8301 8201 714c 640b 640c  rLt.d.....qLd.d.
 00000400: 8400 7404 7c02 7c01 8302 4400 8301 7d09  ..t.|.|...D...}.
 00000410: 7408 a009 640d 640c 8400 7404 7c03 7c09  t...d.d...t.|.|.
 00000420: 8302 4400 8301 6404 a102 7d0a 7408 a009  ..D...d...}.t...
 00000430: 640e 640c 8400 7404 7c03 7c09 8302 4400  d.d...t.|.|...D.
-00000440: 8301 a101 7d0b 7408 6a0a 7c0a 7c04 6404  ....}.t.j.|.|.d.
-00000450: 640f 8d03 7d0c 7408 6a0a 7c0b 6406 7c04  d...}.t.j.|.d.|.
-00000460: 1800 6404 640f 8d03 7d0d 7408 a00b 7401  ..d.d...}.t...t.
-00000470: 7404 7c0c 7c0d 8302 8301 a101 a00c 6410  t.|.|.........d.
-00000480: a101 5300 2911 611c 0700 000a 2020 2020  ..S.).a.....    
-00000490: 2020 2020 436f 7665 7261 6765 2069 6e74      Coverage int
-000004a0: 6572 7661 6c20 6f66 2065 6163 6820 6f66  erval of each of
-000004b0: 2074 6865 2074 6573 7420 696e 7075 7473   the test inputs
-000004c0: 2c20 6174 2074 6865 2064 6573 6972 6564  , at the desired
-000004d0: 2063 6f76 6572 6167 6520 6572 726f 722e   coverage error.
-000004e0: 2054 6869 7320 6973 2073 7570 706f 7274   This is support
-000004f0: 6564 206f 6e6c 7920 666f 720a 2020 2020  ed only for.    
-00000500: 2020 2020 6f6e 652d 6469 6d65 6e73 696f      one-dimensio
-00000510: 6e61 6c20 7461 7267 6574 2076 6172 6961  nal target varia
-00000520: 626c 6573 2e0a 0a20 2020 2020 2020 2050  bles...        P
-00000530: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00000540: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00000550: 2020 2020 2063 726f 7373 5f76 616c 5f6f       cross_val_o
-00000560: 7574 7075 7473 3a20 4c69 7374 5b41 7272  utputs: List[Arr
-00000570: 6179 5d0a 2020 2020 2020 2020 2020 2020  ay].            
-00000580: 4f75 7470 7574 7320 6f66 2074 6865 206d  Outputs of the m
-00000590: 6f64 656c 7320 7573 6564 2064 7572 696e  odels used durin
-000005a0: 6720 6372 6f73 7320 7661 6c69 6461 7469  g cross validati
-000005b0: 6f6e 2065 7661 6c75 6174 6564 2061 7420  on evaluated at 
-000005c0: 7468 6569 7220 7265 7370 6563 7469 7665  their respective
-000005d0: 2076 616c 6964 6174 696f 6e20 696e 7075   validation inpu
-000005e0: 7473 2e20 4d6f 7265 0a20 2020 2020 2020  ts. More.       
-000005f0: 2020 2020 2070 7265 6369 7365 6c79 2c20       precisely, 
-00000600: 7765 2061 7373 756d 6520 7468 6520 7472  we assume the tr
-00000610: 6169 6e69 6e67 2064 6174 6120 6861 7320  aining data has 
-00000620: 6265 656e 206a 6f69 6e74 6c79 2070 6172  been jointly par
-00000630: 7469 7469 6f6e 6564 2069 6e20 3a63 6f64  titioned in :cod
-00000640: 653a 604b 6020 7375 6273 6574 732e 2054  e:`K` subsets. T
-00000650: 6865 2069 2d74 6820 656c 656d 656e 740a  he i-th element.
-00000660: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-00000670: 6865 206c 6973 7420 6f66 203a 636f 6465  he list of :code
-00000680: 3a20 6063 726f 7373 5f76 616c 5f6f 7574  : `cross_val_out
-00000690: 7075 7473 6020 6973 2061 206d 6f64 656c  puts` is a model
-000006a0: 2074 7261 696e 6564 206f 6e20 616c 6c20   trained on all 
-000006b0: 6461 7461 2062 7574 2074 6865 2069 2d74  data but the i-t
-000006c0: 6820 7061 7274 6974 696f 6e2c 2061 6e64  h partition, and
-000006d0: 2068 6173 0a20 2020 2020 2020 2020 2020   has.           
-000006e0: 2062 6565 6e20 6576 616c 7561 7465 6420   been evaluated 
-000006f0: 6174 2074 6865 2069 6e70 7574 7320 6f66  at the inputs of
-00000700: 2074 6865 2070 6172 7469 7469 6f6e 2069   the partition i
-00000710: 2d74 6820 6974 7365 6c66 2c20 666f 7220  -th itself, for 
-00000720: 3a63 6f64 653a 6069 3d31 2c20 322c 202e  :code:`i=1, 2, .
-00000730: 2e2e 2c20 4b60 2e0a 2020 2020 2020 2020  .., K`..        
-00000740: 6372 6f73 735f 7661 6c5f 7461 7267 6574  cross_val_target
-00000750: 733a 204c 6973 745b 4172 7261 795d 0a20  s: List[Array]. 
-00000760: 2020 2020 2020 2020 2020 2054 6172 6765             Targe
-00000770: 7420 7661 7269 6162 6c65 7320 6f72 6761  t variables orga
-00000780: 6e69 7a65 6420 696e 2074 6865 2073 616d  nized in the sam
-00000790: 6520 7061 7274 6974 696f 6e73 2075 7365  e partitions use
-000007a0: 6420 666f 7220 6063 726f 7373 5f76 616c  d for `cross_val
-000007b0: 5f6f 7574 7075 7473 602e 204d 6f72 6520  _outputs`. More 
-000007c0: 7072 6563 6973 656c 792c 2074 6865 2069  precisely, the i
-000007d0: 2d74 680a 2020 2020 2020 2020 2020 2020  -th.            
-000007e0: 656c 656d 656e 7420 6f66 203a 636f 6465  element of :code
-000007f0: 3a60 6372 6f73 735f 7661 6c5f 7461 7267  :`cross_val_targ
-00000800: 6574 7360 2069 6e63 6c75 6465 7320 7468  ets` includes th
-00000810: 6520 6172 7261 7920 6f66 2074 6172 6765  e array of targe
-00000820: 7420 7661 7269 6162 6c65 7320 6f66 2074  t variables of t
-00000830: 6865 2069 2d74 6820 7061 7274 6974 696f  he i-th partitio
-00000840: 6e20 6f66 2074 6865 0a20 2020 2020 2020  n of the.       
-00000850: 2020 2020 2074 7261 696e 696e 6720 6461       training da
-00000860: 7461 2c20 666f 7220 3a63 6f64 653a 6069  ta, for :code:`i
-00000870: 3d31 2c20 322c 202e 2e2e 2c20 4b60 2e0a  =1, 2, ..., K`..
-00000880: 2020 2020 2020 2020 6372 6f73 735f 7465          cross_te
-00000890: 7374 5f6f 7574 7075 7473 3a20 4c69 7374  st_outputs: List
-000008a0: 5b41 7272 6179 5d0a 2020 2020 2020 2020  [Array].        
-000008b0: 2020 2020 4f75 7470 7574 7320 6f66 2074      Outputs of t
-000008c0: 6865 206d 6f64 656c 7320 7573 6564 2064  he models used d
-000008d0: 7572 696e 6720 6372 6f73 7320 7661 6c69  uring cross vali
-000008e0: 6461 7469 6f6e 2065 7661 6c75 6174 6564  dation evaluated
-000008f0: 2061 7420 7468 6520 7465 7374 2069 6e70   at the test inp
-00000900: 7574 732e 204d 6f72 6520 7072 6563 6973  uts. More precis
-00000910: 656c 792c 2063 6f6e 7369 6465 720a 2020  ely, consider.  
-00000920: 2020 2020 2020 2020 2020 7468 6520 7361            the sa
-00000930: 6d65 2070 6172 7469 7469 6f6e 206f 6620  me partition of 
-00000940: 6461 7461 2061 7320 7468 6520 6f6e 6520  data as the one 
-00000950: 7573 6564 2066 6f72 203a 636f 6465 3a60  used for :code:`
-00000960: 6372 6f73 735f 7661 6c5f 6f75 7470 7574  cross_val_output
-00000970: 7360 2e20 5468 656e 2074 6865 2069 2d74  s`. Then the i-t
-00000980: 6820 656c 656d 656e 7420 6f66 0a20 2020  h element of.   
-00000990: 2020 2020 2020 2020 203a 636f 6465 3a60           :code:`
-000009a0: 6372 6f73 735f 7465 7374 5f6f 7574 7075  cross_test_outpu
-000009b0: 7473 6020 7265 7072 6573 656e 7473 2074  ts` represents t
-000009c0: 6865 206f 7574 7075 7473 206f 6620 7468  he outputs of th
-000009d0: 6520 6d6f 6465 6c20 7468 6174 2068 6173  e model that has
-000009e0: 2062 6565 6e20 7472 6169 6e65 6420 7570   been trained up
-000009f0: 6f6e 2061 6c6c 2074 6865 2074 7261 696e  on all the train
-00000a00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00000a10: 6461 7461 2062 7574 2074 6865 2069 2d74  data but the i-t
-00000a20: 6820 7061 7274 6974 696f 6e2c 2061 6e64  h partition, and
-00000a30: 2065 7661 6c75 6174 6564 2061 7420 7468   evaluated at th
-00000a40: 6520 7465 7374 2069 6e70 7574 732c 2066  e test inputs, f
-00000a50: 6f72 203a 636f 6465 3a60 693d 312c 2032  or :code:`i=1, 2
-00000a60: 2c20 2e2e 2e2c 204b 602e 0a20 2020 2020  , ..., K`..     
-00000a70: 2020 2065 7272 6f72 3a20 666c 6f61 740a     error: float.
-00000a80: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00000a90: 6465 7369 7265 6420 636f 7665 7261 6765  desired coverage
-00000aa0: 2065 7272 6f72 2e20 5468 6973 206d 7573   error. This mus
-00000ab0: 7420 6265 2061 2073 6361 6c61 7220 6265  t be a scalar be
-00000ac0: 7477 6565 6e20 3020 616e 6420 312c 2065  tween 0 and 1, e
-00000ad0: 7874 7265 6d65 7320 696e 636c 7564 6564  xtremes included
-00000ae0: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00000af0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00000b00: 2d0a 2020 2020 2020 2020 6a6e 702e 6e64  -.        jnp.nd
-00000b10: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
-00000b20: 2020 5468 6520 636f 6e66 6f72 6d61 6c20    The conformal 
-00000b30: 696e 7465 7276 616c 732e 2054 6865 2074  intervals. The t
-00000b40: 776f 2063 6f6d 706f 6e65 6e74 7320 6f66  wo components of
-00000b50: 2074 6865 2073 6563 6f6e 6420 6178 6973   the second axis
-00000b60: 2063 6f72 7265 7370 6f6e 6420 746f 2074   correspond to t
-00000b70: 6865 206c 6566 7420 616e 6420 7269 6768  he left and righ
-00000b80: 7420 696e 7465 7276 616c 0a20 2020 2020  t interval.     
-00000b90: 2020 2020 2020 2062 6f75 6e64 732e 0a20         bounds.. 
-00000ba0: 2020 2020 2020 207a 2d60 6372 6f73 735f         z-`cross_
-00000bb0: 7661 6c5f 6f75 7470 7574 7360 206d 7573  val_outputs` mus
-00000bc0: 7420 6265 2061 206c 6973 7420 6f66 2061  t be a list of a
-00000bd0: 7272 6179 732e 7a2d 6063 726f 7373 5f76  rrays.z-`cross_v
-00000be0: 616c 5f74 6172 6765 7473 6020 6d75 7374  al_targets` must
-00000bf0: 2062 6520 6120 6c69 7374 206f 6620 6172   be a list of ar
-00000c00: 7261 7973 2e7a 2e60 6372 6f73 735f 7465  rays.z.`cross_te
-00000c10: 7374 5f6f 7574 7075 7473 6020 6d75 7374  st_outputs` must
-00000c20: 2062 6520 6120 6c69 7374 206f 6620 6172   be a list of ar
-00000c30: 7261 7973 2e72 0100 0000 7a86 5468 6520  rays.r....z.The 
-00000c40: 6669 7273 7420 6469 6d65 6e73 696f 6e20  first dimension 
-00000c50: 6f66 2074 6865 2069 2d74 6820 656c 656d  of the i-th elem
-00000c60: 656e 7420 696e 2060 6372 6f73 735f 7661  ent in `cross_va
-00000c70: 6c5f 6f75 7470 7574 7360 206d 7573 7420  l_outputs` must 
-00000c80: 6265 2074 6865 2073 616d 6520 6173 2074  be the same as t
-00000c90: 6865 206f 6e65 206f 6620 7468 6520 692d  he one of the i-
-00000ca0: 7468 2065 6c65 6d65 6e74 2069 6e20 6063  th element in `c
-00000cb0: 726f 7373 5f76 616c 5f74 6172 6765 7473  ross_val_targets
-00000cc0: 602e e901 0000 004e 7a8c 5468 6973 206d  `......Nz.This m
-00000cd0: 6574 686f 6420 6973 2073 7570 706f 7274  ethod is support
-00000ce0: 6564 206f 6e6c 7920 666f 7220 7363 616c  ed only for scal
-00000cf0: 6172 206d 6f64 656c 206f 7574 7075 7473  ar model outputs
-00000d00: 206f 6e6c 792e 2048 6f77 6576 6572 2c20   only. However, 
-00000d10: 616e 2065 6c65 6d65 6e74 206f 6620 6063  an element of `c
-00000d20: 726f 7373 5f76 616c 5f6f 7574 7075 7473  ross_val_outputs
-00000d30: 6020 6861 7320 7365 636f 6e64 2064 696d  ` has second dim
-00000d40: 656e 7369 6f6e 2067 7265 6174 6572 2074  ension greater t
-00000d50: 6861 6e20 312e 7a8a 5468 6973 206d 6574  han 1.z.This met
-00000d60: 686f 6420 6973 2073 7570 706f 7274 6564  hod is supported
-00000d70: 206f 6e6c 7920 666f 7220 7363 616c 6172   only for scalar
-00000d80: 2074 6172 6765 7420 7661 7269 6162 6c65   target variable
-00000d90: 732e 2048 6f77 6576 6572 2c20 616e 2065  s. However, an e
-00000da0: 6c65 6d65 6e74 206f 6620 6063 726f 7373  lement of `cross
-00000db0: 5f76 616c 5f74 6172 6765 7473 6020 6861  _val_targets` ha
-00000dc0: 7320 7365 636f 6e64 2064 696d 656e 7369  s second dimensi
-00000dd0: 6f6e 2067 7265 6174 6572 2074 6861 6e20  on greater than 
-00000de0: 312e 7a8d 5468 6973 206d 6574 686f 6420  1.z.This method 
-00000df0: 6973 2073 7570 706f 7274 6564 206f 6e6c  is supported onl
-00000e00: 7920 666f 7220 7363 616c 6172 206d 6f64  y for scalar mod
-00000e10: 656c 206f 7574 7075 7473 206f 6e6c 792e  el outputs only.
-00000e20: 2048 6f77 6576 6572 2c20 616e 2065 6c65   However, an ele
-00000e30: 6d65 6e74 206f 6620 6063 726f 7373 5f74  ment of `cross_t
-00000e40: 6573 745f 6f75 7470 7574 7360 2068 6173  est_outputs` has
-00000e50: 2073 6563 6f6e 6420 6469 6d65 6e73 696f   second dimensio
-00000e60: 6e20 6772 6561 7465 7220 7468 616e 2031  n greater than 1
-00000e70: 2e63 0100 0000 0000 0000 0000 0000 0300  .c..............
-00000e80: 0000 0600 0000 5300 0000 731e 0000 0067  ......S...s....g
-00000e90: 007c 005d 165c 027d 017d 0274 00a0 017c  .|.].\.}.}.t...|
-00000ea0: 017c 0218 00a1 0191 0271 0453 00a9 0029  .|.......q.S...)
-00000eb0: 02da 036a 6e70 da03 6162 7329 03da 022e  ...jnp..abs)....
-00000ec0: 30da 0179 da02 6d75 720b 0000 0072 0b00  0..y..mur....r..
-00000ed0: 0000 fa41 2f55 7365 7273 2f64 6574 6f6d  ...A/Users/detom
-00000ee0: 6d61 2f61 7773 2d66 6f72 7475 6e61 2f66  ma/aws-fortuna/f
-00000ef0: 6f72 7475 6e61 2f63 6f6e 666f 726d 616c  ortuna/conformal
-00000f00: 2f72 6567 7265 7373 696f 6e2f 6376 706c  /regression/cvpl
-00000f10: 7573 2e70 79da 0a3c 6c69 7374 636f 6d70  us.py..<listcomp
-00000f20: 3e4b 0000 00f3 0000 0000 7a3f 4356 506c  >K........z?CVPl
-00000f30: 7573 436f 6e66 6f72 6d61 6c52 6567 7265  usConformalRegre
-00000f40: 7373 6f72 2e63 6f6e 666f 726d 616c 5f69  ssor.conformal_i
-00000f50: 6e74 6572 7661 6c2e 3c6c 6f63 616c 733e  nterval.<locals>
-00000f60: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
-00000f70: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-00000f80: 5300 0000 7328 0000 0067 007c 005d 205c  S...s(...g.|.] \
-00000f90: 027d 017d 027c 0164 0019 007c 0264 0064  .}.}.|.d...|.d.d
-00000fa0: 0085 0264 0066 0219 0018 0091 0271 0453  ...d.f.......q.S
-00000fb0: 00a9 014e 720b 0000 00a9 0372 0e00 0000  ...Nr......r....
-00000fc0: 7210 0000 00da 0272 6972 0b00 0000 720b  r......rir....r.
-00000fd0: 0000 0072 1100 0000 7212 0000 004c 0000  ...r....r....L..
-00000fe0: 0072 1300 0000 6301 0000 0000 0000 0000  .r....c.........
-00000ff0: 0000 0003 0000 0006 0000 0053 0000 0073  ...........S...s
-00001000: 2800 0000 6700 7c00 5d20 5c02 7d01 7d02  (...g.|.] \.}.}.
-00001010: 7c01 6400 1900 7c02 6400 6400 8502 6400  |.d...|.d.d...d.
-00001020: 6602 1900 1700 9102 7104 5300 7214 0000  f.......q.S.r...
-00001030: 0072 0b00 0000 7215 0000 0072 0b00 0000  .r....r....r....
-00001040: 720b 0000 0072 1100 0000 7212 0000 004d  r....r....r....M
-00001050: 0000 0072 1300 0000 2902 da01 71da 0461  ...r....)...q..a
-00001060: 7869 73e9 0200 0000 290d da04 7479 7065  xis.....)...type
-00001070: da04 6c69 7374 da09 5479 7065 4572 726f  ..list..TypeErro
-00001080: 72da 0965 6e75 6d65 7261 7465 da03 7a69  r..enumerate..zi
-00001090: 70da 0573 6861 7065 da0a 5661 6c75 6545  p..shape..ValueE
-000010a0: 7272 6f72 da04 6e64 696d 720c 0000 00da  rror..ndimr.....
-000010b0: 0b63 6f6e 6361 7465 6e61 7465 da08 7175  .concatenate..qu
-000010c0: 616e 7469 6c65 da05 6172 7261 79da 0773  antile..array..s
-000010d0: 7175 6565 7a65 290e da04 7365 6c66 7205  queeze)...selfr.
-000010e0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-000010f0: 0000 da01 6972 1000 0000 720f 0000 005a  ....ir....r....Z
-00001100: 076d 755f 7465 7374 da01 72da 046c 6566  .mu_test..r..lef
-00001110: 74da 0572 6967 6874 5a05 716c 6566 745a  t..rightZ.qleftZ
-00001120: 0671 7269 6768 7472 0b00 0000 720b 0000  .qrightr....r...
-00001130: 0072 1100 0000 da12 636f 6e66 6f72 6d61  .r......conforma
-00001140: 6c5f 696e 7465 7276 616c 0d00 0000 733a  l_interval....s:
-00001150: 0000 0000 230c 0108 010c 0108 010c 0108  ....#...........
-00001160: 011e 0114 0108 020a 0116 010e 0102 0102  ................
-00001170: ff04 030a 0116 010e 0108 020c 0116 010e  ................
-00001180: 010a 0314 011c 011a 0210 0114 017a 2b43  .............z+C
-00001190: 5650 6c75 7343 6f6e 666f 726d 616c 5265  VPlusConformalRe
-000011a0: 6772 6573 736f 722e 636f 6e66 6f72 6d61  gressor.conforma
-000011b0: 6c5f 696e 7465 7276 616c 4e29 0ada 085f  l_intervalN)..._
-000011c0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000011d0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000011e0: 5fda 075f 5f64 6f63 5f5f 7203 0000 0072  _..__doc__r....r
-000011f0: 0200 0000 da05 666c 6f61 7472 0c00 0000  ......floatr....
-00001200: da07 6e64 6172 7261 7972 2b00 0000 720b  ..ndarrayr+...r.
-00001210: 0000 0072 0b00 0000 720b 0000 0072 1100  ...r....r....r..
-00001220: 0000 7204 0000 0006 0000 0073 0e00 0000  ..r........s....
-00001230: 0801 0408 0601 0601 0601 0201 04fa 7204  ..............r.
-00001240: 0000 0029 08da 096a 6178 2e6e 756d 7079  ...)...jax.numpy
-00001250: da05 6e75 6d70 7972 0c00 0000 da0e 666f  ..numpyr......fo
-00001260: 7274 756e 612e 7479 7069 6e67 7202 0000  rtuna.typingr...
-00001270: 00da 0674 7970 696e 6772 0300 0000 7204  ...typingr....r.
-00001280: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-00001290: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000012a0: 3e01 0000 0073 0600 0000 0c01 0c01 0c03  >....s..........
+00000440: 8301 6404 a102 7d0b 7408 6a0a 7c0a 7c04  ..d...}.t.j.|.|.
+00000450: 6404 640f 8d03 7d0c 7408 6a0a 7c0b 6406  d.d...}.t.j.|.d.
+00000460: 7c04 1800 6404 640f 8d03 7d0d 7408 a00b  |...d.d...}.t...
+00000470: 7401 7404 7c0c 7c0d 8302 8301 a101 a00c  t.t.|.|.........
+00000480: 6410 a101 5300 2911 611c 0700 000a 2020  d...S.).a.....  
+00000490: 2020 2020 2020 436f 7665 7261 6765 2069        Coverage i
+000004a0: 6e74 6572 7661 6c20 6f66 2065 6163 6820  nterval of each 
+000004b0: 6f66 2074 6865 2074 6573 7420 696e 7075  of the test inpu
+000004c0: 7473 2c20 6174 2074 6865 2064 6573 6972  ts, at the desir
+000004d0: 6564 2063 6f76 6572 6167 6520 6572 726f  ed coverage erro
+000004e0: 722e 2054 6869 7320 6973 2073 7570 706f  r. This is suppo
+000004f0: 7274 6564 206f 6e6c 7920 666f 720a 2020  rted only for.  
+00000500: 2020 2020 2020 6f6e 652d 6469 6d65 6e73        one-dimens
+00000510: 696f 6e61 6c20 7461 7267 6574 2076 6172  ional target var
+00000520: 6961 626c 6573 2e0a 0a20 2020 2020 2020  iables...       
+00000530: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00000540: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00000550: 2020 2020 2020 2063 726f 7373 5f76 616c         cross_val
+00000560: 5f6f 7574 7075 7473 3a20 4c69 7374 5b41  _outputs: List[A
+00000570: 7272 6179 5d0a 2020 2020 2020 2020 2020  rray].          
+00000580: 2020 4f75 7470 7574 7320 6f66 2074 6865    Outputs of the
+00000590: 206d 6f64 656c 7320 7573 6564 2064 7572   models used dur
+000005a0: 696e 6720 6372 6f73 7320 7661 6c69 6461  ing cross valida
+000005b0: 7469 6f6e 2065 7661 6c75 6174 6564 2061  tion evaluated a
+000005c0: 7420 7468 6569 7220 7265 7370 6563 7469  t their respecti
+000005d0: 7665 2076 616c 6964 6174 696f 6e20 696e  ve validation in
+000005e0: 7075 7473 2e20 4d6f 7265 0a20 2020 2020  puts. More.     
+000005f0: 2020 2020 2020 2070 7265 6369 7365 6c79         precisely
+00000600: 2c20 7765 2061 7373 756d 6520 7468 6520  , we assume the 
+00000610: 7472 6169 6e69 6e67 2064 6174 6120 6861  training data ha
+00000620: 7320 6265 656e 206a 6f69 6e74 6c79 2070  s been jointly p
+00000630: 6172 7469 7469 6f6e 6564 2069 6e20 3a63  artitioned in :c
+00000640: 6f64 653a 604b 6020 7375 6273 6574 732e  ode:`K` subsets.
+00000650: 2054 6865 2069 2d74 6820 656c 656d 656e   The i-th elemen
+00000660: 740a 2020 2020 2020 2020 2020 2020 6f66  t.            of
+00000670: 2074 6865 206c 6973 7420 6f66 203a 636f   the list of :co
+00000680: 6465 3a20 6063 726f 7373 5f76 616c 5f6f  de: `cross_val_o
+00000690: 7574 7075 7473 6020 6973 2061 206d 6f64  utputs` is a mod
+000006a0: 656c 2074 7261 696e 6564 206f 6e20 616c  el trained on al
+000006b0: 6c20 6461 7461 2062 7574 2074 6865 2069  l data but the i
+000006c0: 2d74 6820 7061 7274 6974 696f 6e2c 2061  -th partition, a
+000006d0: 6e64 2068 6173 0a20 2020 2020 2020 2020  nd has.         
+000006e0: 2020 2062 6565 6e20 6576 616c 7561 7465     been evaluate
+000006f0: 6420 6174 2074 6865 2069 6e70 7574 7320  d at the inputs 
+00000700: 6f66 2074 6865 2070 6172 7469 7469 6f6e  of the partition
+00000710: 2069 2d74 6820 6974 7365 6c66 2c20 666f   i-th itself, fo
+00000720: 7220 3a63 6f64 653a 6069 3d31 2c20 322c  r :code:`i=1, 2,
+00000730: 202e 2e2e 2c20 4b60 2e0a 2020 2020 2020   ..., K`..      
+00000740: 2020 6372 6f73 735f 7661 6c5f 7461 7267    cross_val_targ
+00000750: 6574 733a 204c 6973 745b 4172 7261 795d  ets: List[Array]
+00000760: 0a20 2020 2020 2020 2020 2020 2054 6172  .            Tar
+00000770: 6765 7420 7661 7269 6162 6c65 7320 6f72  get variables or
+00000780: 6761 6e69 7a65 6420 696e 2074 6865 2073  ganized in the s
+00000790: 616d 6520 7061 7274 6974 696f 6e73 2075  ame partitions u
+000007a0: 7365 6420 666f 7220 6063 726f 7373 5f76  sed for `cross_v
+000007b0: 616c 5f6f 7574 7075 7473 602e 204d 6f72  al_outputs`. Mor
+000007c0: 6520 7072 6563 6973 656c 792c 2074 6865  e precisely, the
+000007d0: 2069 2d74 680a 2020 2020 2020 2020 2020   i-th.          
+000007e0: 2020 656c 656d 656e 7420 6f66 203a 636f    element of :co
+000007f0: 6465 3a60 6372 6f73 735f 7661 6c5f 7461  de:`cross_val_ta
+00000800: 7267 6574 7360 2069 6e63 6c75 6465 7320  rgets` includes 
+00000810: 7468 6520 6172 7261 7920 6f66 2074 6172  the array of tar
+00000820: 6765 7420 7661 7269 6162 6c65 7320 6f66  get variables of
+00000830: 2074 6865 2069 2d74 6820 7061 7274 6974   the i-th partit
+00000840: 696f 6e20 6f66 2074 6865 0a20 2020 2020  ion of the.     
+00000850: 2020 2020 2020 2074 7261 696e 696e 6720         training 
+00000860: 6461 7461 2c20 666f 7220 3a63 6f64 653a  data, for :code:
+00000870: 6069 3d31 2c20 322c 202e 2e2e 2c20 4b60  `i=1, 2, ..., K`
+00000880: 2e0a 2020 2020 2020 2020 6372 6f73 735f  ..        cross_
+00000890: 7465 7374 5f6f 7574 7075 7473 3a20 4c69  test_outputs: Li
+000008a0: 7374 5b41 7272 6179 5d0a 2020 2020 2020  st[Array].      
+000008b0: 2020 2020 2020 4f75 7470 7574 7320 6f66        Outputs of
+000008c0: 2074 6865 206d 6f64 656c 7320 7573 6564   the models used
+000008d0: 2064 7572 696e 6720 6372 6f73 7320 7661   during cross va
+000008e0: 6c69 6461 7469 6f6e 2065 7661 6c75 6174  lidation evaluat
+000008f0: 6564 2061 7420 7468 6520 7465 7374 2069  ed at the test i
+00000900: 6e70 7574 732e 204d 6f72 6520 7072 6563  nputs. More prec
+00000910: 6973 656c 792c 2063 6f6e 7369 6465 720a  isely, consider.
+00000920: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00000930: 7361 6d65 2070 6172 7469 7469 6f6e 206f  same partition o
+00000940: 6620 6461 7461 2061 7320 7468 6520 6f6e  f data as the on
+00000950: 6520 7573 6564 2066 6f72 203a 636f 6465  e used for :code
+00000960: 3a60 6372 6f73 735f 7661 6c5f 6f75 7470  :`cross_val_outp
+00000970: 7574 7360 2e20 5468 656e 2074 6865 2069  uts`. Then the i
+00000980: 2d74 6820 656c 656d 656e 7420 6f66 0a20  -th element of. 
+00000990: 2020 2020 2020 2020 2020 203a 636f 6465             :code
+000009a0: 3a60 6372 6f73 735f 7465 7374 5f6f 7574  :`cross_test_out
+000009b0: 7075 7473 6020 7265 7072 6573 656e 7473  puts` represents
+000009c0: 2074 6865 206f 7574 7075 7473 206f 6620   the outputs of 
+000009d0: 7468 6520 6d6f 6465 6c20 7468 6174 2068  the model that h
+000009e0: 6173 2062 6565 6e20 7472 6169 6e65 6420  as been trained 
+000009f0: 7570 6f6e 2061 6c6c 2074 6865 2074 7261  upon all the tra
+00000a00: 696e 696e 670a 2020 2020 2020 2020 2020  ining.          
+00000a10: 2020 6461 7461 2062 7574 2074 6865 2069    data but the i
+00000a20: 2d74 6820 7061 7274 6974 696f 6e2c 2061  -th partition, a
+00000a30: 6e64 2065 7661 6c75 6174 6564 2061 7420  nd evaluated at 
+00000a40: 7468 6520 7465 7374 2069 6e70 7574 732c  the test inputs,
+00000a50: 2066 6f72 203a 636f 6465 3a60 693d 312c   for :code:`i=1,
+00000a60: 2032 2c20 2e2e 2e2c 204b 602e 0a20 2020   2, ..., K`..   
+00000a70: 2020 2020 2065 7272 6f72 3a20 666c 6f61       error: floa
+00000a80: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
+00000a90: 6520 6465 7369 7265 6420 636f 7665 7261  e desired covera
+00000aa0: 6765 2065 7272 6f72 2e20 5468 6973 206d  ge error. This m
+00000ab0: 7573 7420 6265 2061 2073 6361 6c61 7220  ust be a scalar 
+00000ac0: 6265 7477 6565 6e20 3020 616e 6420 312c  between 0 and 1,
+00000ad0: 2065 7874 7265 6d65 7320 696e 636c 7564   extremes includ
+00000ae0: 6564 2e0a 2020 2020 2020 2020 5265 7475  ed..        Retu
+00000af0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00000b00: 2d2d 2d0a 2020 2020 2020 2020 6a6e 702e  ---.        jnp.
+00000b10: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+00000b20: 2020 2020 5468 6520 636f 6e66 6f72 6d61      The conforma
+00000b30: 6c20 696e 7465 7276 616c 732e 2054 6865  l intervals. The
+00000b40: 2074 776f 2063 6f6d 706f 6e65 6e74 7320   two components 
+00000b50: 6f66 2074 6865 2073 6563 6f6e 6420 6178  of the second ax
+00000b60: 6973 2063 6f72 7265 7370 6f6e 6420 746f  is correspond to
+00000b70: 2074 6865 206c 6566 7420 616e 6420 7269   the left and ri
+00000b80: 6768 7420 696e 7465 7276 616c 0a20 2020  ght interval.   
+00000b90: 2020 2020 2020 2020 2062 6f75 6e64 732e           bounds.
+00000ba0: 0a20 2020 2020 2020 207a 2d60 6372 6f73  .        z-`cros
+00000bb0: 735f 7661 6c5f 6f75 7470 7574 7360 206d  s_val_outputs` m
+00000bc0: 7573 7420 6265 2061 206c 6973 7420 6f66  ust be a list of
+00000bd0: 2061 7272 6179 732e 7a2d 6063 726f 7373   arrays.z-`cross
+00000be0: 5f76 616c 5f74 6172 6765 7473 6020 6d75  _val_targets` mu
+00000bf0: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
+00000c00: 6172 7261 7973 2e7a 2e60 6372 6f73 735f  arrays.z.`cross_
+00000c10: 7465 7374 5f6f 7574 7075 7473 6020 6d75  test_outputs` mu
+00000c20: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
+00000c30: 6172 7261 7973 2e72 0100 0000 7a86 5468  arrays.r....z.Th
+00000c40: 6520 6669 7273 7420 6469 6d65 6e73 696f  e first dimensio
+00000c50: 6e20 6f66 2074 6865 2069 2d74 6820 656c  n of the i-th el
+00000c60: 656d 656e 7420 696e 2060 6372 6f73 735f  ement in `cross_
+00000c70: 7661 6c5f 6f75 7470 7574 7360 206d 7573  val_outputs` mus
+00000c80: 7420 6265 2074 6865 2073 616d 6520 6173  t be the same as
+00000c90: 2074 6865 206f 6e65 206f 6620 7468 6520   the one of the 
+00000ca0: 692d 7468 2065 6c65 6d65 6e74 2069 6e20  i-th element in 
+00000cb0: 6063 726f 7373 5f76 616c 5f74 6172 6765  `cross_val_targe
+00000cc0: 7473 602e e901 0000 004e 7a8c 5468 6973  ts`......Nz.This
+00000cd0: 206d 6574 686f 6420 6973 2073 7570 706f   method is suppo
+00000ce0: 7274 6564 206f 6e6c 7920 666f 7220 7363  rted only for sc
+00000cf0: 616c 6172 206d 6f64 656c 206f 7574 7075  alar model outpu
+00000d00: 7473 206f 6e6c 792e 2048 6f77 6576 6572  ts only. However
+00000d10: 2c20 616e 2065 6c65 6d65 6e74 206f 6620  , an element of 
+00000d20: 6063 726f 7373 5f76 616c 5f6f 7574 7075  `cross_val_outpu
+00000d30: 7473 6020 6861 7320 7365 636f 6e64 2064  ts` has second d
+00000d40: 696d 656e 7369 6f6e 2067 7265 6174 6572  imension greater
+00000d50: 2074 6861 6e20 312e 7a8a 5468 6973 206d   than 1.z.This m
+00000d60: 6574 686f 6420 6973 2073 7570 706f 7274  ethod is support
+00000d70: 6564 206f 6e6c 7920 666f 7220 7363 616c  ed only for scal
+00000d80: 6172 2074 6172 6765 7420 7661 7269 6162  ar target variab
+00000d90: 6c65 732e 2048 6f77 6576 6572 2c20 616e  les. However, an
+00000da0: 2065 6c65 6d65 6e74 206f 6620 6063 726f   element of `cro
+00000db0: 7373 5f76 616c 5f74 6172 6765 7473 6020  ss_val_targets` 
+00000dc0: 6861 7320 7365 636f 6e64 2064 696d 656e  has second dimen
+00000dd0: 7369 6f6e 2067 7265 6174 6572 2074 6861  sion greater tha
+00000de0: 6e20 312e 7a8d 5468 6973 206d 6574 686f  n 1.z.This metho
+00000df0: 6420 6973 2073 7570 706f 7274 6564 206f  d is supported o
+00000e00: 6e6c 7920 666f 7220 7363 616c 6172 206d  nly for scalar m
+00000e10: 6f64 656c 206f 7574 7075 7473 206f 6e6c  odel outputs onl
+00000e20: 792e 2048 6f77 6576 6572 2c20 616e 2065  y. However, an e
+00000e30: 6c65 6d65 6e74 206f 6620 6063 726f 7373  lement of `cross
+00000e40: 5f74 6573 745f 6f75 7470 7574 7360 2068  _test_outputs` h
+00000e50: 6173 2073 6563 6f6e 6420 6469 6d65 6e73  as second dimens
+00000e60: 696f 6e20 6772 6561 7465 7220 7468 616e  ion greater than
+00000e70: 2031 2e63 0100 0000 0000 0000 0000 0000   1.c............
+00000e80: 0300 0000 0600 0000 5300 0000 731e 0000  ........S...s...
+00000e90: 0067 007c 005d 165c 027d 017d 0274 00a0  .g.|.].\.}.}.t..
+00000ea0: 017c 017c 0218 00a1 0191 0271 0453 00a9  .|.|.......q.S..
+00000eb0: 0029 02da 036a 6e70 da03 6162 7329 03da  .)...jnp..abs)..
+00000ec0: 022e 30da 0179 da02 6d75 720b 0000 0072  ..0..y..mur....r
+00000ed0: 0b00 0000 fa41 2f55 7365 7273 2f64 6574  .....A/Users/det
+00000ee0: 6f6d 6d61 2f61 7773 2d66 6f72 7475 6e61  omma/aws-fortuna
+00000ef0: 2f66 6f72 7475 6e61 2f63 6f6e 666f 726d  /fortuna/conform
+00000f00: 616c 2f72 6567 7265 7373 696f 6e2f 6376  al/regression/cv
+00000f10: 706c 7573 2e70 79da 0a3c 6c69 7374 636f  plus.py..<listco
+00000f20: 6d70 3e4b 0000 00f3 0000 0000 7a3f 4356  mp>K........z?CV
+00000f30: 506c 7573 436f 6e66 6f72 6d61 6c52 6567  PlusConformalReg
+00000f40: 7265 7373 6f72 2e63 6f6e 666f 726d 616c  ressor.conformal
+00000f50: 5f69 6e74 6572 7661 6c2e 3c6c 6f63 616c  _interval.<local
+00000f60: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00000f70: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00000f80: 0000 5300 0000 7328 0000 0067 007c 005d  ..S...s(...g.|.]
+00000f90: 205c 027d 017d 027c 0164 0019 007c 0264   \.}.}.|.d...|.d
+00000fa0: 0064 0085 0264 0066 0219 0018 0091 0271  .d...d.f.......q
+00000fb0: 0453 00a9 014e 720b 0000 00a9 0372 0e00  .S...Nr......r..
+00000fc0: 0000 7210 0000 00da 0272 6972 0b00 0000  ..r......rir....
+00000fd0: 720b 0000 0072 1100 0000 7212 0000 004c  r....r....r....L
+00000fe0: 0000 0072 1300 0000 6301 0000 0000 0000  ...r....c.......
+00000ff0: 0000 0000 0003 0000 0006 0000 0053 0000  .............S..
+00001000: 0073 2800 0000 6700 7c00 5d20 5c02 7d01  .s(...g.|.] \.}.
+00001010: 7d02 7c01 6400 1900 7c02 6400 6400 8502  }.|.d...|.d.d...
+00001020: 6400 6602 1900 1700 9102 7104 5300 7214  d.f.......q.S.r.
+00001030: 0000 0072 0b00 0000 7215 0000 0072 0b00  ...r....r....r..
+00001040: 0000 720b 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00001050: 004d 0000 0072 1300 0000 2902 da01 71da  .M...r....)...q.
+00001060: 0461 7869 73e9 0200 0000 290d da04 7479  .axis.....)...ty
+00001070: 7065 da04 6c69 7374 da09 5479 7065 4572  pe..list..TypeEr
+00001080: 726f 72da 0965 6e75 6d65 7261 7465 da03  ror..enumerate..
+00001090: 7a69 70da 0573 6861 7065 da0a 5661 6c75  zip..shape..Valu
+000010a0: 6545 7272 6f72 da04 6e64 696d 720c 0000  eError..ndimr...
+000010b0: 00da 0b63 6f6e 6361 7465 6e61 7465 da08  ...concatenate..
+000010c0: 7175 616e 7469 6c65 da05 6172 7261 79da  quantile..array.
+000010d0: 0773 7175 6565 7a65 290e da04 7365 6c66  .squeeze)...self
+000010e0: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+000010f0: 0800 0000 da01 6972 1000 0000 720f 0000  ......ir....r...
+00001100: 005a 076d 755f 7465 7374 da01 72da 046c  .Z.mu_test..r..l
+00001110: 6566 74da 0572 6967 6874 5a05 716c 6566  eft..rightZ.qlef
+00001120: 745a 0671 7269 6768 7472 0b00 0000 720b  tZ.qrightr....r.
+00001130: 0000 0072 1100 0000 da12 636f 6e66 6f72  ...r......confor
+00001140: 6d61 6c5f 696e 7465 7276 616c 0d00 0000  mal_interval....
+00001150: 733a 0000 0000 230c 0108 010c 0108 010c  s:....#.........
+00001160: 0108 011e 0114 0108 020a 0116 010e 0102  ................
+00001170: 0102 ff04 030a 0116 010e 0108 020c 0116  ................
+00001180: 010e 010a 0314 011c 011c 0210 0114 017a  ...............z
+00001190: 2b43 5650 6c75 7343 6f6e 666f 726d 616c  +CVPlusConformal
+000011a0: 5265 6772 6573 736f 722e 636f 6e66 6f72  Regressor.confor
+000011b0: 6d61 6c5f 696e 7465 7276 616c 4e29 0ada  mal_intervalN)..
+000011c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000011d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000011e0: 655f 5fda 075f 5f64 6f63 5f5f 7203 0000  e__..__doc__r...
+000011f0: 0072 0200 0000 da05 666c 6f61 7472 0c00  .r......floatr..
+00001200: 0000 da07 6e64 6172 7261 7972 2b00 0000  ....ndarrayr+...
+00001210: 720b 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+00001220: 1100 0000 7204 0000 0006 0000 0073 0e00  ....r........s..
+00001230: 0000 0801 0408 0601 0601 0601 0201 04fa  ................
+00001240: 7204 0000 0029 08da 096a 6178 2e6e 756d  r....)...jax.num
+00001250: 7079 da05 6e75 6d70 7972 0c00 0000 da0e  py..numpyr......
+00001260: 666f 7274 756e 612e 7479 7069 6e67 7202  fortuna.typingr.
+00001270: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
+00001280: 7204 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+00001290: 0b00 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
+000012a0: 6c65 3e01 0000 0073 0600 0000 0c01 0c01  le>....s........
+000012b0: 0c03                                     ..
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/jackknife_minmax.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/jackknife_minmax.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 15:12:04 2023 UTC, .py size: 3845 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 443a b863 050f 0000  a.......D:.c....
+00000000: 610d 0d0a 0000 0000 79bd c663 050f 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 8302 5a05 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da05 4172 7261 7963 0000 0000 0000  )...Arrayc......
 00000070: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/jackknifeplus.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/jackknifeplus.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 15:12:14 2023 UTC, .py size: 3837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 4e3a b863 fd0e 0000  a.......N:.c....
+00000000: 610d 0d0a 0000 0000 79bd c663 fd0e 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 8302 5a05 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da05 4172 7261 7963 0000 0000 0000  )...Arrayc......
 00000070: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/onedim_uncertainty.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/onedim_uncertainty.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 11:06:28 2023 UTC, .py size: 5993 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b400 b863 6917 0000  a..........ci...
+00000000: 610d 0d0a 0000 0000 79bd c663 6917 0000  a.......y..ci...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a07  ..G.d.d...d...Z.
 00000060: 6402 5300 2906 e900 0000 0029 01da 084f  d.S.)......)...O
 00000070: 7074 696f 6e61 6c4e 2901 da05 4172 7261  ptionalN)...Arra
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/__pycache__/quantile.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/conformal/regression/__pycache__/quantile.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 11:05:55 2023 UTC, .py size: 7050 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9300 b863 8a1b 0000  a..........c....
+00000000: 610d 0d0a 0000 0000 79bd c663 8a1b 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a07  ..G.d.d...d...Z.
 00000060: 6402 5300 2906 e900 0000 0029 01da 084f  d.S.)......)...O
 00000070: 7074 696f 6e61 6c4e 2901 da05 4172 7261  ptionalN)...Arra
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/cvplus.py` & `aws_fortuna-0.1.9/fortuna/conformal/regression/cvplus.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,12 @@
                 cross_test_outputs[i] = mu_test[:, None]
             elif mu_test.shape[1] != 1:
                 raise ValueError("This method is supported only for scalar model outputs only. However, an element of "
                                  "`cross_test_outputs` has second dimension greater than 1.")
 
         r = [jnp.abs(y - mu) for y, mu in zip(cross_val_targets, cross_val_outputs)]
         left = jnp.concatenate([mu[None] - ri[:, None] for mu, ri in zip(cross_test_outputs, r)], 0)
-        right = jnp.concatenate([mu[None] + ri[:, None] for mu, ri in zip(cross_test_outputs, r)])
+        right = jnp.concatenate([mu[None] + ri[:, None] for mu, ri in zip(cross_test_outputs, r)], 0)
 
         qleft = jnp.quantile(left, q=error, axis=0)
         qright = jnp.quantile(right, q=1 - error, axis=0)
         return jnp.array(list(zip(qleft, qright))).squeeze(2)
```

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/jackknife_minmax.py` & `aws_fortuna-0.1.9/fortuna/conformal/regression/jackknife_minmax.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/jackknifeplus.py` & `aws_fortuna-0.1.9/fortuna/conformal/regression/jackknifeplus.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/onedim_uncertainty.py` & `aws_fortuna-0.1.9/fortuna/conformal/regression/onedim_uncertainty.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/conformal/regression/quantile.py` & `aws_fortuna-0.1.9/fortuna/conformal/regression/quantile.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/data/.DS_Store` & `aws_fortuna-0.1.9/fortuna/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/data/__pycache__/loader.cpython-311.pyc` & `aws_fortuna-0.1.9/fortuna/data/__pycache__/loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/data/__pycache__/loader.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/data/__pycache__/loader.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Dec 31 17:01:08 2022 UTC, .py size: 26663 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d46a b063 2768 0000  a........j.c'h..
+00000000: 610d 0d0a 0000 0000 79bd c663 2768 0000  a.......y..c'h..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0173 e801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a07 6400 6403 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a09 6400 6404 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
@@ -1135,15 +1135,15 @@
 000046e0: 0000 0000 0003 0000 0040 0000 0173 2200  .........@...s".
 000046f0: 0000 6500 5a01 6400 5a02 6401 6402 9c01  ..e.Z.d.Z.d.d...
 00004700: 6403 6404 8404 5a03 6405 6406 8400 5a04  d.d...Z.d.d...Z.
 00004710: 6407 5300 2908 7226 0000 0072 2300 0000  d.S.).r&...r#...
 00004720: a901 7225 0000 0063 0200 0000 0000 0000  ..r%...c........
 00004730: 0000 0000 0200 0000 0200 0000 4300 0001  ............C...
 00004740: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
-00004750: 1500 0000 a901 da04 5f66 756e a902 7211  ........_fun..r.
+00004750: 1500 0000 a901 5a04 5f66 756e a902 7211  ......Z._fun..r.
 00004760: 0000 0072 2500 0000 7212 0000 0072 1200  ...r%...r....r..
 00004770: 0000 7213 0000 0072 1400 0000 4a02 0000  ..r....r....J...
 00004780: 7302 0000 0000 037a 2946 726f 6d43 616c  s......z)FromCal
 00004790: 6c61 626c 6549 7465 7261 626c 6554 6f44  lableIterableToD
 000047a0: 6174 614c 6f61 6465 722e 5f5f 696e 6974  ataLoader.__init
 000047b0: 5f5f 6301 0000 0000 0000 0000 0000 0003  __c.............
 000047c0: 0000 0002 0000 004f 0000 0173 0800 0000  .......O...s....
@@ -1161,23 +1161,23 @@
 00004880: 0000 0040 0000 0173 2200 0000 6500 5a01  ...@...s"...e.Z.
 00004890: 6400 5a02 6401 6402 9c01 6403 6404 8404  d.Z.d.d...d.d...
 000048a0: 5a03 6405 6406 8400 5a04 6407 5300 2908  Z.d.d...Z.d.S.).
 000048b0: 725c 0000 0072 5b00 0000 728d 0000 0063  r\...r[...r....c
 000048c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 000048d0: 0200 0000 4300 0001 730a 0000 007c 017c  ....C...s....|.|
 000048e0: 005f 0064 0053 0072 1500 0000 728e 0000  ._.d.S.r....r...
-000048f0: 0072 9000 0000 7212 0000 0072 1200 0000  .r....r....r....
+000048f0: 0072 8f00 0000 7212 0000 0072 1200 0000  .r....r....r....
 00004900: 7213 0000 0072 1400 0000 5402 0000 7302  r....r....T...s.
 00004910: 0000 0000 037a 2b46 726f 6d43 616c 6c61  .....z+FromCalla
 00004920: 626c 6549 7465 7261 626c 6554 6f49 6e70  bleIterableToInp
 00004930: 7574 734c 6f61 6465 722e 5f5f 696e 6974  utsLoader.__init
 00004940: 5f5f 6301 0000 0000 0000 0000 0000 0003  __c.............
 00004950: 0000 0002 0000 004f 0000 0173 0800 0000  .......O...s....
 00004960: 7c00 a000 a100 5300 7215 0000 0072 8e00  |.....S.r....r..
-00004970: 0000 7291 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00004970: 0000 7290 0000 0072 1200 0000 7212 0000  ..r....r....r...
 00004980: 0072 1300 0000 7273 0000 0059 0200 0073  .r....rs...Y...s
 00004990: 0200 0000 0001 7a2b 4672 6f6d 4361 6c6c  ......z+FromCall
 000049a0: 6162 6c65 4974 6572 6162 6c65 546f 496e  ableIterableToIn
 000049b0: 7075 7473 4c6f 6164 6572 2e5f 5f63 616c  putsLoader.__cal
 000049c0: 6c5f 5f4e 7274 0000 0072 1200 0000 7212  l__Nrt...r....r.
 000049d0: 0000 0072 1200 0000 7213 0000 0072 5c00  ...r....r....r\.
 000049e0: 0000 5302 0000 7304 0000 0008 010e 0572  ..S...s........r
@@ -1185,23 +1185,23 @@
 00004a00: 0000 0000 0003 0000 0040 0000 0173 2200  .........@...s".
 00004a10: 0000 6500 5a01 6400 5a02 6401 6402 9c01  ..e.Z.d.Z.d.d...
 00004a20: 6403 6404 8404 5a03 6405 6406 8400 5a04  d.d...Z.d.d...Z.
 00004a30: 6407 5300 2908 726a 0000 0072 5b00 0000  d.S.).rj...r[...
 00004a40: 728d 0000 0063 0200 0000 0000 0000 0000  r....c..........
 00004a50: 0000 0200 0000 0200 0000 4300 0001 730a  ..........C...s.
 00004a60: 0000 007c 017c 005f 0064 0053 0072 1500  ...|.|._.d.S.r..
-00004a70: 0000 728e 0000 0072 9000 0000 7212 0000  ..r....r....r...
+00004a70: 0000 728e 0000 0072 8f00 0000 7212 0000  ..r....r....r...
 00004a80: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
 00004a90: 5e02 0000 7302 0000 0000 037a 2c46 726f  ^...s......z,Fro
 00004aa0: 6d43 616c 6c61 626c 6549 7465 7261 626c  mCallableIterabl
 00004ab0: 6554 6f54 6172 6765 7473 4c6f 6164 6572  eToTargetsLoader
 00004ac0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
 00004ad0: 0000 0000 0000 0300 0000 0200 0000 4f00  ..............O.
 00004ae0: 0001 7308 0000 007c 00a0 00a1 0053 0072  ..s....|.....S.r
-00004af0: 1500 0000 728e 0000 0072 9100 0000 7212  ....r....r....r.
+00004af0: 1500 0000 728e 0000 0072 9000 0000 7212  ....r....r....r.
 00004b00: 0000 0072 1200 0000 7213 0000 0072 7300  ...r....r....rs.
 00004b10: 0000 6302 0000 7302 0000 0000 017a 2c46  ..c...s......z,F
 00004b20: 726f 6d43 616c 6c61 626c 6549 7465 7261  romCallableItera
 00004b30: 626c 6554 6f54 6172 6765 7473 4c6f 6164  bleToTargetsLoad
 00004b40: 6572 2e5f 5f63 616c 6c5f 5f4e 7274 0000  er.__call__Nrt..
 00004b50: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
 00004b60: 7213 0000 0072 6a00 0000 5d02 0000 7304  r....rj...]...s.
@@ -1211,23 +1211,23 @@
 00004ba0: 5a02 6401 6402 9c01 6403 6404 8404 5a03  Z.d.d...d.d...Z.
 00004bb0: 6405 6406 8400 5a04 6407 5300 2908 722c  d.d...Z.d.S.).r,
 00004bc0: 0000 0072 2900 0000 2901 da0c 6261 7463  ...r)...)...batc
 00004bd0: 6865 645f 6461 7461 6302 0000 0000 0000  hed_datac.......
 00004be0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00004bf0: 0173 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
 00004c00: 7215 0000 00a9 015a 0d5f 6261 7463 6865  r......Z._batche
-00004c10: 645f 6461 7461 2902 7211 0000 0072 9200  d_data).r....r..
+00004c10: 645f 6461 7461 2902 7211 0000 0072 9100  d_data).r....r..
 00004c20: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
 00004c30: 0072 1400 0000 6802 0000 7302 0000 0000  .r....h...s.....
 00004c40: 037a 2146 726f 6d49 7465 7261 626c 6554  .z!FromIterableT
 00004c50: 6f44 6174 614c 6f61 6465 722e 5f5f 696e  oDataLoader.__in
 00004c60: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
 00004c70: 0003 0000 0001 0000 004f 0000 0173 0600  .........O...s..
-00004c80: 0000 7c00 6a00 5300 7215 0000 0072 9300  ..|.j.S.r....r..
-00004c90: 0000 7291 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00004c80: 0000 7c00 6a00 5300 7215 0000 0072 9200  ..|.j.S.r....r..
+00004c90: 0000 7290 0000 0072 1200 0000 7212 0000  ..r....r....r...
 00004ca0: 0072 1300 0000 7273 0000 006d 0200 0073  .r....rs...m...s
 00004cb0: 0200 0000 0001 7a21 4672 6f6d 4974 6572  ......z!FromIter
 00004cc0: 6162 6c65 546f 4461 7461 4c6f 6164 6572  ableToDataLoader
 00004cd0: 2e5f 5f63 616c 6c5f 5f4e 7274 0000 0072  .__call__Nrt...r
 00004ce0: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
 00004cf0: 0000 0072 2c00 0000 6702 0000 7304 0000  ...r,...g...s...
 00004d00: 0008 010e 0572 2c00 0000 6300 0000 0000  .....r,...c.....
@@ -1237,22 +1237,22 @@
 00004d40: 6406 8400 5a04 6407 5300 2908 725e 0000  d...Z.d.S.).r^..
 00004d50: 0072 5d00 0000 2901 da0e 6261 7463 6865  .r]...)...batche
 00004d60: 645f 696e 7075 7473 6302 0000 0000 0000  d_inputsc.......
 00004d70: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00004d80: 0173 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
 00004d90: 7215 0000 00a9 015a 0f5f 6261 7463 6865  r......Z._batche
 00004da0: 645f 696e 7075 7473 2902 7211 0000 0072  d_inputs).r....r
-00004db0: 9400 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00004db0: 9300 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
 00004dc0: 0000 0072 1400 0000 7202 0000 7302 0000  ...r....r...s...
 00004dd0: 0000 037a 2346 726f 6d49 7465 7261 626c  ...z#FromIterabl
 00004de0: 6554 6f49 6e70 7574 734c 6f61 6465 722e  eToInputsLoader.
 00004df0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
 00004e00: 0000 0000 0003 0000 0001 0000 004f 0000  .............O..
 00004e10: 0173 0600 0000 7c00 6a00 5300 7215 0000  .s....|.j.S.r...
-00004e20: 0072 9500 0000 7291 0000 0072 1200 0000  .r....r....r....
+00004e20: 0072 9400 0000 7290 0000 0072 1200 0000  .r....r....r....
 00004e30: 7212 0000 0072 1300 0000 7273 0000 0077  r....r....rs...w
 00004e40: 0200 0073 0200 0000 0001 7a23 4672 6f6d  ...s......z#From
 00004e50: 4974 6572 6162 6c65 546f 496e 7075 7473  IterableToInputs
 00004e60: 4c6f 6164 6572 2e5f 5f63 616c 6c5f 5f4e  Loader.__call__N
 00004e70: 7274 0000 0072 1200 0000 7212 0000 0072  rt...r....r....r
 00004e80: 1200 0000 7213 0000 0072 5e00 0000 7102  ....r....r^...q.
 00004e90: 0000 7304 0000 0008 010e 0572 5e00 0000  ..s........r^...
@@ -1262,23 +1262,23 @@
 00004ed0: 8404 5a03 6405 6406 8400 5a04 6407 5300  ..Z.d.d...Z.d.S.
 00004ee0: 2908 726b 0000 0072 5d00 0000 2901 da0f  ).rk...r]...)...
 00004ef0: 6261 7463 6865 645f 7461 7267 6574 7363  batched_targetsc
 00004f00: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 00004f10: 0200 0000 4300 0001 730a 0000 007c 017c  ....C...s....|.|
 00004f20: 005f 0064 0053 0072 1500 0000 a901 5a10  ._.d.S.r......Z.
 00004f30: 5f62 6174 6368 6564 5f74 6172 6765 7473  _batched_targets
-00004f40: 2902 7211 0000 0072 9600 0000 7212 0000  ).r....r....r...
+00004f40: 2902 7211 0000 0072 9500 0000 7212 0000  ).r....r....r...
 00004f50: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
 00004f60: 7c02 0000 7302 0000 0000 037a 2446 726f  |...s......z$Fro
 00004f70: 6d49 7465 7261 626c 6554 6f54 6172 6765  mIterableToTarge
 00004f80: 7473 4c6f 6164 6572 2e5f 5f69 6e69 745f  tsLoader.__init_
 00004f90: 5f63 0100 0000 0000 0000 0000 0000 0300  _c..............
 00004fa0: 0000 0100 0000 4f00 0001 7306 0000 007c  ......O...s....|
-00004fb0: 006a 0053 0072 1500 0000 7297 0000 0072  .j.S.r....r....r
-00004fc0: 9100 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00004fb0: 006a 0053 0072 1500 0000 7296 0000 0072  .j.S.r....r....r
+00004fc0: 9000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
 00004fd0: 0000 0072 7300 0000 8102 0000 7302 0000  ...rs.......s...
 00004fe0: 0000 017a 2446 726f 6d49 7465 7261 626c  ...z$FromIterabl
 00004ff0: 6554 6f54 6172 6765 7473 4c6f 6164 6572  eToTargetsLoader
 00005000: 2e5f 5f63 616c 6c5f 5f4e 7274 0000 0072  .__call__Nrt...r
 00005010: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
 00005020: 0000 0072 6b00 0000 7b02 0000 7304 0000  ...rk...{...s...
 00005030: 0008 010e 0572 6b00 0000 6300 0000 0000  .....rk...c.....
@@ -1296,15 +1296,15 @@
 000050f0: 6f72 466c 6f77 4461 7461 4c6f 6164 6572  orFlowDataLoader
 00005100: 546f 4461 7461 4c6f 6164 6572 2e5f 5f69  ToDataLoader.__i
 00005110: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
 00005120: 0000 0500 0000 0400 0000 6f00 0001 7326  ..........o...s&
 00005130: 0000 007c 006a 0044 005d 1a5c 027d 037d  ...|.j.D.].\.}.}
 00005140: 047c 03a0 01a1 007c 04a0 01a1 0066 0256  .|.....|.....f.V
 00005150: 0001 0071 0664 0053 0072 1500 0000 2902  ...q.d.S.r....).
-00005160: 7298 0000 00da 056e 756d 7079 a905 7211  r......numpy..r.
+00005160: 7297 0000 00da 056e 756d 7079 a905 7211  r......numpy..r.
 00005170: 0000 0072 7000 0000 7271 0000 0072 3c00  ...rp...rq...r<.
 00005180: 0000 723d 0000 0072 1200 0000 7212 0000  ..r=...r....r...
 00005190: 0072 1300 0000 7273 0000 0089 0200 0073  .r....rs.......s
 000051a0: 0400 0000 0001 0e01 7a2d 4672 6f6d 5465  ........z-FromTe
 000051b0: 6e73 6f72 466c 6f77 4461 7461 4c6f 6164  nsorFlowDataLoad
 000051c0: 6572 546f 4461 7461 4c6f 6164 6572 2e5f  erToDataLoader._
 000051d0: 5f63 616c 6c5f 5f4e 7274 0000 0072 1200  _call__Nrt...r..
@@ -1324,16 +1324,16 @@
 000052b0: 7302 0000 0000 017a 2846 726f 6d54 6f72  s......z(FromTor
 000052c0: 6368 4461 7461 4c6f 6164 6572 546f 4461  chDataLoaderToDa
 000052d0: 7461 4c6f 6164 6572 2e5f 5f69 6e69 745f  taLoader.__init_
 000052e0: 5f63 0100 0000 0000 0000 0000 0000 0500  _c..............
 000052f0: 0000 0400 0000 6f00 0001 7326 0000 007c  ......o...s&...|
 00005300: 006a 0044 005d 1a5c 027d 037d 047c 03a0  .j.D.].\.}.}.|..
 00005310: 01a1 007c 04a0 01a1 0066 0256 0001 0071  ...|.....f.V...q
-00005320: 0664 0053 0072 1500 0000 2902 729b 0000  .d.S.r....).r...
-00005330: 0072 9900 0000 729a 0000 0072 1200 0000  .r....r....r....
+00005320: 0664 0053 0072 1500 0000 2902 729a 0000  .d.S.r....).r...
+00005330: 0072 9800 0000 7299 0000 0072 1200 0000  .r....r....r....
 00005340: 7212 0000 0072 1300 0000 7273 0000 0092  r....r....rs....
 00005350: 0200 0073 0400 0000 0001 0e01 7a28 4672  ...s........z(Fr
 00005360: 6f6d 546f 7263 6844 6174 614c 6f61 6465  omTorchDataLoade
 00005370: 7254 6f44 6174 614c 6f61 6465 722e 5f5f  rToDataLoader.__
 00005380: 6361 6c6c 5f5f 4e72 7400 0000 7212 0000  call__Nrt...r...
 00005390: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
 000053a0: 7234 0000 008e 0200 0073 0400 0000 0801  r4.......s......
@@ -1361,16 +1361,16 @@
 00005500: 3a00 0000 723c 0000 0072 3d00 0000 7212  :...r<...r=...r.
 00005510: 0000 0072 1200 0000 7213 0000 0072 7300  ...r....r....rs.
 00005520: 0000 9b02 0000 7308 0000 0000 0104 010e  ......s.........
 00005530: 010c 017a 2446 726f 6d44 6174 614c 6f61  ...z$FromDataLoa
 00005540: 6465 7254 6f41 7272 6179 496e 7075 7473  derToArrayInputs
 00005550: 2e5f 5f63 616c 6c5f 5f4e 7274 0000 0072  .__call__Nrt...r
 00005560: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00005570: 0000 0072 9c00 0000 9702 0000 7304 0000  ...r........s...
-00005580: 0008 010e 0372 9c00 0000 6300 0000 0000  .....r....c.....
+00005570: 0000 0072 9b00 0000 9702 0000 7304 0000  ...r........s...
+00005580: 0008 010e 0372 9b00 0000 6300 0000 0000  .....r....c.....
 00005590: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
 000055a0: 0000 0173 2200 0000 6500 5a01 6400 5a02  ...s"...e.Z.d.Z.
 000055b0: 6401 6402 9c01 6403 6404 8404 5a03 6405  d.d...d.d...Z.d.
 000055c0: 6406 8400 5a04 6407 5300 2908 da1c 4672  d...Z.d.S.)...Fr
 000055d0: 6f6d 4461 7461 4c6f 6164 6572 546f 4172  omDataLoaderToAr
 000055e0: 7261 7954 6172 6765 7473 720b 0000 0072  rayTargetsr....r
 000055f0: 0c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
@@ -1390,16 +1390,16 @@
 000056d0: 7100 0000 723b 0000 0072 3c00 0000 723d  q...r;...r<...r=
 000056e0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
 000056f0: 0000 7273 0000 00a6 0200 0073 0800 0000  ..rs.......s....
 00005700: 0001 0401 0e01 0c01 7a25 4672 6f6d 4461  ........z%FromDa
 00005710: 7461 4c6f 6164 6572 546f 4172 7261 7954  taLoaderToArrayT
 00005720: 6172 6765 7473 2e5f 5f63 616c 6c5f 5f4e  argets.__call__N
 00005730: 7274 0000 0072 1200 0000 7212 0000 0072  rt...r....r....r
-00005740: 1200 0000 7213 0000 0072 9d00 0000 a202  ....r....r......
-00005750: 0000 7304 0000 0008 010e 0372 9d00 0000  ..s........r....
+00005740: 1200 0000 7213 0000 0072 9c00 0000 a202  ....r....r......
+00005750: 0000 7304 0000 0008 010e 0372 9c00 0000  ..s........r....
 00005760: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00005770: 0003 0000 0040 0000 0173 2200 0000 6500  .....@...s"...e.
 00005780: 5a01 6400 5a02 6401 6402 9c01 6403 6404  Z.d.Z.d.d...d.d.
 00005790: 8404 5a03 6405 6406 8400 5a04 6407 5300  ..Z.d.d...Z.d.S.
 000057a0: 2908 da1d 4672 6f6d 496e 7075 7473 4c6f  )...FromInputsLo
 000057b0: 6164 6572 546f 4172 7261 7949 6e70 7574  aderToArrayInput
 000057c0: 7372 4200 0000 7250 0000 0063 0200 0000  srB...rP...c....
@@ -1419,16 +1419,16 @@
 000058a0: 0000 0072 7100 0000 723a 0000 0072 3c00  ...rq...r:...r<.
 000058b0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
 000058c0: 0072 7300 0000 b102 0000 7308 0000 0000  .rs.......s.....
 000058d0: 0104 010a 010c 017a 2646 726f 6d49 6e70  .......z&FromInp
 000058e0: 7574 734c 6f61 6465 7254 6f41 7272 6179  utsLoaderToArray
 000058f0: 496e 7075 7473 2e5f 5f63 616c 6c5f 5f4e  Inputs.__call__N
 00005900: 7274 0000 0072 1200 0000 7212 0000 0072  rt...r....r....r
-00005910: 1200 0000 7213 0000 0072 9e00 0000 ad02  ....r....r......
-00005920: 0000 7304 0000 0008 010e 0372 9e00 0000  ..s........r....
+00005910: 1200 0000 7213 0000 0072 9d00 0000 ad02  ....r....r......
+00005920: 0000 7304 0000 0008 010e 0372 9d00 0000  ..s........r....
 00005930: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00005940: 0006 0000 0040 0000 0173 2a00 0000 6500  .....@...s*...e.
 00005950: 5a01 6400 5a02 640b 6403 6404 6405 6405  Z.d.Z.d.d.d.d.d.
 00005960: 6406 9c04 6407 6408 8405 5a03 6409 640a  d...d.d...Z.d.d.
 00005970: 8400 5a04 6401 5300 290c 7258 0000 004e  ..Z.d.S.).rX...N
 00005980: 4672 0900 0000 7218 0000 0072 1900 0000  Fr....r....r....
 00005990: 2904 723a 0000 0072 1b00 0000 721c 0000  ).r:...r....r...
@@ -1464,18 +1464,18 @@
 00005b70: 1200 0000 a901 7276 0000 00a9 0172 8300  ......rv.....r..
 00005b80: 0000 7212 0000 0072 1300 0000 7284 0000  ..r....r....r...
 00005b90: 00d3 0200 0073 0400 0000 0001 0801 7a38  .....s........z8
 00005ba0: 4672 6f6d 4172 7261 7949 6e70 7574 7354  FromArrayInputsT
 00005bb0: 6f49 6e70 7574 734c 6f61 6465 722e 5f5f  oInputsLoader.__
 00005bc0: 6361 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e  call__.<locals>.
 00005bd0: 6d61 6b65 5f67 656e 290b 727a 0000 0072  make_gen).rz...r
-00005be0: 3800 0000 7285 0000 0072 8600 0000 729f  8...r....r....r.
+00005be0: 3800 0000 7285 0000 0072 8600 0000 729e  8...r....r....r.
 00005bf0: 0000 0072 8700 0000 7279 0000 0072 8800  ...r....ry...r..
 00005c00: 0000 7289 0000 0072 7b00 0000 728a 0000  ..r....r{...r...
-00005c10: 0072 8b00 0000 7212 0000 0072 a100 0000  .r....r....r....
+00005c10: 0072 8b00 0000 7212 0000 0072 a000 0000  .r....r....r....
 00005c20: 7213 0000 0072 7300 0000 c502 0000 731a  r....rs.......s.
 00005c30: 0000 0000 0106 0106 0116 ff06 030a 010a  ................
 00005c40: 0204 0114 0118 0102 fd06 060c 047a 2646  .............z&F
 00005c50: 726f 6d41 7272 6179 496e 7075 7473 546f  romArrayInputsTo
 00005c60: 496e 7075 7473 4c6f 6164 6572 2e5f 5f63  InputsLoader.__c
 00005c70: 616c 6c5f 5f29 034e 4646 7274 0000 0072  all__).NFFrt...r
 00005c80: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
@@ -1520,15 +1520,15 @@
 00005ef0: e602 0000 7302 0000 0000 037a 2646 726f  ....s......z&Fro
 00005f00: 6d44 6174 614c 6f61 6465 7254 6f54 6172  mDataLoaderToTar
 00005f10: 6765 7473 4c6f 6164 6572 2e5f 5f69 6e69  getsLoader.__ini
 00005f20: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
 00005f30: 0500 0000 0300 0000 6f00 0001 731a 0000  ........o...s...
 00005f40: 007c 006a 0044 005d 0e5c 027d 037d 047c  .|.j.D.].\.}.}.|
 00005f50: 0456 0001 0071 0664 0053 0072 1500 0000  .V...q.d.S.r....
-00005f60: 720e 0000 0072 a200 0000 7212 0000 0072  r....r....r....r
+00005f60: 720e 0000 0072 a100 0000 7212 0000 0072  r....r....r....r
 00005f70: 1200 0000 7213 0000 0072 7300 0000 eb02  ....r....rs.....
 00005f80: 0000 7304 0000 0000 010e 017a 2646 726f  ..s........z&Fro
 00005f90: 6d44 6174 614c 6f61 6465 7254 6f54 6172  mDataLoaderToTar
 00005fa0: 6765 7473 4c6f 6164 6572 2e5f 5f63 616c  getsLoader.__cal
 00005fb0: 6c5f 5f4e 7274 0000 0072 1200 0000 7212  l__Nrt...r....r.
 00005fc0: 0000 0072 1200 0000 7213 0000 0072 6600  ...r....r....rf.
 00005fd0: 0000 e502 0000 7304 0000 0008 010e 0572  ......s........r
@@ -1556,16 +1556,16 @@
 00006130: 723b 0000 0072 3d00 0000 7212 0000 0072  r;...r=...r....r
 00006140: 1200 0000 7213 0000 0072 7300 0000 f402  ....r....rs.....
 00006150: 0000 7308 0000 0000 0104 010a 010c 017a  ..s............z
 00006160: 2846 726f 6d54 6172 6765 7473 4c6f 6164  (FromTargetsLoad
 00006170: 6572 546f 4172 7261 7954 6172 6765 7473  erToArrayTargets
 00006180: 2e5f 5f63 616c 6c5f 5f4e 7274 0000 0072  .__call__Nrt...r
 00006190: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-000061a0: 0000 0072 a300 0000 f002 0000 7304 0000  ...r........s...
-000061b0: 0008 010e 0372 a300 0000 6300 0000 0000  .....r....c.....
+000061a0: 0000 0072 a200 0000 f002 0000 7304 0000  ...r........s...
+000061b0: 0008 010e 0372 a200 0000 6300 0000 0000  .....r....c.....
 000061c0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
 000061d0: 0000 0173 2a00 0000 6500 5a01 6400 5a02  ...s*...e.Z.d.Z.
 000061e0: 640b 6403 6404 6405 6405 6406 9c04 6407  d.d.d.d.d.d...d.
 000061f0: 6408 8405 5a03 6409 640a 8400 5a04 6401  d...Z.d.d...Z.d.
 00006200: 5300 290c 7267 0000 004e 4672 0900 0000  S.).rg...NFr....
 00006210: 7218 0000 0072 1900 0000 2904 723b 0000  r....r....).r;..
 00006220: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
@@ -1594,25 +1594,25 @@
 00006390: 7d04 7c00 6a09 7290 740a 7c04 8300 8301  }.|.j.r.t.|.....
 000063a0: 6e04 7c04 8300 4500 6400 4800 0100 6400  n.|...E.d.H...d.
 000063b0: 5300 2907 4e72 0100 0000 4672 7c00 0000  S.).Nr....Fr|...
 000063c0: 727e 0000 0063 0000 0000 0000 0000 0000  r~...c..........
 000063d0: 0000 0100 0000 0200 0000 3300 0001 7314  ..........3...s.
 000063e0: 0000 0088 0044 005d 0a7d 007c 0056 0001  .....D.].}.|.V..
 000063f0: 0071 0464 0053 0072 1500 0000 7212 0000  .q.d.S.r....r...
-00006400: 0072 a000 0000 72a1 0000 0072 1200 0000  .r....r....r....
+00006400: 0072 9f00 0000 72a0 0000 0072 1200 0000  .r....r....r....
 00006410: 7213 0000 0072 8400 0000 1603 0000 7304  r....r........s.
 00006420: 0000 0000 0108 017a 3a46 726f 6d41 7272  .......z:FromArr
 00006430: 6179 5461 7267 6574 7354 6f54 6172 6765  ayTargetsToTarge
 00006440: 7473 4c6f 6164 6572 2e5f 5f63 616c 6c5f  tsLoader.__call_
 00006450: 5f2e 3c6c 6f63 616c 733e 2e6d 616b 655f  _.<locals>.make_
 00006460: 6765 6e29 0b72 7a00 0000 7238 0000 0072  gen).rz...r8...r
-00006470: 8500 0000 7286 0000 0072 a400 0000 7287  ....r....r....r.
+00006470: 8500 0000 7286 0000 0072 a300 0000 7287  ....r....r....r.
 00006480: 0000 0072 7900 0000 7288 0000 0072 8900  ...ry...r....r..
 00006490: 0000 727b 0000 0072 8a00 0000 728b 0000  ..r{...r....r...
-000064a0: 0072 1200 0000 72a1 0000 0072 1300 0000  .r....r....r....
+000064a0: 0072 1200 0000 72a0 0000 0072 1300 0000  .r....r....r....
 000064b0: 7273 0000 0008 0300 0073 1a00 0000 0001  rs.......s......
 000064c0: 0601 0601 16ff 0603 0a01 0a02 0401 1401  ................
 000064d0: 1801 02fd 0606 0c04 7a28 4672 6f6d 4172  ........z(FromAr
 000064e0: 7261 7954 6172 6765 7473 546f 5461 7267  rayTargetsToTarg
 000064f0: 6574 734c 6f61 6465 722e 5f5f 6361 6c6c  etsLoader.__call
 00006500: 5f5f 2903 4e46 4672 7400 0000 7212 0000  __).NFFrt...r...
 00006510: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
@@ -1641,32 +1641,32 @@
 00006680: 7213 0000 0072 1700 0000 2303 0000 7302  r....r....#...s.
 00006690: 0000 0000 017a 1c50 7265 6665 7463 6865  .....z.Prefetche
 000066a0: 6447 656e 6572 6174 6f72 2e5f 5f69 7465  dGenerator.__ite
 000066b0: 725f 5f63 0100 0000 0000 0000 0000 0000  r__c............
 000066c0: 0100 0000 0200 0000 4300 0001 731a 0000  ........C...s...
 000066d0: 007c 006a 0073 0e7c 00a0 01a1 0001 0064  .|.j.s.|.......d
 000066e0: 017c 005f 007c 006a 0253 0029 024e 4629  .|._.|.j.S.).NF)
-000066f0: 0372 a900 0000 727b 0000 0072 a700 0000  .r....r{...r....
+000066f0: 0372 a800 0000 727b 0000 0072 a600 0000  .r....r{...r....
 00006700: 7216 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00006710: 1300 0000 72a6 0000 0026 0300 0073 0800  ....r....&...s..
+00006710: 1300 0000 72a5 0000 0026 0300 0073 0800  ....r....&...s..
 00006720: 0000 0001 0601 0801 0601 7a1c 5072 6566  ..........z.Pref
 00006730: 6574 6368 6564 4765 6e65 7261 746f 722e  etchedGenerator.
 00006740: 5f5f 6e65 7874 5f5f 6301 0000 0000 0000  __next__c.......
 00006750: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
 00006760: 0173 1c00 0000 7c00 6a00 7318 7c00 6a01  .s....|.j.s.|.j.
 00006770: a002 a100 7c00 5f03 6401 7c00 5f00 6400  ....|._.d.|._.d.
-00006780: 5300 72a5 0000 0029 0472 a900 0000 72a8  S.r....).r....r.
-00006790: 0000 0072 a600 0000 72a7 0000 0072 1600  ...r....r....r..
+00006780: 5300 72a4 0000 0029 0472 a800 0000 72a7  S.r....).r....r.
+00006790: 0000 0072 a500 0000 72a6 0000 0072 1600  ...r....r....r..
 000067a0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
 000067b0: 0072 7b00 0000 2c03 0000 7306 0000 0000  .r{...,...s.....
 000067c0: 0106 010c 017a 1d50 7265 6665 7463 6865  .....z.Prefetche
 000067d0: 6447 656e 6572 6174 6f72 2e5f 7072 6566  dGenerator._pref
 000067e0: 6574 6368 4e29 0772 4c00 0000 724d 0000  etchN).rL...rM..
 000067f0: 0072 4e00 0000 7214 0000 0072 1700 0000  .rN...r....r....
-00006800: 72a6 0000 0072 7b00 0000 7212 0000 0072  r....r{...r....r
+00006800: 72a5 0000 0072 7b00 0000 7212 0000 0072  r....r{...r....r
 00006810: 1200 0000 7212 0000 0072 1300 0000 728a  ....r....r....r.
 00006820: 0000 001d 0300 0073 0800 0000 0801 0805  .......s........
 00006830: 0803 0806 728a 0000 0063 0000 0000 0000  ....r....c......
 00006840: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
 00006850: 0001 7324 0000 0065 005a 0164 005a 0264  ..s$...e.Z.d.Z.d
 00006860: 0164 0264 039c 0264 0464 0584 045a 0364  .d.d...d.d...Z.d
 00006870: 0664 0784 005a 0464 0853 0029 0972 4a00  .d...Z.d.S.).rJ.
@@ -1684,15 +1684,15 @@
 00006930: 0600 0000 0500 0000 6f00 0001 7356 0000  ........o...sV..
 00006940: 007c 006a 0044 005d 4a5c 027d 037d 047c  .|.j.D.]J\.}.}.|
 00006950: 046a 0164 0119 007c 006a 0216 007d 057c  .j.d...|.j...}.|
 00006960: 0564 016b 0272 327c 037c 0466 0256 0001  .d.k.r2|.|.f.V..
 00006970: 0071 067c 0364 007c 050b 0085 0219 007c  .q.|.d.|.......|
 00006980: 0464 007c 050b 0085 0219 0066 0256 0001  .d.|.......f.V..
 00006990: 0071 0664 0053 0072 6f00 0000 2903 720f  .q.d.S.ro...).r.
-000069a0: 0000 0072 8700 0000 72ab 0000 0029 0672  ...r....r....).r
+000069a0: 0000 0072 8700 0000 72aa 0000 0029 0672  ...r....r....).r
 000069b0: 1100 0000 7270 0000 0072 7100 0000 723a  ....rp...rq...r:
 000069c0: 0000 0072 3b00 0000 da08 7265 6d69 6e64  ...r;.....remind
 000069d0: 6572 7212 0000 0072 1200 0000 7213 0000  err....r....r...
 000069e0: 0072 7300 0000 3703 0000 730a 0000 0000  .rs...7...s.....
 000069f0: 010e 0110 0108 010c 027a 1a43 686f 7070  .........z.Chopp
 00006a00: 6564 4461 7461 4c6f 6164 6572 2e5f 5f63  edDataLoader.__c
 00006a10: 616c 6c5f 5f4e 7274 0000 0072 1200 0000  all__Nrt...r....
@@ -1703,29 +1703,29 @@
 00006a60: 2400 0000 6500 5a01 6400 5a02 6401 6402  $...e.Z.d.Z.d.d.
 00006a70: 6403 9c02 6404 6405 8404 5a03 6406 6407  d...d.d...Z.d.d.
 00006a80: 8400 5a04 6408 5300 2909 7260 0000 0072  ..Z.d.S.).r`...r
 00006a90: 4200 0000 7247 0000 0072 5f00 0000 6303  B...rG...r_...c.
 00006aa0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
 00006ab0: 0000 0043 0000 0173 1000 0000 7c01 7c00  ...C...s....|.|.
 00006ac0: 5f00 7c02 7c00 5f01 6400 5300 7215 0000  _.|.|._.d.S.r...
-00006ad0: 0029 0272 5300 0000 72ab 0000 0029 0372  .).rS...r....).r
+00006ad0: 0029 0272 5300 0000 72aa 0000 0029 0372  .).rS...r....).r
 00006ae0: 1100 0000 7251 0000 0072 4800 0000 7212  ....rQ...rH...r.
 00006af0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
 00006b00: 0000 4103 0000 7304 0000 0000 0106 017a  ..A...s........z
 00006b10: 1c43 686f 7070 6564 496e 7075 7473 4c6f  .ChoppedInputsLo
 00006b20: 6164 6572 2e5f 5f69 6e69 745f 5f63 0100  ader.__init__c..
 00006b30: 0000 0000 0000 0000 0000 0500 0000 0400  ................
 00006b40: 0000 6f00 0001 7340 0000 007c 006a 0044  ..o...s@...|.j.D
 00006b50: 005d 347d 037c 036a 0164 0119 007c 006a  .]4}.|.j.d...|.j
 00006b60: 0216 007d 047c 0464 016b 0272 2a7c 0356  ...}.|.d.k.r*|.V
 00006b70: 0001 0071 067c 0364 007c 040b 0085 0219  ...q.|.d.|......
 00006b80: 0056 0001 0071 0664 0053 0072 6f00 0000  .V...q.d.S.ro...
-00006b90: 2903 7253 0000 0072 8700 0000 72ab 0000  ).rS...r....r...
+00006b90: 2903 7253 0000 0072 8700 0000 72aa 0000  ).rS...r....r...
 00006ba0: 0029 0572 1100 0000 7270 0000 0072 7100  .).r....rp...rq.
-00006bb0: 0000 723a 0000 0072 ac00 0000 7212 0000  ..r:...r....r...
+00006bb0: 0000 723a 0000 0072 ab00 0000 7212 0000  ..r:...r....r...
 00006bc0: 0072 1200 0000 7213 0000 0072 7300 0000  .r....r....rs...
 00006bd0: 4503 0000 730a 0000 0000 010a 0110 0108  E...s...........
 00006be0: 0108 027a 1c43 686f 7070 6564 496e 7075  ...z.ChoppedInpu
 00006bf0: 7473 4c6f 6164 6572 2e5f 5f63 616c 6c5f  tsLoader.__call_
 00006c00: 5f4e 7274 0000 0072 1200 0000 7212 0000  _Nrt...r....r...
 00006c10: 0072 1200 0000 7213 0000 0072 6000 0000  .r....r....r`...
 00006c20: 4003 0000 7304 0000 0008 0110 0472 6000  @...s........r`.
@@ -1734,29 +1734,29 @@
 00006c50: 6500 5a01 6400 5a02 6401 6402 6403 9c02  e.Z.d.Z.d.d.d...
 00006c60: 6404 6405 8404 5a03 6406 6407 8400 5a04  d.d...Z.d.d...Z.
 00006c70: 6408 5300 2909 726d 0000 0072 4500 0000  d.S.).rm...rE...
 00006c80: 7247 0000 0072 6c00 0000 6303 0000 0000  rG...rl...c.....
 00006c90: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
 00006ca0: 0000 0173 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
 00006cb0: 7c00 5f01 6400 5300 7215 0000 0029 0272  |._.d.S.r....).r
-00006cc0: 6400 0000 72ab 0000 0029 0372 1100 0000  d...r....).r....
+00006cc0: 6400 0000 72aa 0000 0029 0372 1100 0000  d...r....).r....
 00006cd0: 7262 0000 0072 4800 0000 7212 0000 0072  rb...rH...r....r
 00006ce0: 1200 0000 7213 0000 0072 1400 0000 4f03  ....r....r....O.
 00006cf0: 0000 7304 0000 0000 0106 017a 1d43 686f  ..s........z.Cho
 00006d00: 7070 6564 5461 7267 6574 734c 6f61 6465  ppedTargetsLoade
 00006d10: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
 00006d20: 0000 0000 0000 0005 0000 0004 0000 006f  ...............o
 00006d30: 0000 0173 4000 0000 7c00 6a00 4400 5d34  ...s@...|.j.D.]4
 00006d40: 7d03 7c03 6a01 6401 1900 7c00 6a02 1600  }.|.j.d...|.j...
 00006d50: 7d04 7c04 6401 6b02 722a 7c03 5600 0100  }.|.d.k.r*|.V...
 00006d60: 7106 7c03 6400 7c04 0b00 8502 1900 5600  q.|.d.|.......V.
 00006d70: 0100 7106 6400 5300 726f 0000 0029 0372  ..q.d.S.ro...).r
-00006d80: 6400 0000 7287 0000 0072 ab00 0000 2905  d...r....r....).
+00006d80: 6400 0000 7287 0000 0072 aa00 0000 2905  d...r....r....).
 00006d90: 7211 0000 0072 7000 0000 7271 0000 0072  r....rp...rq...r
-00006da0: 3b00 0000 72ac 0000 0072 1200 0000 7212  ;...r....r....r.
+00006da0: 3b00 0000 72ab 0000 0072 1200 0000 7212  ;...r....r....r.
 00006db0: 0000 0072 1300 0000 7273 0000 0053 0300  ...r....rs...S..
 00006dc0: 0073 0a00 0000 0001 0a01 1001 0801 0802  .s..............
 00006dd0: 7a1d 4368 6f70 7065 6454 6172 6765 7473  z.ChoppedTargets
 00006de0: 4c6f 6164 6572 2e5f 5f63 616c 6c5f 5f4e  Loader.__call__N
 00006df0: 7274 0000 0072 1200 0000 7212 0000 0072  rt...r....r....r
 00006e00: 1200 0000 7213 0000 0072 6d00 0000 4e03  ....r....rm...N.
 00006e10: 0000 7304 0000 0008 0110 0472 6d00 0000  ..s........rm...
@@ -1791,15 +1791,15 @@
 00006fe0: 2061 7661 696c 6162 6c65 2064 6576 6963   available devic
 00006ff0: 6573 2e20 486f 7765 7665 722c 2061 2062  es. However, a b
 00007000: 6174 6368 2077 6974 6820 7368 6170 6520  atch with shape 
 00007010: fa31 2077 6173 2066 6f75 6e64 2e20 506c  .1 was found. Pl
 00007020: 6561 7365 2073 6574 2061 6e20 6170 7072  ease set an appr
 00007030: 6f70 7269 6174 6520 6261 7463 6820 7369  opriate batch si
 00007040: 7a65 2ee9 ffff ffff 7280 0000 00a9 05da  ze......r.......
-00007050: 036a 6178 da12 6c6f 6361 6c5f 6465 7669  .jax..local_devi
+00007050: 036a 6178 5a12 6c6f 6361 6c5f 6465 7669  .jaxZ.local_devi
 00007060: 6365 5f63 6f75 6e74 7287 0000 00da 0a56  ce_countr......V
 00007070: 616c 7565 4572 726f 72da 0772 6573 6861  alueError..resha
 00007080: 7065 2902 7272 0000 00da 096e 5f64 6576  pe).rr.....n_dev
 00007090: 6963 6573 7212 0000 0072 1200 0000 7213  icesr....r....r.
 000070a0: 0000 00da 0e5f 7265 7368 6170 655f 6261  ....._reshape_ba
 000070b0: 7463 6860 0300 0073 1000 0000 0002 0801  tch`...s........
 000070c0: 1201 0201 0801 08ff 06ff 0405 7a31 4465  ............z1De
@@ -1810,15 +1810,15 @@
 00007110: 0400 0000 2f00 0001 732e 0000 0074 0087  ..../...s....t..
 00007120: 0066 0164 0164 0284 0888 006a 0183 027d  .f.d.d.....j...}
 00007130: 0374 02a0 037c 0364 03a1 027d 037c 0345  .t...|.d...}.|.E
 00007140: 0064 0048 0001 0064 0053 0029 044e 6301  .d.H...d.S.).Nc.
 00007150: 0000 0000 0000 0000 0000 0001 0000 0003  ................
 00007160: 0000 0013 0000 0173 0c00 0000 7400 8800  .......s....t...
 00007170: 6a01 7c00 8302 5300 7215 0000 0029 0272  j.|...S.r....).r
-00007180: 0800 0000 72b6 0000 0029 0172 7200 0000  ....r....).rr...
+00007180: 0800 0000 72b4 0000 0029 0172 7200 0000  ....r....).rr...
 00007190: 7216 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
 000071a0: 083c 6c61 6d62 6461 3e6d 0300 00f3 0000  .<lambda>m......
 000071b0: 0000 7a3d 4465 7669 6365 4469 6d65 6e73  ..z=DeviceDimens
 000071c0: 696f 6e41 7567 6d65 6e74 6564 4461 7461  ionAugmentedData
 000071d0: 4c6f 6164 6572 2e5f 5f69 7465 725f 5f2e  Loader.__iter__.
 000071e0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
 000071f0: 3ee9 0200 0000 2904 da03 6d61 7072 0f00  >.....)...mapr..
@@ -1828,18 +1828,18 @@
 00007230: 0072 1200 0000 7216 0000 0072 1300 0000  .r....r....r....
 00007240: 7217 0000 006b 0300 0073 0a00 0000 0001  r....k...s......
 00007250: 0201 0eff 0403 0c01 7a2b 4465 7669 6365  ........z+Device
 00007260: 4469 6d65 6e73 696f 6e41 7567 6d65 6e74  DimensionAugment
 00007270: 6564 4461 7461 4c6f 6164 6572 2e5f 5f69  edDataLoader.__i
 00007280: 7465 725f 5f4e 2907 724c 0000 0072 4d00  ter__N).rL...rM.
 00007290: 0000 724e 0000 0072 1400 0000 da0c 7374  ..rN...r......st
-000072a0: 6174 6963 6d65 7468 6f64 72b6 0000 0072  aticmethodr....r
+000072a0: 6174 6963 6d65 7468 6f64 72b4 0000 0072  aticmethodr....r
 000072b0: 1700 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-000072c0: 0000 0072 1300 0000 72ad 0000 005c 0300  ...r....r....\..
-000072d0: 0073 0800 0000 0801 0e03 0201 0a0a 72ad  .s............r.
+000072c0: 0000 0072 1300 0000 72ac 0000 005c 0300  ...r....r....\..
+000072d0: 0073 0800 0000 0801 0e03 0201 0a0a 72ac  .s............r.
 000072e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 000072f0: 0000 0000 0300 0000 4000 0001 732e 0000  ........@...s...
 00007300: 0065 005a 0164 005a 0264 0164 029c 0164  .e.Z.d.Z.d.d...d
 00007310: 0364 0484 045a 0365 0464 0564 0684 0083  .d...Z.e.d.d....
 00007320: 015a 0564 0764 0884 005a 0664 0953 0029  .Z.d.d...Z.d.S.)
 00007330: 0ada 2444 6576 6963 6544 696d 656e 7369  ..$DeviceDimensi
 00007340: 6f6e 4175 676d 656e 7465 6449 6e70 7574  onAugmentedInput
@@ -1864,68 +1864,68 @@
 00007470: 6261 7463 6865 7320 6f66 2069 6e70 7574  batches of input
 00007480: 7320 6d75 7374 2062 6520 6120 6d75 6c74  s must be a mult
 00007490: 6970 6c65 206f 6620 7a51 2c20 7468 6174  iple of zQ, that
 000074a0: 2069 7320 7468 6520 6e75 6d62 6572 206f   is the number o
 000074b0: 6620 6176 6169 6c61 626c 6520 6465 7669  f available devi
 000074c0: 6365 732e 2048 6f77 6576 6572 2c20 6120  ces. However, a 
 000074d0: 6261 7463 6820 6f66 2069 6e70 7574 7320  batch of inputs 
-000074e0: 7769 7468 2073 6861 7065 2072 ae00 0000  with shape r....
-000074f0: 72af 0000 0072 8000 0000 72b0 0000 0029  r....r....r....)
-00007500: 0272 3a00 0000 72b5 0000 0072 1200 0000  .r:...r....r....
+000074e0: 7769 7468 2073 6861 7065 2072 ad00 0000  with shape r....
+000074f0: 72ae 0000 0072 8000 0000 72af 0000 0029  r....r....r....)
+00007500: 0272 3a00 0000 72b3 0000 0072 1200 0000  .r:...r....r....
 00007510: 7212 0000 0072 1300 0000 da0f 5f72 6573  r....r......_res
 00007520: 6861 7065 5f69 6e70 7574 7377 0300 0073  hape_inputsw...s
 00007530: 1000 0000 0002 0801 1201 0201 0801 08ff  ................
 00007540: 06ff 0405 7a34 4465 7669 6365 4469 6d65  ....z4DeviceDime
 00007550: 6e73 696f 6e41 7567 6d65 6e74 6564 496e  nsionAugmentedIn
 00007560: 7075 7473 4c6f 6164 6572 2e5f 7265 7368  putsLoader._resh
 00007570: 6170 655f 696e 7075 7473 6301 0000 0000  ape_inputsc.....
 00007580: 0000 0000 0000 0004 0000 0004 0000 002f  .............../
 00007590: 0000 0173 2e00 0000 7400 8700 6601 6401  ...s....t...f.d.
 000075a0: 6402 8408 8800 6a01 8302 7d03 7402 a003  d.....j...}.t...
 000075b0: 7c03 6403 a102 7d03 7c03 4500 6400 4800  |.d...}.|.E.d.H.
 000075c0: 0100 6400 5300 2904 4e63 0100 0000 0000  ..d.S.).Nc......
 000075d0: 0000 0000 0000 0100 0000 0300 0000 1300  ................
 000075e0: 0001 730a 0000 0088 00a0 007c 00a1 0153  ..s........|...S
-000075f0: 0072 1500 0000 2901 72be 0000 0029 0172  .r....).r....).r
+000075f0: 0072 1500 0000 2901 72bc 0000 0029 0172  .r....).r....).r
 00007600: 3a00 0000 7216 0000 0072 1200 0000 7213  :...r....r....r.
-00007610: 0000 0072 b700 0000 8403 0000 72b8 0000  ...r........r...
+00007610: 0000 0072 b500 0000 8403 0000 72b6 0000  ...r........r...
 00007620: 007a 3f44 6576 6963 6544 696d 656e 7369  .z?DeviceDimensi
 00007630: 6f6e 4175 676d 656e 7465 6449 6e70 7574  onAugmentedInput
 00007640: 734c 6f61 6465 722e 5f5f 6974 6572 5f5f  sLoader.__iter__
 00007650: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00007660: 613e 72b9 0000 0029 0472 ba00 0000 7253  a>r....).r....rS
-00007670: 0000 0072 0700 0000 72bb 0000 0029 0472  ...r....r....).r
+00007660: 613e 72b7 0000 0029 0472 b800 0000 7253  a>r....).r....rS
+00007670: 0000 0072 0700 0000 72b9 0000 0029 0472  ...r....r....).r
 00007680: 1100 0000 7270 0000 0072 7100 0000 7251  ....rp...rq...rQ
 00007690: 0000 0072 1200 0000 7216 0000 0072 1300  ...r....r....r..
 000076a0: 0000 7217 0000 0082 0300 0073 0a00 0000  ..r........s....
 000076b0: 0001 0201 0eff 0403 0c01 7a2d 4465 7669  ..........z-Devi
 000076c0: 6365 4469 6d65 6e73 696f 6e41 7567 6d65  ceDimensionAugme
 000076d0: 6e74 6564 496e 7075 7473 4c6f 6164 6572  ntedInputsLoader
 000076e0: 2e5f 5f69 7465 725f 5f4e 2907 724c 0000  .__iter__N).rL..
 000076f0: 0072 4d00 0000 724e 0000 0072 1400 0000  .rM...rN...r....
-00007700: 72bc 0000 0072 be00 0000 7217 0000 0072  r....r....r....r
+00007700: 72ba 0000 0072 bc00 0000 7217 0000 0072  r....r....r....r
 00007710: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00007720: 0000 0072 bd00 0000 7303 0000 7308 0000  ...r....s...s...
-00007730: 0008 010e 0302 010a 0a72 bd00 0000 292d  .........r....)-
+00007720: 0000 0072 bb00 0000 7303 0000 7308 0000  ...r....s...s...
+00007730: 0008 010e 0302 010a 0a72 bb00 0000 292d  .........r....)-
 00007740: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
 00007750: 00da 0674 7970 696e 6772 0300 0000 7204  ...typingr....r.
-00007760: 0000 0072 0500 0000 7206 0000 0072 b100  ...r....r....r..
-00007770: 0000 7299 0000 0072 3800 0000 da04 666c  ..r....r8.....fl
-00007780: 6178 7207 0000 00da 0d6a 6178 2e74 7265  axr......jax.tre
-00007790: 655f 7574 696c 7208 0000 00da 0e66 6f72  e_utilr......for
+00007760: 0000 0072 0500 0000 7206 0000 0072 b000  ...r....r....r..
+00007770: 0000 7298 0000 0072 3800 0000 5a04 666c  ..r....r8...Z.fl
+00007780: 6178 7207 0000 005a 0d6a 6178 2e74 7265  axr....Z.jax.tre
+00007790: 655f 7574 696c 7208 0000 005a 0e66 6f72  e_utilr....Z.for
 000077a0: 7475 6e61 2e74 7970 696e 6772 0900 0000  tuna.typingr....
 000077b0: 720a 0000 0072 0b00 0000 7242 0000 0072  r....r....rB...r
 000077c0: 4500 0000 726e 0000 0072 7500 0000 7220  E...rn...ru...r 
 000077d0: 0000 0072 2600 0000 725c 0000 0072 6a00  ...r&...r\...rj.
 000077e0: 0000 722c 0000 0072 5e00 0000 726b 0000  ..r,...r^...rk..
-000077f0: 0072 3100 0000 7234 0000 0072 9c00 0000  .r1...r4...r....
-00007800: 729d 0000 0072 9e00 0000 7258 0000 0072  r....r....rX...r
-00007810: 5600 0000 7266 0000 0072 a300 0000 7267  V...rf...r....rg
+000077f0: 0072 3100 0000 7234 0000 0072 9b00 0000  .r1...r4...r....
+00007800: 729c 0000 0072 9d00 0000 7258 0000 0072  r....r....rX...r
+00007810: 5600 0000 7266 0000 0072 a200 0000 7267  V...rf...r....rg
 00007820: 0000 0072 8a00 0000 724a 0000 0072 6000  ...r....rJ...r`.
-00007830: 0000 726d 0000 0072 ad00 0000 72bd 0000  ..rm...r....r...
+00007830: 0000 726d 0000 0072 ac00 0000 72bb 0000  ..rm...r....r...
 00007840: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
 00007850: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
 00007860: 0000 0073 4a00 0000 0c02 1802 0801 0801  ...sJ...........
 00007870: 0c01 0c02 1003 0e7f 0060 0e7f 0012 0e7f  .........`......
 00007880: 0012 0e0b 0e09 0e27 0e0a 0e0a 0e0a 0e0a  .......'........
 00007890: 0e0a 0e0a 0e09 0e09 0e0b 0e0b 0e0b 0e22  ..............."
 000078a0: 0e0b 0e0b 0e0b 0e22 0e15 0e0e 0e0e 0e0e  ......."........
```

### Comparing `aws_fortuna-0.1.8/fortuna/data/loader.py` & `aws_fortuna-0.1.9/fortuna/data/loader.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/distribution/.DS_Store` & `aws_fortuna-0.1.9/fortuna/distribution/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/distribution/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/distribution/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/distribution/__pycache__/gaussian.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/distribution/__pycache__/gaussian.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/distribution/gaussian.py` & `aws_fortuna-0.1.9/fortuna/distribution/gaussian.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/make_data.py` & `aws_fortuna-0.1.9/fortuna/make_data.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/metric/.DS_Store` & `aws_fortuna-0.1.9/fortuna/metric/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/metric/__pycache__/classification.cpython-311.pyc` & `aws_fortuna-0.1.9/fortuna/metric/__pycache__/classification.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/metric/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/metric/__pycache__/classification.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Dec 29 11:49:13 2022 UTC, .py size: 6597 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,424 +1,425 @@
-00000000: 610d 0d0a 0000 0000 b97e ad63 c519 0000  a........~.c....
+00000000: 610d 0d0a 0000 0000 9e29 d963 e119 0000  a........).c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
+00000020: 000a 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 5a06 6400  m.Z...d.d.l.Z.d.
 00000050: 6402 6c07 6d08 5a09 0100 6400 6403 6c0a  d.l.m.Z...d.d.l.
 00000060: 6d0b 5a0b 0100 6400 6404 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0e 6d0f 5a0f 0100 650f  ..d.d.l.m.Z...e.
 00000080: 650f 6509 6a10 6406 9c03 6407 6408 8404  e.e.j.d...d.d...
 00000090: 5a11 6418 650f 650f 650f 6512 6502 6501  Z.d.e.e.e.e.e.e.
 000000a0: 1900 6503 6509 6a10 6509 6a10 6509 6a10  ..e.e.j.e.j.e.j.
 000000b0: 6603 1900 640a 9c06 640b 640c 8405 5a13  f...d...d.d...Z.
 000000c0: 6419 650f 650f 650f 6512 6502 6501 1900  d.e.e.e.e.e.e...
 000000d0: 6509 6a10 640a 9c06 640d 640e 8405 5a14  e.j.d...d.d...Z.
 000000e0: 641a 650f 650f 650f 6512 6502 6501 1900  d.e.e.e.e.e.e...
-000000f0: 6515 640a 9c06 640f 6410 8405 5a16 641b  e.d...d.d...Z.d.
-00000100: 650f 650f 650f 6512 6502 6501 1900 6509  e.e.e.e.e.e...e.
-00000110: 6a10 640a 9c06 6411 6412 8405 5a17 641c  j.d...d.d...Z.d.
-00000120: 650f 650f 650f 6512 6502 6501 1900 6515  e.e.e.e.e.e...e.
-00000130: 640a 9c06 6413 6414 8405 5a18 650f 6504  d...d.d...Z.e.e.
-00000140: 650b 650f 6602 1900 6509 6a10 6415 9c03  e.e.f...e.j.d...
-00000150: 6416 6417 8404 5a19 6402 5300 291d e900  d.d...Z.d.S.)...
-00000160: 0000 0029 04da 0444 6963 74da 084f 7074  ...)...Dict..Opt
-00000170: 696f 6e61 6cda 0554 7570 6c65 da05 556e  ional..Tuple..Un
-00000180: 696f 6e4e 2901 da0d 5461 7267 6574 734c  ionN)...TargetsL
-00000190: 6f61 6465 7229 01da 1870 6c6f 745f 7265  oader)...plot_re
-000001a0: 6c69 6162 696c 6974 795f 6469 6167 7261  liability_diagra
-000001b0: 6d29 01da 0541 7272 6179 2903 da05 7072  m)...Array)...pr
-000001c0: 6564 73da 0774 6172 6765 7473 da06 7265  eds..targets..re
-000001d0: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
-000001e0: 0002 0000 0004 0000 0043 0000 0073 3200  .........C...s2.
-000001f0: 0000 7c00 6a00 6401 6b04 7212 7401 6402  ..|.j.d.k.r.t.d.
-00000200: 8301 8201 7c01 6a00 6401 6b04 7224 7401  ....|.j.d.k.r$t.
-00000210: 6403 8301 8201 7402 a003 7c00 7c01 6b02  d.....t...|.|.k.
-00000220: a101 5300 2904 6145 0100 000a 2020 2020  ..S.).aE....    
-00000230: 436f 6d70 7574 6520 7468 6520 6163 6375  Compute the accu
-00000240: 7261 6379 2067 6976 656e 2070 7265 6469  racy given predi
-00000250: 6374 696f 6e73 2061 6e64 2074 6172 6765  ctions and targe
-00000260: 7420 7661 7269 6162 6c65 732e 0a0a 2020  t variables...  
-00000270: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000280: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000290: 7072 6564 733a 2041 7272 6179 0a20 2020  preds: Array.   
-000002a0: 2020 2020 2041 206f 6e65 2d64 696d 656e       A one-dimen
-000002b0: 7369 6f6e 616c 2061 7272 6179 206f 6620  sional array of 
-000002c0: 7072 6564 6963 7469 6f6e 7320 6f76 6572  predictions over
-000002d0: 2074 6865 2064 6174 6120 706f 696e 7473   the data points
-000002e0: 2e0a 2020 2020 7461 7267 6574 733a 2041  ..    targets: A
-000002f0: 7272 6179 0a20 2020 2020 2020 2041 206f  rray.        A o
-00000300: 6e65 2d64 696d 656e 7369 6f6e 616c 2061  ne-dimensional a
-00000310: 7272 6179 206f 6620 7461 7267 6574 2076  rray of target v
-00000320: 6172 6961 626c 6573 2e0a 0a20 2020 2052  ariables...    R
-00000330: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00000340: 2d2d 0a20 2020 2066 6c6f 6174 0a20 2020  --.    float.   
-00000350: 2020 2020 2054 6865 2063 6f6d 7075 7465       The compute
-00000360: 6420 6163 6375 7261 6379 2e0a 2020 2020  d accuracy..    
-00000370: e901 0000 007a 3d60 7072 6564 7360 206d  .....z=`preds` m
-00000380: 7573 7420 6265 2061 206f 6e65 2d64 696d  ust be a one-dim
-00000390: 656e 7369 6f6e 616c 2061 7272 6179 206f  ensional array o
-000003a0: 6620 7072 6564 6963 7465 6420 636c 6173  f predicted clas
-000003b0: 7365 732e 7a3c 6074 6172 6765 7473 6020  ses.z<`targets` 
-000003c0: 6d75 7374 2062 6520 6120 6f6e 652d 6469  must be a one-di
-000003d0: 6d65 6e73 696f 6e61 6c20 6172 7261 7920  mensional array 
-000003e0: 6f66 2074 6172 6765 7420 636c 6173 7365  of target classe
-000003f0: 732e 2904 da04 6e64 696d da0a 5661 6c75  s.)...ndim..Valu
-00000400: 6545 7272 6f72 da03 6a6e 70da 046d 6561  eError..jnp..mea
-00000410: 6e29 0272 0900 0000 720a 0000 00a9 0072  n).r....r......r
-00000420: 1100 0000 fa3b 2f55 7365 7273 2f64 6574  .....;/Users/det
-00000430: 6f6d 6d61 2f61 7773 2d66 6f72 7475 6e61  omma/aws-fortuna
-00000440: 2f66 6f72 7475 6e61 2f6d 6574 7269 632f  /fortuna/metric/
-00000450: 636c 6173 7369 6669 6361 7469 6f6e 2e70  classification.p
-00000460: 79da 0861 6363 7572 6163 790b 0000 0073  y..accuracy....s
-00000470: 1200 0000 0010 0a01 0201 02ff 0403 0a01  ................
-00000480: 0201 02ff 0403 7213 0000 0046 2906 7209  ......r....F).r.
-00000490: 0000 00da 0570 726f 6273 720a 0000 00da  .....probsr.....
-000004a0: 0470 6c6f 74da 0c70 6c6f 745f 6f70 7469  .plot..plot_opti
-000004b0: 6f6e 7372 0b00 0000 6305 0000 0000 0000  onsr....c.......
-000004c0: 0000 0000 000a 0000 0006 0000 0003 0000  ................
-000004d0: 0073 f400 0000 8801 6a00 6401 6b03 7212  .s......j.d.k.r.
-000004e0: 7401 6402 8301 8201 7402 a003 6403 8801  t.d.....t...d...
-000004f0: 6a04 6403 1900 1b00 6403 6404 a103 8902  j.d.....d.d.....
-00000500: 8801 a005 6403 a101 8901 7402 a006 8801  ....d.....t.....
-00000510: a101 8901 7402 a007 8801 8802 6405 1900  ....t.......d...
-00000520: 6b01 a101 6405 1900 6701 7d05 7c05 8701  k...d...g.}.|...
-00000530: 8702 6602 6406 6407 8408 7408 6403 7409  ..f.d.d...t.d.t.
-00000540: 8802 8301 8302 4400 8301 3700 7d05 7402  ......D...7.}.t.
-00000550: a006 6408 6407 8400 7c05 4400 8301 a101  ..d.d...|.D.....
-00000560: 7d06 7c02 7c00 1800 8900 7402 a006 8700  }.|.|.....t.....
-00000570: 6601 6409 6407 8408 7c05 4400 8301 a101  f.d.d...|.D.....
-00000580: 7d07 7402 a006 8701 6601 640a 6407 8408  }.t.....f.d.d...
-00000590: 7c05 4400 8301 a101 7d08 7c03 72ea 7c08  |.D.....}.|.r.|.
-000005a0: 6405 6b03 7d09 740a 7c07 7c09 1900 7c08  d.k.}.t.|.|...|.
-000005b0: 7c09 1900 6602 6900 7c04 a401 8e01 0100  |...f.i.|.......
-000005c0: 7c06 7c08 7c07 6603 5300 290b 615a 0300  |.|.|.f.S.).aZ..
-000005d0: 000a 2020 2020 4269 6e20 7468 6520 636f  ..    Bin the co
-000005e0: 6e66 6964 656e 6365 2073 636f 7265 7320  nfidence scores 
-000005f0: 286d 6178 696d 756d 2070 726f 6261 6269  (maximum probabi
-00000600: 6c69 7479 2920 616e 6420 666f 7220 6561  lity) and for ea
-00000610: 6368 206f 6620 7468 656d 2063 6f6d 7075  ch of them compu
-00000620: 7465 3a0a 2020 2020 2020 2020 2d20 7468  te:.        - th
-00000630: 6520 6e75 6d62 6572 206f 6620 696e 7075  e number of inpu
-00000640: 7473 3b0a 2020 2020 2020 2020 2d20 7468  ts;.        - th
-00000650: 6520 6176 6572 6167 6520 636f 6e66 6964  e average confid
-00000660: 656e 6365 2073 636f 7265 2066 6f72 2065  ence score for e
-00000670: 6163 6820 6269 6e3b 0a20 2020 2020 2020  ach bin;.       
-00000680: 202d 2074 6865 2061 7665 7261 6765 2061   - the average a
-00000690: 6363 7572 6163 7920 6f76 6572 2065 6163  ccuracy over eac
-000006a0: 6820 6269 6e2e 0a0a 2020 2020 5061 7261  h bin...    Para
-000006b0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-000006c0: 2d2d 2d2d 2d0a 2020 2020 7072 6564 733a  -----.    preds:
-000006d0: 2041 7272 6179 0a20 2020 2020 2020 2041   Array.        A
-000006e0: 206f 6e65 2d64 696d 656e 7369 6f6e 616c   one-dimensional
-000006f0: 2061 7272 6179 206f 6620 7072 6564 6963   array of predic
-00000700: 7469 6f6e 7320 6f76 6572 2074 6865 2064  tions over the d
-00000710: 6174 6120 706f 696e 7473 2e0a 2020 2020  ata points..    
-00000720: 7072 6f62 733a 2041 7272 6179 0a20 2020  probs: Array.   
-00000730: 2020 2020 2041 2074 776f 2d64 696d 656e       A two-dimen
-00000740: 7369 6f6e 616c 2061 7272 6179 206f 6620  sional array of 
-00000750: 636c 6173 7320 7072 6f62 6162 696c 6974  class probabilit
-00000760: 6965 7320 666f 7220 6561 6368 2064 6174  ies for each dat
-00000770: 6120 706f 696e 742e 0a20 2020 2074 6172  a point..    tar
-00000780: 6765 7473 3a20 4172 7261 790a 2020 2020  gets: Array.    
-00000790: 2020 2020 4120 6f6e 652d 6469 6d65 6e73      A one-dimens
-000007a0: 696f 6e61 6c20 6172 7261 7920 6f66 2074  ional array of t
-000007b0: 6172 6765 7420 7661 7269 6162 6c65 732e  arget variables.
-000007c0: 0a20 2020 2070 6c6f 743a 2062 6f6f 6c0a  .    plot: bool.
-000007d0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-000007e0: 746f 2070 6c6f 7420 6120 7265 6c69 6162  to plot a reliab
-000007f0: 696c 6974 7920 6469 6167 7261 6d2e 0a20  ility diagram.. 
-00000800: 2020 2070 6c6f 745f 6f70 7469 6f6e 733a     plot_options:
-00000810: 2064 6963 740a 2020 2020 2020 2020 4f70   dict.        Op
-00000820: 7469 6f6e 7320 666f 7220 7468 6520 7265  tions for the re
-00000830: 6c69 6162 696c 6974 7920 6469 6167 7261  liability diagra
-00000840: 6d20 706c 6f74 3b20 7365 6520 3a66 756e  m plot; see :fun
-00000850: 633a 607e 666f 7274 756e 612e 706c 6f74  c:`~fortuna.plot
-00000860: 2e70 6c6f 745f 7265 6c69 6162 696c 6974  .plot_reliabilit
-00000870: 795f 6469 6167 7261 6d60 2e0a 0a20 2020  y_diagram`...   
-00000880: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-00000890: 2d2d 2d2d 0a20 2020 2054 7570 6c65 5b6a  ----.    Tuple[j
-000008a0: 6e70 2e6e 6461 7272 6179 2c20 6a6e 702e  np.ndarray, jnp.
-000008b0: 6e64 6172 7261 792c 206a 6e70 2e6e 6461  ndarray, jnp.nda
-000008c0: 7272 6179 5d0a 2020 2020 2020 2020 4e75  rray].        Nu
-000008d0: 6d62 6572 206f 6620 696e 7075 7473 2070  mber of inputs p
-000008e0: 6572 2062 696e 2c20 6176 6572 6167 6520  er bin, average 
-000008f0: 636f 6e66 6964 656e 6365 2073 636f 7265  confidence score
-00000900: 2070 6572 2062 696e 2061 6e64 2061 7665   per bin and ave
-00000910: 7261 6765 2061 6363 7572 6163 7920 7065  rage accuracy pe
-00000920: 7220 6269 6e2e 0a20 2020 20e9 0200 0000  r bin..    .....
-00000930: 7a28 6070 726f 6273 6020 6d75 7374 2062  z(`probs` must b
-00000940: 6520 6120 7477 6f2d 6469 6d65 6e73 696f  e a two-dimensio
-00000950: 6e61 6c20 6172 7261 792e 720c 0000 00e9  nal array.r.....
-00000960: 0a00 0000 7201 0000 0063 0100 0000 0000  ....r....c......
-00000970: 0000 0000 0000 0200 0000 0900 0000 1300  ................
-00000980: 0000 7332 0000 0067 007c 005d 2a7d 0174  ..s2...g.|.]*}.t
-00000990: 00a0 0188 0088 017c 0119 006b 0188 0088  .......|...k....
-000009a0: 017c 0164 0018 0019 006b 0440 00a1 0164  .|.d.....k.@...d
-000009b0: 0119 0091 0271 0453 0029 0272 0c00 0000  .....q.S.).r....
-000009c0: 7201 0000 0029 0272 0f00 0000 da05 7768  r....).r......wh
-000009d0: 6572 6529 02da 022e 30da 0169 2902 7214  ere)....0..i).r.
-000009e0: 0000 00da 0a74 6872 6573 686f 6c64 7372  .....thresholdsr
-000009f0: 1100 0000 7212 0000 00da 0a3c 6c69 7374  ....r......<list
-00000a00: 636f 6d70 3e4b 0000 0073 0400 0000 0602  comp>K...s......
-00000a10: 02ff 7a2d 636f 6d70 7574 655f 636f 756e  ..z-compute_coun
-00000a20: 7473 5f63 6f6e 6673 5f61 6363 732e 3c6c  ts_confs_accs.<l
-00000a30: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000a40: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
-00000a50: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-00000a60: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
-00000a70: 0453 0072 1100 0000 2901 da03 6c65 6ea9  .S.r....)...len.
-00000a80: 0272 1a00 0000 da03 6964 7872 1100 0000  .r......idxr....
-00000a90: 7211 0000 0072 1200 0000 721d 0000 004f  r....r....r....O
-00000aa0: 0000 00f3 0000 0000 6301 0000 0000 0000  ........c.......
-00000ab0: 0000 0000 0002 0000 0008 0000 0013 0000  ................
-00000ac0: 0073 2400 0000 6700 7c00 5d1c 7d01 7400  .s$...g.|.].}.t.
-00000ad0: a001 7400 a002 8800 7c01 1900 6400 6b02  ..t.....|...d.k.
-00000ae0: a101 a101 9102 7104 5300 2901 7201 0000  ......q.S.).r...
-00000af0: 00a9 0372 0f00 0000 5a0a 6e61 6e5f 746f  ...r....Z.nan_to
-00000b00: 5f6e 756d 7210 0000 0072 1f00 0000 2901  _numr....r....).
-00000b10: da04 6469 6666 7211 0000 0072 1200 0000  ..diffr....r....
-00000b20: 721d 0000 0052 0000 0072 2100 0000 6301  r....R...r!...c.
-00000b30: 0000 0000 0000 0000 0000 0002 0000 0008  ................
-00000b40: 0000 0013 0000 0073 2000 0000 6700 7c00  .......s ...g.|.
-00000b50: 5d18 7d01 7400 a001 7400 a002 8800 7c01  ].}.t...t.....|.
-00000b60: 1900 a101 a101 9102 7104 5300 7211 0000  ........q.S.r...
-00000b70: 0072 2200 0000 721f 0000 0029 0172 1400  .r"...r....).r..
-00000b80: 0000 7211 0000 0072 1200 0000 721d 0000  ..r....r....r...
-00000b90: 0053 0000 0072 2100 0000 290b 720d 0000  .S...r!...).r...
-00000ba0: 0072 0e00 0000 720f 0000 005a 086c 696e  .r....r....Z.lin
-00000bb0: 7370 6163 65da 0573 6861 7065 da03 6d61  space..shape..ma
-00000bc0: 785a 0561 7272 6179 7219 0000 00da 0572  xZ.arrayr......r
-00000bd0: 616e 6765 721e 0000 0072 0700 0000 290a  anger....r....).
-00000be0: 7209 0000 0072 1400 0000 720a 0000 0072  r....r....r....r
-00000bf0: 1500 0000 7216 0000 00da 0769 6e64 6963  ....r......indic
-00000c00: 6573 da06 636f 756e 7473 da04 6163 6373  es..counts..accs
-00000c10: da05 636f 6e66 7372 2000 0000 7211 0000  ..confsr ...r...
-00000c20: 0029 0372 2300 0000 7214 0000 0072 1c00  .).r#...r....r..
-00000c30: 0000 7212 0000 00da 1963 6f6d 7075 7465  ..r......compute
-00000c40: 5f63 6f75 6e74 735f 636f 6e66 735f 6163  _counts_confs_ac
-00000c50: 6373 2600 0000 7322 0000 0000 1f0a 0108  cs&...s"........
-00000c60: 0118 010a 010a 0118 010e 020c fe08 0414  ................
-00000c70: 0208 0118 0118 0204 0108 011a 0272 2b00  .............r+.
-00000c80: 0000 6305 0000 0000 0000 0000 0000 0009  ..c.............
-00000c90: 0000 0006 0000 0043 0000 0073 3a00 0000  .......C...s:...
-00000ca0: 7400 7c00 7c01 7c02 7c03 7c04 8305 5c03  t.|.|.|.|.|...\.
-00000cb0: 7d05 7d06 7d07 7401 a002 7c05 7c07 7c06  }.}.}.t...|.|.|.
-00000cc0: 1800 6401 1300 1400 a101 7c00 6a03 6402  ..d.......|.j.d.
-00000cd0: 1900 1b00 7d08 7c08 5300 2903 6138 0300  ....}.|.S.).a8..
-00000ce0: 000a 2020 2020 436f 6d70 7574 6520 7468  ..    Compute th
-00000cf0: 6520 4578 7065 6374 6564 2043 616c 6962  e Expected Calib
-00000d00: 7261 7469 6f6e 2045 7272 6f72 2028 4543  ration Error (EC
-00000d10: 4529 0a20 2020 2028 7365 6520 604e 6165  E).    (see `Nae
-00000d20: 696e 6920 6574 2061 6c2e 2c20 3230 3135  ini et al., 2015
-00000d30: 203c 6874 7470 733a 2f2f 7065 6f70 6c65   <https://people
-00000d40: 2e63 732e 7069 7474 2e65 6475 2f7e 6d69  .cs.pitt.edu/~mi
-00000d50: 6c6f 732f 7265 7365 6172 6368 2f41 4141  los/research/AAA
-00000d60: 495f 4361 6c69 6272 6174 696f 6e2e 7064  I_Calibration.pd
-00000d70: 663e 605f 5f20 616e 640a 2020 2020 6047  f>`__ and.    `G
-00000d80: 756f 2065 7420 616c 2e2c 2032 3031 3720  uo et al., 2017 
-00000d90: 3c68 7474 703a 2f2f 7072 6f63 6565 6469  <http://proceedi
-00000da0: 6e67 732e 6d6c 722e 7072 6573 732f 7637  ngs.mlr.press/v7
-00000db0: 302f 6775 6f31 3761 2f67 756f 3137 612e  0/guo17a/guo17a.
-00000dc0: 7064 663e 605f 5f29 2e20 4f70 7469 6f6e  pdf>`__). Option
-00000dd0: 616c 6c79 2c20 706c 6f74 2061 6e64 2073  ally, plot and s
-00000de0: 6176 6520 6120 7265 6c69 6162 696c 6974  ave a reliabilit
-00000df0: 790a 2020 2020 6469 6167 7261 6d2e 0a0a  y.    diagram...
-00000e00: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000e10: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000e20: 2020 7072 6564 733a 2041 7272 6179 0a20    preds: Array. 
-00000e30: 2020 2020 2020 2041 206f 6e65 2d64 696d         A one-dim
-00000e40: 656e 7369 6f6e 616c 2061 7272 6179 206f  ensional array o
-00000e50: 6620 7072 6564 6963 7469 6f6e 7320 6f76  f predictions ov
-00000e60: 6572 2074 6865 2064 6174 6120 706f 696e  er the data poin
-00000e70: 7473 2e0a 2020 2020 7072 6f62 733a 2041  ts..    probs: A
-00000e80: 7272 6179 0a20 2020 2020 2020 2041 2074  rray.        A t
-00000e90: 776f 2d64 696d 656e 7369 6f6e 616c 2061  wo-dimensional a
-00000ea0: 7272 6179 206f 6620 636c 6173 7320 7072  rray of class pr
-00000eb0: 6f62 6162 696c 6974 6965 7320 666f 7220  obabilities for 
-00000ec0: 6561 6368 2064 6174 6120 706f 696e 742e  each data point.
-00000ed0: 0a20 2020 2074 6172 6765 7473 3a20 4172  .    targets: Ar
-00000ee0: 7261 790a 2020 2020 2020 2020 4120 6f6e  ray.        A on
-00000ef0: 652d 6469 6d65 6e73 696f 6e61 6c20 6172  e-dimensional ar
-00000f00: 7261 7920 6f66 2074 6172 6765 7420 7661  ray of target va
-00000f10: 7269 6162 6c65 732e 0a20 2020 2070 6c6f  riables..    plo
-00000f20: 743a 2062 6f6f 6c0a 2020 2020 2020 2020  t: bool.        
-00000f30: 5768 6574 6865 7220 746f 2070 6c6f 7420  Whether to plot 
-00000f40: 6120 7265 6c69 6162 696c 6974 7920 6469  a reliability di
-00000f50: 6167 7261 6d2e 0a20 2020 2070 6c6f 745f  agram..    plot_
-00000f60: 6f70 7469 6f6e 733a 2064 6963 740a 2020  options: dict.  
-00000f70: 2020 2020 2020 4f70 7469 6f6e 7320 666f        Options fo
-00000f80: 7220 7468 6520 7265 6c69 6162 696c 6974  r the reliabilit
-00000f90: 7920 6469 6167 7261 6d20 706c 6f74 3b20  y diagram plot; 
-00000fa0: 7365 6520 3a66 756e 633a 607e 666f 7274  see :func:`~fort
-00000fb0: 756e 612e 706c 6f74 2e70 6c6f 745f 7265  una.plot.plot_re
-00000fc0: 6c69 6162 696c 6974 795f 6469 6167 7261  liability_diagra
-00000fd0: 6d60 2e0a 0a20 2020 2052 6574 7572 6e73  m`...    Returns
-00000fe0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00000ff0: 2066 6c6f 6174 0a20 2020 2020 2020 2054   float.        T
-00001000: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00001010: 4543 452e 0a20 2020 2072 1700 0000 7201  ECE..    r....r.
-00001020: 0000 0029 0472 2b00 0000 720f 0000 00da  ...).r+...r.....
-00001030: 0373 756d 7224 0000 0029 0972 0900 0000  .sumr$...).r....
-00001040: 7214 0000 0072 0a00 0000 7215 0000 0072  r....r....r....r
-00001050: 1600 0000 7228 0000 0072 2a00 0000 7229  ....r(...r*...r)
-00001060: 0000 00da 0365 6365 7211 0000 0072 1100  .....ecer....r..
-00001070: 0000 7212 0000 00da 1a65 7870 6563 7465  ..r......expecte
-00001080: 645f 6361 6c69 6272 6174 696f 6e5f 6572  d_calibration_er
-00001090: 726f 725c 0000 0073 0a00 0000 001f 0201  ror\...s........
-000010a0: 0aff 0a03 2001 722e 0000 0063 0500 0000  .... .r....c....
-000010b0: 0000 0000 0000 0000 0500 0000 0600 0000  ................
-000010c0: 4300 0000 7310 0000 0074 007c 007c 017c  C...s....t.|.|.|
-000010d0: 027c 037c 0483 0553 0029 017a 2853 6565  .|.|...S.).z(See
-000010e0: 203a 6675 6e63 3a60 2e65 7870 6563 7465   :func:`.expecte
-000010f0: 645f 6361 6c69 6272 6174 696f 6e5f 6572  d_calibration_er
-00001100: 726f 7260 2e29 0172 2e00 0000 a905 7209  ror`.).r......r.
-00001110: 0000 0072 1400 0000 720a 0000 0072 1500  ...r....r....r..
-00001120: 0000 7216 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00001130: 0072 1200 0000 722d 0000 0082 0000 0073  .r....r-.......s
-00001140: 0200 0000 0008 722d 0000 0063 0500 0000  ......r-...c....
-00001150: 0000 0000 0000 0000 0900 0000 0600 0000  ................
-00001160: 4300 0000 7330 0000 0074 007c 007c 017c  C...s0...t.|.|.|
-00001170: 027c 037c 0483 055c 037d 057d 067d 0774  .|.|...\.}.}.}.t
-00001180: 01a0 027c 057c 077c 0618 0064 0113 0014  ...|.|.|...d....
-00001190: 00a1 017d 087c 0853 0029 0261 e502 0000  ...}.|.S.).a....
-000011a0: 0a20 2020 2043 6f6d 7075 7465 2074 6865  .    Compute the
-000011b0: 204d 6178 696d 756d 2043 616c 6962 7261   Maximum Calibra
-000011c0: 7469 6f6e 2045 7272 6f72 2028 4d43 4529  tion Error (MCE)
-000011d0: 0a20 2020 2028 7365 6520 604e 6165 696e  .    (see `Naein
-000011e0: 6920 6574 2061 6c2e 2c20 3230 3135 203c  i et al., 2015 <
-000011f0: 6874 7470 733a 2f2f 7065 6f70 6c65 2e63  https://people.c
-00001200: 732e 7069 7474 2e65 6475 2f7e 6d69 6c6f  s.pitt.edu/~milo
-00001210: 732f 7265 7365 6172 6368 2f41 4141 495f  s/research/AAAI_
-00001220: 4361 6c69 6272 6174 696f 6e2e 7064 663e  Calibration.pdf>
-00001230: 605f 5f29 2e20 4f70 7469 6f6e 616c 6c79  `__). Optionally
-00001240: 2c20 706c 6f74 0a20 2020 2061 6e64 2073  , plot.    and s
-00001250: 6176 6520 6120 7265 6c69 6162 696c 6974  ave a reliabilit
-00001260: 7920 6469 6167 7261 6d2e 0a0a 2020 2020  y diagram...    
-00001270: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00001280: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7072  ---------.    pr
-00001290: 6564 733a 2041 7272 6179 0a20 2020 2020  eds: Array.     
-000012a0: 2020 2041 206f 6e65 2d64 696d 656e 7369     A one-dimensi
-000012b0: 6f6e 616c 2061 7272 6179 206f 6620 7072  onal array of pr
-000012c0: 6564 6963 7469 6f6e 7320 6f76 6572 2074  edictions over t
-000012d0: 6865 2064 6174 6120 706f 696e 7473 2e0a  he data points..
-000012e0: 2020 2020 7072 6f62 733a 2041 7272 6179      probs: Array
-000012f0: 0a20 2020 2020 2020 2041 2074 776f 2d64  .        A two-d
-00001300: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
-00001310: 206f 6620 636c 6173 7320 7072 6f62 6162   of class probab
-00001320: 696c 6974 6965 7320 666f 7220 6561 6368  ilities for each
-00001330: 2064 6174 6120 706f 696e 742e 0a20 2020   data point..   
-00001340: 2074 6172 6765 7473 3a20 4172 7261 790a   targets: Array.
-00001350: 2020 2020 2020 2020 4120 6f6e 652d 6469          A one-di
-00001360: 6d65 6e73 696f 6e61 6c20 6172 7261 7920  mensional array 
-00001370: 6f66 2074 6172 6765 7420 7661 7269 6162  of target variab
-00001380: 6c65 732e 0a20 2020 2070 6c6f 743a 2062  les..    plot: b
-00001390: 6f6f 6c0a 2020 2020 2020 2020 5768 6574  ool.        Whet
-000013a0: 6865 7220 746f 2070 6c6f 7420 6120 7265  her to plot a re
-000013b0: 6c69 6162 696c 6974 7920 6469 6167 7261  liability diagra
-000013c0: 6d2e 0a20 2020 2070 6c6f 745f 6f70 7469  m..    plot_opti
-000013d0: 6f6e 733a 2064 6963 740a 2020 2020 2020  ons: dict.      
-000013e0: 2020 4f70 7469 6f6e 7320 666f 7220 7468    Options for th
-000013f0: 6520 7265 6c69 6162 696c 6974 7920 6469  e reliability di
-00001400: 6167 7261 6d20 706c 6f74 3b20 7365 6520  agram plot; see 
-00001410: 3a66 756e 633a 607e 666f 7274 756e 612e  :func:`~fortuna.
-00001420: 706c 6f74 2e70 6c6f 745f 7265 6c69 6162  plot.plot_reliab
-00001430: 696c 6974 795f 6469 6167 7261 6d60 2e0a  ility_diagram`..
-00001440: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-00001450: 202d 2d2d 2d2d 2d2d 0a20 2020 2066 6c6f   -------.    flo
-00001460: 6174 0a20 2020 2020 2020 2054 6865 2076  at.        The v
-00001470: 616c 7565 206f 6620 7468 6520 4d43 452e  alue of the MCE.
-00001480: 0a20 2020 2072 1700 0000 2903 722b 0000  .    r....).r+..
-00001490: 0072 0f00 0000 7225 0000 0029 0972 0900  .r....r%...).r..
-000014a0: 0000 7214 0000 0072 0a00 0000 7215 0000  ..r....r....r...
-000014b0: 0072 1600 0000 7228 0000 0072 2a00 0000  .r....r(...r*...
-000014c0: 7229 0000 00da 036d 6365 7211 0000 0072  r).....mcer....r
-000014d0: 1100 0000 7212 0000 00da 196d 6178 696d  ....r......maxim
-000014e0: 756d 5f63 616c 6962 7261 7469 6f6e 5f65  um_calibration_e
-000014f0: 7272 6f72 8d00 0000 730a 0000 0000 1e02  rror....s.......
-00001500: 010a ff0a 0316 0172 3100 0000 6305 0000  .......r1...c...
-00001510: 0000 0000 0000 0000 0005 0000 0006 0000  ................
-00001520: 0043 0000 0073 1000 0000 7400 7c00 7c01  .C...s....t.|.|.
-00001530: 7c02 7c03 7c04 8305 5300 2901 7a27 5365  |.|.|...S.).z'Se
-00001540: 6520 3a66 756e 633a 602e 6d61 7869 6d75  e :func:`.maximu
-00001550: 6d5f 6361 6c69 6272 6174 696f 6e5f 6572  m_calibration_er
-00001560: 726f 7260 2e29 0172 3100 0000 722f 0000  ror`.).r1...r/..
-00001570: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00001580: 7230 0000 00b2 0000 0073 0200 0000 0008  r0.......s......
-00001590: 7230 0000 0029 0372 1400 0000 720a 0000  r0...).r....r...
-000015a0: 0072 0b00 0000 6302 0000 0000 0000 0000  .r....c.........
-000015b0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-000015c0: 5600 0000 7c00 6a00 6401 6b03 7212 7401  V...|.j.d.k.r.t.
-000015d0: 6402 8301 8201 7402 7c01 8301 7403 6b02  d.....t.|...t.k.
-000015e0: 7226 7c01 a004 a100 7d01 7405 6a06 a007  r&|.....}.t.j...
-000015f0: 7c01 7c00 6a08 6403 1900 a102 7d01 7409  |.|.j.d.....}.t.
-00001600: a00a 7409 6a0b 7c00 7c01 1800 6401 1300  ..t.j.|.|...d...
-00001610: 6403 6404 8d02 a101 5300 2905 61e0 0100  d.d.....S.).a...
-00001620: 000a 2020 2020 4272 6965 7220 7363 6f72  ..    Brier scor
-00001630: 6520 2873 6565 2060 4272 6965 722c 2031  e (see `Brier, 1
-00001640: 3935 3020 3c68 7474 7073 3a2f 2f77 6562  950 <https://web
-00001650: 2e61 7263 6869 7665 2e6f 7267 2f77 6562  .archive.org/web
-00001660: 2f32 3031 3731 3032 3330 3132 3733 372f  /20171023012737/
-00001670: 0a20 2020 2068 7474 7073 3a2f 2f64 6f63  .    https://doc
-00001680: 732e 6c69 622e 6e6f 6161 2e67 6f76 2f72  s.lib.noaa.gov/r
-00001690: 6573 6375 652f 6d77 722f 3037 382f 6d77  escue/mwr/078/mw
-000016a0: 722d 3037 382d 3031 2d30 3030 312e 7064  r-078-01-0001.pd
-000016b0: 663e 605f 5f29 2e20 5468 6973 2063 616e  f>`__). This can
-000016c0: 2062 6520 7573 6564 2066 6f72 2062 6f74   be used for bot
-000016d0: 6820 6269 6e61 7279 2061 6e64 206d 756c  h binary and mul
-000016e0: 7469 2d63 6c61 7373 0a20 2020 2063 6c61  ti-class.    cla
-000016f0: 7373 6966 6963 6174 696f 6e2e 0a0a 2020  ssification...  
-00001700: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00001710: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00001720: 7072 6f62 733a 2041 7272 6179 0a20 2020  probs: Array.   
-00001730: 2020 2020 2041 2074 776f 2d64 696d 656e       A two-dimen
-00001740: 7369 6f6e 616c 2061 7272 6179 206f 6620  sional array of 
-00001750: 636c 6173 7320 7072 6f62 6162 696c 6974  class probabilit
-00001760: 6965 7320 666f 7220 6561 6368 2064 6174  ies for each dat
-00001770: 6120 706f 696e 742e 0a20 2020 2074 6172  a point..    tar
-00001780: 6765 7473 3a20 4172 7261 790a 2020 2020  gets: Array.    
-00001790: 2020 2020 4120 6f6e 652d 6469 6d65 6e73      A one-dimens
-000017a0: 696f 6e61 6c20 6172 7261 7920 6f66 2074  ional array of t
-000017b0: 6172 6765 7420 7661 7269 6162 6c65 732e  arget variables.
-000017c0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-000017d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 666c    -------.    fl
-000017e0: 6f61 740a 2020 2020 2020 2020 5468 6520  oat.        The 
-000017f0: 4272 6965 7220 7363 6f72 652e 0a20 2020  Brier score..   
-00001800: 2072 1700 0000 7a64 6070 726f 6273 6020   r....zd`probs` 
-00001810: 6d75 7374 2062 6520 6120 7477 6f2d 6469  must be a two-di
-00001820: 6d65 6e73 696f 6e61 6c20 6172 7261 7920  mensional array 
-00001830: 6f66 2070 726f 6261 6269 6c69 7469 6573  of probabilities
-00001840: 2066 6f72 2065 6163 6820 636c 6173 7320   for each class 
-00001850: 616e 6420 6561 6368 2064 6174 610a 2020  and each data.  
-00001860: 2020 2020 2020 706f 696e 742e 720c 0000        point.r...
-00001870: 0029 015a 0461 7869 7329 0c72 0d00 0000  .).Z.axis).r....
-00001880: 720e 0000 00da 0474 7970 6572 0600 0000  r......typer....
-00001890: 5a10 746f 5f61 7272 6179 5f74 6172 6765  Z.to_array_targe
-000018a0: 7473 da03 6a61 785a 026e 6e5a 076f 6e65  ts..jaxZ.nnZ.one
-000018b0: 5f68 6f74 7224 0000 0072 0f00 0000 7210  _hotr$...r....r.
-000018c0: 0000 0072 2c00 0000 2902 7214 0000 0072  ...r,...).r....r
-000018d0: 0a00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-000018e0: 0000 00da 0b62 7269 6572 5f73 636f 7265  .....brier_score
-000018f0: bd00 0000 7310 0000 0000 120a 0102 0102  ....s...........
-00001900: ff04 040c 0108 0114 0172 3400 0000 2902  .........r4...).
-00001910: 464e 2902 464e 2902 464e 2902 464e 2902  FN).FN).FN).FN).
-00001920: 464e 291a da06 7479 7069 6e67 7202 0000  FN)...typingr...
-00001930: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
-00001940: 5a06 6a61 782e 6e6e 7233 0000 005a 096a  Z.jax.nnr3...Z.j
-00001950: 6178 2e6e 756d 7079 5a05 6e75 6d70 7972  ax.numpyZ.numpyr
-00001960: 0f00 0000 5a13 666f 7274 756e 612e 6461  ....Z.fortuna.da
-00001970: 7461 2e6c 6f61 6465 7272 0600 0000 5a0c  ta.loaderr....Z.
-00001980: 666f 7274 756e 612e 706c 6f74 7207 0000  fortuna.plotr...
-00001990: 005a 0e66 6f72 7475 6e61 2e74 7970 696e  .Z.fortuna.typin
-000019a0: 6772 0800 0000 5a07 6e64 6172 7261 7972  gr....Z.ndarrayr
-000019b0: 1300 0000 da04 626f 6f6c 722b 0000 0072  ......boolr+...r
-000019c0: 2e00 0000 da05 666c 6f61 7472 2d00 0000  ......floatr-...
-000019d0: 7231 0000 0072 3000 0000 7234 0000 0072  r1...r0...r4...r
-000019e0: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-000019f0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001a00: 0073 7200 0000 1802 0801 0c02 0c01 0c01  .sr.............
-00001a10: 0c03 141f 0001 00fb 0201 0201 0201 0201  ................
-00001a20: 0201 0601 12fa 0c3a 0001 00fb 0201 0201  .......:........
-00001a30: 0201 0201 0201 0601 04fa 0c2a 0001 00fb  ...........*....
-00001a40: 0201 0201 0201 0201 0201 0601 02fa 0c0f  ................
-00001a50: 0001 00fb 0201 0201 0201 0201 0201 0601  ................
-00001a60: 04fa 0c29 0001 00fb 0201 0201 0201 0201  ...)............
-00001a70: 0201 0601 02fa 0c0b                      ........
+000000f0: 6509 6a10 640a 9c06 640f 6410 8405 5a15  e.j.d...d.d...Z.
+00000100: 641b 650f 650f 650f 6512 6502 6501 1900  d.e.e.e.e.e.e...
+00000110: 6509 6a10 640a 9c06 6411 6412 8405 5a16  e.j.d...d.d...Z.
+00000120: 641c 650f 650f 650f 6512 6502 6501 1900  d.e.e.e.e.e.e...
+00000130: 6509 6a10 640a 9c06 6413 6414 8405 5a17  e.j.d...d.d...Z.
+00000140: 650f 6504 650b 650f 6602 1900 6509 6a10  e.e.e.e.f...e.j.
+00000150: 6415 9c03 6416 6417 8404 5a18 6402 5300  d...d.d...Z.d.S.
+00000160: 291d e900 0000 0029 04da 0444 6963 74da  )......)...Dict.
+00000170: 084f 7074 696f 6e61 6cda 0554 7570 6c65  .Optional..Tuple
+00000180: da05 556e 696f 6e4e 2901 da0d 5461 7267  ..UnionN)...Targ
+00000190: 6574 734c 6f61 6465 7229 01da 1870 6c6f  etsLoader)...plo
+000001a0: 745f 7265 6c69 6162 696c 6974 795f 6469  t_reliability_di
+000001b0: 6167 7261 6d29 01da 0541 7272 6179 2903  agram)...Array).
+000001c0: da05 7072 6564 73da 0774 6172 6765 7473  ..preds..targets
+000001d0: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+000001e0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000001f0: 0073 3200 0000 7c00 6a00 6401 6b04 7212  .s2...|.j.d.k.r.
+00000200: 7401 6402 8301 8201 7c01 6a00 6401 6b04  t.d.....|.j.d.k.
+00000210: 7224 7401 6403 8301 8201 7402 a003 7c00  r$t.d.....t...|.
+00000220: 7c01 6b02 a101 5300 2904 6145 0100 000a  |.k...S.).aE....
+00000230: 2020 2020 436f 6d70 7574 6520 7468 6520      Compute the 
+00000240: 6163 6375 7261 6379 2067 6976 656e 2070  accuracy given p
+00000250: 7265 6469 6374 696f 6e73 2061 6e64 2074  redictions and t
+00000260: 6172 6765 7420 7661 7269 6162 6c65 732e  arget variables.
+00000270: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00000280: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000290: 2020 2020 7072 6564 733a 2041 7272 6179      preds: Array
+000002a0: 0a20 2020 2020 2020 2041 206f 6e65 2d64  .        A one-d
+000002b0: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
+000002c0: 206f 6620 7072 6564 6963 7469 6f6e 7320   of predictions 
+000002d0: 6f76 6572 2074 6865 2064 6174 6120 706f  over the data po
+000002e0: 696e 7473 2e0a 2020 2020 7461 7267 6574  ints..    target
+000002f0: 733a 2041 7272 6179 0a20 2020 2020 2020  s: Array.       
+00000300: 2041 206f 6e65 2d64 696d 656e 7369 6f6e   A one-dimension
+00000310: 616c 2061 7272 6179 206f 6620 7461 7267  al array of targ
+00000320: 6574 2076 6172 6961 626c 6573 2e0a 0a20  et variables... 
+00000330: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00000340: 2d2d 2d2d 2d2d 0a20 2020 2066 6c6f 6174  ------.    float
+00000350: 0a20 2020 2020 2020 2054 6865 2063 6f6d  .        The com
+00000360: 7075 7465 6420 6163 6375 7261 6379 2e0a  puted accuracy..
+00000370: 2020 2020 e901 0000 007a 3d60 7072 6564      .....z=`pred
+00000380: 7360 206d 7573 7420 6265 2061 206f 6e65  s` must be a one
+00000390: 2d64 696d 656e 7369 6f6e 616c 2061 7272  -dimensional arr
+000003a0: 6179 206f 6620 7072 6564 6963 7465 6420  ay of predicted 
+000003b0: 636c 6173 7365 732e 7a3c 6074 6172 6765  classes.z<`targe
+000003c0: 7473 6020 6d75 7374 2062 6520 6120 6f6e  ts` must be a on
+000003d0: 652d 6469 6d65 6e73 696f 6e61 6c20 6172  e-dimensional ar
+000003e0: 7261 7920 6f66 2074 6172 6765 7420 636c  ray of target cl
+000003f0: 6173 7365 732e 2904 da04 6e64 696d da0a  asses.)...ndim..
+00000400: 5661 6c75 6545 7272 6f72 da03 6a6e 70da  ValueError..jnp.
+00000410: 046d 6561 6e29 0272 0900 0000 720a 0000  .mean).r....r...
+00000420: 00a9 0072 1100 0000 fa3b 2f55 7365 7273  ...r.....;/Users
+00000430: 2f64 6574 6f6d 6d61 2f61 7773 2d66 6f72  /detomma/aws-for
+00000440: 7475 6e61 2f66 6f72 7475 6e61 2f6d 6574  tuna/fortuna/met
+00000450: 7269 632f 636c 6173 7369 6669 6361 7469  ric/classificati
+00000460: 6f6e 2e70 79da 0861 6363 7572 6163 790b  on.py..accuracy.
+00000470: 0000 0073 1200 0000 0010 0a01 0201 02ff  ...s............
+00000480: 0403 0a01 0201 02ff 0403 7213 0000 0046  ..........r....F
+00000490: 2906 7209 0000 00da 0570 726f 6273 720a  ).r......probsr.
+000004a0: 0000 00da 0470 6c6f 74da 0c70 6c6f 745f  .....plot..plot_
+000004b0: 6f70 7469 6f6e 7372 0b00 0000 6305 0000  optionsr....c...
+000004c0: 0000 0000 0000 0000 000a 0000 0006 0000  ................
+000004d0: 0003 0000 0073 f400 0000 8801 6a00 6401  .....s......j.d.
+000004e0: 6b03 7212 7401 6402 8301 8201 7402 a003  k.r.t.d.....t...
+000004f0: 6403 8801 6a04 6403 1900 1b00 6403 6404  d...j.d.....d.d.
+00000500: a103 8902 8801 a005 6403 a101 8901 7402  ........d.....t.
+00000510: a006 8801 a101 8901 7402 a007 8801 8802  ........t.......
+00000520: 6405 1900 6b01 a101 6405 1900 6701 7d05  d...k...d...g.}.
+00000530: 7c05 8701 8702 6602 6406 6407 8408 7408  |.....f.d.d...t.
+00000540: 6403 7409 8802 8301 8302 4400 8301 3700  d.t.......D...7.
+00000550: 7d05 7402 a006 6408 6407 8400 7c05 4400  }.t...d.d...|.D.
+00000560: 8301 a101 7d06 7c02 7c00 1800 8900 7402  ....}.|.|.....t.
+00000570: a006 8700 6601 6409 6407 8408 7c05 4400  ....f.d.d...|.D.
+00000580: 8301 a101 7d07 7402 a006 8701 6601 640a  ....}.t.....f.d.
+00000590: 6407 8408 7c05 4400 8301 a101 7d08 7c03  d...|.D.....}.|.
+000005a0: 72ea 7c08 6405 6b03 7d09 740a 7c07 7c09  r.|.d.k.}.t.|.|.
+000005b0: 1900 7c08 7c09 1900 6602 6900 7c04 a401  ..|.|...f.i.|...
+000005c0: 8e01 0100 7c06 7c08 7c07 6603 5300 290b  ....|.|.|.f.S.).
+000005d0: 615a 0300 000a 2020 2020 4269 6e20 7468  aZ....    Bin th
+000005e0: 6520 636f 6e66 6964 656e 6365 2073 636f  e confidence sco
+000005f0: 7265 7320 286d 6178 696d 756d 2070 726f  res (maximum pro
+00000600: 6261 6269 6c69 7479 2920 616e 6420 666f  bability) and fo
+00000610: 7220 6561 6368 206f 6620 7468 656d 2063  r each of them c
+00000620: 6f6d 7075 7465 3a0a 2020 2020 2020 2020  ompute:.        
+00000630: 2d20 7468 6520 6e75 6d62 6572 206f 6620  - the number of 
+00000640: 696e 7075 7473 3b0a 2020 2020 2020 2020  inputs;.        
+00000650: 2d20 7468 6520 6176 6572 6167 6520 636f  - the average co
+00000660: 6e66 6964 656e 6365 2073 636f 7265 2066  nfidence score f
+00000670: 6f72 2065 6163 6820 6269 6e3b 0a20 2020  or each bin;.   
+00000680: 2020 2020 202d 2074 6865 2061 7665 7261       - the avera
+00000690: 6765 2061 6363 7572 6163 7920 6f76 6572  ge accuracy over
+000006a0: 2065 6163 6820 6269 6e2e 0a0a 2020 2020   each bin...    
+000006b0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000006c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7072  ---------.    pr
+000006d0: 6564 733a 2041 7272 6179 0a20 2020 2020  eds: Array.     
+000006e0: 2020 2041 206f 6e65 2d64 696d 656e 7369     A one-dimensi
+000006f0: 6f6e 616c 2061 7272 6179 206f 6620 7072  onal array of pr
+00000700: 6564 6963 7469 6f6e 7320 6f76 6572 2074  edictions over t
+00000710: 6865 2064 6174 6120 706f 696e 7473 2e0a  he data points..
+00000720: 2020 2020 7072 6f62 733a 2041 7272 6179      probs: Array
+00000730: 0a20 2020 2020 2020 2041 2074 776f 2d64  .        A two-d
+00000740: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
+00000750: 206f 6620 636c 6173 7320 7072 6f62 6162   of class probab
+00000760: 696c 6974 6965 7320 666f 7220 6561 6368  ilities for each
+00000770: 2064 6174 6120 706f 696e 742e 0a20 2020   data point..   
+00000780: 2074 6172 6765 7473 3a20 4172 7261 790a   targets: Array.
+00000790: 2020 2020 2020 2020 4120 6f6e 652d 6469          A one-di
+000007a0: 6d65 6e73 696f 6e61 6c20 6172 7261 7920  mensional array 
+000007b0: 6f66 2074 6172 6765 7420 7661 7269 6162  of target variab
+000007c0: 6c65 732e 0a20 2020 2070 6c6f 743a 2062  les..    plot: b
+000007d0: 6f6f 6c0a 2020 2020 2020 2020 5768 6574  ool.        Whet
+000007e0: 6865 7220 746f 2070 6c6f 7420 6120 7265  her to plot a re
+000007f0: 6c69 6162 696c 6974 7920 6469 6167 7261  liability diagra
+00000800: 6d2e 0a20 2020 2070 6c6f 745f 6f70 7469  m..    plot_opti
+00000810: 6f6e 733a 2064 6963 740a 2020 2020 2020  ons: dict.      
+00000820: 2020 4f70 7469 6f6e 7320 666f 7220 7468    Options for th
+00000830: 6520 7265 6c69 6162 696c 6974 7920 6469  e reliability di
+00000840: 6167 7261 6d20 706c 6f74 3b20 7365 6520  agram plot; see 
+00000850: 3a66 756e 633a 607e 666f 7274 756e 612e  :func:`~fortuna.
+00000860: 706c 6f74 2e70 6c6f 745f 7265 6c69 6162  plot.plot_reliab
+00000870: 696c 6974 795f 6469 6167 7261 6d60 2e0a  ility_diagram`..
+00000880: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00000890: 202d 2d2d 2d2d 2d2d 0a20 2020 2054 7570   -------.    Tup
+000008a0: 6c65 5b6a 6e70 2e6e 6461 7272 6179 2c20  le[jnp.ndarray, 
+000008b0: 6a6e 702e 6e64 6172 7261 792c 206a 6e70  jnp.ndarray, jnp
+000008c0: 2e6e 6461 7272 6179 5d0a 2020 2020 2020  .ndarray].      
+000008d0: 2020 4e75 6d62 6572 206f 6620 696e 7075    Number of inpu
+000008e0: 7473 2070 6572 2062 696e 2c20 6176 6572  ts per bin, aver
+000008f0: 6167 6520 636f 6e66 6964 656e 6365 2073  age confidence s
+00000900: 636f 7265 2070 6572 2062 696e 2061 6e64  core per bin and
+00000910: 2061 7665 7261 6765 2061 6363 7572 6163   average accurac
+00000920: 7920 7065 7220 6269 6e2e 0a20 2020 20e9  y per bin..    .
+00000930: 0200 0000 7a28 6070 726f 6273 6020 6d75  ....z(`probs` mu
+00000940: 7374 2062 6520 6120 7477 6f2d 6469 6d65  st be a two-dime
+00000950: 6e73 696f 6e61 6c20 6172 7261 792e 720c  nsional array.r.
+00000960: 0000 00e9 0a00 0000 7201 0000 0063 0100  ........r....c..
+00000970: 0000 0000 0000 0000 0000 0200 0000 0900  ................
+00000980: 0000 1300 0000 7332 0000 0067 007c 005d  ......s2...g.|.]
+00000990: 2a7d 0174 00a0 0188 0088 017c 0119 006b  *}.t.......|...k
+000009a0: 0188 0088 017c 0164 0018 0019 006b 0440  .....|.d.....k.@
+000009b0: 00a1 0164 0119 0091 0271 0453 0029 0272  ...d.....q.S.).r
+000009c0: 0c00 0000 7201 0000 0029 0272 0f00 0000  ....r....).r....
+000009d0: da05 7768 6572 6529 02da 022e 30da 0169  ..where)....0..i
+000009e0: 2902 7214 0000 00da 0a74 6872 6573 686f  ).r......thresho
+000009f0: 6c64 7372 1100 0000 7212 0000 00da 0a3c  ldsr....r......<
+00000a00: 6c69 7374 636f 6d70 3e4b 0000 0073 0400  listcomp>K...s..
+00000a10: 0000 0602 02ff 7a2d 636f 6d70 7574 655f  ......z-compute_
+00000a20: 636f 756e 7473 5f63 6f6e 6673 5f61 6363  counts_confs_acc
+00000a30: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+00000a40: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00000a50: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00000a60: 0000 0067 007c 005d 0c7d 0174 007c 0183  ...g.|.].}.t.|..
+00000a70: 0191 0271 0453 0072 1100 0000 2901 da03  ...q.S.r....)...
+00000a80: 6c65 6ea9 0272 1a00 0000 da03 6964 7872  len..r......idxr
+00000a90: 1100 0000 7211 0000 0072 1200 0000 721d  ....r....r....r.
+00000aa0: 0000 004f 0000 00f3 0000 0000 6301 0000  ...O........c...
+00000ab0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
+00000ac0: 0013 0000 0073 2400 0000 6700 7c00 5d1c  .....s$...g.|.].
+00000ad0: 7d01 7400 a001 7400 a002 8800 7c01 1900  }.t...t.....|...
+00000ae0: 6400 6b02 a101 a101 9102 7104 5300 2901  d.k.......q.S.).
+00000af0: 7201 0000 00a9 0372 0f00 0000 da0a 6e61  r......r......na
+00000b00: 6e5f 746f 5f6e 756d 7210 0000 0072 1f00  n_to_numr....r..
+00000b10: 0000 2901 da04 6469 6666 7211 0000 0072  ..)...diffr....r
+00000b20: 1200 0000 721d 0000 0052 0000 0072 2100  ....r....R...r!.
+00000b30: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000b40: 0000 0008 0000 0013 0000 0073 2000 0000  ...........s ...
+00000b50: 6700 7c00 5d18 7d01 7400 a001 7400 a002  g.|.].}.t...t...
+00000b60: 8800 7c01 1900 a101 a101 9102 7104 5300  ..|.........q.S.
+00000b70: 7211 0000 0072 2200 0000 721f 0000 0029  r....r"...r....)
+00000b80: 0172 1400 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000b90: 721d 0000 0053 0000 0072 2100 0000 290b  r....S...r!...).
+00000ba0: 720d 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+00000bb0: 086c 696e 7370 6163 65da 0573 6861 7065  .linspace..shape
+00000bc0: da03 6d61 78da 0561 7272 6179 7219 0000  ..max..arrayr...
+00000bd0: 00da 0572 616e 6765 721e 0000 0072 0700  ...ranger....r..
+00000be0: 0000 290a 7209 0000 0072 1400 0000 720a  ..).r....r....r.
+00000bf0: 0000 0072 1500 0000 7216 0000 00da 0769  ...r....r......i
+00000c00: 6e64 6963 6573 da06 636f 756e 7473 da04  ndices..counts..
+00000c10: 6163 6373 da05 636f 6e66 7372 2000 0000  accs..confsr ...
+00000c20: 7211 0000 0029 0372 2400 0000 7214 0000  r....).r$...r...
+00000c30: 0072 1c00 0000 7212 0000 00da 1963 6f6d  .r....r......com
+00000c40: 7075 7465 5f63 6f75 6e74 735f 636f 6e66  pute_counts_conf
+00000c50: 735f 6163 6373 2600 0000 7322 0000 0000  s_accs&...s"....
+00000c60: 1f0a 0108 0118 010a 010a 0118 010e 020c  ................
+00000c70: fe08 0414 0208 0118 0118 0204 0108 011a  ................
+00000c80: 0272 2e00 0000 6305 0000 0000 0000 0000  .r....c.........
+00000c90: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
+00000ca0: 3c00 0000 7400 7c00 7c01 7c02 7c03 7c04  <...t.|.|.|.|.|.
+00000cb0: 8305 5c03 7d05 7d06 7d07 7401 a002 7c05  ..\.}.}.}.t...|.
+00000cc0: 7401 a003 7c07 7c06 1800 a101 1400 a101  t...|.|.........
+00000cd0: 7c00 6a04 6401 1900 1b00 7d08 7c08 5300  |.j.d.....}.|.S.
+00000ce0: 2902 613e 0300 000a 2020 2020 436f 6d70  ).a>....    Comp
+00000cf0: 7574 6520 7468 6520 4578 7065 6374 6564  ute the Expected
+00000d00: 2043 616c 6962 7261 7469 6f6e 2045 7272   Calibration Err
+00000d10: 6f72 2028 4543 4529 0a20 2020 2028 7365  or (ECE).    (se
+00000d20: 6520 604e 6165 696e 6920 6574 2061 6c2e  e `Naeini et al.
+00000d30: 2c20 3230 3135 203c 6874 7470 733a 2f2f  , 2015 <https://
+00000d40: 7065 6f70 6c65 2e63 732e 7069 7474 2e65  people.cs.pitt.e
+00000d50: 6475 2f7e 6d69 6c6f 732f 7265 7365 6172  du/~milos/resear
+00000d60: 6368 2f41 4141 495f 4361 6c69 6272 6174  ch/AAAI_Calibrat
+00000d70: 696f 6e2e 7064 663e 605f 5f20 616e 640a  ion.pdf>`__ and.
+00000d80: 2020 2020 6047 756f 2065 7420 616c 2e2c      `Guo et al.,
+00000d90: 2032 3031 3720 3c68 7474 703a 2f2f 7072   2017 <http://pr
+00000da0: 6f63 6565 6469 6e67 732e 6d6c 722e 7072  oceedings.mlr.pr
+00000db0: 6573 732f 7637 302f 6775 6f31 3761 2f67  ess/v70/guo17a/g
+00000dc0: 756f 3137 612e 7064 663e 605f 5f29 2e20  uo17a.pdf>`__). 
+00000dd0: 4f70 7469 6f6e 616c 6c79 2c20 706c 6f74  Optionally, plot
+00000de0: 2061 6e64 2073 6176 6520 6120 7265 6c69   and save a reli
+00000df0: 6162 696c 6974 790a 2020 2020 6469 6167  ability.    diag
+00000e00: 7261 6d2e 0a0a 2020 2020 5061 7261 6d65  ram...    Parame
+00000e10: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00000e20: 2d2d 2d0a 2020 2020 7072 6564 733a 2041  ---.    preds: A
+00000e30: 7272 6179 0a20 2020 2020 2020 2041 206f  rray.        A o
+00000e40: 6e65 2d64 696d 656e 7369 6f6e 616c 2061  ne-dimensional a
+00000e50: 7272 6179 206f 6620 7072 6564 6963 7469  rray of predicti
+00000e60: 6f6e 7320 6f76 6572 2074 6865 2064 6174  ons over the dat
+00000e70: 6120 706f 696e 7473 2e0a 2020 2020 7072  a points..    pr
+00000e80: 6f62 733a 2041 7272 6179 0a20 2020 2020  obs: Array.     
+00000e90: 2020 2041 2074 776f 2d64 696d 656e 7369     A two-dimensi
+00000ea0: 6f6e 616c 2061 7272 6179 206f 6620 636c  onal array of cl
+00000eb0: 6173 7320 7072 6f62 6162 696c 6974 6965  ass probabilitie
+00000ec0: 7320 666f 7220 6561 6368 2064 6174 6120  s for each data 
+00000ed0: 706f 696e 742e 0a20 2020 2074 6172 6765  point..    targe
+00000ee0: 7473 3a20 4172 7261 790a 2020 2020 2020  ts: Array.      
+00000ef0: 2020 4120 6f6e 652d 6469 6d65 6e73 696f    A one-dimensio
+00000f00: 6e61 6c20 6172 7261 7920 6f66 2074 6172  nal array of tar
+00000f10: 6765 7420 7661 7269 6162 6c65 732e 0a20  get variables.. 
+00000f20: 2020 2070 6c6f 743a 2062 6f6f 6c0a 2020     plot: bool.  
+00000f30: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+00000f40: 2070 6c6f 7420 6120 7265 6c69 6162 696c   plot a reliabil
+00000f50: 6974 7920 6469 6167 7261 6d2e 0a20 2020  ity diagram..   
+00000f60: 2070 6c6f 745f 6f70 7469 6f6e 733a 2064   plot_options: d
+00000f70: 6963 740a 2020 2020 2020 2020 4f70 7469  ict.        Opti
+00000f80: 6f6e 7320 666f 7220 7468 6520 7265 6c69  ons for the reli
+00000f90: 6162 696c 6974 7920 6469 6167 7261 6d20  ability diagram 
+00000fa0: 706c 6f74 3b20 7365 6520 3a66 756e 633a  plot; see :func:
+00000fb0: 607e 666f 7274 756e 612e 706c 6f74 2e70  `~fortuna.plot.p
+00000fc0: 6c6f 745f 7265 6c69 6162 696c 6974 795f  lot_reliability_
+00000fd0: 6469 6167 7261 6d60 2e0a 0a20 2020 2052  diagram`...    R
+00000fe0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00000ff0: 2d2d 0a20 2020 206a 6e70 2e6e 6461 7272  --.    jnp.ndarr
+00001000: 6179 0a20 2020 2020 2020 2054 6865 2076  ay.        The v
+00001010: 616c 7565 206f 6620 7468 6520 4543 452e  alue of the ECE.
+00001020: 0a20 2020 2072 0100 0000 2905 722e 0000  .    r....).r...
+00001030: 0072 0f00 0000 da03 7375 6dda 0361 6273  .r......sum..abs
+00001040: 7226 0000 0029 0972 0900 0000 7214 0000  r&...).r....r...
+00001050: 0072 0a00 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001060: 722b 0000 0072 2d00 0000 722c 0000 00da  r+...r-...r,....
+00001070: 0365 6365 7211 0000 0072 1100 0000 7212  .ecer....r....r.
+00001080: 0000 00da 1a65 7870 6563 7465 645f 6361  .....expected_ca
+00001090: 6c69 6272 6174 696f 6e5f 6572 726f 725c  libration_error\
+000010a0: 0000 0073 0a00 0000 001f 0201 0aff 0a03  ...s............
+000010b0: 2201 7232 0000 0063 0500 0000 0000 0000  ".r2...c........
+000010c0: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+000010d0: 7310 0000 0074 007c 007c 017c 027c 037c  s....t.|.|.|.|.|
+000010e0: 0483 0553 0029 017a 2853 6565 203a 6675  ...S.).z(See :fu
+000010f0: 6e63 3a60 2e65 7870 6563 7465 645f 6361  nc:`.expected_ca
+00001100: 6c69 6272 6174 696f 6e5f 6572 726f 7260  libration_error`
+00001110: 2e29 0172 3200 0000 a905 7209 0000 0072  .).r2.....r....r
+00001120: 1400 0000 720a 0000 0072 1500 0000 7216  ....r....r....r.
+00001130: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00001140: 0000 7231 0000 0082 0000 0073 0200 0000  ..r1.......s....
+00001150: 0008 7231 0000 0063 0500 0000 0000 0000  ..r1...c........
+00001160: 0000 0000 0900 0000 0700 0000 4300 0000  ............C...
+00001170: 7332 0000 0074 007c 007c 017c 027c 037c  s2...t.|.|.|.|.|
+00001180: 0483 055c 037d 057d 067d 0774 01a0 027c  ...\.}.}.}.t...|
+00001190: 0574 01a0 037c 077c 0618 00a1 0114 00a1  .t...|.|........
+000011a0: 017d 087c 0853 0029 0161 eb02 0000 0a20  .}.|.S.).a..... 
+000011b0: 2020 2043 6f6d 7075 7465 2074 6865 204d     Compute the M
+000011c0: 6178 696d 756d 2043 616c 6962 7261 7469  aximum Calibrati
+000011d0: 6f6e 2045 7272 6f72 2028 4d43 4529 0a20  on Error (MCE). 
+000011e0: 2020 2028 7365 6520 604e 6165 696e 6920     (see `Naeini 
+000011f0: 6574 2061 6c2e 2c20 3230 3135 203c 6874  et al., 2015 <ht
+00001200: 7470 733a 2f2f 7065 6f70 6c65 2e63 732e  tps://people.cs.
+00001210: 7069 7474 2e65 6475 2f7e 6d69 6c6f 732f  pitt.edu/~milos/
+00001220: 7265 7365 6172 6368 2f41 4141 495f 4361  research/AAAI_Ca
+00001230: 6c69 6272 6174 696f 6e2e 7064 663e 605f  libration.pdf>`_
+00001240: 5f29 2e20 4f70 7469 6f6e 616c 6c79 2c20  _). Optionally, 
+00001250: 706c 6f74 0a20 2020 2061 6e64 2073 6176  plot.    and sav
+00001260: 6520 6120 7265 6c69 6162 696c 6974 7920  e a reliability 
+00001270: 6469 6167 7261 6d2e 0a0a 2020 2020 5061  diagram...    Pa
+00001280: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00001290: 2d2d 2d2d 2d2d 2d0a 2020 2020 7072 6564  -------.    pred
+000012a0: 733a 2041 7272 6179 0a20 2020 2020 2020  s: Array.       
+000012b0: 2041 206f 6e65 2d64 696d 656e 7369 6f6e   A one-dimension
+000012c0: 616c 2061 7272 6179 206f 6620 7072 6564  al array of pred
+000012d0: 6963 7469 6f6e 7320 6f76 6572 2074 6865  ictions over the
+000012e0: 2064 6174 6120 706f 696e 7473 2e0a 2020   data points..  
+000012f0: 2020 7072 6f62 733a 2041 7272 6179 0a20    probs: Array. 
+00001300: 2020 2020 2020 2041 2074 776f 2d64 696d         A two-dim
+00001310: 656e 7369 6f6e 616c 2061 7272 6179 206f  ensional array o
+00001320: 6620 636c 6173 7320 7072 6f62 6162 696c  f class probabil
+00001330: 6974 6965 7320 666f 7220 6561 6368 2064  ities for each d
+00001340: 6174 6120 706f 696e 742e 0a20 2020 2074  ata point..    t
+00001350: 6172 6765 7473 3a20 4172 7261 790a 2020  argets: Array.  
+00001360: 2020 2020 2020 4120 6f6e 652d 6469 6d65        A one-dime
+00001370: 6e73 696f 6e61 6c20 6172 7261 7920 6f66  nsional array of
+00001380: 2074 6172 6765 7420 7661 7269 6162 6c65   target variable
+00001390: 732e 0a20 2020 2070 6c6f 743a 2062 6f6f  s..    plot: boo
+000013a0: 6c0a 2020 2020 2020 2020 5768 6574 6865  l.        Whethe
+000013b0: 7220 746f 2070 6c6f 7420 6120 7265 6c69  r to plot a reli
+000013c0: 6162 696c 6974 7920 6469 6167 7261 6d2e  ability diagram.
+000013d0: 0a20 2020 2070 6c6f 745f 6f70 7469 6f6e  .    plot_option
+000013e0: 733a 2064 6963 740a 2020 2020 2020 2020  s: dict.        
+000013f0: 4f70 7469 6f6e 7320 666f 7220 7468 6520  Options for the 
+00001400: 7265 6c69 6162 696c 6974 7920 6469 6167  reliability diag
+00001410: 7261 6d20 706c 6f74 3b20 7365 6520 3a66  ram plot; see :f
+00001420: 756e 633a 607e 666f 7274 756e 612e 706c  unc:`~fortuna.pl
+00001430: 6f74 2e70 6c6f 745f 7265 6c69 6162 696c  ot.plot_reliabil
+00001440: 6974 795f 6469 6167 7261 6d60 2e0a 0a20  ity_diagram`... 
+00001450: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00001460: 2d2d 2d2d 2d2d 0a20 2020 206a 6e70 2e6e  ------.    jnp.n
+00001470: 6461 7272 6179 0a20 2020 2020 2020 2054  darray.        T
+00001480: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00001490: 4d43 452e 0a20 2020 2029 0472 2e00 0000  MCE..    ).r....
+000014a0: 720f 0000 0072 2700 0000 7230 0000 0029  r....r'...r0...)
+000014b0: 0972 0900 0000 7214 0000 0072 0a00 0000  .r....r....r....
+000014c0: 7215 0000 0072 1600 0000 722b 0000 0072  r....r....r+...r
+000014d0: 2d00 0000 722c 0000 00da 036d 6365 7211  -...r,.....mcer.
+000014e0: 0000 0072 1100 0000 7212 0000 00da 196d  ...r....r......m
+000014f0: 6178 696d 756d 5f63 616c 6962 7261 7469  aximum_calibrati
+00001500: 6f6e 5f65 7272 6f72 8d00 0000 730a 0000  on_error....s...
+00001510: 0000 1e02 010a ff0a 0318 0172 3500 0000  ...........r5...
+00001520: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00001530: 0006 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
+00001540: 7c00 7c01 7c02 7c03 7c04 8305 5300 2901  |.|.|.|.|...S.).
+00001550: 7a27 5365 6520 3a66 756e 633a 602e 6d61  z'See :func:`.ma
+00001560: 7869 6d75 6d5f 6361 6c69 6272 6174 696f  ximum_calibratio
+00001570: 6e5f 6572 726f 7260 2e29 0172 3500 0000  n_error`.).r5...
+00001580: 7233 0000 0072 1100 0000 7211 0000 0072  r3...r....r....r
+00001590: 1200 0000 7234 0000 00b2 0000 0073 0200  ....r4.......s..
+000015a0: 0000 0008 7234 0000 0029 0372 1400 0000  ....r4...).r....
+000015b0: 720a 0000 0072 0b00 0000 6302 0000 0000  r....r....c.....
+000015c0: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
+000015d0: 0000 0073 5600 0000 7c00 6a00 6401 6b03  ...sV...|.j.d.k.
+000015e0: 7212 7401 6402 8301 8201 7402 7c01 8301  r.t.d.....t.|...
+000015f0: 7403 6b02 7226 7c01 a004 a100 7d01 7405  t.k.r&|.....}.t.
+00001600: 6a06 a007 7c01 7c00 6a08 6403 1900 a102  j...|.|.j.d.....
+00001610: 7d01 7409 a00a 7409 6a0b 7c00 7c01 1800  }.t...t.j.|.|...
+00001620: 6401 1300 6403 6404 8d02 a101 5300 2905  d...d.d.....S.).
+00001630: 61e0 0100 000a 2020 2020 4272 6965 7220  a.....    Brier 
+00001640: 7363 6f72 6520 2873 6565 2060 4272 6965  score (see `Brie
+00001650: 722c 2031 3935 3020 3c68 7474 7073 3a2f  r, 1950 <https:/
+00001660: 2f77 6562 2e61 7263 6869 7665 2e6f 7267  /web.archive.org
+00001670: 2f77 6562 2f32 3031 3731 3032 3330 3132  /web/20171023012
+00001680: 3733 372f 0a20 2020 2068 7474 7073 3a2f  737/.    https:/
+00001690: 2f64 6f63 732e 6c69 622e 6e6f 6161 2e67  /docs.lib.noaa.g
+000016a0: 6f76 2f72 6573 6375 652f 6d77 722f 3037  ov/rescue/mwr/07
+000016b0: 382f 6d77 722d 3037 382d 3031 2d30 3030  8/mwr-078-01-000
+000016c0: 312e 7064 663e 605f 5f29 2e20 5468 6973  1.pdf>`__). This
+000016d0: 2063 616e 2062 6520 7573 6564 2066 6f72   can be used for
+000016e0: 2062 6f74 6820 6269 6e61 7279 2061 6e64   both binary and
+000016f0: 206d 756c 7469 2d63 6c61 7373 0a20 2020   multi-class.   
+00001700: 2063 6c61 7373 6966 6963 6174 696f 6e2e   classification.
+00001710: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00001720: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00001730: 2020 2020 7072 6f62 733a 2041 7272 6179      probs: Array
+00001740: 0a20 2020 2020 2020 2041 2074 776f 2d64  .        A two-d
+00001750: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
+00001760: 206f 6620 636c 6173 7320 7072 6f62 6162   of class probab
+00001770: 696c 6974 6965 7320 666f 7220 6561 6368  ilities for each
+00001780: 2064 6174 6120 706f 696e 742e 0a20 2020   data point..   
+00001790: 2074 6172 6765 7473 3a20 4172 7261 790a   targets: Array.
+000017a0: 2020 2020 2020 2020 4120 6f6e 652d 6469          A one-di
+000017b0: 6d65 6e73 696f 6e61 6c20 6172 7261 7920  mensional array 
+000017c0: 6f66 2074 6172 6765 7420 7661 7269 6162  of target variab
+000017d0: 6c65 732e 0a0a 2020 2020 5265 7475 726e  les...    Return
+000017e0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+000017f0: 2020 666c 6f61 740a 2020 2020 2020 2020    float.        
+00001800: 5468 6520 4272 6965 7220 7363 6f72 652e  The Brier score.
+00001810: 0a20 2020 2072 1700 0000 7a64 6070 726f  .    r....zd`pro
+00001820: 6273 6020 6d75 7374 2062 6520 6120 7477  bs` must be a tw
+00001830: 6f2d 6469 6d65 6e73 696f 6e61 6c20 6172  o-dimensional ar
+00001840: 7261 7920 6f66 2070 726f 6261 6269 6c69  ray of probabili
+00001850: 7469 6573 2066 6f72 2065 6163 6820 636c  ties for each cl
+00001860: 6173 7320 616e 6420 6561 6368 2064 6174  ass and each dat
+00001870: 610a 2020 2020 2020 2020 706f 696e 742e  a.        point.
+00001880: 720c 0000 0029 01da 0461 7869 7329 0c72  r....)...axis).r
+00001890: 0d00 0000 720e 0000 00da 0474 7970 6572  ....r......typer
+000018a0: 0600 0000 da10 746f 5f61 7272 6179 5f74  ......to_array_t
+000018b0: 6172 6765 7473 da03 6a61 78da 026e 6eda  argets..jax..nn.
+000018c0: 076f 6e65 5f68 6f74 7226 0000 0072 0f00  .one_hotr&...r..
+000018d0: 0000 7210 0000 0072 2f00 0000 2902 7214  ..r....r/...).r.
+000018e0: 0000 0072 0a00 0000 7211 0000 0072 1100  ...r....r....r..
+000018f0: 0000 7212 0000 00da 0b62 7269 6572 5f73  ..r......brier_s
+00001900: 636f 7265 bd00 0000 7310 0000 0000 120a  core....s.......
+00001910: 0102 0102 ff04 040c 0108 0114 0172 3c00  .............r<.
+00001920: 0000 2902 464e 2902 464e 2902 464e 2902  ..).FN).FN).FN).
+00001930: 464e 2902 464e 2919 da06 7479 7069 6e67  FN).FN)...typing
+00001940: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+00001950: 0500 0000 5a06 6a61 782e 6e6e 7239 0000  ....Z.jax.nnr9..
+00001960: 00da 096a 6178 2e6e 756d 7079 da05 6e75  ...jax.numpy..nu
+00001970: 6d70 7972 0f00 0000 da13 666f 7274 756e  mpyr......fortun
+00001980: 612e 6461 7461 2e6c 6f61 6465 7272 0600  a.data.loaderr..
+00001990: 0000 5a0c 666f 7274 756e 612e 706c 6f74  ..Z.fortuna.plot
+000019a0: 7207 0000 00da 0e66 6f72 7475 6e61 2e74  r......fortuna.t
+000019b0: 7970 696e 6772 0800 0000 da07 6e64 6172  ypingr......ndar
+000019c0: 7261 7972 1300 0000 da04 626f 6f6c 722e  rayr......boolr.
+000019d0: 0000 0072 3200 0000 7231 0000 0072 3500  ...r2...r1...r5.
+000019e0: 0000 7234 0000 0072 3c00 0000 7211 0000  ..r4...r<...r...
+000019f0: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00001a00: da08 3c6d 6f64 756c 653e 0100 0000 7372  ..<module>....sr
+00001a10: 0000 0018 0208 010c 020c 010c 010c 0314  ................
+00001a20: 1f00 0100 fb02 0102 0102 0102 0102 0106  ................
+00001a30: 0112 fa0c 3a00 0100 fb02 0102 0102 0102  ....:...........
+00001a40: 0102 0106 0104 fa0c 2a00 0100 fb02 0102  ........*.......
+00001a50: 0102 0102 0102 0106 0104 fa0c 0f00 0100  ................
+00001a60: fb02 0102 0102 0102 0102 0106 0104 fa0c  ................
+00001a70: 2900 0100 fb02 0102 0102 0102 0102 0106  )...............
+00001a80: 0104 fa0c 0b                             .....
```

### Comparing `aws_fortuna-0.1.8/fortuna/metric/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/metric/__pycache__/regression.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jan  6 17:10:57 2023 UTC, .py size: 4892 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2156 b863 1c13 0000  a.......!V.c....
+00000000: 610d 0d0a 0000 0000 79bd c663 1c13 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 6504 6504 6505 6403 9c03  m.Z...e.e.e.d...
 00000050: 6404 6405 8404 5a06 6504 6504 6505 6403  d.d...Z.e.e.e.d.
 00000060: 9c03 6406 6407 8404 5a07 6504 6504 6504  ..d.d...Z.e.e.e.
 00000070: 6403 9c03 6408 6409 8404 5a08 6504 6504  d...d.d...Z.e.e.
@@ -293,17 +293,17 @@
 00001240: 0353 0029 017a 3653 6565 203a 6675 6e63  .S.).z6See :func
 00001250: 3a60 2e70 7265 6469 6374 696f 6e5f 696e  :`.prediction_in
 00001260: 7465 7276 616c 5f63 6f76 6572 6167 655f  terval_coverage_
 00001270: 7072 6f62 6162 696c 6974 7960 2e29 0172  probability`.).r
 00001280: 2000 0000 2903 721a 0000 0072 1b00 0000   ...).r....r....
 00001290: 7204 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
 000012a0: 1000 0000 da04 7069 6370 9a00 0000 7302  ......picp....s.
-000012b0: 0000 0000 0272 2100 0000 2910 5a09 6a61  .....r!...).Z.ja
+000012b0: 0000 0000 0272 2100 0000 2910 da09 6a61  .....r!...)...ja
 000012c0: 782e 6e75 6d70 79da 056e 756d 7079 720a  x.numpy..numpyr.
-000012d0: 0000 005a 0e66 6f72 7475 6e61 2e74 7970  ...Z.fortuna.typ
+000012d0: 0000 00da 0e66 6f72 7475 6e61 2e74 7970  .....fortuna.typ
 000012e0: 696e 6772 0200 0000 da05 666c 6f61 7472  ingr......floatr
 000012f0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
 00001300: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
 00001310: 0000 7219 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
 00001320: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
 00001330: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
 00001340: 0000 0073 1a00 0000 0c02 0c03 1213 1205  ...s............
```

### Comparing `aws_fortuna-0.1.8/fortuna/metric/classification.py` & `aws_fortuna-0.1.9/fortuna/metric/classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     preds: Array
         A one-dimensional array of predictions over the data points.
     targets: Array
         A one-dimensional array of target variables.
 
     Returns
     -------
-    float
+    jnp.ndarray
         The computed accuracy.
     """
     if preds.ndim > 1:
         raise ValueError(
             """`preds` must be a one-dimensional array of predicted classes."""
         )
     if targets.ndim > 1:
@@ -113,31 +113,31 @@
     plot: bool
         Whether to plot a reliability diagram.
     plot_options: dict
         Options for the reliability diagram plot; see :func:`~fortuna.plot.plot_reliability_diagram`.
 
     Returns
     -------
-    float
+    jnp.ndarray
         The value of the ECE.
     """
     counts, confs, accs = compute_counts_confs_accs(
         preds, probs, targets, plot, plot_options
     )
-    ece = jnp.sum(counts * (accs - confs) ** 2) / preds.shape[0]
+    ece = jnp.sum(counts * jnp.abs(accs - confs)) / preds.shape[0]
     return ece
 
 
 def ece(
     preds: Array,
     probs: Array,
     targets: Array,
     plot: bool = False,
     plot_options: Optional[Dict] = None,
-) -> float:
+) -> jnp.ndarray:
     """See :func:`.expected_calibration_error`."""
     return expected_calibration_error(preds, probs, targets, plot, plot_options)
 
 
 def maximum_calibration_error(
     preds: Array,
     probs: Array,
@@ -161,31 +161,31 @@
     plot: bool
         Whether to plot a reliability diagram.
     plot_options: dict
         Options for the reliability diagram plot; see :func:`~fortuna.plot.plot_reliability_diagram`.
 
     Returns
     -------
-    float
+    jnp.ndarray
         The value of the MCE.
     """
     counts, confs, accs = compute_counts_confs_accs(
         preds, probs, targets, plot, plot_options
     )
-    mce = jnp.max(counts * (accs - confs) ** 2)
+    mce = jnp.max(counts * jnp.abs(accs - confs))
     return mce
 
 
 def mce(
     preds: Array,
     probs: Array,
     targets: Array,
     plot: bool = False,
     plot_options: Optional[Dict] = None,
-) -> float:
+) -> jnp.ndarray:
     """See :func:`.maximum_calibration_error`."""
     return maximum_calibration_error(preds, probs, targets, plot, plot_options)
 
 
 def brier_score(probs: Array, targets: Union[TargetsLoader, Array]) -> jnp.ndarray:
     """
     Brier score (see `Brier, 1950 <https://web.archive.org/web/20171023012737/
@@ -197,15 +197,15 @@
     probs: Array
         A two-dimensional array of class probabilities for each data point.
     targets: Array
         A one-dimensional array of target variables.
 
     Returns
     -------
-    float
+    jnp.ndarray
         The Brier score.
     """
     if probs.ndim != 2:
         raise ValueError(
             """`probs` must be a two-dimensional array of probabilities for each class and each data
         point."""
         )
```

### Comparing `aws_fortuna-0.1.8/fortuna/metric/regression.py` & `aws_fortuna-0.1.9/fortuna/metric/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/.DS_Store` & `aws_fortuna-0.1.9/fortuna/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/__pycache__/cnn.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/__pycache__/cnn.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/__pycache__/lenet.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/__pycache__/lenet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/__pycache__/linear.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/__pycache__/linear.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jan  5 10:54:40 2023 UTC, .py size: 400 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 70ac b663 9001 0000  a.......p..c....
+00000000: 610d 0d0a 0000 0000 79bd c663 9001 0000  a.......y..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a05 0100 6400 6402 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6502 6a08  ..G.d.d...d.e.j.
 00000060: 8303 5a09 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da05 4172 7261 7963 0000 0000 0000  )...Arrayc......
```

### Comparing `aws_fortuna-0.1.8/fortuna/model/__pycache__/mlp.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/__pycache__/mlp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/__pycache__/resnet.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/__pycache__/resnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/__pycache__/wideresnet.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/__pycache__/wideresnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/cnn.py` & `aws_fortuna-0.1.9/fortuna/model/cnn.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/lenet.py` & `aws_fortuna-0.1.9/fortuna/model/lenet.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/mlp.py` & `aws_fortuna-0.1.9/fortuna/model/mlp.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/.DS_Store` & `aws_fortuna-0.1.9/fortuna/model/model_manager/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/__pycache__/state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/model/model_manager/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/base.py` & `aws_fortuna-0.1.9/fortuna/model/model_manager/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/classification.py` & `aws_fortuna-0.1.9/fortuna/model/model_manager/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/regression.py` & `aws_fortuna-0.1.9/fortuna/model/model_manager/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/model_manager/state.py` & `aws_fortuna-0.1.9/fortuna/model/model_manager/state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/resnet.py` & `aws_fortuna-0.1.9/fortuna/model/resnet.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/model/wideresnet.py` & `aws_fortuna-0.1.9/fortuna/model/wideresnet.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/.DS_Store` & `aws_fortuna-0.1.9/fortuna/output_calibrator/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/output_calibrator/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/output_calibrator/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/classification.py` & `aws_fortuna-0.1.9/fortuna/output_calibrator/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/.DS_Store` & `aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/__pycache__/state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/base.py` & `aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/output_calib_manager/state.py` & `aws_fortuna-0.1.9/fortuna/output_calibrator/output_calib_manager/state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/output_calibrator/regression.py` & `aws_fortuna-0.1.9/fortuna/output_calibrator/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/plot.py` & `aws_fortuna-0.1.9/fortuna/plot.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/prob_model_calibrator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/prob_model_calibrator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/__init__.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/checkpointer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/checkpointer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/monitor.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/monitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/optimizer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/optimizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/__pycache__/processor.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/__pycache__/processor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/checkpointer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/checkpointer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/monitor.py` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/monitor.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/optimizer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/optimizer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/calib_config/processor.py` & `aws_fortuna-0.1.9/fortuna/prob_model/calib_config/processor.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/classification.py` & `aws_fortuna-0.1.9/fortuna/prob_model/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/__init__.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/checkpointer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/checkpointer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/monitor.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/monitor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/optimizer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/optimizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/__pycache__/processor.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/__pycache__/processor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/checkpointer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/checkpointer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/monitor.py` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/monitor.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/optimizer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/optimizer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/fit_config/processor.py` & `aws_fortuna-0.1.9/fortuna/prob_model/fit_config/processor.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/joint/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/joint/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/joint/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/joint/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/joint/__pycache__/state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/joint/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/joint/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/joint/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/joint/state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/joint/state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/classification.py` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/likelihood/regression.py` & `aws_fortuna-0.1.9/fortuna/prob_model/likelihood/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__init__.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/__init__.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/name_to_posterior_state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/name_to_posterior_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_approximations.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_approximations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_mixin.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_mixin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/posterior_state_repository.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/posterior_state_repository.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/__pycache__/state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_approximator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_approximator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_posterior.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_posterior.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_repositories.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/__pycache__/deep_ensemble_repositories.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_approximator.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_approximator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_posterior.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_posterior.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_repositories.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/deep_ensemble/deep_ensemble_repositories.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/laplace_approximator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/laplace_approximator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/laplace_posterior.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/laplace_posterior.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/__pycache__/laplace_state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/__pycache__/laplace_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/laplace_approximator.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/laplace_approximator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/laplace_posterior.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/laplace_posterior.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/laplace/laplace_state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/laplace/laplace_state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_approximator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_approximator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_posterior.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_posterior.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/__pycache__/map_trainer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/__pycache__/map_trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/map_posterior.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/map_posterior.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/map/map_trainer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/map/map_trainer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/name_to_posterior_state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/name_to_posterior_state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/__pycache__/normalizing_flow_trainer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/__pycache__/normalizing_flow_trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_approximator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_approximator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_architecture.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_architecture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_posterior.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_posterior.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_trainer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/__pycache__/advi_trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_approximator.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_approximator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_architecture.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_architecture.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_posterior.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_posterior.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/advi/advi_state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/advi/advi_state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/normalizing_flow/normalizing_flow_trainer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/normalizing_flow/normalizing_flow_trainer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_approximations.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_approximations.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_mixin.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_mixin.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/posterior_state_repository.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/posterior_state_repository.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_approximator.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_approximator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_posterior.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_posterior.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/__pycache__/swag_trainer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/__pycache__/swag_trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_approximator.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_approximator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_posterior.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_posterior.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/posterior/swag/swag_trainer.py` & `aws_fortuna-0.1.9/fortuna/prob_model/posterior/swag/swag_trainer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/classification.py` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/predictive/regression.py` & `aws_fortuna-0.1.9/fortuna/prob_model/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/prior/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_model/prior/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/prior/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/prior/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/prior/__pycache__/gaussian.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_model/prior/__pycache__/gaussian.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/prior/base.py` & `aws_fortuna-0.1.9/fortuna/prob_model/prior/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/prior/gaussian.py` & `aws_fortuna-0.1.9/fortuna/prob_model/prior/gaussian.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/prob_model_calibrator.py` & `aws_fortuna-0.1.9/fortuna/prob_model/prob_model_calibrator.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/regression.py` & `aws_fortuna-0.1.9/fortuna/prob_model/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_model/state.py` & `aws_fortuna-0.1.9/fortuna/prob_model/state.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/.DS_Store` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/base.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/classification.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/classification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/__pycache__/regression.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/__pycache__/regression.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/base.py` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/base.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/classification.py` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/classification.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/prob_output_layer/regression.py` & `aws_fortuna-0.1.9/fortuna/prob_output_layer/regression.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/.DS_Store` & `aws_fortuna-0.1.9/fortuna/training/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/__pycache__/mixin.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/training/__pycache__/mixin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/__pycache__/train_state.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/training/__pycache__/train_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/__pycache__/train_state_repository.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/training/__pycache__/train_state_repository.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/__pycache__/trainer.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/training/__pycache__/trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/mixin.py` & `aws_fortuna-0.1.9/fortuna/training/mixin.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/train_state_repository.py` & `aws_fortuna-0.1.9/fortuna/training/train_state_repository.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/training/trainer.py` & `aws_fortuna-0.1.9/fortuna/training/trainer.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/typing.py` & `aws_fortuna-0.1.9/fortuna/typing.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/.DS_Store` & `aws_fortuna-0.1.9/fortuna/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/__pycache__/builtins.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/utils/__pycache__/builtins.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/__pycache__/data.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/utils/__pycache__/data.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/__pycache__/device.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/utils/__pycache__/device.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/__pycache__/nested_dicts.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/utils/__pycache__/nested_dicts.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/__pycache__/random.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/utils/__pycache__/random.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/__pycache__/strings.cpython-39.pyc` & `aws_fortuna-0.1.9/fortuna/utils/__pycache__/strings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/builtins.py` & `aws_fortuna-0.1.9/fortuna/utils/builtins.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/data.py` & `aws_fortuna-0.1.9/fortuna/utils/data.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/device.py` & `aws_fortuna-0.1.9/fortuna/utils/device.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/nested_dicts.py` & `aws_fortuna-0.1.9/fortuna/utils/nested_dicts.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/fortuna/utils/random.py` & `aws_fortuna-0.1.9/fortuna/utils/random.py`

 * *Files identical despite different names*

### Comparing `aws_fortuna-0.1.8/pyproject.toml` & `aws_fortuna-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-fortuna"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Library for Uncertainty Quantification."
 authors = ["Gianluca Detommaso <gianluca.detommaso@gmail.com>", "Alberto Gasparin <albgas@amazon.de>"]
 license = "Apache-2.0"
 readme = "README.rst"
 documentation = "https://aws-fortuna.readthedocs.io/en/latest/"
 packages = [{include = "fortuna"}]
```

### Comparing `aws_fortuna-0.1.8/setup.py` & `aws_fortuna-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
           'sphinx-gallery>=0.11.1,<0.12.0',
           'pydata-sphinx-theme>=0.12.0,<0.13.0',
           'ipython>=8.7.0,<9.0.0'],
  'notebooks': ['jupyter>=1.0.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'aws-fortuna',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A Library for Uncertainty Quantification.',
     'long_description': 'Fortuna\n#######\n\n.. image:: https://img.shields.io/pypi/status/Fortuna\n    :target: https://img.shields.io/pypi/status/Fortuna\n    :alt: PyPI - Status\n.. image:: https://img.shields.io/pypi/dm/aws-fortuna\n    :target: https://pypistats.org/packages/aws-fortuna\n    :alt: PyPI - Downloads\n.. image:: https://img.shields.io/pypi/v/aws-fortuna\n    :target: https://img.shields.io/pypi/v/aws-fortuna\n    :alt: PyPI - Version\n.. image:: https://img.shields.io/github/license/awslabs/Fortuna\n    :target: https://github.com/awslabs/Fortuna/blob/main/LICENSE\n    :alt: License\n.. image:: https://readthedocs.org/projects/aws-fortuna/badge/?version=latest\n    :target: https://aws-fortuna.readthedocs.io\n    :alt: Documentation Status\n\nA Library for Uncertainty Quantification\n========================================\nProper estimation of predictive uncertainty is fundamental in applications that involve critical decisions.\nUncertainty can be used to assess reliability of model predictions, trigger human intervention,\nor decide whether a model can be safely deployed in the wild.\n\nFortuna is a library for uncertainty quantification that makes it easy for users to run benchmarks and bring uncertainty to production systems.\nFortuna provides calibration and conformal methods starting from pre-trained models written in any framework,\nand it further supports several Bayesian inference methods starting from deep learning models written in `Flax <https://flax.readthedocs.io/en/latest/index.html>`_.\nThe language is designed to be intuitive for practitioners unfamiliar with uncertainty quantification,\nand is highly configurable.\n\nCheck the `documentation <https://aws-fortuna.readthedocs.io/en/latest/>`_ for a quickstart, examples and references.\n\nUsage modes\n===========\nFortuna offers three different usage modes:\n`From uncertainty estimates <https://github.com/awslabs/fortuna#from-uncertainty-estimates>`_,\n`From model outputs <https://github.com/awslabs/fortuna#from-model-outputs>`_ and\n`From Flax models <https://github.com/awslabs/fortuna#from-flax-models>`_.\nThese serve users according to the constraints dictated by their own applications.\nTheir pipelines are depicted in the following figure, each starting from one of the green panels.\n\n.. image:: https://github.com/awslabs/fortuna/raw/main/docs/source/_static/pipeline.png\n    :target: https://github.com/awslabs/fortuna/raw/main/docs/source/_static/pipeline.png\n\nFrom uncertainty estimates\n---------------------------\nStarting from uncertainty estimates has minimal compatibility requirements and it is the quickest level of interaction with the library.\nThis usage mode offers conformal prediction methods for both classification and regression.\nThese take uncertainty estimates in input,\nand return rigorous sets of predictions that retain a user-given level of probability.\nIn one-dimensional regression tasks, conformal sets may be thought as calibrated versions of confidence or credible intervals.\n\nMind that if the uncertainty estimates that you provide in inputs are inaccurate,\nconformal sets might be large and unusable.\nFor this reason, if your application allows it,\nplease consider the `From model outputs <https://github.com/awslabs/fortuna#from-model-outputs>`_ and\n`From Flax models <https://github.com/awslabs/fortuna#from-flax-models>`_ usage modes.\n\n**Example.** Suppose you want to calibrate credible intervals with coverage error :code:`error`,\neach corresponding to a different test input variable.\nWe assume that credible intervals are passed as arrays of lower and upper bounds,\nrespectively :code:`test_lower_bounds` and :code:`test_upper_bounds`.\nYou also have lower and upper bounds of credible intervals computed for several validation inputs,\nrespectively :code:`val_lower_bounds` and :code:`val_upper_bounds`.\nThe corresponding array of validation targets is denoted by :code:`val_targets`.\nThe following code produces *conformal prediction intervals*,\ni.e. calibrated versions of you test credible intervals.\n\n.. code-block:: python\n\n from fortuna.conformal.regression import QuantileConformalRegressor\n conformal_intervals = QuantileConformalRegressor().conformal_interval(\n      val_lower_bounds=val_lower_bounds, val_upper_bounds=val_upper_bounds,\n      test_lower_bounds=test_lower_bounds, test_upper_bounds=test_upper_bounds,\n      val_targets=val_targets, error=error)\n\nFrom model outputs\n------------------\nStarting from model outputs assumes you have already trained a model in some framework,\nand arrive to Fortuna with model outputs in :code:`numpy.ndarray` format for each input data point.\nThis usage mode allows you to calibrate your model outputs, estimate uncertainty,\ncompute metrics and obtain conformal sets.\n\nCompared to the `From uncertainty estimates <https://github.com/awslabs/fortuna#from-uncertainty-estimates>`_ usage mode,\nthis one offers better control,\nas it can make sure uncertainty estimates have been appropriately calibrated.\nHowever, if the model had been trained with classical methods,\nthe resulting quantification of model (a.k.a. epistemic) uncertainty may be poor.\nTo mitigate this problem, please consider the `From Flax models <https://github.com/awslabs/fortuna#from-flax-models>`_\nusage mode.\n\n**Example.**\nSuppose you have validation and test model outputs,\nrespectively :code:`val_outputs` and :code:`test_outputs`.\nFurthermore, you have some arrays of validation and target variables,\nrespectively :code:`val_targets` and :code:`test_targets`.\nThe following code provides a minimal classification example to get calibrated predictive entropy estimates.\n\n.. code-block:: python\n\n  from fortuna.calib_model import CalibClassifier\n  calib_model = CalibClassifier()\n  status = calib_model.calibrate(outputs=val_outputs, targets=val_targets)\n  test_entropies = calib_model.predictive.entropy(outputs=test_outputs)\n\nFrom Flax models\n--------------------------\nStarting from Flax models has higher compatibility requirements than the\n`From uncertainty estimates <https://github.com/awslabs/fortuna#from-uncertainty-estimates>`_\nand `From model outputs <https://github.com/awslabs/fortuna#from-model-outputs>`_ usage modes,\nas it requires deep learning models written in `Flax <https://flax.readthedocs.io/en/latest/index.html>`_.\nHowever, it enables you to replace standard model training with scalable Bayesian inference procedures,\nwhich may significantly improve the quantification of predictive uncertainty.\n\n**Example.** Suppose you have a Flax classification deep learning model :code:`model` from inputs to logits, with output\ndimension given by :code:`output_dim`. Furthermore,\nyou have some training, validation and calibration TensorFlow data loader :code:`train_data_loader`, :code:`val_data_loader`\nand :code:`test_data_loader`, respectively.\nThe following code provides a minimal classification example to get calibrated probability estimates.\n\n.. code-block:: python\n\n  from fortuna.data import DataLoader\n  train_data_loader = DataLoader.from_tensorflow_data_loader(train_data_loader)\n  calib_data_loader = DataLoader.from_tensorflow_data_loader(val_data_loader)\n  test_data_loader = DataLoader.from_tensorflow_data_loader(test_data_loader)\n\n  from fortuna.prob_model import ProbClassifier\n  prob_model = ProbClassifier(model=model)\n  status = prob_model.train(train_data_loader=train_data_loader, calib_data_loader=calib_data_loader)\n  test_means = prob_model.predictive.mean(inputs_loader=test_data_loader.to_inputs_loader())\n\n\nInstallation\n============\n**NOTE:** Before installing Fortuna, you are required to `install JAX <https://github.com/google/jax#installation>`_ in your virtual environment.\n\nYou can install Fortuna by typing\n\n.. code-block::\n\n    pip install aws-fortuna\n\nAlternatively, you can build the package using `Poetry <https://python-poetry.org/docs/>`_.\nIf you choose to pursue this way, first install Poetry and add it to your PATH\n(see `here <https://python-poetry.org/docs/#installation>`_). Then type\n\n.. code-block::\n\n    poetry install\n\nAll the dependecies will be installed at their required versions.\nIf you also want to install the optional Sphinx dependencies to build the documentation,\nadd the flag :code:`-E docs` to the command above.\nFinally, you can either access the virtualenv that Poetry created by typing :code:`poetry shell`,\nor execute commands within the virtualenv using the :code:`run` command, e.g. :code:`poetry run python`.\n\nExamples\n========\nSeveral usage examples are found in the\n`/examples <https://github.com/awslabs/fortuna/tree/main/examples>`_\ndirectory.\n\nMaterial\n========\n- `AWS launch blog post <https://aws.amazon.com/blogs/machine-learning/introducing-fortuna-a-library-for-uncertainty-quantification/>`_\n\nContributing\n============\nIf you wish to contribute to the project, please refer to our `contribution guidelines <https://github.com/awslabs/fortuna/blob/main/CONTRIBUTING.md>`_.\n\n\nLicense\n=======\nThis project is licensed under the Apache-2.0 License.\nSee `LICENSE <https://github.com/awslabs/fortuna/blob/main/LICENSE>`_ for more information.\n',
     'author': 'Gianluca Detommaso',
     'author_email': 'gianluca.detommaso@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aws_fortuna-0.1.8/PKG-INFO` & `aws_fortuna-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-fortuna
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Library for Uncertainty Quantification.
 License: Apache-2.0
 Author: Gianluca Detommaso
 Author-email: gianluca.detommaso@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


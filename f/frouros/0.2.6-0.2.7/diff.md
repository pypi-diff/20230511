# Comparing `tmp/frouros-0.2.6.tar.gz` & `tmp/frouros-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.2.6.tar", last modified: Sun Apr 30 10:27:29 2023, max compression
+gzip compressed data, was "frouros-0.2.7.tar", last modified: Thu May 11 14:08:52 2023, max compression
```

## Comparing `frouros-0.2.6.tar` & `frouros-0.2.7.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-04-30 10:27:15.000000 frouros-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-30 10:27:15.000000 frouros-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-30 10:27:29.016097 frouros-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-04-30 10:27:15.000000 frouros-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     4933 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/concept_drift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.012097 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8231 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8943 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14872 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.016097 frouros-0.2.6/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21066 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-04-30 10:27:15.000000 frouros-0.2.6/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 10:27:29.008097 frouros-0.2.6/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-04-30 10:27:28.000000 frouros-0.2.6/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-04-30 10:27:29.000000 frouros-0.2.6/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 10:27:28.000000 frouros-0.2.6/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 10:27:28.000000 frouros-0.2.6/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-30 10:27:28.000000 frouros-0.2.6/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-30 10:27:28.000000 frouros-0.2.6/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-30 10:27:15.000000 frouros-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 10:27:29.016097 frouros-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-04-30 10:27:15.000000 frouros-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.642778 frouros-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-11 14:08:39.000000 frouros-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-11 14:08:39.000000 frouros-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-05-11 14:08:52.642778 frouros-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-05-11 14:08:39.000000 frouros-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.630777 frouros-0.2.7/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/reset_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6385 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.642778 frouros-0.2.7/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7352 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-05-11 14:08:39.000000 frouros-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 14:08:52.642778 frouros-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-05-11 14:08:39.000000 frouros-0.2.7/setup.py
```

### Comparing `frouros-0.2.6/LICENSE` & `frouros-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/PKG-INFO` & `frouros-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library for drift detection in Machine Learning problems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.2.6 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.7 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.6/README.md` & `frouros-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/base.py` & `frouros-0.2.7/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/batch/base.py` & `frouros-0.2.7/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/batch/permutation_test.py` & `frouros-0.2.7/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/batch/reset_drift.py` & `frouros-0.2.7/frouros/callbacks/batch/reset_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/streaming/base.py` & `frouros-0.2.7/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/streaming/history.py` & `frouros-0.2.7/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.2.7/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/datasets/base.py` & `frouros-0.2.7/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/datasets/real.py` & `frouros-0.2.7/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/datasets/synthetic.py` & `frouros-0.2.7/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/base.py` & `frouros-0.2.7/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/__init__.py` & `frouros-0.2.7/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/base.py` & `frouros-0.2.7/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/base.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/__init__.py` & `frouros-0.2.7/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/base.py` & `frouros-0.2.7/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/base.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """MMD (Maximum Mean Discrepancy) module."""
 
 import itertools
 import math
-from typing import Callable, Iterator, Optional, List, Union
+from typing import Callable, Generator, Optional, List, Union
 
 import numpy as np  # type: ignore
-from scipy.spatial.distance import cdist  # type: ignore
 import tqdm  # type: ignore
+from scipy.spatial.distance import cdist  # type: ignore
 
 from frouros.callbacks import Callback
 from frouros.detectors.data_drift.base import MultivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     DistanceBasedBase,
     DistanceResult,
 )
@@ -65,16 +65,17 @@
                 "kernel": kernel,
             },
             callbacks=callbacks,
         )
         self.kernel = kernel
         self.chunk_size = chunk_size
         self._chunk_size_x = None
-        self._expected_k_x = None
-        self._X_num_samples = None
+        self.X_chunks_combinations = None
+        self.X_num_samples = None
+        self.expected_k_xx = None
 
     @property
     def chunk_size(self) -> Optional[int]:
         """Chunk size property.
 
         :return: chunk size to use
         :rtype: int
@@ -133,53 +134,57 @@
         X: np.ndarray,  # noqa: N803
         **kwargs,
     ) -> None:
         super()._fit(X=X)
         # Add dimension only for the kernel calculation (if dim == 1)
         if X.ndim == 1:
             X = np.expand_dims(X, axis=1)  # noqa: N806
-        self._X_num_samples = len(X)  # type: ignore # noqa: N806
+        self.X_num_samples = len(self.X_ref)  # type: ignore # noqa: N806
 
         self._chunk_size_x = (
-            self._X_num_samples
+            self.X_num_samples
             if self.chunk_size is None
             else self.chunk_size  # type: ignore
         )
 
         X_chunks = self._get_chunks(  # noqa: N806
             data=X,
             chunk_size=self._chunk_size_x,  # type: ignore
         )
-        X_chunks_combinations = itertools.product(X_chunks, repeat=2)  # noqa: N806
+        xx_chunks_combinations = itertools.product(X_chunks, repeat=2)  # noqa: N806
 
         if kwargs.get("verbose", False):
             num_chunks = (
-                math.ceil(self._X_num_samples / self._chunk_size_x) ** 2  # type: ignore
+                math.ceil(self.X_num_samples / self._chunk_size_x) ** 2  # type: ignore
             )
-            k_x_sum = np.array(
-                [
-                    self.kernel(*X_chunk).sum()
-                    for X_chunk in tqdm.tqdm(  # noqa: N806
-                        X_chunks_combinations, total=num_chunks  # noqa: N806
-                    )
-                ]
-            ).sum()
-        else:
-            k_x_sum = np.array(
-                [
-                    self.kernel(*X_chunk).sum()
-                    for X_chunk in X_chunks_combinations  # noqa: N806
-                ]
-            ).sum()
-        self._expected_k_x = k_x_sum / (
-            self._X_num_samples * (self._X_num_samples - 1)  # type: ignore
+            xx_chunks_combinations = tqdm.tqdm(
+                xx_chunks_combinations,
+                total=num_chunks,
+            )
+
+        k_xx_sum = (
+            self._compute_kernel(
+                chunk_combinations=xx_chunks_combinations,  # type: ignore
+                kernel=self.kernel,
+            )
+            # Remove diagonal (j!=i case)
+            - self.X_num_samples  # type: ignore
+        )
+
+        self.expected_k_xx = k_xx_sum / (  # type: ignore
+            self.X_num_samples * (self.X_num_samples - 1)  # type: ignore
         )
 
     @staticmethod
-    def _get_chunks(data: np.ndarray, chunk_size: int) -> Iterator:
+    def _compute_kernel(chunk_combinations: Generator, kernel: Callable) -> float:
+        k_sum = np.array([kernel(*chunk).sum() for chunk in chunk_combinations]).sum()
+        return k_sum
+
+    @staticmethod
+    def _get_chunks(data: np.ndarray, chunk_size: int) -> Generator:
         chunks = (
             data[i : i + chunk_size]  # noqa: E203
             for i in range(0, len(data), chunk_size)
         )
         return chunks
 
     def _mmd(  # pylint: disable=too-many-locals
@@ -195,67 +200,58 @@
             X = np.expand_dims(X, axis=1)  # noqa: N806
             Y = np.expand_dims(Y, axis=1)  # noqa: N806
 
         X_chunks = self._get_chunks(  # noqa: N806
             data=X,
             chunk_size=self._chunk_size_x,  # type: ignore
         )
-        Y_num_samples = len(Y)  # noqa: N806
-        chunk_size_y = Y_num_samples if self.chunk_size is None else self.chunk_size
-        Y_chunks, Y_chunks_copy = itertools.tee(  # noqa: N806
+        y_num_samples = len(Y)  # noqa: N806
+        chunk_size_y = y_num_samples if self.chunk_size is None else self.chunk_size
+        y_chunks, y_chunks_copy = itertools.tee(  # noqa: N806
             self._get_chunks(
                 data=Y,
                 chunk_size=chunk_size_y,  # type: ignore
             ),
             2,
         )
-        Y_chunks_combinations = itertools.product(  # noqa: N806
-            Y_chunks,
+        y_chunks_combinations = itertools.product(  # noqa: N806
+            y_chunks,
             repeat=2,
         )
-        XY_chunks_combinations = itertools.product(  # noqa: N806
+        xy_chunks_combinations = itertools.product(  # noqa: N806
             X_chunks,
-            Y_chunks_copy,
+            y_chunks_copy,
         )
 
         if kwargs.get("verbose", False):
-            num_chunks_y = math.ceil(Y_num_samples / self.chunk_size)  # type: ignore
+            num_chunks_y = math.ceil(y_num_samples / chunk_size_y)  # type: ignore
             num_chunks_y_combinations = num_chunks_y**2
             num_chunks_xy = (
                 math.ceil(len(X) / self._chunk_size_x) * num_chunks_y  # type: ignore
             )
-            sum_y = np.array(
-                [
-                    kernel(*Y_chunk).sum()
-                    for Y_chunk in tqdm.tqdm(  # noqa: N806
-                        Y_chunks_combinations, total=num_chunks_y_combinations
-                    )
-                ]
-            ).sum()
-            sum_xy = np.array(
-                [
-                    kernel(*XY_chunk).sum()
-                    for XY_chunk in tqdm.tqdm(  # noqa: N806
-                        XY_chunks_combinations, total=num_chunks_xy
-                    )
-                ]
-            ).sum()
-        else:
-            sum_y = np.array(
-                [
-                    kernel(*Y_chunk).sum()
-                    for Y_chunk in Y_chunks_combinations  # noqa: N806
-                ]
-            ).sum()
-            sum_xy = np.array(
-                [
-                    kernel(*XY_chunk).sum()
-                    for XY_chunk in XY_chunks_combinations  # noqa: N806
-                ]
-            ).sum()
+            y_chunks_combinations = tqdm.tqdm(
+                y_chunks_combinations,
+                total=num_chunks_y_combinations,
+            )
+            xy_chunks_combinations = tqdm.tqdm(
+                xy_chunks_combinations,
+                total=num_chunks_xy,
+            )
 
+        k_yy_sum = (
+            self._compute_kernel(
+                chunk_combinations=y_chunks_combinations,  # type: ignore
+                kernel=kernel,
+            )
+            # Remove diagonal (j!=i case)
+            - y_num_samples  # type: ignore
+        )
+        k_xy_sum = self._compute_kernel(
+            chunk_combinations=xy_chunks_combinations,  # type: ignore
+            kernel=kernel,
+        )
         mmd = (
-            self._expected_k_x
-            + sum_y / (Y_num_samples * (Y_num_samples - 1))
-            - 2 * sum_xy / (self._X_num_samples * Y_num_samples)  # type: ignore
+            self.expected_k_xx  # type: ignore
+            + k_yy_sum / (y_num_samples * (y_num_samples - 1))
+            - 2 * k_xy_sum / (self.X_num_samples * y_num_samples)  # type: ignore
         )
         return mmd
```

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.2.7/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """MMD (Maximum Mean Discrepancy) module."""
 
-from typing import Callable, Optional, List, Union
+from typing import Any, Callable, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 
 from frouros.callbacks import Callback
+from frouros.detectors.data_drift.base import NumericalData, MultivariateData
 from frouros.detectors.data_drift.batch import MMD as MMDBatch  # noqa: N811
 from frouros.detectors.data_drift.batch.distance_based.mmd import rbf_kernel
-from frouros.detectors.data_drift.base import NumericalData, MultivariateData
 from frouros.detectors.data_drift.streaming.distance_based.base import (
     DistanceBasedBase,
     DistanceResult,
 )
 from frouros.utils.data_structures import CircularQueue
 
 
@@ -23,29 +23,29 @@
     .. [gretton2012kernel] Gretton, Arthur, et al.
         "A kernel two-sample test."
         The Journal of Machine Learning Research 13.1 (2012): 723-773.
     """
 
     def __init__(
         self,
+        window_size: int,
         kernel: Callable = rbf_kernel,
         chunk_size: Optional[int] = None,
         callbacks: Optional[Union[Callback, List[Callback]]] = None,
-        window_size: int = 10,
     ) -> None:
         """Init method.
 
+        :param window_size: window size
+        :type window_size: int
         :param kernel: kernel function
         :type kernel: Callable
         :param chunk_size: chunk size value
         :type chunk_size: Optional[int]
         :param callbacks: callbacks
         :type callbacks: Optional[Union[Callback, List[Callback]]]
-        :param window_size: window size
-        :type window_size: int
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=MultivariateData(),
             callbacks=callbacks,
         )
         self.mmd = MMDBatch(
@@ -77,18 +77,25 @@
         self._window_size = value
 
     def _fit(self, X: np.ndarray) -> None:  # noqa: N803
         self.mmd.fit(X=X)
         self.X_ref = self.mmd.X_ref
 
     def _reset(self) -> None:
+        super()._reset()
         self.mmd.reset()
 
     def _update(self, value: Union[int, float]) -> Optional[DistanceResult]:
         self.X_queue.enqueue(value=value)
 
         if self.num_instances < self.window_size:
             return None
 
         # FIXME: Handle callback logs. Now are ignored.  # pylint: disable=fixme
         distance, _ = self.mmd.compare(X=np.array(self.X_queue))
         return distance
+
+    def _compare(
+        self,
+        X: np.ndarray,  # noqa: N803
+    ) -> Tuple[Optional[DistanceResult], Dict[str, Any]]:  # noqa: N803
+        return self.mmd.compare(X=X)
```

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/metrics/base.py` & `frouros-0.2.7/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/metrics/prequential_error.py` & `frouros-0.2.7/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/tests/conftest.py` & `frouros-0.2.7/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/tests/integration/test_callback.py` & `frouros-0.2.7/frouros/tests/integration/test_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     [
         (BhattacharyyaDistance, 0.55516059, 0.0),
         (EMD, 3.85346006, 0.0),
         (HellingerDistance, 0.74509099, 0.0),
         (HINormalizedComplement, 0.78, 0.0),
         (JS, 0.67010107, 0.0),
         (KL, np.inf, 0.0),
-        (MMD, 0.71529206, 0.0),
+        (MMD, 0.69509004, 0.0),
         (PSI, 461.20379435, 0.0),
     ],
 )
 def test_batch_permutation_test_data_univariate_different_distribution(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,
     detector_class: DataDriftBatchBase,
@@ -238,15 +238,15 @@
 @pytest.mark.parametrize(
     "detector_class,"
     " expected_drift_idx,"
     " expected_distance_mean,"
     " expected_p_value,"
     " expected_likelihood",
     [
-        (MMDStreaming, 31, 0.34147982, 0.0487643, 20.50680424),
+        (MMDStreaming, 5, 0.27193007, 0.00989585, 101.05240437),
     ],
 )
 def test_streaming_msprt_multivariate_different_distribution(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,
     detector_class: DataDriftBatchBase,
     expected_drift_idx: int,
@@ -269,30 +269,32 @@
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     :param expected_likelihood: expected likelihood value
     :type expected_likelihood: float
     """
     np.random.seed(seed=31)
 
-    alpha = 0.05
+    alpha = 0.01
 
     detector = detector_class(  # type: ignore
         callbacks=mSPRT(
             alpha=alpha,
-            sigma=0.5,
+            sigma=1,
+            tau=1,
+            lambda_=32,
         ),
         window_size=5,
     )
     _ = detector.fit(X=X_ref_multivariate)
 
     drift_idx = -1
     for i, sample in enumerate(X_test_multivariate, start=1):
         value, callbacks_logs = detector.update(value=sample)
         if value is not None:
             if callbacks_logs["mSPRT"]["p_value"] < alpha:
                 drift_idx = i
                 break
 
-    assert np.isclose(drift_idx, expected_drift_idx)
+    assert drift_idx == expected_drift_idx
     assert np.isclose(callbacks_logs["mSPRT"]["distance_mean"], expected_distance_mean)
     assert np.isclose(callbacks_logs["mSPRT"]["p_value"], expected_p_value)
     assert np.isclose(callbacks_logs["mSPRT"]["likelihood"], expected_likelihood)
```

### Comparing `frouros-0.2.6/frouros/tests/integration/test_concept_drift.py` & `frouros-0.2.7/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/tests/integration/test_data_drift.py` & `frouros-0.2.7/frouros/tests/integration/test_data_drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     _ = detector.fit(X=X_ref[:, 0])
     (statistic, p_value), _ = detector.compare(X=X_test[:, 0])
 
     assert np.isclose(statistic, expected_statistic)
     assert np.isclose(p_value, expected_p_value)
 
 
-@pytest.mark.parametrize("detector, expected_distance", [(MMD(), 0.12183835)])
+@pytest.mark.parametrize("detector, expected_distance", [(MMD(), 0.10163633)])
 def test_batch_distance_based_multivariate_different_distribution(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,  # noqa: N803
     detector: DataDriftBatchBase,
     expected_distance: float,
 ) -> None:
     """Test batch distance based multivariate different distribution method.
@@ -210,15 +210,15 @@
     """
     _ = detector.fit(X=X_ref_multivariate)
     statistic, _ = detector.compare(X=X_test_multivariate)
 
     assert np.isclose(statistic, expected_distance)
 
 
-@pytest.mark.parametrize("detector, expected_distance", [(MMD(), 0.03590599)])
+@pytest.mark.parametrize("detector, expected_distance", [(MMD(), 0.01570397)])
 def test_batch_distance_based_multivariate_same_distribution(
     multivariate_distribution_p: Tuple[np.ndarray, np.ndarray],
     detector: DataDriftBatchBase,
     expected_distance: float,
     num_samples: int = 100,
 ) -> None:
     """Test batch distance based multivariate same distribution method.
@@ -244,15 +244,15 @@
     statistic, _ = detector.compare(X=X_test)
 
     assert np.isclose(statistic, expected_distance)
 
 
 @pytest.mark.parametrize(
     "detector, expected_distance",
-    [(MMD(chunk_size=10), 0.12183835), (MMD(chunk_size=None), 0.12183835)],
+    [(MMD(chunk_size=10), 0.10163633), (MMD(chunk_size=None), 0.10163633)],
 )
 def test_batch_distance_based_chunk_size_valid(
     X_ref_multivariate: np.ndarray,  # noqa: N803
     X_test_multivariate: np.ndarray,  # noqa: N803
     detector: DataDriftBatchBase,
     expected_distance: float,
 ) -> None:
@@ -266,15 +266,15 @@
     :type detector: DataDriftBatchBase
     :param expected_distance: expected distance value
     :type expected_distance: float
     """
     _ = detector.fit(X=X_ref_multivariate)
     statistic, _ = detector.compare(X=X_test_multivariate)
 
-    assert np.isclose(statistic, expected_distance)
+    assert np.isclose(statistic.distance, expected_distance)
 
 
 @pytest.mark.parametrize(
     "chunk_size, expected_exception",
     [
         (1.5, TypeError),
         ("10", TypeError),
@@ -372,15 +372,15 @@
     assert np.isclose(test.statistic, expected_statistic)
     assert np.isclose(test.p_value, expected_p_value)
 
 
 @pytest.mark.parametrize(
     "detector, expected_distance",
     [
-        (MMDStreaming(), 0.09793799),
+        (MMDStreaming(window_size=10), -0.02327412),
     ],
 )
 def test_streaming_distance_based_univariate_same_distribution(
     univariate_distribution_p: Tuple[float, float],
     detector: DataDriftBatchBase,
     expected_distance: float,
 ) -> None:
@@ -405,15 +405,15 @@
     # Check last distance
     assert np.isclose(result.distance, expected_distance)
 
 
 @pytest.mark.parametrize(
     "detector, expected_distance",
     [
-        (MMDStreaming(), 0.98688562),
+        (MMDStreaming(window_size=10), 0.8656735),
     ],
 )
 def test_streaming_distance_based_univariate_different_distribution(
     univariate_distribution_p: Tuple[float, float],
     univariate_distribution_q: Tuple[float, float],
     detector: DataDriftBatchBase,
     expected_distance: float,
```

### Comparing `frouros-0.2.6/frouros/tests/integration/test_real.py` & `frouros-0.2.7/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/tests/integration/test_synthetic.py` & `frouros-0.2.7/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.2.7/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/utils/data_structures.py` & `frouros-0.2.7/frouros/utils/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Data structures module."""
 
-from typing import Optional, List, Union  # noqa: TYP001
-
+from typing import Any, Optional, List, Union
 
 import numpy as np  # type: ignore
 
 
 class EmptyQueueError(Exception):
     """Empty queue exception."""
 
@@ -111,28 +110,28 @@
         :raises ValueError: Value error exception
         """
         if value < 0:
             raise ValueError("max_len must be greater or equal than 0.")
         self._max_len = value
 
     @property
-    def queue(self) -> List[Optional[bool]]:
+    def queue(self) -> List[Optional[Any]]:
         """Queue property.
 
         :return: queue
-        :rtype: List[Optional[bool]]
+        :rtype: List[Optional[Any]]
         """
         return self._queue
 
     @queue.setter
-    def queue(self, value: List[Optional[bool]]) -> None:
+    def queue(self, value: List[Optional[Any]]) -> None:
         """Queue setter.
 
         :param value: value to be set
-        :type value: List[Optional[bool]]
+        :type value: List[Optional[Any]]
         :raises ValueError: Value error exception
         """
         if not isinstance(value, list):
             raise TypeError("queue must be of type list.")
         self._queue = value
 
     @property
@@ -147,38 +146,40 @@
     def clear(self) -> None:
         """Clear queue."""
         self.count = 0
         self.first = 0
         self.last = -1
         self.queue = [None] * self.max_len
 
-    def dequeue(self) -> bool:
+    def dequeue(self) -> Any:
         """Dequeue oldest element.
 
-        :rtype: bool
+        :rtype: value: Any
         :raises EmptyQueue: Empty queue error exception
         """
         if self.is_empty():
             raise EmptyQueueError()
         element = self.queue[self.first]
         self.first = (self.first + 1) % self.max_len
         self.count -= 1
         return element  # type: ignore
 
-    def enqueue(self, value: Union[np.ndarray, float]) -> None:
+    def enqueue(self, value: Union[np.ndarray, int, float]) -> Optional[Any]:
         """Enqueue element/s.
 
         :param value: value to be enqueued
         :type value: Union[np.ndarray, float]
+        :return element: dequeued element
+        :rtype: Optional[Any]
         """
-        if self.is_full():
-            _ = self.dequeue()
+        element = self.dequeue() if self.is_full() else None
         self.last = (self.last + 1) % self.max_len
         self.queue[self.last] = value  # type: ignore
         self.count += 1
+        return element
 
     def is_empty(self) -> bool:
         """Check if queue is empty.
 
         :return: check if queue is empty
         :rtype: bool
         """
@@ -201,21 +202,21 @@
         return self.size
 
     def maintain_last_element(self) -> None:
         """Clear all elements except the last one."""
         self.first = self.last
         self.count = 1
 
-    def __getitem__(self, idx: int) -> float:
+    def __getitem__(self, idx: int) -> Any:
         """Get queue item by position.
 
         :param idx: position index
         :type idx: int
         :return: queue item
-        :rtype: float
+        :rtype: Any
         """
         return self.queue[idx]  # type: ignore
 
 
 class AccuracyQueue(CircularQueue):
     """Class representing an accuracy queue."""
```

### Comparing `frouros-0.2.6/frouros/utils/decorators.py` & `frouros-0.2.7/frouros/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/frouros/utils/stats.py` & `frouros-0.2.7/frouros/utils/stats.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from multiprocessing import Pool
 from typing import Any, Callable, Dict, Optional, List, Union
 
 import numpy as np  # type: ignore
 from tqdm import tqdm  # type: ignore
 
 from frouros.utils.logger import logger
+from frouros.utils.data_structures import CircularQueue
 
 
 class Stat(abc.ABC):
     """Abstract class representing an statistic."""
 
     @abc.abstractmethod
     def get(self) -> float:
@@ -85,21 +86,60 @@
         :param value: value to use to update the mean
         :type value: int
         :raises TypeError: Type error exception
         """
         if not isinstance(value, (int, float)):
             raise TypeError("value must be of type int or float.")
         self.num_values += 1
-        self.mean += (value - self.mean) / self.num_values
+        self.mean += self.incremental_op(
+            value=value,
+            element=self.mean,
+            size=self.num_values,
+        )
+
+    @staticmethod
+    def incremental_op(
+        value: Union[int, float],
+        element: Union[int, float],
+        size: int,
+    ) -> float:
+        """Incremental operation."""
+        return (value - element) / size
 
     def get(self) -> float:
         """Get method."""
         return self.mean
 
 
+class CircularMean(Mean):
+    """Circular mean class."""
+
+    def __init__(self, size: int) -> None:
+        """Init method."""
+        super().__init__()
+        self.queue = CircularQueue(max_len=size)
+
+    def update(self, value: Union[int, float]) -> None:
+        """Update the mean value sequentially.
+
+        :param value: value to use to update the mean
+        :type value: int
+        :raises TypeError: Type error exception
+        """
+        if not isinstance(value, (int, float)):
+            raise TypeError("value must be of type int or float.")
+        element = self.queue.enqueue(value=value)
+        self.num_values = len(self.queue)
+        self.mean += self.incremental_op(
+            value=value,
+            element=self.mean if element is None else element,
+            size=self.num_values,
+        )
+
+
 class EWMA(IncrementalStat):
     """EWMA (Exponential Weighted Moving Average) class."""
 
     def __init__(self, alpha: float) -> None:
         """Init method.
 
         :param alpha:
```

### Comparing `frouros-0.2.6/frouros.egg-info/PKG-INFO` & `frouros-0.2.7/frouros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library for drift detection in Machine Learning problems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.2.6 Summary: A Python library
+Metadata-Version: 2.1 Name: frouros Version: 0.2.7 Summary: A Python library
 for drift detection in Machine Learning problems Home-page: https://github.com/
 IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.2.6/frouros.egg-info/SOURCES.txt` & `frouros-0.2.7/frouros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frouros-0.2.6/pyproject.toml` & `frouros-0.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.2.6"
+version = "0.2.7"
 description = "A Python library for drift detection in Machine Learning problems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
```

### Comparing `frouros-0.2.6/setup.py` & `frouros-0.2.7/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/mitiq-0.9.2.tar.gz` & `tmp/mitiq-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mitiq-0.9.2.tar", last modified: Wed Jun 30 21:04:36 2021, max compression
+gzip compressed data, was "dist/mitiq-0.9.3.tar", last modified: Wed Jul  7 09:48:01 2021, max compression
```

## Comparing `mitiq-0.9.2.tar` & `mitiq-0.9.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/
--rw-r--r--   0 andrea    (1000) andrea    (1000)    35149 2020-05-27 15:07:32.000000 mitiq-0.9.2/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      177 2021-05-25 13:13:27.000000 mitiq-0.9.2/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8746 2021-06-30 21:04:36.000000 mitiq-0.9.2/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6653 2021-06-30 09:01:48.000000 mitiq-0.9.2/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        6 2021-06-30 20:52:48.000000 mitiq-0.9.2/VERSION.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2021-06-30 09:01:48.000000 mitiq-0.9.2/dev_requirements.txt
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/docs/
--rw-r--r--   0 andrea    (1000) andrea    (1000)       90 2020-05-27 15:07:32.000000 mitiq-0.9.2/docs/pytest.ini
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      833 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2449 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/_about.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1819 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/_typing.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       22 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/_version.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/benchmarks/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      746 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/benchmarks/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6085 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/benchmarks/maxcut.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4708 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/benchmarks/random_circuits.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2934 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/benchmarks/randomized_benchmarking.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1593 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/benchmarks/utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/cdr/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2021-06-18 09:22:40.000000 mitiq-0.9.2/mitiq/cdr/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3376 2021-06-30 20:52:48.000000 mitiq-0.9.2/mitiq/cdr/_testing.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8739 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/cdr/cdr.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    14697 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/cdr/clifford_training_data.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1710 2021-06-18 09:22:40.000000 mitiq-0.9.2/mitiq/cdr/data_regression.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2704 2021-06-30 20:52:48.000000 mitiq-0.9.2/mitiq/cdr/execute.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7549 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/collector.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/interface/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      938 2021-06-24 10:03:34.000000 mitiq-0.9.2/mitiq/interface/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8064 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/interface/conversions.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/interface/mitiq_braket/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      748 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_braket/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15597 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/interface/mitiq_braket/conversions.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/interface/mitiq_cirq/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      847 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_cirq/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3383 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/interface/mitiq_cirq/cirq_utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/interface/mitiq_pyquil/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      789 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_pyquil/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8643 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/interface/mitiq_pyquil/compiler.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2521 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_pyquil/conversions.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_pyquil/pyquil_utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/interface/mitiq_qiskit/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      978 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_qiskit/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8495 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/interface/mitiq_qiskit/conversions.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6196 2021-06-18 10:29:39.000000 mitiq-0.9.2/mitiq/interface/mitiq_qiskit/qiskit_utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/observable/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      719 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/observable/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4819 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/observable/pauli.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/pec/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1181 2021-06-17 17:00:19.000000 mitiq-0.9.2/mitiq/pec/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7063 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/pec/channels.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11219 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/pec/pec.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/pec/representations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1277 2021-06-17 17:00:19.000000 mitiq-0.9.2/mitiq/pec/representations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3776 2021-06-17 17:00:19.000000 mitiq-0.9.2/mitiq/pec/representations/damping.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13431 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/pec/representations/depolarizing.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5371 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/pec/representations/optimal.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5411 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/pec/sampling.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/pec/types/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      775 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/pec/types/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18284 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/pec/types/types.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7266 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/utils.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/zne/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      969 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/zne/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    63374 2021-06-30 20:52:48.000000 mitiq-0.9.2/mitiq/zne/inference.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq/zne/scaling/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      955 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/zne/scaling/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28455 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/zne/scaling/folding.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5088 2021-06-30 09:01:48.000000 mitiq-0.9.2/mitiq/zne/scaling/parameter.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4936 2021-05-25 13:13:27.000000 mitiq-0.9.2/mitiq/zne/zne.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8746 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1697 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      369 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        6 2021-06-30 21:04:36.000000 mitiq-0.9.2/mitiq.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      279 2021-05-25 13:13:27.000000 mitiq-0.9.2/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       40 2021-06-18 09:22:40.000000 mitiq-0.9.2/requirements.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2021-06-30 21:04:36.000000 mitiq-0.9.2/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2113 2021-06-30 09:01:48.000000 mitiq-0.9.2/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)    35149 2020-05-27 15:07:32.000000 mitiq-0.9.3/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      177 2021-05-25 13:13:27.000000 mitiq-0.9.3/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8867 2021-07-07 09:48:01.000000 mitiq-0.9.3/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6758 2021-07-07 09:35:05.000000 mitiq-0.9.3/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        6 2021-07-07 09:36:13.000000 mitiq-0.9.3/VERSION.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2021-07-07 09:34:51.000000 mitiq-0.9.3/dev_requirements.txt
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/docs/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)       90 2020-05-27 15:07:32.000000 mitiq-0.9.3/docs/pytest.ini
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      833 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2449 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/_about.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1819 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/_typing.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       22 2021-07-07 09:48:00.000000 mitiq-0.9.3/mitiq/_version.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/benchmarks/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      746 2021-05-25 13:13:27.000000 mitiq-0.9.3/mitiq/benchmarks/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6085 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/benchmarks/maxcut.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4708 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/benchmarks/random_circuits.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2934 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/benchmarks/randomized_benchmarking.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1593 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/benchmarks/utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/cdr/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2021-06-18 09:22:40.000000 mitiq-0.9.3/mitiq/cdr/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3376 2021-06-30 20:52:48.000000 mitiq-0.9.3/mitiq/cdr/_testing.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8739 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/cdr/cdr.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    14697 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/cdr/clifford_training_data.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1710 2021-06-18 09:22:40.000000 mitiq-0.9.3/mitiq/cdr/data_regression.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2704 2021-06-30 20:52:48.000000 mitiq-0.9.3/mitiq/cdr/execute.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7549 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/collector.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/interface/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      938 2021-06-24 10:03:34.000000 mitiq-0.9.3/mitiq/interface/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8064 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/interface/conversions.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/interface/mitiq_braket/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      748 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_braket/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15597 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/interface/mitiq_braket/conversions.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/interface/mitiq_cirq/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      847 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_cirq/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3383 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/interface/mitiq_cirq/cirq_utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/interface/mitiq_pyquil/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      789 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_pyquil/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8643 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/interface/mitiq_pyquil/compiler.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2521 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_pyquil/conversions.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_pyquil/pyquil_utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/interface/mitiq_qiskit/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      978 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_qiskit/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8498 2021-07-07 09:35:05.000000 mitiq-0.9.3/mitiq/interface/mitiq_qiskit/conversions.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6196 2021-06-18 10:29:39.000000 mitiq-0.9.3/mitiq/interface/mitiq_qiskit/qiskit_utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/observable/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      719 2021-05-25 13:13:27.000000 mitiq-0.9.3/mitiq/observable/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4819 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/observable/pauli.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/pec/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1181 2021-06-17 17:00:19.000000 mitiq-0.9.3/mitiq/pec/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7063 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/pec/channels.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11219 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/pec/pec.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/pec/representations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1277 2021-06-17 17:00:19.000000 mitiq-0.9.3/mitiq/pec/representations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3776 2021-06-17 17:00:19.000000 mitiq-0.9.3/mitiq/pec/representations/damping.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13431 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/pec/representations/depolarizing.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5371 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/pec/representations/optimal.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5411 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/pec/sampling.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/pec/types/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      775 2021-05-25 13:13:27.000000 mitiq-0.9.3/mitiq/pec/types/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18284 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/pec/types/types.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7266 2021-05-25 13:13:27.000000 mitiq-0.9.3/mitiq/utils.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/zne/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      969 2021-05-25 13:13:27.000000 mitiq-0.9.3/mitiq/zne/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    63374 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/zne/inference.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq/zne/scaling/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      996 2021-07-07 09:35:05.000000 mitiq-0.9.3/mitiq/zne/scaling/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28455 2021-07-07 09:34:51.000000 mitiq-0.9.3/mitiq/zne/scaling/folding.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5172 2021-07-07 09:35:05.000000 mitiq-0.9.3/mitiq/zne/scaling/parameter.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4936 2021-05-25 13:13:27.000000 mitiq-0.9.3/mitiq/zne/zne.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8867 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1697 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      369 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        6 2021-07-07 09:48:01.000000 mitiq-0.9.3/mitiq.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      279 2021-05-25 13:13:27.000000 mitiq-0.9.3/pyproject.toml
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       40 2021-06-18 09:22:40.000000 mitiq-0.9.3/requirements.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2021-07-07 09:48:01.000000 mitiq-0.9.3/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2113 2021-07-07 09:34:51.000000 mitiq-0.9.3/setup.py
```

### Comparing `mitiq-0.9.2/LICENSE` & `mitiq-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/PKG-INFO` & `mitiq-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitiq
-Version: 0.9.2
+Version: 0.9.3
 Summary: UNKNOWN
 Home-page: https://unitary.fund
 Author: Unitary Fund
 License: GPL v3.0
 Description: # Mitiq
         [![build](https://github.com/unitaryfund/mitiq/workflows/build/badge.svg)](https://github.com/unitaryfund/mitiq/actions)
         [![codecov](https://codecov.io/gh/unitaryfund/mitiq/branch/master/graph/badge.svg)](https://codecov.io/gh/unitaryfund/mitiq)
@@ -54,15 +54,15 @@
         guidelines](https://mitiq.readthedocs.io/en/stable/toc_contributing.html) for
         more information.
         
         ### Supported quantum programming libraries
         
         Mitiq can currently interface with:
         
-        * [Cirq](https://github.com/quantumlib/Cirq),
+        * [Cirq](https://quantumai.google/cirq),
         * [Qiskit](https://qiskit.org/),
         * [pyQuil](https://github.com/rigetti/pyquil),
         * [Braket](https://github.com/aws/amazon-braket-sdk-python).
         
         Cirq is a core requirement of Mitiq and is automatically installed. To use
         Mitiq with other quantum programming libraries, install the optional package(s)
         following the instructions linked above.
@@ -124,16 +124,18 @@
         
         ![Alt Text](docs/source/img/cirq.gif)
         
         
         ## Error mitigation techniques
         
         Mitiq currently implements:
+        
         * [Zero-Noise Extrapolation](https://mitiq.readthedocs.io/en/stable/guide/guide-zne.html),
         * [Probabilistic Error Cancellation](https://mitiq.readthedocs.io/en/stable/guide/guide-getting-started.html#error-mitigation-with-probabilistic-error-cancellation),
+        * [(Variable noise) Clifford data regression](https://mitiq.readthedocs.io/en/stable/examples/cdr_api.html),
         
         and is designed to support [additional techniques](https://github.com/unitaryfund/mitiq/wiki).
         
         ## Documentation
         
         Mitiq's documentation is hosted at [mitiq.readthedocs.io](https://mitiq.readthedocs.io).
```

### Comparing `mitiq-0.9.2/README.md` & `mitiq-0.9.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 guidelines](https://mitiq.readthedocs.io/en/stable/toc_contributing.html) for
 more information.
 
 ### Supported quantum programming libraries
 
 Mitiq can currently interface with:
 
-* [Cirq](https://github.com/quantumlib/Cirq),
+* [Cirq](https://quantumai.google/cirq),
 * [Qiskit](https://qiskit.org/),
 * [pyQuil](https://github.com/rigetti/pyquil),
 * [Braket](https://github.com/aws/amazon-braket-sdk-python).
 
 Cirq is a core requirement of Mitiq and is automatically installed. To use
 Mitiq with other quantum programming libraries, install the optional package(s)
 following the instructions linked above.
@@ -117,16 +117,18 @@
 
 ![Alt Text](docs/source/img/cirq.gif)
 
 
 ## Error mitigation techniques
 
 Mitiq currently implements:
+
 * [Zero-Noise Extrapolation](https://mitiq.readthedocs.io/en/stable/guide/guide-zne.html),
 * [Probabilistic Error Cancellation](https://mitiq.readthedocs.io/en/stable/guide/guide-getting-started.html#error-mitigation-with-probabilistic-error-cancellation),
+* [(Variable noise) Clifford data regression](https://mitiq.readthedocs.io/en/stable/examples/cdr_api.html),
 
 and is designed to support [additional techniques](https://github.com/unitaryfund/mitiq/wiki).
 
 ## Documentation
 
 Mitiq's documentation is hosted at [mitiq.readthedocs.io](https://mitiq.readthedocs.io).
```

### Comparing `mitiq-0.9.2/mitiq/__init__.py` & `mitiq-0.9.3/mitiq/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/_about.py` & `mitiq-0.9.3/mitiq/_about.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/_typing.py` & `mitiq-0.9.3/mitiq/_typing.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/benchmarks/__init__.py` & `mitiq-0.9.3/mitiq/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/benchmarks/maxcut.py` & `mitiq-0.9.3/mitiq/benchmarks/maxcut.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/benchmarks/random_circuits.py` & `mitiq-0.9.3/mitiq/benchmarks/random_circuits.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/benchmarks/randomized_benchmarking.py` & `mitiq-0.9.3/mitiq/benchmarks/randomized_benchmarking.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/benchmarks/utils.py` & `mitiq-0.9.3/mitiq/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/cdr/__init__.py` & `mitiq-0.9.3/mitiq/cdr/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/cdr/_testing.py` & `mitiq-0.9.3/mitiq/cdr/_testing.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/cdr/cdr.py` & `mitiq-0.9.3/mitiq/cdr/cdr.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/cdr/clifford_training_data.py` & `mitiq-0.9.3/mitiq/cdr/clifford_training_data.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/cdr/data_regression.py` & `mitiq-0.9.3/mitiq/cdr/data_regression.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/cdr/execute.py` & `mitiq-0.9.3/mitiq/cdr/execute.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/collector.py` & `mitiq-0.9.3/mitiq/collector.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/__init__.py` & `mitiq-0.9.3/mitiq/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/conversions.py` & `mitiq-0.9.3/mitiq/interface/conversions.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_braket/__init__.py` & `mitiq-0.9.3/mitiq/interface/mitiq_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_braket/conversions.py` & `mitiq-0.9.3/mitiq/interface/mitiq_braket/conversions.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_cirq/__init__.py` & `mitiq-0.9.3/mitiq/interface/mitiq_cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_cirq/cirq_utils.py` & `mitiq-0.9.3/mitiq/interface/mitiq_cirq/cirq_utils.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_pyquil/__init__.py` & `mitiq-0.9.3/mitiq/interface/mitiq_pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_pyquil/compiler.py` & `mitiq-0.9.3/mitiq/interface/mitiq_pyquil/compiler.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_pyquil/conversions.py` & `mitiq-0.9.3/mitiq/interface/mitiq_pyquil/conversions.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_pyquil/pyquil_utils.py` & `mitiq-0.9.3/mitiq/interface/mitiq_pyquil/pyquil_utils.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_qiskit/__init__.py` & `mitiq-0.9.3/mitiq/interface/mitiq_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_qiskit/conversions.py` & `mitiq-0.9.3/mitiq/interface/mitiq_qiskit/conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,18 +174,18 @@
             "Input circuit is required to have <= 1 quantum register but has "
             f"{len(circuit.qregs)} quantum registers."
         )
 
     qreg_sizes = [qreg.size for qreg in new_qregs]
     nqubits_in_circuit = sum(qreg.size for qreg in circuit.qregs)
 
-    if len(qreg_sizes) and sum(qreg_sizes) != nqubits_in_circuit:
+    if len(qreg_sizes) and sum(qreg_sizes) < nqubits_in_circuit:
         raise ValueError(
-            f"The circuit has {nqubits_in_circuit} qubits, but the provided "
-            f"quantum registers have {sum(qreg_sizes)} qubits."
+            f"The circuit has {nqubits_in_circuit} qubit(s), but the provided "
+            f"quantum registers have {sum(qreg_sizes)} qubit(s)."
         )
 
     # Assign the new registers.
     if len(qreg_sizes):
         circuit.qregs = list(new_qregs)
 
     # Map the qubits in operations to the new qubits.
```

### Comparing `mitiq-0.9.2/mitiq/interface/mitiq_qiskit/qiskit_utils.py` & `mitiq-0.9.3/mitiq/interface/mitiq_qiskit/qiskit_utils.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/observable/__init__.py` & `mitiq-0.9.3/mitiq/observable/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/observable/pauli.py` & `mitiq-0.9.3/mitiq/observable/pauli.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/__init__.py` & `mitiq-0.9.3/mitiq/pec/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/channels.py` & `mitiq-0.9.3/mitiq/pec/channels.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/pec.py` & `mitiq-0.9.3/mitiq/pec/pec.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/representations/__init__.py` & `mitiq-0.9.3/mitiq/pec/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/representations/damping.py` & `mitiq-0.9.3/mitiq/pec/representations/damping.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/representations/depolarizing.py` & `mitiq-0.9.3/mitiq/pec/representations/depolarizing.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/representations/optimal.py` & `mitiq-0.9.3/mitiq/pec/representations/optimal.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/sampling.py` & `mitiq-0.9.3/mitiq/pec/sampling.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/types/__init__.py` & `mitiq-0.9.3/mitiq/pec/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/pec/types/types.py` & `mitiq-0.9.3/mitiq/pec/types/types.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/utils.py` & `mitiq-0.9.3/mitiq/utils.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/zne/__init__.py` & `mitiq-0.9.3/mitiq/zne/__init__.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/zne/inference.py` & `mitiq-0.9.3/mitiq/zne/inference.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/zne/scaling/__init__.py` & `mitiq-0.9.3/mitiq/zne/scaling/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 from mitiq.zne.scaling.folding import (
     fold_all,
     fold_gates_from_left,
     fold_gates_from_right,
     fold_gates_at_random,
     fold_global,
 )
-from mitiq.zne.scaling.parameter import scale_parameters
+from mitiq.zne.scaling.parameter import (
+    scale_parameters,
+    compute_parameter_variance,
+)
```

### Comparing `mitiq-0.9.2/mitiq/zne/scaling/folding.py` & `mitiq-0.9.3/mitiq/zne/scaling/folding.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq/zne/scaling/parameter.py` & `mitiq-0.9.3/mitiq/zne/scaling/parameter.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Optional, Callable, Iterable
+from typing import Optional, Callable, List, cast
 import numpy as np
 
 import copy
 
 from cirq import Circuit, EigenGate, Moment
 from cirq import (
     ZPowGate,
     YPowGate,
     XPowGate,
     HPowGate,
     CXPowGate,
     CZPowGate,
     MeasurementGate,
-    Gate,
     Qid,
 )
 from mitiq.interface import noise_scaling_converter
 from mitiq import QPROGRAM
 
 
 class GateTypeException(Exception):
@@ -39,30 +38,29 @@
 
 
 def _get_base_gate(gate: EigenGate) -> EigenGate:
     BASE_GATES = [ZPowGate, HPowGate, XPowGate, YPowGate, CXPowGate, CZPowGate]
 
     for base_gate in BASE_GATES:
         if isinstance(gate, base_gate):
-            return base_gate
+            return cast(EigenGate, base_gate)
     raise GateTypeException(
         "Must have circuit be made of rotation gates. "
         "Your gate {} may not be supported".format(gate)
     )
 
 
 class CircuitMismatchException(Exception):
     pass
 
 
 def _generate_parameter_calibration_circuit(
-    qubits: Iterable, depth: int, gate: EigenGate
+    qubits: List[Qid], depth: int, gate: EigenGate
 ) -> Circuit:
-    """
-    Generates a circuit which should be the identity. Given a rotation
+    """Generates a circuit which should be the identity. Given a rotation
     gate R(param), it applies R(2 * pi / depth) depth times, resulting
     in R(2*pi). Requires that the gate is periodic in 2*pi.
 
     Args:
         qubits: A list of qubits.
         depth: The length of the circuit to create.
         gate: The base gate to apply several times, must be periodic
@@ -78,22 +76,25 @@
             "Number of qubits does not match domain size of gate."
         )
     return Circuit(
         gate(exponent=2 * np.pi / depth).on(*qubits) for _ in range(depth)
     )
 
 
-def _parameter_calibration(
-    executor: Callable[..., float], gate: Gate, qubit: Qid, depth: int = 100
+def compute_parameter_variance(
+    executor: Callable[..., float],
+    gate: EigenGate,
+    qubit: Qid,
+    depth: int = 100,
 ) -> float:
-    """
-    Given an executor and a gate, determines the effective
-    variance in the control parameter
-    that can be used for parameter noise scaling later on.
-    Only works for one qubit gates for now.
+    """Given an executor and a gate, determines the effective variance in the
+    control parameter that can be used as the ``base_variance`` argument in
+    ``mitiq.zne.scaling.scale_parameters``.
+
+    Note: Only works for one qubit gates for now.
 
     Args:
         executor: A function that takes in a quantum circuit and returns
             an expectation value.
         gate: The quantum gate that you wish to profile.
         qubit: The index of the qubit you wish to profile.
         depth: The number of operations you would like to use to profile
@@ -135,15 +136,15 @@
         The parameter noise scaled circuit.
     """
     final_moments = []
     noise = (scale_factor - 1) * base_variance
     rng = np.random.RandomState(seed)
     for moment in circuit:
         curr_moment = []
-        for op in moment.operations:
+        for op in moment.operations:  # type: ignore
             gate = copy.deepcopy(op.gate)
             qubits = op.qubits
             if isinstance(gate, MeasurementGate):
                 curr_moment.append(gate(*qubits))
             else:
                 assert isinstance(gate, EigenGate)
                 base_gate = _get_base_gate(gate)
```

### Comparing `mitiq-0.9.2/mitiq/zne/zne.py` & `mitiq-0.9.3/mitiq/zne/zne.py`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/mitiq.egg-info/PKG-INFO` & `mitiq-0.9.3/mitiq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitiq
-Version: 0.9.2
+Version: 0.9.3
 Summary: UNKNOWN
 Home-page: https://unitary.fund
 Author: Unitary Fund
 License: GPL v3.0
 Description: # Mitiq
         [![build](https://github.com/unitaryfund/mitiq/workflows/build/badge.svg)](https://github.com/unitaryfund/mitiq/actions)
         [![codecov](https://codecov.io/gh/unitaryfund/mitiq/branch/master/graph/badge.svg)](https://codecov.io/gh/unitaryfund/mitiq)
@@ -54,15 +54,15 @@
         guidelines](https://mitiq.readthedocs.io/en/stable/toc_contributing.html) for
         more information.
         
         ### Supported quantum programming libraries
         
         Mitiq can currently interface with:
         
-        * [Cirq](https://github.com/quantumlib/Cirq),
+        * [Cirq](https://quantumai.google/cirq),
         * [Qiskit](https://qiskit.org/),
         * [pyQuil](https://github.com/rigetti/pyquil),
         * [Braket](https://github.com/aws/amazon-braket-sdk-python).
         
         Cirq is a core requirement of Mitiq and is automatically installed. To use
         Mitiq with other quantum programming libraries, install the optional package(s)
         following the instructions linked above.
@@ -124,16 +124,18 @@
         
         ![Alt Text](docs/source/img/cirq.gif)
         
         
         ## Error mitigation techniques
         
         Mitiq currently implements:
+        
         * [Zero-Noise Extrapolation](https://mitiq.readthedocs.io/en/stable/guide/guide-zne.html),
         * [Probabilistic Error Cancellation](https://mitiq.readthedocs.io/en/stable/guide/guide-getting-started.html#error-mitigation-with-probabilistic-error-cancellation),
+        * [(Variable noise) Clifford data regression](https://mitiq.readthedocs.io/en/stable/examples/cdr_api.html),
         
         and is designed to support [additional techniques](https://github.com/unitaryfund/mitiq/wiki).
         
         ## Documentation
         
         Mitiq's documentation is hosted at [mitiq.readthedocs.io](https://mitiq.readthedocs.io).
```

### Comparing `mitiq-0.9.2/mitiq.egg-info/SOURCES.txt` & `mitiq-0.9.3/mitiq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitiq-0.9.2/setup.py` & `mitiq-0.9.3/setup.py`

 * *Files identical despite different names*


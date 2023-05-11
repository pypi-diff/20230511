# Comparing `tmp/Renate-0.2.0.tar.gz` & `tmp/Renate-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Renate-0.2.0.tar", last modified: Mon Apr 24 16:17:52 2023, max compression
+gzip compressed data, was "Renate-0.2.1.tar", last modified: Thu May 11 10:21:33 2023, max compression
```

## Comparing `Renate-0.2.0.tar` & `Renate-0.2.1.tar`

### file list

```diff
@@ -1,260 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/hooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/scripts/build_docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/scripts/prepend_license.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/integration_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/run_renate.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/test_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 16:17:43.000000 Renate-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 16:17:43.000000 Renate-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-24 16:17:43.000000 Renate-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 16:17:43.000000 Renate-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 16:17:43.000000 Renate-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-24 16:17:52.039463 Renate-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-24 16:17:43.000000 Renate-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 16:17:43.000000 Renate-0.2.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 16:17:43.000000 Renate-0.2.0/dev_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/_images/improvement_renate.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/_images/improvement_tuning.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/benchmarking/custom_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/benchmarking/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/benchmarking/renate_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/examples/train_classifier_sagemaker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/examples/train_mlp_locally.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/avalanche.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/how_to_renate_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/how_to_run_training.rst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/supported_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/benchmarking/class_incremental_learning_cifar10_der.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/getting_started/renate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/nlp_finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/nlp_finetuning/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/nlp_finetuning/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/simple_classifier_cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/start_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/start_without_hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/train_mlp_locally/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/start_training_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/start_training_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 16:17:43.000000 Renate-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 16:17:43.000000 Renate-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:17:52.039463 Renate-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/Renate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/datasets/nlp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/datasets/vision_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/experimentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/run_experiment_with_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/run_remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/data/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/performance_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/memory/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/memory/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/layers/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/prediction_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/renate_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/training/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25819 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/training/training.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/updaters/avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/model_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.023463 Renate-0.2.0/src/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/er.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/gdumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/offline_er.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.023463 Renate-0.2.0/src/renate/updaters/learner_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/reinitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.023463 Renate-0.2.0/src/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/avalanche.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/config_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/syne_tune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-04-24 16:17:43.000000 Renate-0.2.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-24 16:17:43.000000 Renate-0.2.0/test/dummy_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/test/integration_tests/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/configs/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/cifar10.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/cifar100.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/fashionmnist.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/mnist.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/configs/models/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/models/mlp-200.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/models/resnet18-cifar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/configs/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/class-incremental-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/hue-shift-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/iid-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/permutation-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/rotation-10updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/rotation-2updates.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/test/integration_tests/configs/suites/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.031463 Renate-0.2.0/test/integration_tests/configs/suites/quick/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-ewc.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-icarl.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-lwf.json
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/cls-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/der.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/er.json
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/fine-tuning.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/gdumb.json
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/joint.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/offline-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/pod-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/super-er.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/integration_tests/configs/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-ewc.json
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-lwf.json
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/cls-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/der-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/fine-tuning.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/gdumb-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/joint.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/offline-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/pod-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/super-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/run_quick_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/models/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/models/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/models/test_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/test_experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/test_experimentation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/test_scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/cli/test_parsing_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/data/test_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/data/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/test/renate/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/evaluation/metrics/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/evaluation/metrics/test_regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/memory/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/memory/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/models/test_renate_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/renate_config_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/renate_config_files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/test_renate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/training/
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/training/test_run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/updaters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/updaters/avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_er.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/test_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/test_model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_avalanche.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.616688 Renate-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/hooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/scripts/build_docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/scripts/prepend_license.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/integration_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/run_renate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 10:21:22.000000 Renate-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-11 10:21:22.000000 Renate-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-11 10:21:22.000000 Renate-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 10:21:22.000000 Renate-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 10:21:22.000000 Renate-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-11 10:21:33.616688 Renate-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-11 10:21:22.000000 Renate-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-11 10:21:22.000000 Renate-0.2.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-11 10:21:22.000000 Renate-0.2.1/dev_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/_images/improvement_renate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/_images/improvement_tuning.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/benchmarking/custom_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/benchmarking/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/benchmarking/renate_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/nlp_finetuning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/train_classifier_sagemaker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/train_mlp_locally.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/avalanche.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/how_to_renate_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/how_to_run_training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/supported_algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.588688 Renate-0.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/benchmarking/class_incremental_learning_cifar10_der.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/getting_started/renate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/nlp_finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/nlp_finetuning/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/nlp_finetuning/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/simple_classifier_cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/start_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/start_without_hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/train_mlp_locally/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/start_training_with_er_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/start_training_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/start_training_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-11 10:21:22.000000 Renate-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 10:21:22.000000 Renate-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:21:33.616688 Renate-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.588688 Renate-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/Renate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/datasets/nlp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/datasets/vision_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/experimentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/run_experiment_with_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/run_remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/data/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/performance_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/memory/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/layers/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/prediction_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/renate_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25769 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/gdumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/offline_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/learner_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/reinitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/config_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-11 10:21:22.000000 Renate-0.2.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-11 10:21:22.000000 Renate-0.2.1/test/dummy_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/test/integration_tests/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/cifar10.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/cifar100.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/fashionmnist.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/mnist.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/models/mlp-200.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/models/resnet18-cifar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/class-incremental-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/hue-shift-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/iid-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/permutation-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/rotation-10updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/rotation-2updates.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/test/integration_tests/configs/suites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/suites/quick/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-icarl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/cls-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/der.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/gdumb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/offline-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/pod-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/super-er.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/integration_tests/configs/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/cls-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/der-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/gdumb-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/offline-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/pod-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/super-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/run_quick_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/models/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/models/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/models/test_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/test_experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/test_experimentation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/test_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/cli/test_parsing_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/data/test_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/data/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/test/renate/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/evaluation/metrics/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/evaluation/metrics/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/memory/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/memory/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/models/test_renate_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/renate_config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/renate_config_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/renate_config_files/config_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/test_renate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/training/test_run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/updaters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/test_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/test_model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.616688 Renate-0.2.1/test/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_syne_tune.py
```

### Comparing `Renate-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `Renate-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `Renate-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/codeql.yml` & `Renate-0.2.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/coverage.yml` & `Renate-0.2.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/integration_tests.yml` & `Renate-0.2.1/.github/workflows/integration_tests.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/pypi_publish.yml` & `Renate-0.2.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/run_renate.yml` & `Renate-0.2.1/.github/workflows/run_renate.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/run_unit_tests.yml` & `Renate-0.2.1/.github/workflows/run_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/.github/workflows/test_docs.yml` & `Renate-0.2.1/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/CONTRIBUTING.md` & `Renate-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/LICENSE` & `Renate-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/PKG-INFO` & `Renate-0.2.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: Renate
-Version: 0.2.0
-Summary: Library for Continual Learning for Practitioners
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: avalanche
-Provides-Extra: dev
-License-File: LICENSE
-License-File: NOTICE
-
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
-    :target: https://github.com/awslabs/Renate/releases/tag/v0.1.0
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.2.0
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
     :target: https://pypistats.org/packages/renate
     :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
@@ -85,19 +68,37 @@
 ============
 
 * Easy to scale and run in the cloud
 * Designed for real-world retraining pipelines
 * Advanced HPO functionalities available out-of-the-box
 * Open for experimentation 
 
-Blog posts
-==========
+Resources
+=========
+
+* (blog) `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+* (paper) `Renate: A Library for Real-World Continual Learning <https://arxiv.org/abs/2304.12067>`_
 
-* `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+Cite Renate
+===========
 
+    .. code-block:: bibtex
+    
+      @misc{renate2023,
+        title           = {Renate: A Library for Real-World Continual Learning}, 
+        author          = {Martin Wistuba and
+                           Martin Ferianc and
+                           Lukas Balles and
+                           Cedric Archambeau and
+                           Giovanni Zappella},
+        year            = {2023},
+        eprint          = {2304.12067},
+        archivePrefix   = {arXiv},
+        primaryClass    = {cs.LG}
+      }
 
 What are you looking for?
 =========================
 
 * `Installation Instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
     .. code-block:: bash
```

### Comparing `Renate-0.2.0/README.rst` & `Renate-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+Metadata-Version: 2.1
+Name: Renate
+Version: 0.2.1
+Summary: Library for Continual Learning for Practitioners
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: <3.11,>=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: avalanche
+Provides-Extra: dev
+License-File: LICENSE
+License-File: NOTICE
+
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
-    :target: https://github.com/awslabs/Renate/releases/tag/v0.1.0
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.2.0
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
     :target: https://pypistats.org/packages/renate
     :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
@@ -68,19 +85,37 @@
 ============
 
 * Easy to scale and run in the cloud
 * Designed for real-world retraining pipelines
 * Advanced HPO functionalities available out-of-the-box
 * Open for experimentation 
 
-Blog posts
-==========
+Resources
+=========
+
+* (blog) `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+* (paper) `Renate: A Library for Real-World Continual Learning <https://arxiv.org/abs/2304.12067>`_
 
-* `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+Cite Renate
+===========
 
+    .. code-block:: bibtex
+    
+      @misc{renate2023,
+        title           = {Renate: A Library for Real-World Continual Learning}, 
+        author          = {Martin Wistuba and
+                           Martin Ferianc and
+                           Lukas Balles and
+                           Cedric Archambeau and
+                           Giovanni Zappella},
+        year            = {2023},
+        eprint          = {2304.12067},
+        archivePrefix   = {arXiv},
+        primaryClass    = {cs.LG}
+      }
 
 What are you looking for?
 =========================
 
 * `Installation Instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
     .. code-block:: bash
```

### Comparing `Renate-0.2.0/doc/_images/improvement_renate.svg` & `Renate-0.2.1/doc/_images/improvement_renate.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/_images/improvement_tuning.svg` & `Renate-0.2.1/doc/_images/improvement_tuning.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/benchmarking/custom_benchmarks.rst` & `Renate-0.2.1/doc/benchmarking/custom_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/benchmarking/index.rst` & `Renate-0.2.1/doc/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/benchmarking/renate_benchmarks.rst` & `Renate-0.2.1/doc/benchmarking/renate_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/conf.py` & `Renate-0.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/examples/train_classifier_sagemaker.rst` & `Renate-0.2.1/doc/examples/train_classifier_sagemaker.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/examples/train_mlp_locally.rst` & `Renate-0.2.1/doc/examples/train_mlp_locally.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/avalanche.rst` & `Renate-0.2.1/doc/getting_started/avalanche.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/how_to_renate_config.rst` & `Renate-0.2.1/doc/getting_started/how_to_renate_config.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/how_to_run_training.rst` & `Renate-0.2.1/doc/getting_started/how_to_run_training.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/index.rst` & `Renate-0.2.1/doc/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/install.rst` & `Renate-0.2.1/doc/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/output.rst` & `Renate-0.2.1/doc/getting_started/output.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/doc/getting_started/supported_algorithms.rst` & `Renate-0.2.1/doc/getting_started/supported_algorithms.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/benchmarking/class_incremental_learning_cifar10_der.py` & `Renate-0.2.1/examples/benchmarking/class_incremental_learning_cifar10_der.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/getting_started/renate_config.py` & `Renate-0.2.1/examples/getting_started/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/nlp_finetuning/renate_config.py` & `Renate-0.2.1/examples/nlp_finetuning/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/nlp_finetuning/start.py` & `Renate-0.2.1/examples/nlp_finetuning/start.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/simple_classifier_cifar10/renate_config.py` & `Renate-0.2.1/examples/simple_classifier_cifar10/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/simple_classifier_cifar10/start_with_hpo.py` & `Renate-0.2.1/examples/simple_classifier_cifar10/start_with_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/simple_classifier_cifar10/start_without_hpo.py` & `Renate-0.2.1/examples/simple_classifier_cifar10/start_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/train_mlp_locally/renate_config.py` & `Renate-0.2.1/examples/train_mlp_locally/renate_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py` & `Renate-0.2.1/examples/train_mlp_locally/start_training_with_er_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/train_mlp_locally/start_training_with_hpo.py` & `Renate-0.2.1/examples/train_mlp_locally/start_training_with_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/examples/train_mlp_locally/start_training_without_hpo.py` & `Renate-0.2.1/examples/train_mlp_locally/start_training_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/pyproject.toml` & `Renate-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/Renate.egg-info/PKG-INFO` & `Renate-0.2.1/src/Renate.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
-    :target: https://github.com/awslabs/Renate/releases/tag/v0.1.0
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.2.0
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
     :target: https://pypistats.org/packages/renate
     :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
@@ -85,19 +85,37 @@
 ============
 
 * Easy to scale and run in the cloud
 * Designed for real-world retraining pipelines
 * Advanced HPO functionalities available out-of-the-box
 * Open for experimentation 
 
-Blog posts
-==========
+Resources
+=========
 
-* `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+* (blog) `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+* (paper) `Renate: A Library for Real-World Continual Learning <https://arxiv.org/abs/2304.12067>`_
 
+Cite Renate
+===========
+
+    .. code-block:: bibtex
+    
+      @misc{renate2023,
+        title           = {Renate: A Library for Real-World Continual Learning}, 
+        author          = {Martin Wistuba and
+                           Martin Ferianc and
+                           Lukas Balles and
+                           Cedric Archambeau and
+                           Giovanni Zappella},
+        year            = {2023},
+        eprint          = {2304.12067},
+        archivePrefix   = {arXiv},
+        primaryClass    = {cs.LG}
+      }
 
 What are you looking for?
 =========================
 
 * `Installation Instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
     .. code-block:: bash
```

### Comparing `Renate-0.2.0/src/Renate.egg-info/SOURCES.txt` & `Renate-0.2.1/src/Renate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 doc/requirements.txt
 doc/_images/improvement_renate.svg
 doc/_images/improvement_tuning.svg
 doc/benchmarking/custom_benchmarks.rst
 doc/benchmarking/index.rst
 doc/benchmarking/renate_benchmarks.rst
 doc/examples/index.rst
+doc/examples/nlp_finetuning.rst
 doc/examples/train_classifier_sagemaker.rst
 doc/examples/train_mlp_locally.rst
 doc/getting_started/avalanche.rst
 doc/getting_started/how_to_renate_config.rst
 doc/getting_started/how_to_run_training.rst
 doc/getting_started/index.rst
 doc/getting_started/install.rst
@@ -176,14 +177,15 @@
 test/renate/data/test_datasets.py
 test/renate/evaluation/metrics/test_classification.py
 test/renate/evaluation/metrics/test_regression_metrics.py
 test/renate/memory/test_buffer.py
 test/renate/memory/test_storage.py
 test/renate/models/test_renate_module.py
 test/renate/renate_config_files/config.py
+test/renate/renate_config_files/config_scenario.py
 test/renate/training/test_run_training.py
 test/renate/updaters/test_learner.py
 test/renate/updaters/test_model_updater.py
 test/renate/updaters/avalanche/test_avalanche_learner.py
 test/renate/updaters/avalanche/test_avalanche_model_updater.py
 test/renate/updaters/avalanche/test_avalanche_plugins.py
 test/renate/updaters/experimental/test_er.py
```

### Comparing `Renate-0.2.0/src/Renate.egg-info/requires.txt` & `Renate-0.2.1/src/Renate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/__init__.py` & `Renate-0.2.1/src/renate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     _handler = logging.StreamHandler()
     _handler.setFormatter(
         logging.Formatter("[%(asctime)s] %(levelname)s [%(name)s:%(lineno)s] %(message)s")
     )
     _renate_logger.addHandler(_handler)
     _renate_logger.propagate = False
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `Renate-0.2.0/src/renate/benchmark/datasets/nlp_datasets.py` & `Renate-0.2.1/src/renate/benchmark/datasets/nlp_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/datasets/vision_datasets.py` & `Renate-0.2.1/src/renate/benchmark/datasets/vision_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/experiment_config.py` & `Renate-0.2.1/src/renate/benchmark/experiment_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/experimentation.py` & `Renate-0.2.1/src/renate/benchmark/experimentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     logger.info(f"Loading model {model_fn_kwargs.get('model_name', '')}")
     model = get_model(config_module, **model_fn_kwargs)
     data_module_fn_kwargs = get_data_module_fn_kwargs(config_module, config_space)
     logger.info(f"Prepare dataset {data_module_fn_kwargs.get('dataset_name', '')}")
     data_module = get_and_prepare_data_module(
         config_module,
         data_path=data_url,
-        chunk_id=defaults.CHUNK_ID,
+        chunk_id=0,
         seed=seed,
         **data_module_fn_kwargs,
     )
     data_module.setup()
     assert num_updates == len(
         data_module.test_data()
     ), f"The dataset has {len(data_module.test_data())} chunks, expected {num_updates}."
```

### Comparing `Renate-0.2.0/src/renate/benchmark/models/__init__.py` & `Renate-0.2.1/src/renate/benchmark/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/models/base.py` & `Renate-0.2.1/src/renate/benchmark/models/base.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/models/mlp.py` & `Renate-0.2.1/src/renate/benchmark/models/mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/models/resnet.py` & `Renate-0.2.1/src/renate/benchmark/models/resnet.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/models/vision_transformer.py` & `Renate-0.2.1/src/renate/benchmark/models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/benchmark/scenarios.py` & `Renate-0.2.1/src/renate/benchmark/scenarios.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/cli/parsing_functions.py` & `Renate-0.2.1/src/renate/cli/parsing_functions.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/cli/run_experiment_with_scenario.py` & `Renate-0.2.1/src/renate/cli/run_experiment_with_scenario.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/cli/run_remote_job.py` & `Renate-0.2.1/src/renate/cli/run_remote_job.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/cli/run_training.py` & `Renate-0.2.1/src/renate/cli/run_training.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/data/data_module.py` & `Renate-0.2.1/src/renate/data/data_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/data/datasets.py` & `Renate-0.2.1/src/renate/data/datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/defaults.py` & `Renate-0.2.1/src/renate/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 N_WORKERS = 1
 INSTANCE_TYPE = "ml.c5.xlarge"
 PYTHON_VERSION = "py38"
 FRAMEWORK_VERSION = "1.12.0"
 
 TASK_ID = "default_task"
 SUPPORTED_TASKS_TYPE = Literal["classification", "regression"]
-CHUNK_ID = 0
 WORKING_DIRECTORY = "renate_working_dir"
 LOGGER = TensorBoardLogger
 LOGGER_KWARGS = {
     "save_dir": os.path.expanduser(os.path.join("~", ".renate", WORKING_DIRECTORY)),
     "version": 1,
     "name": "lightning_logs",
 }
```

### Comparing `Renate-0.2.0/src/renate/evaluation/evaluator.py` & `Renate-0.2.1/src/renate/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/evaluation/metrics/classification.py` & `Renate-0.2.1/src/renate/evaluation/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/evaluation/metrics/performance_regression_metrics.py` & `Renate-0.2.1/src/renate/evaluation/metrics/performance_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/evaluation/metrics/utils.py` & `Renate-0.2.1/src/renate/evaluation/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/memory/buffer.py` & `Renate-0.2.1/src/renate/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/memory/storage.py` & `Renate-0.2.1/src/renate/memory/storage.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/models/layers/cn.py` & `Renate-0.2.1/src/renate/models/layers/cn.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/models/prediction_strategies.py` & `Renate-0.2.1/src/renate/models/prediction_strategies.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/models/renate_module.py` & `Renate-0.2.1/src/renate/models/renate_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/training/training.py` & `Renate-0.2.1/src/renate/training/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     mode: defaults.SUPPORTED_TUNING_MODE_TYPE,
     config_space: Dict[str, Any],
     metric: str,
     backend: defaults.SUPPORTED_BACKEND_TYPE,
     updater: str = defaults.LEARNER,
     max_epochs: int = defaults.MAX_EPOCHS,
     task_id: str = defaults.TASK_ID,
-    chunk_id: int = defaults.CHUNK_ID,
+    chunk_id: Optional[int] = None,
     input_state_url: Optional[str] = None,
     output_state_url: Optional[str] = None,
     working_directory: Optional[str] = defaults.WORKING_DIRECTORY,
     source_dir: Optional[str] = None,
     config_file: Optional[str] = None,
     requirements_file: Optional[str] = None,
     role: Optional[str] = None,
@@ -401,16 +401,14 @@
 def _verify_validation_set_for_hpo_and_checkpointing(
     config_space: Dict[str, Any],
     config_file: str,
     tune_hyperparameters: bool,
     metric: str,
     mode: defaults.SUPPORTED_TUNING_MODE_TYPE,
     working_directory: str,
-    chunk_id: int,
-    seed: int,
 ) -> Tuple[str, defaults.SUPPORTED_TUNING_MODE_TYPE]:
     """Checks if validation set is provided when needed and updates config_space such that
     checkpointing works.
 
     If a validation set exists, the metric is forwarded such that we store the checkpoint which
     performs best on validation. This is a side effect changing `config_space`. Otherwise, the
     checkpoint of the last epoch is used.
@@ -512,15 +510,16 @@
     See renate.train.run_training_job for a description of arguments.
     """
     tune_hyperparameters = is_syne_tune_config_space(config_space)
     config_space["updater"] = updater
     config_space["max_epochs"] = max_epochs
     config_space["config_file"] = config_file
     config_space["prepare_data"] = False
-    config_space["chunk_id"] = chunk_id
+    if chunk_id is not None:
+        config_space["chunk_id"] = chunk_id
     config_space["task_id"] = task_id
     config_space["working_directory"] = working_directory
     config_space["seed"] = seed
     config_space["accelerator"] = accelerator
     config_space["devices"] = devices
     config_space["deterministic_trainer"] = deterministic_trainer
     if input_state_url is not None:
@@ -529,16 +528,14 @@
     metric, mode = _verify_validation_set_for_hpo_and_checkpointing(
         config_space=config_space,
         config_file=config_file,
         tune_hyperparameters=tune_hyperparameters,
         metric=metric,
         mode=mode,
         working_directory=working_directory,
-        chunk_id=chunk_id,
-        seed=seed,
     )
 
     training_script = str(Path(renate.__path__[0]) / "cli" / "run_training.py")
     assert Path(training_script).is_file(), f"Could not find training script {training_script}."
     logger.info("Start updating the model.")
     if tune_hyperparameters:
         logger.info(
```

### Comparing `Renate-0.2.0/src/renate/updaters/avalanche/learner.py` & `Renate-0.2.1/src/renate/updaters/avalanche/learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/avalanche/model_updater.py` & `Renate-0.2.1/src/renate/updaters/avalanche/model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/avalanche/plugins.py` & `Renate-0.2.1/src/renate/updaters/avalanche/plugins.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/experimental/er.py` & `Renate-0.2.1/src/renate/updaters/experimental/er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/experimental/fine_tuning.py` & `Renate-0.2.1/src/renate/updaters/experimental/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/experimental/gdumb.py` & `Renate-0.2.1/src/renate/updaters/experimental/gdumb.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/experimental/joint.py` & `Renate-0.2.1/src/renate/updaters/experimental/joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/experimental/offline_er.py` & `Renate-0.2.1/src/renate/updaters/experimental/offline_er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/experimental/repeated_distill.py` & `Renate-0.2.1/src/renate/updaters/experimental/repeated_distill.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/learner.py` & `Renate-0.2.1/src/renate/updaters/learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/learner_components/component.py` & `Renate-0.2.1/src/renate/updaters/learner_components/component.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/learner_components/losses.py` & `Renate-0.2.1/src/renate/updaters/learner_components/losses.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/learner_components/reinitialization.py` & `Renate-0.2.1/src/renate/updaters/learner_components/reinitialization.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/updaters/model_updater.py` & `Renate-0.2.1/src/renate/updaters/model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/avalanche.py` & `Renate-0.2.1/src/renate/utils/avalanche.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/config_spaces.py` & `Renate-0.2.1/src/renate/utils/config_spaces.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/file.py` & `Renate-0.2.1/src/renate/utils/file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/module.py` & `Renate-0.2.1/src/renate/utils/module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/optimizer.py` & `Renate-0.2.1/src/renate/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/pytorch.py` & `Renate-0.2.1/src/renate/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/src/renate/utils/syne_tune.py` & `Renate-0.2.1/src/renate/utils/syne_tune.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/conftest.py` & `Renate-0.2.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/dummy_datasets.py` & `Renate-0.2.1/test/dummy_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/integration_tests/configs/updaters/super-er-buffer500.json` & `Renate-0.2.1/test/integration_tests/configs/updaters/super-er-buffer500.json`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/integration_tests/run_experiment.py` & `Renate-0.2.1/test/integration_tests/run_experiment.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/integration_tests/run_quick_test.py` & `Renate-0.2.1/test/integration_tests/run_quick_test.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/benchmark/models/test_mlp.py` & `Renate-0.2.1/test/renate/benchmark/models/test_mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/benchmark/models/test_resnet.py` & `Renate-0.2.1/test/renate/benchmark/models/test_resnet.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/benchmark/models/test_vision_transformer.py` & `Renate-0.2.1/test/renate/benchmark/models/test_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/benchmark/test_experimentation.py` & `Renate-0.2.1/test/renate/benchmark/test_experimentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from renate.benchmark.experimentation import execute_experiment_job
 
 
 @pytest.fixture
 def experiment_job_kwargs():
     return {
         "backend": "local",
-        "config_file": str(Path(__file__).parent.parent / "renate_config_files" / "config.py"),
-        "config_space": {"updater": "ER", "use_scenario": True, "max_epochs": 5},
+        "config_file": str(
+            Path(__file__).parent.parent / "renate_config_files" / "config_scenario.py"
+        ),
+        "config_space": {"updater": "ER", "max_epochs": 5},
         "mode": "max",
         "metric": "val_accuracy",
         "num_updates": 2,
         "max_time": 15,
         "seed": 0,
     }
```

### Comparing `Renate-0.2.0/test/renate/benchmark/test_experimentation_config.py` & `Renate-0.2.1/test/renate/benchmark/test_experimentation_config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/benchmark/test_scenarios.py` & `Renate-0.2.1/test/renate/benchmark/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/cli/test_parsing_functions.py` & `Renate-0.2.1/test/renate/cli/test_parsing_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,56 +83,43 @@
         ),
     ],
     ids=("No all_args, no ignore_args", "no all_args", "all_args"),
 )
 def test_get_function_args(all_args, ignore_args):
     expected_args = [
         "data_path",
-        "chunk_id",
         "val_size",
         "seed",
-        "use_scenario",
         "class_groupings",
         "optional_tuple",
         "optional_float",
         "list_param",
+        "bool_param",
     ]
     expected_all_args = {
         **all_args,
         **{
             "data_path": {
                 "type": str,
                 "argument_group": CUSTOM_ARGS_GROUP,
                 "required": True,
                 "true_type": str,
             },
-            "chunk_id": {
-                "type": int,
-                "argument_group": CUSTOM_ARGS_GROUP,
-                "default": None,
-                "true_type": int,
-            },
             "val_size": {
                 "type": float,
                 "argument_group": CUSTOM_ARGS_GROUP,
                 "default": 0.0,
                 "true_type": float,
             },
             "seed": {
                 "type": int,
                 "argument_group": CUSTOM_ARGS_GROUP,
                 "default": 0,
                 "true_type": int,
             },
-            "use_scenario": {
-                "type": str,
-                "argument_group": CUSTOM_ARGS_GROUP,
-                "default": "False",
-                "true_type": bool,
-            },
             "class_groupings": {
                 "type": str,
                 "argument_group": CUSTOM_ARGS_GROUP,
                 "default": "((0,1),(2,3,4))",
                 "true_type": tuple,
             },
             "optional_tuple": {
@@ -149,14 +136,20 @@
             },
             "list_param": {
                 "type": str,
                 "argument_group": CUSTOM_ARGS_GROUP,
                 "default": "[1,2]",
                 "true_type": list,
             },
+            "bool_param": {
+                "type": str,
+                "argument_group": CUSTOM_ARGS_GROUP,
+                "default": "False",
+                "true_type": bool,
+            },
         },
     }
     for arg in ignore_args:
         del expected_all_args[arg]
     args = get_function_args(
         config_module=config_module,
         function_name="data_module_fn",
@@ -210,24 +203,24 @@
 
 def test_get_fn_kwargs_helper_functions():
     """Tests whether the different helper functions correctly create kwargs given a dictionary
     and the Python function."""
     expected_data_module_kwargs = {
         "data_path": "home/data/path",
         "class_groupings": ((1, 2), (3, 4)),
-        "use_scenario": False,
         "optional_float": None,
+        "bool_param": False,
     }
     config_space = {
         "data_path": expected_data_module_kwargs["data_path"],
         "model_state_url": "home/model/state",
         "unused_config": 1,
         "class_groupings": to_dense_str(expected_data_module_kwargs["class_groupings"]),
-        "use_scenario": to_dense_str(expected_data_module_kwargs["use_scenario"]),
         "optional_float": to_dense_str(expected_data_module_kwargs["optional_float"]),
+        "bool_param": to_dense_str(expected_data_module_kwargs["bool_param"]),
     }
     data_module_kwargs = get_data_module_fn_kwargs(
         config_module=config_module, config_space=config_space, cast_arguments=True
     )
     assert data_module_kwargs == expected_data_module_kwargs
     model_kwargs = get_model_fn_kwargs(
         config_module=config_module, config_space=config_space, cast_arguments=True
```

### Comparing `Renate-0.2.0/test/renate/data/test_data_module.py` & `Renate-0.2.1/test/renate/data/test_data_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/data/test_datasets.py` & `Renate-0.2.1/test/renate/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/evaluation/metrics/test_classification.py` & `Renate-0.2.1/test/renate/evaluation/metrics/test_classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/evaluation/metrics/test_regression_metrics.py` & `Renate-0.2.1/test/renate/evaluation/metrics/test_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/memory/test_buffer.py` & `Renate-0.2.1/test/renate/memory/test_buffer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/memory/test_storage.py` & `Renate-0.2.1/test/renate/memory/test_storage.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/models/test_renate_module.py` & `Renate-0.2.1/test/renate/models/test_renate_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/renate_config_files/config.py` & `Renate-0.2.1/test/renate/renate_config_files/config_scenario.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,15 @@
 
 
 def data_module_fn(
     data_path: str,
     chunk_id: Optional[int] = None,
     val_size: float = 0.0,
     seed: int = 0,
-    use_scenario: bool = False,
     class_groupings: Tuple[Tuple[int]] = ((0, 1), (2, 3, 4)),
-    optional_tuple: Optional[Tuple[float]] = None,
-    optional_float: Optional[float] = None,
-    list_param: list = [1, 2],
 ) -> RenateDataModule:
     data_module = DummyTorchVisionDataModule(transform=None, val_size=val_size, seed=seed)
-    if use_scenario:
-        return ClassIncrementalScenario(
-            data_module=data_module,
-            chunk_id=chunk_id,
-            class_groupings=class_groupings,
-        )
-    return data_module
+    return ClassIncrementalScenario(
+        data_module=data_module,
+        chunk_id=chunk_id,
+        class_groupings=class_groupings,
+    )
```

### Comparing `Renate-0.2.0/test/renate/training/test_run_training.py` & `Renate-0.2.1/test/renate/training/test_run_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,14 @@
         return _verify_validation_set_for_hpo_and_checkpointing(
             config_space=config_space,
             config_file=config_file,
             tune_hyperparameters=tune_hyperparameters,
             metric=expected_metric,
             mode=expected_mode,
             working_directory=tmpdir,
-            chunk_id=0,
-            seed=0,
         )
 
     if tune_hyperparameters and val_size == 0:
         with pytest.raises(AssertionError):
             verify_validation_set()
     else:
         metric, mode = verify_validation_set()
```

### Comparing `Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_learner.py` & `Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py` & `Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_plugins.py` & `Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_plugins.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/experimental/test_er.py` & `Renate-0.2.1/test/renate/updaters/experimental/test_er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/experimental/test_fine_tuning.py` & `Renate-0.2.1/test/renate/updaters/experimental/test_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/experimental/test_joint.py` & `Renate-0.2.1/test/renate/updaters/experimental/test_joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/experimental/test_repeated_distill.py` & `Renate-0.2.1/test/renate/updaters/experimental/test_repeated_distill.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/test_learner.py` & `Renate-0.2.1/test/renate/updaters/test_learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/updaters/test_model_updater.py` & `Renate-0.2.1/test/renate/updaters/test_model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/utils/test_avalanche.py` & `Renate-0.2.1/test/renate/utils/test_avalanche.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/utils/test_file.py` & `Renate-0.2.1/test/renate/utils/test_file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/utils/test_metrics_utils.py` & `Renate-0.2.1/test/renate/utils/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/utils/test_optimizer.py` & `Renate-0.2.1/test/renate/utils/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/utils/test_pytorch.py` & `Renate-0.2.1/test/renate/utils/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.0/test/renate/utils/test_syne_tune.py` & `Renate-0.2.1/test/renate/utils/test_syne_tune.py`

 * *Files identical despite different names*


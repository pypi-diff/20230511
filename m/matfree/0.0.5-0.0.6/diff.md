# Comparing `tmp/matfree-0.0.5.tar.gz` & `tmp/matfree-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.5.tar", last modified: Tue May  9 10:18:46 2023, max compression
+gzip compressed data, was "matfree-0.0.6.tar", last modified: Thu May 11 05:39:24 2023, max compression
```

## Comparing `matfree-0.0.5.tar` & `matfree-0.0.6.tar`

### file list

```diff
@@ -1,82 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.610597 matfree-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.610597 matfree-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-09 10:18:32.000000 matfree-0.0.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-09 10:18:32.000000 matfree-0.0.5/.github/workflows/doc-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-09 10:18:32.000000 matfree-0.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-09 10:18:32.000000 matfree-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-09 10:18:32.000000 matfree-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 10:18:32.000000 matfree-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-09 10:18:32.000000 matfree-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-09 10:18:46.618598 matfree-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-09 10:18:32.000000 matfree-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.610597 matfree-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/hutch.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/benchmarks/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/benchmarks/jacobian_squared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/matfree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/benchmark_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-09 10:18:32.000000 matfree-0.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-09 10:18:32.000000 matfree-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 10:18:46.622598 matfree-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 10:18:32.000000 matfree-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_decomp/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/test_gkl_full_reortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/test_lanczos_full_reortho.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/test_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_hutch/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_frobeniusnorm_squared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_trace_and_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_trace_with_variance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_montecarlo/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/test_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/test_multiestimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/test_van_der_corput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_slq/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_slq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_slq/test_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_slq/test_logdet_autodiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.995245 matfree-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.979245 matfree-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.983245 matfree-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-11 05:39:06.000000 matfree-0.0.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-11 05:39:06.000000 matfree-0.0.6/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-11 05:39:06.000000 matfree-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-11 05:39:06.000000 matfree-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-11 05:39:06.000000 matfree-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 05:39:06.000000 matfree-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 05:39:06.000000 matfree-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-11 05:39:24.995245 matfree-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-11 05:39:06.000000 matfree-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.983245 matfree-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.983245 matfree-0.0.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/decomp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/hutchinson.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/montecarlo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/api/slq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/benchmarks/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/benchmarks/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/benchmarks/jacobian_squared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/control_variates.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/dev/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/higher_moments.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/log_determinants.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-11 05:39:06.000000 matfree-0.0.6/docs/vector_calculus.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/matfree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/benchmark_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/hutchinson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-11 05:39:06.000000 matfree-0.0.6/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.987245 matfree-0.0.6/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 05:39:24.000000 matfree-0.0.6/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-11 05:39:06.000000 matfree-0.0.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-11 05:39:06.000000 matfree-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-11 05:39:24.995245 matfree-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 05:39:06.000000 matfree-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/tests/test_decomp/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/test_gkl_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/test_lanczos_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_decomp/test_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.991245 matfree-0.0.6/tests/test_hutchinson/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_frobeniusnorm_squared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_trace_and_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_hutchinson/test_trace_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.995245 matfree-0.0.6/tests/test_montecarlo/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/test_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/test_multiestimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_montecarlo/test_van_der_corput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:39:24.995245 matfree-0.0.6/tests/test_slq/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_slq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_slq/test_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 05:39:06.000000 matfree-0.0.6/tests/test_slq/test_logdet_autodiff.py
```

### Comparing `matfree-0.0.5/.github/workflows/ci.yaml` & `matfree-0.0.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/.github/workflows/doc-publish.yml` & `matfree-0.0.6/.github/workflows/doc-publish.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/.github/workflows/release.yml` & `matfree-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/.gitignore` & `matfree-0.0.6/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 matfree/_version.py
 
+# Don't version jupyter notebooks. Track synced markdown files.
+*.ipynb
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `matfree-0.0.5/.pre-commit-config.yaml` & `matfree-0.0.6/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         language_version: python3
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.265
     hooks:
       - id: ruff
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
         args: [--no-strict-optional, --ignore-missing-imports]
```

### Comparing `matfree-0.0.5/LICENSE` & `matfree-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/docs/benchmarks/control_variates.py` & `matfree-0.0.6/docs/benchmarks/control_variates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Control_variates benchmark.
 
 Runtime: ~10 seconds.
 """
 
-from matfree import benchmark_util, hutch, montecarlo
+from matfree import benchmark_util, hutchinson, montecarlo
 from matfree.backend import func, linalg, np, plt, prng, progressbar
 
 
 def problem(n):
     """Create an example problem."""
 
     # This function has a Jacobian with x-shaped sparsity pattern
@@ -36,23 +36,23 @@
 
     error_fun = func.partial(benchmark_util.rmse_relative, expected=trace)
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def fun1(num, key):
         """Estimate the trace conventionally."""
-        return hutch.trace(
+        return hutchinson.trace(
             Av, key=key, sample_fun=sample_fun, num_batches=num, num_samples_per_batch=1
         )
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def fun2(num, key):
         """Estimate trace and diagonal jointly and discard the diagonal."""
-        trace2, _ = hutch.trace_and_diagonal(
+        trace2, _ = hutchinson.trace_and_diagonal(
             Av, key=key, num_levels=num, sample_fun=sample_fun
         )
         return trace2
 
     errors1, stds1, times1 = [], [], []
     errors2, stds2, times2 = [], [], []
```

### Comparing `matfree-0.0.5/docs/benchmarks/jacobian_squared.py` & `matfree-0.0.6/docs/benchmarks/jacobian_squared.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """What is the fastest way of computing trace(A^5)."""
-from matfree import benchmark_util, hutch, montecarlo, slq
+from matfree import benchmark_util, hutchinson, montecarlo, slq
 from matfree.backend import func, linalg, np, plt, prng
 from matfree.backend.progressbar import progressbar
 
 
 def problem(n):
     """Create an example problem."""
 
@@ -51,26 +51,26 @@
 if __name__ == "__main__":
     dim = 10
     num_samples = 2 ** np.arange(4, 12)
     num_restarts = 10
 
     (matfun, jvp, Av, trace, JJ), (k, sample_fun) = problem(dim)
 
-    x = hutch.trace(Av, key=k, sample_fun=sample_fun)
+    x = hutchinson.trace(Av, key=k, sample_fun=sample_fun)
     y = slq.trace_of_matfun_symmetric(matfun, jvp, 5, key=k, sample_fun=sample_fun)
     assert np.allclose(x, trace, atol=1e-1, rtol=1e-1), (x, trace)
     assert np.allclose(y, trace, atol=1e-1, rtol=1e-1), (y, trace)
 
     error_fun = func.partial(benchmark_util.rmse_relative, expected=trace)
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def matvec(num, key):
         """Matrix-vector mult."""
-        return hutch.trace(
+        return hutchinson.trace(
             Av, key=key, sample_fun=sample_fun, num_samples_per_batch=num
         )
 
     @func.partial(benchmark_util.error_and_time, error_fun=error_fun)
     @func.partial(func.jit, static_argnums=0)
     def slq_low(num, key):
         """SLQ(1)"""  # noqa: D400,D415
```

### Comparing `matfree-0.0.5/matfree/backend/control_flow.py` & `matfree-0.0.6/matfree/backend/control_flow.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/matfree/backend/func.py` & `matfree-0.0.6/matfree/backend/func.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/matfree/backend/linalg.py` & `matfree-0.0.6/matfree/backend/linalg.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import jax.numpy as jnp
 
 
 def vector_norm(x, /):
     return jnp.linalg.norm(x)
 
 
-def matrix_norm(x, /):
-    return jnp.linalg.norm(x)
+def matrix_norm(x, /, which):
+    return jnp.linalg.norm(x, ord=which)
 
 
 def qr(x, /, *, mode="reduced"):
     return jnp.linalg.qr(x, mode=mode)
 
 
 def eigh(x, /):
```

### Comparing `matfree-0.0.5/matfree/backend/np.py` & `matfree-0.0.6/matfree/backend/np.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/matfree/backend/prng.py` & `matfree-0.0.6/matfree/backend/prng.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/matfree/benchmark_util.py` & `matfree-0.0.6/matfree/benchmark_util.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/matfree/decomp.py` & `matfree-0.0.6/matfree/decomp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Matrix decomposition algorithms."""
 
 from matfree.backend import containers, control_flow, func, linalg, np
 from matfree.backend.typing import Any, Array, Callable, Tuple
 
 
-def svd(v0: Array, depth: int, Av: Callable, vA: Callable, matrix_shape: Tuple[int]):
+def svd(
+    v0: Array, depth: int, Av: Callable, vA: Callable, matrix_shape: Tuple[int, ...]
+):
     """Approximate singular value decomposition.
 
     Uses GKL with full reorthogonalisation to bi-diagonalise the target matrix
     and computes the full SVD of the (small) bidiagonal matrix.
 
     Parameters
     ----------
@@ -22,16 +24,16 @@
         Matrix-vector product function.
     vA:
         Vector-matrix product function.
     matrix_shape:
         Shape of the matrix involved in matrix-vector and vector-matrix products.
     """
     # Factorise the matrix
-    alg = gkl_full_reortho(depth, matrix_shape=matrix_shape)
-    u, (d, e), vt, _ = decompose_fori_loop(0, depth + 1, v0, Av, vA, alg=alg)
+    algorithm = gkl_full_reortho(depth, matrix_shape=matrix_shape)
+    u, (d, e), vt, _ = decompose_fori_loop(v0, Av, vA, algorithm=algorithm)
 
     # Compute SVD of factorisation
     B = _bidiagonal_dense(d, e)
     U, S, Vt = linalg.svd(B, full_matrices=False)
 
     # Combine orthogonal transformations
     return u @ U, S, Vt @ vt
@@ -39,68 +41,82 @@
 
 def _bidiagonal_dense(d, e):
     diag = linalg.diagonal_matrix(d)
     offdiag = linalg.diagonal_matrix(e, 1)
     return diag + offdiag
 
 
-class DecompAlg(containers.NamedTuple):
+class _DecompAlg(containers.NamedTuple):
     """Matrix decomposition algorithm."""
 
     init: Callable
     """Initialise the state of the algorithm. Usually, this involves pre-allocation."""
 
     step: Callable
     """Compute the next iteration."""
 
     extract: Callable
     """Extract the solution from the state of the algorithm."""
 
+    lower_upper: Tuple[int, int]
+    """Range of the for-loop used to decompose a matrix."""
+
+
+AlgorithmType = Tuple[Callable, Callable, Callable, Tuple[int, int]]
+"""Decomposition algorithm type.
+
+For example, the output of
+[matfree.decomp.lanczos_full_reortho(...)][matfree.decomp.lanczos_full_reortho].
+"""
+
 
 # all arguments are positional-only because we will rename arguments a lot
-def decompose_fori_loop(lower, upper, v0, *matvec_funs, alg: DecompAlg):
+def decompose_fori_loop(v0, *matvec_funs, algorithm: AlgorithmType):
     r"""Decompose a matrix purely based on matvec-products with A.
 
-    This behaviour of this function is equivalent to
+    The behaviour of this function is equivalent to
 
     ```python
-    def decompose(lower, upper, v0, *matvec_funs, alg):
-        state = alg.init(v0)
+    def decompose(v0, *matvec_funs, algorithm):
+        init, step, extract, (lower, upper) = algorithm
+        state = init(v0)
         for _ in range(lower, upper):
-            state = alg.step(state, *matvec_funs)
-        return alg.extract(state)
+            state = step(state, *matvec_funs)
+        return extract(state)
     ```
 
     but the implementation uses JAX' fori_loop.
     """
     # todo: turn the "practically equivalent" bit above into a doctest.
-    init_val = alg.init(v0)
+    init, step, extract, (lower, upper) = algorithm
+    init_val = init(v0)
 
     def body_fun(_, s):
-        return alg.step(s, *matvec_funs)
+        return step(s, *matvec_funs)
 
     result = control_flow.fori_loop(lower, upper, body_fun=body_fun, init_val=init_val)
-    return alg.extract(result)
+    return extract(result)
 
 
-def lanczos_full_reortho(depth, /) -> DecompAlg:
+def lanczos_full_reortho(depth, /) -> AlgorithmType:
     """**Lanczos** algorithm with pre-allocation & full reorthogonalisation.
 
     Decompose a matrix into a product of orthogonal-**tridiagonal**-orthogonal matrices.
     Use this algorithm for approximate **eigenvalue** decompositions.
 
     Lanczos' algorithm assumes a symmetric matrix.
     """
     # this algorithm is massively unstable.
     # but despite this instability, quadrature might be stable?
     # https://www.sciencedirect.com/science/article/abs/pii/S0920563200918164
-    return DecompAlg(
+    return _DecompAlg(
         init=func.partial(_lanczos_full_reortho_init, depth),
         step=_lanczos_full_reortho_apply,
         extract=_lanczos_full_reortho_extract,
+        lower_upper=(0, depth + 1),
     )
 
 
 class _LanczosState(containers.NamedTuple):
     i: int
     basis: Any
     tridiag: Any
@@ -148,24 +164,25 @@
 
 
 def _lanczos_full_reortho_extract(state: _LanczosState, /):
     _, basis, (diag, offdiag), _ = state
     return basis, (diag, offdiag)
 
 
-def gkl_full_reortho(depth, /, matrix_shape) -> DecompAlg:
+def gkl_full_reortho(depth, /, matrix_shape) -> AlgorithmType:
     """**Golub-Kahan-Lanczos** algorithm with pre-allocation & full reorthogonalisation.
 
     Decompose a matrix into a product of orthogonal-**bidiagonal**-orthogonal matrices.
     Use this algorithm for approximate **singular value** decompositions.
     """
-    return DecompAlg(
+    return _DecompAlg(
         init=func.partial(_gkl_full_reortho_init, depth, matrix_shape),
         step=_gkl_full_reortho_apply,
         extract=_gkl_full_reortho_extract,
+        lower_upper=(0, depth + 1),
     )
 
 
 class _GKLState(containers.NamedTuple):
     i: int
     Us: Any
     Vs: Any
```

### Comparing `matfree-0.0.5/matfree/hutch.py` & `matfree-0.0.6/matfree/hutchinson.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Hutchinson-style trace and diagonal estimation."""
 
 
 from matfree import montecarlo
 from matfree.backend import containers, control_flow, func, linalg, np, prng
-from matfree.backend.typing import Any, Array, Callable
+from matfree.backend.typing import Any, Array, Callable, Sequence
 
 
 def trace(Av: Callable, /, **kwargs) -> Array:
     """Estimate the trace of a matrix stochastically.
 
     Parameters
     ----------
@@ -20,39 +20,43 @@
 
     def quadform(vec):
         return linalg.vecdot(vec, Av(vec))
 
     return montecarlo.estimate(quadform, **kwargs)
 
 
-def trace_with_variance(Av: Callable, /, **kwargs) -> Array:
+def trace_moments(Av: Callable, /, moments: Sequence[int] = (1, 2), **kwargs) -> Array:
     """Estimate the trace of a matrix and the variance of the estimator.
 
     Parameters
     ----------
     Av:
         Matrix-vector product function.
+    moments:
+        Which moments to compute. For example, selection `moments=(1,2)` computes
+        the first and second moment.
     **kwargs:
         Keyword-arguments to be passed to
-        [montecarlo.estimate()][matfree.montecarlo.estimate].
+        [montecarlo.multiestimate(...)][matfree.montecarlo.multiestimate].
     """
 
     def quadform(vec):
         return linalg.vecdot(vec, Av(vec))
 
-    def mean_squared_fun(x, axis):
-        return np.mean(x**2, axis=axis)
+    def moment(x, axis, *, power):
+        return np.mean(x**power, axis=axis)
 
-    mean, second_moment = montecarlo.multiestimate(
+    statistics_batch = [func.partial(moment, power=m) for m in moments]
+    statistics_combine = [np.mean] * len(moments)
+    return montecarlo.multiestimate(
         quadform,
-        statistics_batch=[np.mean, mean_squared_fun],
-        statistics_combine=[np.mean, np.mean],
+        statistics_batch=statistics_batch,
+        statistics_combine=statistics_combine,
         **kwargs,
     )
-    return mean, second_moment - mean**2
 
 
 def frobeniusnorm_squared(Av: Callable, /, **kwargs) -> Array:
     r"""Estimate the squared Frobenius norm of a matrix stochastically.
 
     The Frobenius norm of a matrix $A$ is defined as
 
@@ -133,15 +137,15 @@
         Sampling function.
         Usually, either [montecarlo.normal][matfree.montecarlo.normal]
         or [montecarlo.rademacher][matfree.montecarlo.normal].
     key:
         Pseudo-random number generator key.
     **kwargs:
         Keyword-arguments to be passed to
-        [diagonal_multilevel()][matfree.hutch.diagonal_multilevel].
+        [diagonal_multilevel()][matfree.hutchinson.diagonal_multilevel].
 
 
     See:
     Adams et al., Estimating the Spectral Density of Large Implicit Matrices, 2018.
     """
     fx_value = func.eval_shape(sample_fun, key)
     init = np.zeros(shape=fx_value.shape, dtype=fx_value.dtype)
```

### Comparing `matfree-0.0.5/matfree/montecarlo.py` & `matfree-0.0.6/matfree/montecarlo.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/matfree/slq.py` & `matfree-0.0.6/matfree/slq.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def quadratic_form_slq_symmetric(matfun, Av, order, /):
     """Approximate quadratic form for stochastic Lanczos quadrature."""
 
     def quadform(v0, /):
         algorithm = decomp.lanczos_full_reortho(order)
-        _, tridiag = decomp.decompose_fori_loop(0, order + 1, v0, Av, alg=algorithm)
+        _, tridiag = decomp.decompose_fori_loop(v0, Av, algorithm=algorithm)
         (diag, off_diag) = tridiag
 
         # todo: once jax supports eigh_tridiagonal(eigvals_only=False),
         #  use it here. Until then: an eigen-decomposition of size (order + 1)
         #  does not hurt too much...
         diag = linalg.diagonal_matrix(diag)
         offdiag1 = linalg.diagonal_matrix(off_diag, -1)
```

### Comparing `matfree-0.0.5/matfree/test_util.py` & `matfree-0.0.6/matfree/test_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def symmetric_matrix_from_eigenvalues(eigvals, /):
     """Generate a symmetric matrix with prescribed eigenvalues."""
     (n,) = eigvals.shape
 
     # Need _some_ matrix to start with
     A = np.reshape(np.arange(1.0, n**2 + 1.0), (n, n))
-    A = A / linalg.matrix_norm(A)
+    A = A / linalg.matrix_norm(A, which="fro")
     X = A.T @ A + np.eye(n)
 
     # QR decompose. We need the orthogonal matrix.
     # Treat Q as a stack of eigenvectors.
     Q, R = linalg.qr(X)
 
     # Treat Q as eigenvectors, and 'D' as eigenvalues.
```

### Comparing `matfree-0.0.5/matfree.egg-info/SOURCES.txt` & `matfree-0.0.6/matfree.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 mkdocs.yml
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/ci.yaml
 .github/workflows/doc-publish.yml
 .github/workflows/release.yml
+docs/control_variates.md
+docs/higher_moments.md
 docs/index.md
+docs/log_determinants.md
+docs/vector_calculus.md
 docs/api/decomp.md
-docs/api/hutch.md
+docs/api/hutchinson.md
 docs/api/montecarlo.md
 docs/api/slq.md
 docs/benchmarks/control_variates.py
 docs/benchmarks/index.md
 docs/benchmarks/jacobian_squared.py
 docs/dev/index.md
 docs/javascripts/mathjax.js
 matfree/__init__.py
 matfree/_version.py
 matfree/benchmark_util.py
 matfree/decomp.py
-matfree/hutch.py
+matfree/hutchinson.py
 matfree/montecarlo.py
 matfree/slq.py
 matfree/test_util.py
 matfree.egg-info/PKG-INFO
 matfree.egg-info/SOURCES.txt
 matfree.egg-info/dependency_links.txt
 matfree.egg-info/requires.txt
@@ -46,20 +50,20 @@
 matfree/backend/time.py
 matfree/backend/typing.py
 tests/__init__.py
 tests/test_decomp/__init__.py
 tests/test_decomp/test_gkl_full_reortho.py
 tests/test_decomp/test_lanczos_full_reortho.py
 tests/test_decomp/test_svd.py
-tests/test_hutch/__init__.py
-tests/test_hutch/test_diagonal.py
-tests/test_hutch/test_frobeniusnorm_squared.py
-tests/test_hutch/test_trace.py
-tests/test_hutch/test_trace_and_diagonal.py
-tests/test_hutch/test_trace_with_variance.py
+tests/test_hutchinson/__init__.py
+tests/test_hutchinson/test_diagonal.py
+tests/test_hutchinson/test_frobeniusnorm_squared.py
+tests/test_hutchinson/test_trace.py
+tests/test_hutchinson/test_trace_and_diagonal.py
+tests/test_hutchinson/test_trace_moments.py
 tests/test_montecarlo/__init__.py
 tests/test_montecarlo/test_estimate.py
 tests/test_montecarlo/test_multiestimate.py
 tests/test_montecarlo/test_van_der_corput.py
 tests/test_slq/__init__.py
 tests/test_slq/test_logdet.py
 tests/test_slq/test_logdet_autodiff.py
```

### Comparing `matfree-0.0.5/mkdocs.yml` & `matfree-0.0.6/mkdocs.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 ---
 site_name: matfree documentation
 repo_url: https://github.com/pnkraemer/matfree
 repo_name: pnkraemer/matfree
 nav:
-  - Get started: [index.md]
+  - Get started: index.md
+  - Tutorials:
+      - control_variates.md
+      - log_determinants.md
+      - higher_moments.md
+      - vector_calculus.md
   - API documentation:
-      - api/montecarlo.md
-      - api/decomp.md
-      - api/hutch.md
-      - api/slq.md
-  - dev/index.md
-  - benchmarks/index.md
+      - matfree.montecarlo: api/montecarlo.md
+      - matfree.decomp: api/decomp.md
+      - matfree.hutchinson: api/hutchinson.md
+      - matfree.slq: api/slq.md
+  - Developer documentation: dev/index.md
+  - Benchmarks: benchmarks/index.md
 theme:
   name: material
   palette:
 
     # Palette toggle for light mode
     - media: '(prefers-color-scheme: light)'
       scheme: default
@@ -28,27 +33,34 @@
       scheme: slate
       primary: black
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   font:
     text: Fira Sans
-  features: [navigation.tabs, navigation.footer]
+  features: [navigation.sections, navigation.footer]
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
           options:
-            show_root_members_full_path: false
-            show_category_heading: false
+            show_root_heading: true
+            show_root_toc_entry: true
+            show_root_full_path: true
+            show_root_members_full_path: true
+            show_object_full_path: false
+            show_category_heading: true
             docstring_style: numpy
             show_if_no_docstring: true
-            show_signature_annotations: true
             members_order: alphabetical
+            annotations_path: brief
+            show_signature: true
+            show_signature_annotations: true
+            separate_signature: false
             docstring_section_style: list
 watch: [matfree]
 extra:
   social:
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/@pnkraemer
       name: Nico
```

### Comparing `matfree-0.0.5/pyproject.toml` & `matfree-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/setup.cfg` & `matfree-0.0.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 	jax[cpu]
 test = 
 	pytest
 	pytest-cases
 lint = 
 	%(test)s
 	pre-commit
-	ruff
-	mypy
 format = 
 	isort
 	black
 doc = 
 	mkdocs
 	mkdocs-material
 	mkdocstrings
```

### Comparing `matfree-0.0.5/tests/test_decomp/test_gkl_full_reortho.py` & `matfree-0.0.6/tests/test_decomp/test_gkl_full_reortho.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def Av(v):
         return A @ v
 
     def vA(v):
         return v @ A
 
-    Us, Bs, Vs, (b, v) = decomp.decompose_fori_loop(0, order + 1, v0, Av, vA, alg=alg)
+    Us, Bs, Vs, (b, v) = decomp.decompose_fori_loop(v0, Av, vA, algorithm=alg)
     (d_m, e_m) = Bs
 
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     assert np.shape(Us) == (nrows, order + 1)
     assert np.allclose(Us.T @ Us, np.eye(order + 1), **tols_decomp), Us.T @ Us
```

### Comparing `matfree-0.0.5/tests/test_decomp/test_lanczos_full_reortho.py` & `matfree-0.0.6/tests/test_decomp/test_lanczos_full_reortho.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,40 +11,23 @@
     d = np.arange(n) + 10.0
     d = d.at[num_significant_eigvals:].set(0.001)
 
     return test_util.symmetric_matrix_from_eigenvalues(d)
 
 
 @testing.parametrize("n", [6])
-@testing.parametrize("num_significant_eigvals", [4])
-def test_error_for_too_high_order(A):
-    """Assert graceful failure if the depth matches or exceeds the number of columns."""
-    n, _ = np.shape(A)
-    key = prng.prng_key(1)
-    v0 = prng.normal(key, shape=(n,))
-    with testing.raises(ValueError):
-        alg = decomp.lanczos_full_reortho(n + 10)
-        _ = decomp.decompose_fori_loop(0, n + 10, v0, lambda v: A @ v, alg=alg)
-    with testing.raises(ValueError):
-        alg = decomp.lanczos_full_reortho(n)
-        _ = decomp.decompose_fori_loop(0, n + 1, v0, lambda v: A @ v, alg=alg)
-
-
-@testing.parametrize("n", [6])
 @testing.parametrize("num_significant_eigvals", [6])
 def test_max_order(A):
     """If m == n, the matrix should be equal to the full tridiagonal."""
     n, _ = np.shape(A)
     order = n - 1
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     alg = decomp.lanczos_full_reortho(order)
-    Q, (d_m, e_m) = decomp.decompose_fori_loop(
-        0, order + 1, v0, lambda v: A @ v, alg=alg
-    )
+    Q, (d_m, e_m) = decomp.decompose_fori_loop(v0, lambda v: A @ v, algorithm=alg)
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     # Since full-order mode: Q must be unitary
     assert np.shape(Q) == (order + 1, n)
     assert np.allclose(Q @ Q.T, np.eye(n), **tols_decomp), Q @ Q.T
@@ -77,15 +60,15 @@
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
 def test_identity(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     alg = decomp.lanczos_full_reortho(order)
-    Q, tridiag = decomp.decompose_fori_loop(0, order + 1, v0, lambda v: A @ v, alg=alg)
+    Q, tridiag = decomp.decompose_fori_loop(v0, lambda v: A @ v, algorithm=alg)
     (d_m, e_m) = tridiag
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     assert np.shape(Q) == (order + 1, n)
     assert np.allclose(Q @ Q.T, np.eye(order + 1), **tols_decomp), Q @ Q.T
```

### Comparing `matfree-0.0.5/tests/test_decomp/test_svd.py` & `matfree-0.0.6/tests/test_decomp/test_svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
     n = min(nrows, ncols)
     d = np.arange(n) + 10.0
     d = d.at[num_significant_singular_vals:].set(0.001)
     return test_util.asymmetric_matrix_from_singular_values(d, nrows=nrows, ncols=ncols)
 
 
-def test_max_depth(A):
+def test_equal_to_linalg_svd(A):
     """The output of full-depth SVD should be equal (*) to linalg.svd().
 
     (*) Note: The singular values should be identical,
     and the orthogonal matrices should be orthogonal. They are not unique.
     """
     nrows, ncols = np.shape(A)
     depth = min(nrows, ncols) - 1
```

### Comparing `matfree-0.0.5/tests/test_hutch/test_diagonal.py` & `matfree-0.0.6/tests/test_hutchinson/test_diagonal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for basic trace estimators."""
 
-from matfree import hutch, montecarlo
+from matfree import hutchinson, montecarlo
 from matfree.backend import func, linalg, np, prng, testing
 
 
 @testing.fixture(name="fun")
 def fixture_fun():
     """Create a nonlinear, to-be-differentiated function."""
 
@@ -29,15 +29,15 @@
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))  # random lin. point
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
 
     # Estimate the trace
     fun = sample_fun(shape=np.shape(x0), dtype=np.dtype(x0))
-    estimate = hutch.diagonal(
+    estimate = hutchinson.diagonal(
         jvp,
         num_batches=num_batches,
         key=key,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
     )
     truth = linalg.diagonal(J)
```

### Comparing `matfree-0.0.5/tests/test_hutch/test_frobeniusnorm_squared.py` & `matfree-0.0.6/tests/test_hutchinson/test_frobeniusnorm_squared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for basic trace estimators."""
 
-from matfree import hutch, montecarlo
+from matfree import hutchinson, montecarlo
 from matfree.backend import func, linalg, np, prng, testing
 
 
 @testing.fixture(name="fun")
 def fixture_fun():
     """Create a nonlinear, to-be-differentiated function."""
 
@@ -31,15 +31,15 @@
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))  # random lin. point
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
 
     # Estimate the trace
     fun = sample_fun(shape=np.shape(x0), dtype=np.dtype(x0))
-    estimate = hutch.frobeniusnorm_squared(
+    estimate = hutchinson.frobeniusnorm_squared(
         jvp,
         num_batches=num_batches,
         key=key,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
     )
     truth = linalg.trace(J.T @ J)
```

### Comparing `matfree-0.0.5/tests/test_hutch/test_trace.py` & `matfree-0.0.6/tests/test_hutchinson/test_trace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for basic trace estimators."""
 
-from matfree import hutch, montecarlo
+from matfree import hutchinson, montecarlo
 from matfree.backend import func, linalg, np, prng, testing
 
 
 @testing.fixture(name="fun")
 def fixture_fun():
     """Create a nonlinear, to-be-differentiated function."""
 
@@ -29,15 +29,15 @@
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))  # random lin. point
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
 
     # Estimate the trace
     fun = sample_fun(shape=np.shape(x0), dtype=np.dtype(x0))
-    estimate = hutch.trace(
+    estimate = hutchinson.trace(
         jvp,
         num_batches=num_batches,
         key=key,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
     )
     truth = linalg.trace(J)
```

### Comparing `matfree-0.0.5/tests/test_hutch/test_trace_and_diagonal.py` & `matfree-0.0.6/tests/test_hutchinson/test_trace_and_diagonal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for basic trace estimators."""
 
-from matfree import hutch, montecarlo
+from matfree import hutchinson, montecarlo
 from matfree.backend import func, linalg, np, prng, testing
 
 
 @testing.fixture(name="fun")
 def fixture_fun():
     """Create a nonlinear, to-be-differentiated function."""
 
@@ -28,15 +28,15 @@
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
 
     # Estimate the trace
     fun = sample_fun(shape=np.shape(x0), dtype=np.dtype(x0))
-    trace, diag = hutch.trace_and_diagonal(
+    trace, diag = hutchinson.trace_and_diagonal(
         jvp, key=key, num_levels=num_samples, sample_fun=fun
     )
 
     # Print errors if test fails
     error_diag = linalg.vector_norm(diag - linalg.diagonal(J))
     error_trace = linalg.vector_norm(trace - linalg.trace(J))
     assert np.allclose(diag, linalg.diagonal(J), rtol=1e-2), error_diag
```

### Comparing `matfree-0.0.5/tests/test_hutch/test_trace_with_variance.py` & `matfree-0.0.6/tests/test_hutchinson/test_trace_moments.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,78 @@
 """Tests for estimating traces."""
 
-from matfree import hutch, montecarlo
+from matfree import hutchinson, montecarlo
 from matfree.backend import func, linalg, np, prng, testing
 
 
-@testing.fixture(name="fun")
-def fixture_fun():
-    """Create a nonlinear, to-be-differentiated function."""
-
-    def f(x):
-        return np.sin(np.flip(np.cos(x)) + 1.0) * np.sin(x) + 1.0
-
-    return f
-
-
 @testing.fixture(name="key")
 def fixture_key():
     """Fix a pseudo-random number generator."""
     return prng.prng_key(seed=1)
 
 
-@testing.parametrize("num_batches", [1_000])
-@testing.parametrize("num_samples_per_batch", [1_000])
-@testing.parametrize("dim", [1, 10])
-def test_normal(fun, key, num_batches, num_samples_per_batch, dim):
-    """Assert that the estimated trace approximates the true trace accurately."""
+@testing.fixture(name="J_and_jvp")
+def fixture_J_and_jvp(key, dim):
+    """Create a nonlinear, to-be-differentiated function."""
+
+    def fun(x):
+        return np.sin(np.flip(np.cos(x)) + 1.0) * np.sin(x) + 1.0
+
     # Linearise function
     x0 = prng.uniform(key, shape=(dim,))  # random lin. point
     _, jvp = func.linearize(fun, x0)
     J = func.jacfwd(fun)(x0)
 
+    return J, jvp
+
+
+@testing.parametrize("num_batches", [1_000])
+@testing.parametrize("num_samples_per_batch", [1_000])
+@testing.parametrize("dim", [1, 10])
+def test_variance_normal(J_and_jvp, key, num_batches, num_samples_per_batch, dim):
+    """Assert that the estimated trace approximates the true trace accurately."""
     # Estimate the trace
-    fun = montecarlo.normal(shape=np.shape(x0), dtype=np.dtype(x0))
-    trace, variance = hutch.trace_with_variance(
+    J, jvp = J_and_jvp
+    fun = montecarlo.normal(shape=(dim,), dtype=float)
+    first, second = hutchinson.trace_moments(
         jvp,
         key=key,
         num_batches=num_batches,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
+        moments=(1, 2),
     )
 
     # Assert the trace is correct
     truth = linalg.trace(J)
-    assert np.allclose(trace, truth, rtol=1e-2)
+    assert np.allclose(first, truth, rtol=1e-2)
 
     # Assert the variance is correct:
-    norm = hutch.frobeniusnorm_squared(
-        jvp,
-        key=key,
-        num_batches=num_batches,
-        num_samples_per_batch=num_samples_per_batch,
-        sample_fun=fun,
-    )
-    assert np.allclose(variance, norm * 2, rtol=1e-2)
+    norm = linalg.matrix_norm(J, which="fro") ** 2
+    assert np.allclose(second - first**2, norm * 2, rtol=1e-2)
 
 
 @testing.parametrize("num_batches", [1_000])
 @testing.parametrize("num_samples_per_batch", [1_000])
 @testing.parametrize("dim", [1, 10])
-def test_rademacher(fun, key, num_batches, num_samples_per_batch, dim):
+def test_variance_rademacher(J_and_jvp, key, num_batches, num_samples_per_batch, dim):
     """Assert that the estimated trace approximates the true trace accurately."""
-    # Linearise function
-    x0 = prng.uniform(key, shape=(dim,))  # random lin. point
-    _, jvp = func.linearize(fun, x0)
-    J = func.jacfwd(fun)(x0)
-
     # Estimate the trace
-    fun = montecarlo.rademacher(shape=np.shape(x0), dtype=np.dtype(x0))
-    trace, variance = hutch.trace_with_variance(
+    J, jvp = J_and_jvp
+    fun = montecarlo.rademacher(shape=(dim,), dtype=float)
+    first, second = hutchinson.trace_moments(
         jvp,
         key=key,
         num_batches=num_batches,
         num_samples_per_batch=num_samples_per_batch,
         sample_fun=fun,
+        moments=(1, 2),
     )
 
     # Assert the trace is correct
     truth = linalg.trace(J)
-    assert np.allclose(trace, truth, rtol=1e-2)
+    assert np.allclose(first, truth, rtol=1e-2)
 
     # Assert the variance is correct:
-    norm = hutch.frobeniusnorm_squared(
-        jvp,
-        key=key,
-        num_batches=num_batches,
-        num_samples_per_batch=num_samples_per_batch,
-        sample_fun=fun,
-    )
+    norm = linalg.matrix_norm(J, which="fro") ** 2
     truth = 2 * (norm - linalg.trace(J**2))
-    assert np.allclose(variance, truth, atol=1e-2, rtol=1e-2)
+    assert np.allclose(second - first**2, truth, atol=1e-2, rtol=1e-2)
```

### Comparing `matfree-0.0.5/tests/test_montecarlo/test_estimate.py` & `matfree-0.0.6/tests/test_montecarlo/test_estimate.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/tests/test_montecarlo/test_multiestimate.py` & `matfree-0.0.6/tests/test_montecarlo/test_multiestimate.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/tests/test_montecarlo/test_van_der_corput.py` & `matfree-0.0.6/tests/test_montecarlo/test_van_der_corput.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/tests/test_slq/test_logdet.py` & `matfree-0.0.6/tests/test_slq/test_logdet.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.5/tests/test_slq/test_logdet_autodiff.py` & `matfree-0.0.6/tests/test_slq/test_logdet_autodiff.py`

 * *Files identical despite different names*


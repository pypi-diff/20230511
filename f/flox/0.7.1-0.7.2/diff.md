# Comparing `tmp/flox-0.7.1.tar.gz` & `tmp/flox-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flox-0.7.1.tar", last modified: Mon May  8 17:58:16 2023, max compression
+gzip compressed data, was "flox-0.7.2.tar", last modified: Thu May 11 20:35:19 2023, max compression
```

## Comparing `flox-0.7.1.tar` & `flox-0.7.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 17:57:50.000000 flox-0.7.1/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 17:57:50.000000 flox-0.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/ci-additional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-08 17:57:50.000000 flox-0.7.1/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-08 17:57:50.000000 flox-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-08 17:57:50.000000 flox-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-08 17:57:50.000000 flox-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-08 17:58:16.539113 flox-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-08 17:57:50.000000 flox-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/asv_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/asv_bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/README_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/cohorts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-08 17:57:50.000000 flox-0.7.1/asv_bench/benchmarks/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-08 17:57:50.000000 flox-0.7.1/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 17:57:50.000000 flox-0.7.1/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 17:57:50.000000 flox-0.7.1/ci/minimal-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 17:57:50.000000 flox-0.7.1/ci/no-dask.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 17:57:50.000000 flox-0.7.1/ci/no-xarray.yml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 17:57:50.000000 flox-0.7.1/ci/upstream-dev-env.yml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 17:57:50.000000 flox-0.7.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.531113 flox-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-08 17:57:50.000000 flox-0.7.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)    43022 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/blockwise.png
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/cohorts-month-chunk4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/cohorts-month-chunk5.png
--rw-r--r--   0 runner    (1001) docker     (123)    46006 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/map-reduce.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-blockwise-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-blockwise.svg
--rw-r--r--   0 runner    (1001) docker     (123)   102136 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-cohorts-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60369 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-cohorts.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105406 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62434 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False.svg
--rw-r--r--   0 runner    (1001) docker     (123)   101278 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62159 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True.svg
--rw-r--r--   0 runner    (1001) docker     (123)   177642 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/new-split-apply-combine-annotated.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61350 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/split-apply-combine.svg
--rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-05-08 17:57:50.000000 flox-0.7.1/docs/diagrams/split-reduce.png
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-08 17:57:50.000000 flox-0.7.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 17:57:50.000000 flox-0.7.1/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/aggregations.md
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/arrays.md
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/engines.md
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/implementation.md
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.535113 flox-0.7.1/docs/source/user-stories/
--rw-r--r--   0 runner    (1001) docker     (123)    74658 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/climatology-hourly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/climatology.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/custom-aggregations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   395737 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/hourly-climatology.html
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories/overlaps.md
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/user-stories.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-08 17:57:50.000000 flox-0.7.1/docs/source/xarray.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/flox/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 17:57:50.000000 flox-0.7.1/flox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 17:58:16.000000 flox-0.7.1/flox/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-08 17:57:50.000000 flox-0.7.1/flox/aggregate_flox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-08 17:57:50.000000 flox-0.7.1/flox/aggregate_npg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-05-08 17:57:50.000000 flox-0.7.1/flox/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 17:57:50.000000 flox-0.7.1/flox/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    72861 2023-05-08 17:57:50.000000 flox-0.7.1/flox/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:57:50.000000 flox-0.7.1/flox/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-08 17:57:50.000000 flox-0.7.1/flox/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-05-08 17:57:50.000000 flox-0.7.1/flox/xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-08 17:57:50.000000 flox-0.7.1/flox/xrdtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-08 17:57:50.000000 flox-0.7.1/flox/xrutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/flox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 17:58:16.000000 flox-0.7.1/flox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-08 17:57:50.000000 flox-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 17:57:50.000000 flox-0.7.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 17:58:16.539113 flox-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 17:57:50.000000 flox-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:16.539113 flox-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-08 17:57:50.000000 flox-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-08 17:57:50.000000 flox-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    47162 2023-05-08 17:57:50.000000 flox-0.7.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-05-08 17:57:50.000000 flox-0.7.1/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.634070 flox-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 20:34:47.000000 flox-0.7.2/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.606068 flox-0.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 20:34:47.000000 flox-0.7.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.606068 flox-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-11 20:34:47.000000 flox-0.7.2/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-11 20:34:47.000000 flox-0.7.2/.github/workflows/ci-additional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-11 20:34:47.000000 flox-0.7.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-11 20:34:47.000000 flox-0.7.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 20:34:47.000000 flox-0.7.2/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-11 20:34:47.000000 flox-0.7.2/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-11 20:34:47.000000 flox-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-11 20:34:47.000000 flox-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-11 20:34:47.000000 flox-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-11 20:35:19.634070 flox-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-11 20:34:47.000000 flox-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.606068 flox-0.7.2/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-11 20:34:47.000000 flox-0.7.2/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.610069 flox-0.7.2/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-11 20:34:47.000000 flox-0.7.2/asv_bench/benchmarks/README_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-11 20:34:47.000000 flox-0.7.2/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-11 20:34:47.000000 flox-0.7.2/asv_bench/benchmarks/cohorts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-11 20:34:47.000000 flox-0.7.2/asv_bench/benchmarks/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-11 20:34:47.000000 flox-0.7.2/asv_bench/benchmarks/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.610069 flox-0.7.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-11 20:34:47.000000 flox-0.7.2/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-11 20:34:47.000000 flox-0.7.2/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 20:34:47.000000 flox-0.7.2/ci/minimal-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 20:34:47.000000 flox-0.7.2/ci/no-dask.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-11 20:34:47.000000 flox-0.7.2/ci/no-xarray.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-11 20:34:47.000000 flox-0.7.2/ci/upstream-dev-env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-11 20:34:47.000000 flox-0.7.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.614069 flox-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-11 20:34:47.000000 flox-0.7.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.618069 flox-0.7.2/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)    43022 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/blockwise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/cohorts-month-chunk4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/cohorts-month-chunk5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46006 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/map-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-blockwise-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-blockwise.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   102136 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-cohorts-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60369 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-cohorts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105406 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-map-reduce-reindex-False-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62434 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-map-reduce-reindex-False.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   101278 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-map-reduce-reindex-True-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62159 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-map-reduce-reindex-True.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   177642 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/new-split-apply-combine-annotated.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61350 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/split-apply-combine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-05-11 20:34:47.000000 flox-0.7.2/docs/diagrams/split-reduce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-11 20:34:47.000000 flox-0.7.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 20:34:47.000000 flox-0.7.2/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.622069 flox-0.7.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.626070 flox-0.7.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/aggregations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/arrays.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/engines.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.626070 flox-0.7.2/docs/source/user-stories/
+-rw-r--r--   0 runner    (1001) docker     (123)    74658 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/user-stories/climatology-hourly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/user-stories/climatology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/user-stories/custom-aggregations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   395737 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/user-stories/hourly-climatology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/user-stories/overlaps.md
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/user-stories.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-11 20:34:47.000000 flox-0.7.2/docs/source/xarray.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.630070 flox-0.7.2/flox/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-11 20:34:47.000000 flox-0.7.2/flox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 20:35:19.000000 flox-0.7.2/flox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-11 20:34:47.000000 flox-0.7.2/flox/aggregate_flox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-11 20:34:47.000000 flox-0.7.2/flox/aggregate_npg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18832 2023-05-11 20:34:47.000000 flox-0.7.2/flox/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-11 20:34:47.000000 flox-0.7.2/flox/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73983 2023-05-11 20:34:47.000000 flox-0.7.2/flox/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:34:47.000000 flox-0.7.2/flox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-11 20:34:47.000000 flox-0.7.2/flox/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-05-11 20:34:47.000000 flox-0.7.2/flox/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-11 20:34:47.000000 flox-0.7.2/flox/xrdtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-05-11 20:34:47.000000 flox-0.7.2/flox/xrutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.634070 flox-0.7.2/flox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-05-11 20:35:19.000000 flox-0.7.2/flox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-11 20:35:19.000000 flox-0.7.2/flox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:35:19.000000 flox-0.7.2/flox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 20:35:19.000000 flox-0.7.2/flox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 20:35:19.000000 flox-0.7.2/flox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-11 20:34:47.000000 flox-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 20:34:47.000000 flox-0.7.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:35:19.634070 flox-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 20:34:47.000000 flox-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:19.634070 flox-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-11 20:34:47.000000 flox-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 20:34:47.000000 flox-0.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50161 2023-05-11 20:34:47.000000 flox-0.7.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-05-11 20:34:47.000000 flox-0.7.2/tests/test_xarray.py
```

### Comparing `flox-0.7.1/.github/workflows/benchmarks.yml` & `flox-0.7.2/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.github/workflows/ci-additional.yaml` & `flox-0.7.2/.github/workflows/ci-additional.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.github/workflows/ci.yaml` & `flox-0.7.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.github/workflows/pypi.yaml` & `flox-0.7.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.github/workflows/testpypi-release.yaml` & `flox-0.7.2/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.github/workflows/upstream-dev-ci.yaml` & `flox-0.7.2/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.gitignore` & `flox-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/.pre-commit-config.yaml` & `flox-0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/LICENSE` & `flox-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/PKG-INFO` & `flox-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.7.1
+Version: 0.7.2
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.7.1/README.md` & `flox-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/asv_bench/asv.conf.json` & `flox-0.7.2/asv_bench/asv.conf.json`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/asv_bench/benchmarks/README_CI.md` & `flox-0.7.2/asv_bench/benchmarks/README_CI.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/asv_bench/benchmarks/__init__.py` & `flox-0.7.2/asv_bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/asv_bench/benchmarks/cohorts.py` & `flox-0.7.2/asv_bench/benchmarks/cohorts.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/asv_bench/benchmarks/combine.py` & `flox-0.7.2/asv_bench/benchmarks/combine.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/asv_bench/benchmarks/reduce.py` & `flox-0.7.2/asv_bench/benchmarks/reduce.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/Makefile` & `flox-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/blockwise.png` & `flox-0.7.2/docs/diagrams/blockwise.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/cohorts-month-chunk4.png` & `flox-0.7.2/docs/diagrams/cohorts-month-chunk4.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/cohorts-month-chunk5.png` & `flox-0.7.2/docs/diagrams/cohorts-month-chunk5.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/map-reduce.png` & `flox-0.7.2/docs/diagrams/map-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-blockwise-annotated.svg` & `flox-0.7.2/docs/diagrams/new-blockwise-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-blockwise.svg` & `flox-0.7.2/docs/diagrams/new-blockwise.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-cohorts-annotated.svg` & `flox-0.7.2/docs/diagrams/new-cohorts-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-cohorts.svg` & `flox-0.7.2/docs/diagrams/new-cohorts.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False-annotated.svg` & `flox-0.7.2/docs/diagrams/new-map-reduce-reindex-False-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-False.svg` & `flox-0.7.2/docs/diagrams/new-map-reduce-reindex-False.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True-annotated.svg` & `flox-0.7.2/docs/diagrams/new-map-reduce-reindex-True-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-map-reduce-reindex-True.svg` & `flox-0.7.2/docs/diagrams/new-map-reduce-reindex-True.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/new-split-apply-combine-annotated.svg` & `flox-0.7.2/docs/diagrams/new-split-apply-combine-annotated.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/split-apply-combine.svg` & `flox-0.7.2/docs/diagrams/split-apply-combine.svg`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/diagrams/split-reduce.png` & `flox-0.7.2/docs/diagrams/split-reduce.png`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/make.bat` & `flox-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/aggregations.md` & `flox-0.7.2/docs/source/aggregations.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/api.rst` & `flox-0.7.2/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/arrays.md` & `flox-0.7.2/docs/source/arrays.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/conf.py` & `flox-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/engines.md` & `flox-0.7.2/docs/source/engines.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/implementation.md` & `flox-0.7.2/docs/source/implementation.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/index.md` & `flox-0.7.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/intro.md` & `flox-0.7.2/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/user-stories/climatology-hourly.ipynb` & `flox-0.7.2/docs/source/user-stories/climatology-hourly.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/user-stories/climatology.ipynb` & `flox-0.7.2/docs/source/user-stories/climatology.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/user-stories/custom-aggregations.ipynb` & `flox-0.7.2/docs/source/user-stories/custom-aggregations.ipynb`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/user-stories/hourly-climatology.html` & `flox-0.7.2/docs/source/user-stories/hourly-climatology.html`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/user-stories/overlaps.md` & `flox-0.7.2/docs/source/user-stories/overlaps.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/docs/source/xarray.md` & `flox-0.7.2/docs/source/xarray.md`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/flox/aggregate_flox.py` & `flox-0.7.2/flox/aggregate_flox.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/flox/aggregate_npg.py` & `flox-0.7.2/flox/aggregate_npg.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/flox/aggregations.py` & `flox-0.7.2/flox/aggregations.py`

 * *Files 14% similar despite different names*

```diff
@@ -180,14 +180,16 @@
         # Use "chunk_reduce" or "chunk_argreduce"
         self.reduction_type = reduction_type
         self.numpy: FuncTuple = (numpy,) if numpy else (self.name,)
         # initialize blockwise reduction
         self.chunk: FuncTuple = _atleast_1d(chunk)
         # how to aggregate results after first round of reduction
         self.combine: FuncTuple = _atleast_1d(combine)
+        # simpler reductions used with the "simple combine" algorithm
+        self.simple_combine = None
         # final aggregation
         self.aggregate: Callable | str = aggregate if aggregate else self.combine[0]
         # finalize results (see mean)
         self.finalize: Callable | None = finalize
 
         self.fill_value = {}
         # This is used for the final reindexing
@@ -415,28 +417,28 @@
 
 nanargmax = Aggregation(
     "nanargmax",
     preprocess=argreduce_preprocess,
     chunk=("nanmax", "nanargmax"),  # order is important
     combine=("max", "argmax"),
     reduction_type="argreduce",
-    fill_value=(dtypes.NINF, -1),
+    fill_value=(dtypes.NINF, 0),
     final_fill_value=-1,
     finalize=_pick_second,
     dtypes=(None, np.intp),
     final_dtype=np.intp,
 )
 
 nanargmin = Aggregation(
     "nanargmin",
     preprocess=argreduce_preprocess,
     chunk=("nanmin", "nanargmin"),  # order is important
     combine=("min", "argmin"),
     reduction_type="argreduce",
-    fill_value=(dtypes.INF, -1),
+    fill_value=(dtypes.INF, 0),
     final_fill_value=-1,
     finalize=_pick_second,
     dtypes=(None, np.intp),
     final_dtype=np.intp,
 )
 
 first = Aggregation("first", chunk=None, combine=None, fill_value=0)
@@ -573,8 +575,20 @@
         agg.fill_value["intermediate"] += (0,)
         agg.fill_value["numpy"] += (0,)
         agg.dtype["intermediate"] += (np.intp,)
         agg.dtype["numpy"] += (np.intp,)
     else:
         agg.min_count = 0
 
+    simple_combine = []
+    for combine in agg.combine:
+        if isinstance(combine, str):
+            if combine in ["nanfirst", "nanlast"]:
+                simple_combine.append(getattr(xrutils, combine))
+            else:
+                simple_combine.append(getattr(np, combine))
+        else:
+            simple_combine.append(combine)
+
+    agg.simple_combine = tuple(simple_combine)
+
     return agg
```

### Comparing `flox-0.7.1/flox/core.py` & `flox-0.7.2/flox/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 
 def _is_minmax_reduction(func: T_Agg) -> bool:
     return not _is_arg_reduction(func) and (
         isinstance(func, str) and ("max" in func or "min" in func)
     )
 
 
+def _is_first_last_reduction(func: T_Agg) -> bool:
+    return isinstance(func, str) and func in ["nanfirst", "nanlast", "first", "last"]
+
+
 def _get_expected_groups(by: T_By, sort: bool) -> pd.Index:
     if is_duck_dask_array(by):
         raise ValueError("Please provide expected_groups if not grouping by a numpy array.")
     flatby = by.reshape(-1)
     expected = pd.unique(flatby[~isnull(flatby)])
     return _convert_expected_groups_to_index((expected,), isbin=(False,), sort=sort)[0]
 
@@ -950,21 +954,21 @@
         )
     else:
         unique_groups = deepfirst(x_chunk)["groups"]
 
     results: IntermediateDict = {"groups": unique_groups}
     results["intermediates"] = []
     axis_ = axis[:-1] + (DUMMY_AXIS,)
-    for idx, combine in enumerate(agg.combine):
+    for idx, combine in enumerate(agg.simple_combine):
         array = _conc2(x_chunk, key1="intermediates", key2=idx, axis=axis_)
         assert array.ndim >= 2
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", r"All-NaN (slice|axis) encountered")
-            assert isinstance(combine, str)
-            result = getattr(np, combine)(array, axis=axis_, keepdims=True)
+            assert callable(combine)
+            result = combine(array, axis=axis_, keepdims=True)
         if is_aggregate:
             # squeeze out DUMMY_AXIS if this is the last step i.e. called from _aggregate
             result = result.squeeze(axis=DUMMY_AXIS)
         results["intermediates"].append(result)
     return results
 
 
@@ -1315,16 +1319,19 @@
         # This removes an extra rechunk-merge layer that would be
         # added otherwise
         chunks = tuple(array.chunks[ax] if by.shape[ax] != 1 else (1,) for ax in range(-by.ndim, 0))
 
         by = dask.array.from_array(by, chunks=chunks)
     _, (array, by) = dask.array.unify_chunks(array, inds, by, inds[-by.ndim :])
 
-    # preprocess the array: for argreductions, this zips the index together with the array block
-    if agg.preprocess:
+    # preprocess the array:
+    #   - for argreductions, this zips the index together with the array block
+    #   - not necessary for blockwise with argreductions
+    #   - if this is needed later, we can fix this then
+    if agg.preprocess and method != "blockwise":
         array = agg.preprocess(array, axis=axis)
 
     # 1. We first apply the groupby-reduction blockwise to generate "intermediates"
     # 2. These intermediate results are combined to generate the final result using a
     #    "map-reduce" or "tree reduction" approach.
     #    There are two ways:
     #    a. "_simple_combine": Where it makes sense, we tree-reduce the reduction,
@@ -1530,32 +1537,39 @@
     if reindex is True and not all_numpy:
         if _is_arg_reduction(func):
             raise NotImplementedError
         if method in ["blockwise", "cohorts"]:
             raise ValueError(
                 "reindex=True is not a valid choice for method='blockwise' or method='cohorts'."
             )
+        if func in ["first", "last"]:
+            raise ValueError("reindex must be None or False when func is 'first' or 'last.")
 
     if reindex is None:
         if all_numpy:
             return True
 
+        if func in ["first", "last"]:
+            # have to do the grouped_combine since there's no good fill_value
+            reindex = False
+
         if method == "blockwise" or _is_arg_reduction(func):
             reindex = False
 
         elif method == "cohorts":
             reindex = False
 
         elif method == "map-reduce":
             if expected_groups is None and any_by_dask:
                 reindex = False
             else:
                 reindex = True
 
     assert isinstance(reindex, bool)
+
     return reindex
 
 
 def _assert_by_is_aligned(shape: tuple[int, ...], by: T_Bys):
     assert all(b.ndim == by[0].ndim for b in by[1:])
     for idx, b in enumerate(by):
         if not all(j in [i, 1] for i, j in zip(shape[-b.ndim :], b.shape)):
@@ -1871,14 +1885,29 @@
     if axis is None:
         axis_ = tuple(array.ndim + np.arange(-by_.ndim, 0))
     else:
         # TODO: How come this function doesn't exist according to mypy?
         axis_ = np.core.numeric.normalize_axis_tuple(axis, array.ndim)  # type: ignore
     nax = len(axis_)
 
+    has_dask = is_duck_dask_array(array) or is_duck_dask_array(by_)
+
+    if _is_first_last_reduction(func):
+        if has_dask and nax != 1:
+            raise ValueError(
+                "For dask arrays: first, last, nanfirst, nanlast reductions are "
+                "only supported along a single axis. Please reshape appropriately."
+            )
+
+        elif nax not in [1, by_.ndim]:
+            raise ValueError(
+                "first, last, nanfirst, nanlast reductions are only supported "
+                "along a single axis or when reducing across all dimensions of `by`."
+            )
+
     # TODO: make sure expected_groups is unique
     if nax == 1 and by_.ndim > 1 and expected_groups is None:
         if not any_by_dask:
             expected_groups = _get_expected_groups(by_, sort)
         else:
             # When we reduce along all axes, we are guaranteed to see all
             # groups in the final combine stage, so everything works.
@@ -1894,16 +1923,14 @@
     assert nax <= by_.ndim
     if nax < by_.ndim:
         by_ = _move_reduce_dims_to_end(by_, tuple(-array.ndim + ax + by_.ndim for ax in axis_))
         array = _move_reduce_dims_to_end(array, axis_)
         axis_ = tuple(array.ndim + np.arange(-nax, 0))
         nax = len(axis_)
 
-    has_dask = is_duck_dask_array(array) or is_duck_dask_array(by_)
-
     # When axis is a subset of possible values; then npg will
     # apply it to groups that don't exist along a particular axis (for e.g.)
     # since these count as a group that is absent. thoo!
     # fill_value applies to all-NaN groups as well as labels in expected_groups that are not found.
     #     The only way to do this consistently is mask out using min_count
     #     Consider np.sum([np.nan]) = np.nan, np.nansum([np.nan]) = 0
     if min_count is None:
@@ -1982,10 +2009,10 @@
         # now we get rid of them by reindexing
         # This also handles bins with no data
         result = reindex_(
             result, from_=groups[0], to=expected_groups, fill_value=fill_value
         ).reshape(result.shape[:-1] + grp_shape)
         groups = final_groups
 
-    if _is_minmax_reduction(func) and is_bool_array:
+    if is_bool_array and (_is_minmax_reduction(func) or _is_first_last_reduction(func)):
         result = result.astype(bool)
     return (result, *groups)  # type: ignore[return-value]  # Unpack not in mypy yet
```

### Comparing `flox-0.7.1/flox/visualize.py` & `flox-0.7.2/flox/visualize.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/flox/xarray.py` & `flox-0.7.2/flox/xarray.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/flox/xrdtypes.py` & `flox-0.7.2/flox/xrdtypes.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/flox/xrutils.py` & `flox-0.7.2/flox/xrutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # The functions defined here were copied based on the source code
 # defined in xarray
 
-
 import datetime
 from typing import Any, Iterable
 
 import numpy as np
 import pandas as pd
+from numpy.core.multiarray import normalize_axis_index  # type: ignore[attr-defined]
 
 try:
     import cftime
 except ImportError:
     cftime = None
 
 
@@ -279,7 +279,40 @@
             if is_duck_dask_array(sample):
                 sample = sample.compute()
                 if isinstance(sample, np.ndarray):
                     sample = sample.item()
             return isinstance(sample, cftime.datetime)
         else:
             return False
+
+
+def _select_along_axis(values, idx, axis):
+    other_ind = np.ix_(*[np.arange(s) for s in idx.shape])
+    sl = other_ind[:axis] + (idx,) + other_ind[axis:]
+    return values[sl]
+
+
+def nanfirst(values, axis, keepdims=False):
+    if isinstance(axis, tuple):
+        (axis,) = axis
+    values = np.asarray(values)
+    axis = normalize_axis_index(axis, values.ndim)
+    idx_first = np.argmax(~pd.isnull(values), axis=axis)
+    result = _select_along_axis(values, idx_first, axis)
+    if keepdims:
+        return np.expand_dims(result, axis=axis)
+    else:
+        return result
+
+
+def nanlast(values, axis, keepdims=False):
+    if isinstance(axis, tuple):
+        (axis,) = axis
+    values = np.asarray(values)
+    axis = normalize_axis_index(axis, values.ndim)
+    rev = (slice(None),) * axis + (slice(None, None, -1),)
+    idx_last = -1 - np.argmax(~pd.isnull(values)[rev], axis=axis)
+    result = _select_along_axis(values, idx_last, axis)
+    if keepdims:
+        return np.expand_dims(result, axis=axis)
+    else:
+        return result
```

### Comparing `flox-0.7.1/flox.egg-info/PKG-INFO` & `flox-0.7.2/flox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flox
-Version: 0.7.1
+Version: 0.7.2
 Summary: GroupBy operations for dask.array
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flox-0.7.1/flox.egg-info/SOURCES.txt` & `flox-0.7.2/flox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/pyproject.toml` & `flox-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/tests/__init__.py` & `flox-0.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flox-0.7.1/tests/test_core.py` & `flox-0.7.2/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import itertools
 import warnings
 from functools import partial, reduce
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 import pandas as pd
 import pytest
 from numpy_groupies.aggregate_numpy import aggregate
 
+from flox import xrutils
 from flox.aggregations import Aggregation
 from flox.core import (
     _convert_expected_groups_to_index,
     _get_optimal_chunks_for_groups,
     _normalize_indexes,
     _validate_reindex,
     factorize_,
@@ -49,39 +50,56 @@
         return None
 
 
 ALL_FUNCS = (
     "sum",
     "nansum",
     "argmax",
-    pytest.param("nanargmax", marks=(pytest.mark.skip,)),
+    "nanfirst",
+    "nanargmax",
     "prod",
     "nanprod",
     "mean",
     "nanmean",
     "var",
     "nanvar",
     "std",
     "nanstd",
     "max",
     "nanmax",
     "min",
     "nanmin",
     "argmin",
-    pytest.param("nanargmin", marks=(pytest.mark.skip,)),
+    "nanargmin",
     "any",
     "all",
+    "nanlast",
     pytest.param("median", marks=(pytest.mark.skip,)),
     pytest.param("nanmedian", marks=(pytest.mark.skip,)),
 )
 
 if TYPE_CHECKING:
     from flox.core import T_Engine, T_ExpectedGroupsOpt, T_Func2
 
 
+def _get_array_func(func: str) -> Callable:
+    if func == "count":
+
+        def npfunc(x):
+            x = np.asarray(x)
+            return (~np.isnan(x)).sum()
+
+    elif func in ["nanfirst", "nanlast"]:
+        npfunc = getattr(xrutils, func)
+    else:
+        npfunc = getattr(np, func)
+
+    return npfunc
+
+
 def test_alignment_error():
     da = np.ones((12,))
     labels = np.ones((5,))
 
     with pytest.raises(ValueError):
         groupby_reduce(da, labels, func="mean")
 
@@ -211,16 +229,25 @@
                 warnings.filterwarnings("ignore", r"All-NaN (slice|axis) encountered")
                 warnings.filterwarnings("ignore", r"Degrees of freedom <= 0 for slice")
                 warnings.filterwarnings("ignore", r"Mean of empty slice")
 
                 # computing silences a bunch of dask warnings
                 array_ = array.compute() if chunks is not None else array
                 if "arg" in func and add_nan_by:
+                    # NaNs are in by, but we can't call np.argmax([..., NaN, .. ])
+                    # That would return index of the NaN
+                    # This way, we insert NaNs where there are NaNs in by, and
+                    # call np.nanargmax
+                    func_ = f"nan{func}" if "nan" not in func else func
                     array_[..., nanmask] = np.nan
-                    expected = getattr(np, "nan" + func)(array_, axis=-1, **kwargs)
+                    expected = getattr(np, func_)(array_, axis=-1, **kwargs)
+                # elif func in ["first", "last"]:
+                #    expected = getattr(xrutils, f"nan{func}")(array_[..., ~nanmask], axis=-1, **kwargs)
+                elif func in ["nanfirst", "nanlast"]:
+                    expected = getattr(xrutils, func)(array_[..., ~nanmask], axis=-1, **kwargs)
                 else:
                     expected = getattr(np, func)(array_[..., ~nanmask], axis=-1, **kwargs)
         for _ in range(nby):
             expected = np.expand_dims(expected, -1)
 
         actual, *groups = groupby_reduce(array, *by, **flox_kwargs)
         assert actual.ndim == (array.ndim + nby - 1)
@@ -233,29 +260,33 @@
         assert_equal(actual, expected, tolerance)
 
         if not has_dask or chunks is None:
             continue
 
         params = list(itertools.product(["map-reduce"], [True, False, None]))
         params.extend(itertools.product(["cohorts"], [False, None]))
+        if chunks == -1:
+            params.extend([("blockwise", None)])
+
         for method, reindex in params:
             call = partial(
                 groupby_reduce, array, *by, method=method, reindex=reindex, **flox_kwargs
             )
-            if "arg" in func and reindex is True:
+            if ("arg" in func or func in ["first", "last"]) and reindex is True:
                 # simple_combine with argreductions not supported right now
                 with pytest.raises(NotImplementedError):
                     call()
                 continue
             actual, *groups = call()
-            if "arg" not in func:
-                # make sure we use simple combine
-                assert any("simple-combine" in key for key in actual.dask.layers.keys())
-            else:
-                assert any("grouped-combine" in key for key in actual.dask.layers.keys())
+            if method != "blockwise":
+                if "arg" not in func:
+                    # make sure we use simple combine
+                    assert any("simple-combine" in key for key in actual.dask.layers.keys())
+                else:
+                    assert any("grouped-combine" in key for key in actual.dask.layers.keys())
             for actual_group, expect in zip(groups, expected_groups):
                 assert_equal(actual_group, expect, tolerance)
             if "arg" in func:
                 assert actual.dtype.kind == "i"
             assert_equal(actual, expected, tolerance)
 
 
@@ -482,25 +513,51 @@
             da.from_array(array, chunks=(1, 3, 2)),
             da.from_array(by, chunks=(2, 2, 2)),
             func="count",
             axis=2,
         )
 
 
+@pytest.mark.parametrize("func", ["first", "last", "nanfirst", "nanlast"])
+@pytest.mark.parametrize("axis", [(0, 1)])
+def test_first_last_disallowed(axis, func):
+    with pytest.raises(ValueError):
+        groupby_reduce(np.empty((2, 3, 2)), np.ones((2, 3, 2)), func=func, axis=axis)
+
+
+@requires_dask
+@pytest.mark.parametrize("func", ["nanfirst", "nanlast"])
+@pytest.mark.parametrize("axis", [None, (0, 1, 2)])
+def test_nanfirst_nanlast_disallowed_dask(axis, func):
+    with pytest.raises(ValueError):
+        groupby_reduce(dask.array.empty((2, 3, 2)), np.ones((2, 3, 2)), func=func, axis=axis)
+
+
+@requires_dask
+@pytest.mark.parametrize("func", ["first", "last"])
+def test_first_last_disallowed_dask(func):
+    with pytest.raises(NotImplementedError):
+        groupby_reduce(dask.array.empty((2, 3, 2)), np.ones((2, 3, 2)), func=func, axis=-1)
+
+
 @requires_dask
 @pytest.mark.parametrize("func", ALL_FUNCS)
 @pytest.mark.parametrize(
     "axis", [None, (0, 1, 2), (0, 1), (0, 2), (1, 2), 0, 1, 2, (0,), (1,), (2,)]
 )
 def test_groupby_reduce_axis_subset_against_numpy(func, axis, engine):
     if "arg" in func and engine == "flox":
         pytest.skip()
 
-    if not isinstance(axis, int) and "arg" in func and (axis is None or len(axis) > 1):
-        pytest.skip()
+    if not isinstance(axis, int):
+        if "arg" in func and (axis is None or len(axis) > 1):
+            pytest.skip()
+        if ("first" in func or "last" in func) and (axis is not None and len(axis) not in [1, 3]):
+            pytest.skip()
+
     if func in ["all", "any"]:
         fill_value = False
     else:
         fill_value = 123
 
     if "var" in func or "std" in func:
         tolerance = {"rtol": 1e-14, "atol": 1e-16}
@@ -509,25 +566,53 @@
     # tests against the numpy output to make sure dask compute matches
     by = np.broadcast_to(labels2d, (3, *labels2d.shape))
     rng = np.random.default_rng(12345)
     array = rng.random(by.shape)
     kwargs = dict(
         func=func, axis=axis, expected_groups=[0, 2], fill_value=fill_value, engine=engine
     )
+    expected, _ = groupby_reduce(array, by, **kwargs)
+    if engine == "flox":
+        kwargs.pop("engine")
+        expected_npg, _ = groupby_reduce(array, by, **kwargs, engine="numpy")
+        assert_equal(expected_npg, expected)
+
+    if func in ["all", "any"]:
+        fill_value = False
+    else:
+        fill_value = 123
+
+    if "var" in func or "std" in func:
+        tolerance = {"rtol": 1e-14, "atol": 1e-16}
+    else:
+        tolerance = None
+    # tests against the numpy output to make sure dask compute matches
+    by = np.broadcast_to(labels2d, (3, *labels2d.shape))
+    rng = np.random.default_rng(12345)
+    array = rng.random(by.shape)
+    kwargs = dict(
+        func=func, axis=axis, expected_groups=[0, 2], fill_value=fill_value, engine=engine
+    )
+    expected, _ = groupby_reduce(array, by, **kwargs)
+    if engine == "flox":
+        kwargs.pop("engine")
+        expected_npg, _ = groupby_reduce(array, by, **kwargs, engine="numpy")
+        assert_equal(expected_npg, expected)
+
+    if ("first" in func or "last" in func) and (
+        axis is None or (not isinstance(axis, int) and len(axis) != 1)
+    ):
+        return
+
     with raise_if_dask_computes():
         actual, _ = groupby_reduce(
             da.from_array(array, chunks=(-1, 2, 3)),
             da.from_array(by, chunks=(-1, 2, 2)),
             **kwargs,
         )
-    expected, _ = groupby_reduce(array, by, **kwargs)
-    if engine == "flox":
-        kwargs.pop("engine")
-        expected_npg, _ = groupby_reduce(array, by, **kwargs, engine="numpy")
-        assert_equal(expected_npg, expected)
     assert_equal(actual, expected, tolerance)
 
 
 @pytest.mark.parametrize("reindex,chunks", [(None, None), (False, (2, 2, 3)), (True, (2, 2, 3))])
 @pytest.mark.parametrize(
     "axis, groups, expected_shape",
     [
@@ -747,31 +832,25 @@
     # fill_value = np.nan tests promotion of int counts to float
     # This is used by xarray
     if func in ["all", "any"] or "arg" in func:
         pytest.skip()
     if chunks is not None and not has_dask:
         pytest.skip()
 
-    if func == "count":
-
-        def npfunc(x):
-            x = np.asarray(x)
-            return (~np.isnan(x)).sum()
-
-    else:
-        npfunc = getattr(np, func)
-
+    npfunc = _get_array_func(func)
     by = np.array([1, 2, 3, 1, 2, 3])
     array = np.array([np.nan, 1, 1, np.nan, 1, 1])
     if chunks:
         array = dask.array.from_array(array, chunks)
     actual, _ = groupby_reduce(
         array, by, func=func, engine=engine, fill_value=fill_value, expected_groups=[0, 1, 2, 3]
     )
-    expected = np.array([fill_value, fill_value, npfunc([1.0, 1.0]), npfunc([1.0, 1.0])])
+    expected = np.array(
+        [fill_value, fill_value, npfunc([1.0, 1.0], axis=0), npfunc([1.0, 1.0], axis=0)]
+    )
     assert_equal(actual, expected)
 
 
 @requires_dask
 @pytest.mark.parametrize("func", ["mean", "sum"])
 @pytest.mark.parametrize("dtype", ["float32", "float64", "int32", "int64"])
 def test_dtype_preservation(dtype, func, engine):
@@ -828,14 +907,16 @@
     if func in ["any", "all"]:
         fill_value = False
     else:
         fill_value = -123
 
     if axis is not None and method != "map-reduce":
         pytest.xfail()
+    if axis is None and ("first" in func or "last" in func):
+        pytest.skip()
 
     kwargs = dict(func=func, engine=engine, method=method, axis=axis, fill_value=fill_value)
     actual, groups = groupby_reduce(array, by, **kwargs)
     expected, sorted_groups = groupby_reduce(array.compute(), by, **kwargs)
     assert_equal(groups, sorted_groups)
     assert_equal(actual, expected)
 
@@ -893,15 +974,16 @@
 
 @pytest.mark.parametrize("func", ALL_FUNCS)
 def test_bool_reductions(func, engine):
     if "arg" in func and engine == "flox":
         pytest.skip()
     groups = np.array([1, 1, 1])
     data = np.array([True, True, False])
-    expected = np.expand_dims(getattr(np, func)(data), -1)
+    npfunc = _get_array_func(func)
+    expected = np.expand_dims(npfunc(data, axis=0), -1)
     actual, _ = groupby_reduce(data, groups, func=func, engine=engine)
     assert_equal(expected, actual)
 
 
 @requires_dask
 def test_map_reduce_blockwise_mixed() -> None:
     t = pd.date_range("2000-01-01", "2000-12-31", freq="D").to_series()
```

### Comparing `flox-0.7.1/tests/test_xarray.py` & `flox-0.7.2/tests/test_xarray.py`

 * *Files identical despite different names*


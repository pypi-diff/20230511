# Comparing `tmp/napari-spatialdata-0.2.2.tar.gz` & `tmp/napari-spatialdata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-spatialdata-0.2.2.tar", last modified: Thu May  4 14:27:21 2023, max compression
+gzip compressed data, was "napari-spatialdata-0.2.3.tar", last modified: Thu May 11 11:24:02 2023, max compression
```

## Comparing `napari-spatialdata-0.2.2.tar` & `napari-spatialdata-0.2.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.263920 napari-spatialdata-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/extensions/typed_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.275920 napari-spatialdata-0.2.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/notebooks/mibitof_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/notebooks/nanostring_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/notebooks/spatialdata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/template_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.283920 napari-spatialdata-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/examples/spatialdata_mibitof.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/examples/spatialdata_nanostring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/src/napari_spatialdata/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_categoricals_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_spatialdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.212270 napari-spatialdata-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.224270 napari-spatialdata-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.224270 napari-spatialdata-0.2.3/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.232270 napari-spatialdata-0.2.3/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.240270 napari-spatialdata-0.2.3/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/notebooks/mibitof_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/notebooks/nanostring_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/notebooks/spatialdata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/template_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.248269 napari-spatialdata-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/spatialdata_mibitof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/spatialdata_nanostring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/spatialdata_visium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-11 11:24:02.260269 napari-spatialdata-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.216270 napari-spatialdata-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.252269 napari-spatialdata-0.2.3/src/napari_spatialdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_categoricals_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_pkg_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_spatialdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tox.ini
```

### Comparing `napari-spatialdata-0.2.2/.github/workflows/test_and_deploy.yml` & `napari-spatialdata-0.2.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/.gitignore` & `napari-spatialdata-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/.mypy.ini` & `napari-spatialdata-0.2.3/.mypy.ini`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/.napari/DESCRIPTION.md` & `napari-spatialdata-0.2.3/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/.pre-commit-config.yaml` & `napari-spatialdata-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/LICENSE` & `napari-spatialdata-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/PKG-INFO` & `napari-spatialdata-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.2
+Version: 0.2.3
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.2/README.md` & `napari-spatialdata-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/Makefile` & `napari-spatialdata-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/_templates/autosummary/class.rst` & `napari-spatialdata-0.2.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/conf.py` & `napari-spatialdata-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/contributing.md` & `napari-spatialdata-0.2.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/extensions/typed_returns.py` & `napari-spatialdata-0.2.3/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/make.bat` & `napari-spatialdata-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/notebooks/mibitof_analysis.ipynb` & `napari-spatialdata-0.2.3/docs/notebooks/mibitof_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/notebooks/nanostring_analysis.ipynb` & `napari-spatialdata-0.2.3/docs/notebooks/nanostring_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/notebooks/spatialdata.ipynb` & `napari-spatialdata-0.2.3/docs/notebooks/spatialdata.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/references.bib` & `napari-spatialdata-0.2.3/docs/references.bib`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/docs/template_usage.md` & `napari-spatialdata-0.2.3/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/pyproject.toml` & `napari-spatialdata-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/setup.cfg` & `napari-spatialdata-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/__init__.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_categoricals_utils.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_categoricals_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_pkg_constants.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_pkg_constants.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_utils.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_interactive.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_interactive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, Iterable, Union
 
 import napari
 import numpy as np
+import shapely
 from anndata import AnnData
 from loguru import logger
 from multiscale_spatial_image import MultiscaleSpatialImage
 from napari.viewer import Viewer
 from qtpy.QtWidgets import QLabel, QListWidget, QListWidgetItem, QVBoxLayout, QWidget
 from spatialdata import SpatialData
 
-from napari_spatialdata._utils import NDArrayA, _get_transform
+from napari_spatialdata._utils import NDArrayA, _get_transform, _swap_coordinates
 
 
 class ElementWidget(QListWidget):
     def __init__(self, sdata: SpatialData):
         super().__init__()
         self._sdata = sdata
 
@@ -67,17 +68,74 @@
     def _onClick(self, text: str) -> None:
         if self.elements_widget._elements[text] == "labels":
             self._add_label(text)
         elif self.elements_widget._elements[text] == "images":
             self._add_image(text)
         elif self.elements_widget._elements[text] == "points":
             self._add_points(text)
+        elif self.elements_widget._elements[text] == "shapes":
+            self._add_shapes(text)
+
+    def _add_circles(self, key: str) -> None:
+        circles = []
+        df = self._sdata.shapes[key]
+        affine = _get_transform(self._sdata.shapes[key], self.coordinate_system_widget._system)
+
+        for i in range(0, len(df)):
+            circles.append([df.geometry[i].coords[0], [df.radius[i], df.radius[i]]])
+
+        circles = _swap_coordinates(circles)
+
+        self._viewer.add_shapes(
+            circles,
+            name=key,
+            affine=affine,
+            shape_type="ellipse",
+            metadata={
+                "adata": self._sdata.table[
+                    self._sdata.table.obs[self._sdata.table.uns["spatialdata_attrs"]["region_key"]] == key
+                ],
+                "shapes_key": self._sdata.table.uns["spatialdata_attrs"]["region_key"],
+            },
+        )
+
+    def _add_polygons(self, key: str) -> None:
+        polygons = []
+        df = self._sdata.shapes[key]
+        affine = _get_transform(self._sdata.shapes[key], self.coordinate_system_widget._system)
+
+        for i in range(0, len(df)):
+            polygons.append(list(df.geometry[i].exterior.coords))
+
+        polygons = _swap_coordinates(polygons)
+
+        self._viewer.add_shapes(
+            polygons,
+            name=key,
+            affine=affine,
+            shape_type="polygon",
+            metadata={
+                "adata": self._sdata.table[
+                    self._sdata.table.obs[self._sdata.table.uns["spatialdata_attrs"]["region_key"]] == key
+                ],
+                "shapes_key": self._sdata.table.uns["spatialdata_attrs"]["region_key"],
+            },
+        )
+
+    def _add_shapes(self, key: str) -> None:
+        if type(self._sdata.shapes[key].iloc[0][0]) == shapely.geometry.point.Point:
+            self._add_circles(key)
+        elif type(self._sdata.shapes[key].iloc[0][0]) == shapely.geometry.polygon.Polygon:
+            self._add_polygons(key)
+        else:
+            raise TypeError("Incorrect data type passed for shapes (should be Shapely Point or Polygon).")
 
     def _add_label(self, key: str) -> None:
         affine = _get_transform(self._sdata.labels[key], self.coordinate_system_widget._system)
+
         self._viewer.add_labels(
             self._sdata.labels[key],
             name=key,
             affine=affine,
             metadata={
                 "adata": self._sdata.table[
                     self._sdata.table.obs[self._sdata.table.uns["spatialdata_attrs"]["region_key"]] == key
@@ -85,14 +143,15 @@
                 "labels_key": self._sdata.table.uns["spatialdata_attrs"]["instance_key"],
             },
         )
 
     def _add_image(self, key: str) -> None:
         img = self._sdata.images[key]
         affine = _get_transform(self._sdata.images[key], self.coordinate_system_widget._system)
+
         if isinstance(img, MultiscaleSpatialImage):
             img = img["scale0"][key]
         # TODO: type check
         self._viewer.add_image(
             img,
             name=key,
             affine=affine,
```

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_model.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_model.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_scatterwidgets.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_utils.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from dask.dataframe.core import DataFrame as DaskDataFrame
 from geopandas import GeoDataFrame
 from loguru import logger
@@ -166,14 +166,18 @@
     maxx, minn = np.nanmax(vec), np.nanmin(vec)
 
     return (  # type: ignore[no-any-return]
         np.ones_like(vec) if np.isclose(minn, maxx) else ((vec - minn) / (maxx - minn))
     )
 
 
+def _swap_coordinates(data: List[Any]) -> List[Any]:
+    return [[(y, x) for x, y in sublist] for sublist in data]
+
+
 def _get_transform(element: SpatialElement, coordinate_system_name: Optional[str] = None) -> NDArrayA:
     affine: NDArrayA
     transformations = get_transformation(element, get_all=True)
     cs = transformations.keys().__iter__().__next__() if coordinate_system_name is None else coordinate_system_name
     ct = transformations[cs]
     affine = ct.to_affine_matrix(input_axes=("y", "x"), output_axes=("y", "x"))
```

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_view.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_view.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/_widgets.py` & `napari-spatialdata-0.2.3/src/napari_spatialdata/_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata/napari.yaml` & `napari-spatialdata-0.2.3/src/napari_spatialdata/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/PKG-INFO` & `napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.2
+Version: 0.2.3
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/SOURCES.txt` & `napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/extensions/typed_returns.py
 docs/notebooks/mibitof_analysis.ipynb
 docs/notebooks/nanostring_analysis.ipynb
 docs/notebooks/spatialdata.ipynb
 examples/README.md
 examples/spatialdata_mibitof.py
 examples/spatialdata_nanostring.py
+examples/spatialdata_visium.py
 src/napari_spatialdata/__init__.py
 src/napari_spatialdata/_categoricals_utils.py
 src/napari_spatialdata/_interactive.py
 src/napari_spatialdata/_model.py
 src/napari_spatialdata/_scatterwidgets.py
 src/napari_spatialdata/_utils.py
 src/napari_spatialdata/_version.py
```

### Comparing `napari-spatialdata-0.2.2/tests/conftest.py` & `napari-spatialdata-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/tests/test_interactive.py` & `napari-spatialdata-0.2.3/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/tests/test_scatterwidgets.py` & `napari-spatialdata-0.2.3/tests/test_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/tests/test_spatialdata.py` & `napari-spatialdata-0.2.3/tests/test_spatialdata.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/tests/test_utils.py` & `napari-spatialdata-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.2/tox.ini` & `napari-spatialdata-0.2.3/tox.ini`

 * *Files identical despite different names*


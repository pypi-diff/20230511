# Comparing `tmp/pythermalcomfort-2.7.1.tar.gz` & `tmp/pythermalcomfort-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythermalcomfort-2.7.1.tar", last modified: Mon May  8 04:25:15 2023, max compression
+gzip compressed data, was "pythermalcomfort-2.7.2.tar", last modified: Thu May 11 02:25:42 2023, max compression
```

## Comparing `pythermalcomfort-2.7.1.tar` & `pythermalcomfort-2.7.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/appveyor-with-compiler.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/templates/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/ci/templates/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/contact_us.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/reference/pythermalcomfort.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_adaptive_ASHRAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_adaptive_EN.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_jos3.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_phs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_pmv_ppd.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_set_tmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/examples/calc_utci.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.085373 pythermalcomfort-2.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/src/pythermalcomfort/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/thermoregulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   176008 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/optimized_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/psychrometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/shared_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/src/pythermalcomfort/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 04:25:14.000000 pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 04:25:15.089373 pythermalcomfort-2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tests/test_jos3.py
--rw-r--r--   0 runner    (1001) docker     (123)    41005 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tests/test_pythermalcomfort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 04:25:05.000000 pythermalcomfort-2.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/appveyor-with-compiler.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/templates/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/ci/templates/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/contact_us.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.628900 pythermalcomfort-2.7.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/reference/pythermalcomfort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_adaptive_ASHRAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_adaptive_EN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_phs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_pmv_ppd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_set_tmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/examples/calc_utci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.624899 pythermalcomfort-2.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/src/pythermalcomfort/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37644 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/thermoregulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172325 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/optimized_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/psychrometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/shared_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/src/pythermalcomfort/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 02:25:42.000000 pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:25:42.632900 pythermalcomfort-2.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tests/test_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41005 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tests/test_pythermalcomfort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 02:25:30.000000 pythermalcomfort-2.7.2/tox.ini
```

### Comparing `pythermalcomfort-2.7.1/.appveyor.yml` & `pythermalcomfort-2.7.2/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/.cookiecutterrc` & `pythermalcomfort-2.7.2/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/.readthedocs.yml` & `pythermalcomfort-2.7.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/.travis.yml` & `pythermalcomfort-2.7.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/AUTHORS.rst` & `pythermalcomfort-2.7.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/CHANGELOG.rst` & `pythermalcomfort-2.7.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/CONTRIBUTING.rst` & `pythermalcomfort-2.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/LICENSE` & `pythermalcomfort-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/PKG-INFO` & `pythermalcomfort-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pythermalcomfort
-Version: 2.7.1
+Version: 2.7.2
 Summary: Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578
 Home-page: https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort
 Author: Federico Tartarini
 Author-email: cbecomforttool@gmail.com
 License: MIT
 Project-URL: Documentation, https://pythermalcomfort.readthedocs.io/
 Project-URL: Changelog, https://pythermalcomfort.readthedocs.io/en/latest/changelog.html
```

### Comparing `pythermalcomfort-2.7.1/README.rst` & `pythermalcomfort-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/ci/appveyor-with-compiler.cmd` & `pythermalcomfort-2.7.2/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/ci/bootstrap.py` & `pythermalcomfort-2.7.2/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/ci/templates/.appveyor.yml` & `pythermalcomfort-2.7.2/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/ci/templates/.travis.yml` & `pythermalcomfort-2.7.2/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/docs/conf.py` & `pythermalcomfort-2.7.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "pythermalcomfort"
 year = "2019"
 author = "Federico Tartarini"
 copyright = "{0}, {1}".format(year, author)
-version = release = "2.7.1"
+version = release = "2.7.2"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": (
         "https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort/issues/%s",
         "#",
```

### Comparing `pythermalcomfort-2.7.1/docs/contact_us.rst` & `pythermalcomfort-2.7.2/docs/contact_us.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/docs/reference/pythermalcomfort.rst` & `pythermalcomfort-2.7.2/docs/reference/pythermalcomfort.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 -------------------
 
 .. autofunction:: pythermalcomfort.models.cooling_effect
 
 Joint system thermoregulation model (JOS-3)
 -------------------------------------------
 
-.. autofunction:: pythermalcomfort.models.JOS3
-
+.. autoclass:: pythermalcomfort.models.JOS3
+    :members:
+    :undoc-members:
+    :show-inheritance:
 
 Adaptive Thermal Heat Balance (ATHB)
 ------------------------------------
 
 .. autofunction:: pythermalcomfort.models.athb
 
 Adaptive ASHRAE
```

### Comparing `pythermalcomfort-2.7.1/docs/usage.rst` & `pythermalcomfort-2.7.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/examples/calc_adaptive_ASHRAE.py` & `pythermalcomfort-2.7.2/examples/calc_adaptive_ASHRAE.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/examples/calc_adaptive_EN.py` & `pythermalcomfort-2.7.2/examples/calc_adaptive_EN.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/examples/calc_jos3.py` & `pythermalcomfort-2.7.2/examples/calc_jos3.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/examples/calc_phs.py` & `pythermalcomfort-2.7.2/examples/calc_phs.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/examples/calc_pmv_ppd.py` & `pythermalcomfort-2.7.2/examples/calc_pmv_ppd.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/examples/calc_utci.py` & `pythermalcomfort-2.7.2/examples/calc_utci.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/setup.cfg` & `pythermalcomfort-2.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/setup.py` & `pythermalcomfort-2.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="pythermalcomfort",
-    version="2.7.1",
+    version="2.7.2",
     license="MIT",
     description=(
         "Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET,"
         " adaptive) and convert physical variables. Please cite us if you use this"
         " package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python"
         " package for thermal comfort research. SoftwareX 12, 100578."
         " https://doi.org/10.1016/j.softx.2020.100578"
```

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/cli.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/cli.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/construction.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/construction.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/matrix.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/matrix.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/parameters.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/parameters.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/thermoregulation.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/thermoregulation.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/jos3_functions/utilities.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/jos3_functions/utilities.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/models.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,15 @@
         The ASHRAE 55 2020 limits are 10 < tdb [°C] < 40, 10 < tr [°C] < 40,
         0 < vr [m/s] < 2, 1 < met [met] < 4, and 0 < clo [clo] < 1.5.
         The ISO 7730 2005 limits are 10 < tdb [°C] < 30, 10 < tr [°C] < 40,
         0 < vr [m/s] < 1, 0.8 < met [met] < 4, 0 < clo [clo] < 2, and -2 < PMV < 2.
     airspeed_control : boolean default True
         This only applies if standard = "ASHRAE". By default it is assumed that the
         occupant has control over the airspeed. In this case the ASHRAE 55 Standard does
-        not imposes any airspeed limits. On the other hand, if the occupant has no control
+        not impose any airspeed limits. On the other hand, if the occupant has no control
         over the airspeed the ASHRAE 55 imposes an upper limit for v which varies as a
         function of the operative temperature, for more information please consult the
         Standard.
 
     Returns
     -------
     pmv : float or array-like
@@ -3353,172 +3353,85 @@
     ex_output : None, list or "all", optional
         This is used when you want to display results other than the default output parameters (ex.skin temperature);
         by default, JOS outputs only the most necessary parameters in order to reduce the computational load.
         If the parameters other than the default output parameters are needed,
         specify the list of the desired parameter names in string format like ["bf_skin", "bf_core", "t_artery"].
         If you want to display all output results, set ex_output is "all".
 
-    Setter & Getter
-    ---------------
-    tdb : float or array-like
-        dry bulb air temperature [°C].
-    tr : float or list-like
-        Mean radiant temperature [°C].
-    to : float or list-like
-        Operative temperature [°C].
-    v : float or list-like
-        Air speed [m/s].
-    rh : float or list-like
-        Relative humidity [%].
-    clo : float or list-like
-        Clothing insulation [clo].
-        Note: If you want to input clothing insulation to each body part,
-        it can be input using the dictionaly in utilities.py.
-        :py:meth:`pythermalcomfort.utilities.local_clo_typical_ensembles`.
-    par : float
-        Physical activity ratio [-].
-        This equals the ratio of metaboric rate to basal metablic rate.
-        The par of sitting quietly is 1.2.
-    posture : str
-        Choose a posture from standing, sitting or lying.
-    bodytemp : numpy.ndarray (85,)
-        All segment temperatures of JOS-3
-
-    Getter
-    -------
-    bsa : numpy.ndarray (17,)
-        Body surface areas by local body segments [m2].
-    Rt : numpy.ndarray (17,)
-        Dry heat resistances between the skin and ambience areas by local body segments [K.m2/W].
-    Ret : numpy.ndarray (17,)
-        Wet (Evaporative) heat resistances between the skin and ambience areas by local body segments [Pa.m2/W].
-    w : numpy.ndarray (17,)
-        Skin wettedness on local body segments [-].
-    w_mean : float
-        Mean skin wettedness of the whole body [-].
-    t_skin_mean : float
-        Mean skin temperature of the whole body [°C].
-    t_skin : numpy.ndarray (17,)
-        Skin temperatures by the local body segments [°C].
-    t_core : numpy.ndarray (17,)
-        Skin temperatures by the local body segments [°C].
-    t_cb : numpy.ndarray (1,)
-        Core temperatures by the local body segments [°C].
-    t_artery : numpy.ndarray (17,)
-        Arterial temperatures by the local body segments [°C].
-    t_vein : numpy.ndarray (17,)
-        Vein temperatures by the local body segments [°C].
-    t_superficial_vein : numpy.ndarray (12,)
-        Superfical vein temperatures by the local body segments [°C].
-    t_muscle : numpy.ndarray (2,)
-        Muscle temperatures of head and pelvis [°C].
-    t_fat : numpy.ndarray (2,)
-        fat temperatures of head and pelvis  [°C].
-    BMR : float
-        Basal metabolic rate [W/m2].
-    body_names : list (17)
-        JOS3 body names [-].
-        "head", "neck", "chest", "back", "pelvis",
-        "left_shoulder", "left_arm", "left_hand", "right_shoulder", "right_arm", "right_hand",
-        "left_thigh", "left_leg", "left_hand", "right_thigh", "right_leg" and "right_hand".
-    results : dict
-        output as dictionaly format
-
-    Methods
-    -------
-    _reset_setpt():
-        Reset set-point temperature under steady state calculation.
-    simulate(times, dtime, output):
-        Run JOS-3 model for given times.
-    _run(dtime, passive=False, output=True):
-        Run JOS-3 model once and gets the model parameters.
-    dict_results():
-        Get results as a dictionary with pandas.DataFrame values.
-    to_csv(path=None, folder=None, unit=True, meaning=True):
-        Export results as csv format.
-    _set_ex_q(tissue, value):
-        Set extra heat gain by tissue name.
-
-    Returns (default)
-    -----------------
-    output_params : dict
-        A dictionary including the following output parameters:
-        Q_total : total heat production of the whole body [W]
-        cardiac_output: cardiac output (the sum of the whole blood flow) [L/h]
-        cycle_time: the counts of executing one cycle calculation [-]
-        dt      : time step [sec]
-        pythermalcomfort_version: version of pythermalcomfort [-]
-        q_res   : heat loss by respiration [W]
-        q_skin  : total heat loss from the skin (each body part) [W]
-        simulation_time: simulation times [sec]
-        t_core  : core temperature (each body part) [°C]
-        t_skin  : skin temperature (each body part) [°C]
-        t_skin_mean: mean skin temperature [°C]
-        w       : skin wettedness (each body part) [-]
-        w_mean  : mean skin wettedness [-]
-        weight_loss_by_evap_and_res: weight loss by the evaporation and respiration of the whole body [g/sec]
-
-    Returns (optional)
-    ------------------
-    output_params : dict
-        A dictionary including the following parameters:
-        Q_bmr_core: core heat production by basal metabolism (each body part) [W]
-        Q_bmr_muscle: muscle heat production by basal metabolism (each body part) [W]
-        Q_bmr_skin: skin heat production by basal metabolism (each body part) [W]
-        Q_core  : core total heat production (each body part) [W]
-        Q_fat   : fat total heat production (each body part) [W]
-        Q_muscle: muscle total heat production (each body part) [W]
-        Q_nst   : core heat production by non-shivering thermogenesis (each body part) [W]
-        Q_shiv  : core or muscle heat production by shivering thermogenesis (each body part) [W]
-        Q_skin  : skin total heat production (each body part) [W]
-        Q_work  : core or muscle heat production by work (each body part) [W]
-        Ret     : total clothing evaporative heat resistance (each body part) [m2.kPa/W]
-        Rt      : total clothing heat resistance (each body part) [m2.K/W]
-        age     : age [years]
-        bf_ava_foot: AVA blood flow rate of one foot [L/h]
-        bf_ava_hand: AVA blood flow rate of one hand [L/h]
-        bf_core : core blood flow rate (each body part) [L/h]
-        bf_fat  : fat blood flow rate (each body part) [L/h]
-        bf_muscle: muscle blood flow rate (each body part) [L/h]
-        bf_skin : skin blood flow rate (each body part) [L/h]
-        bsa     : body surface area (each body part) [m2]
-        clo     : clothing insulation (each body part) [clo]
-        e_max   : maximum evaporative heat loss from the skin (each body part) [W]
-        e_skin  : evaporative heat loss from the skin (each body part) [W]
-        e_sweat : evaporative heat loss from the skin by only sweating (each body part) [W]
-        fat     : body fat rate [%]
-        height  : body height [m]
-        met_base_fat: fat heat production by basal metabolism (each body part) [W]
-        name    : name of the model [-]
-        par     : physical activity ratio [-]
-        q_res_latent: latent heat loss by respiration (each body part) [W]
-        q_res_sensible: sensible heat loss by respiration (each body part) [W]
-        q_skin_latent: latent heat loss from the skin (each body part) [W]
-        q_skin_sensible: sensible heat loss from the skin (each body part) [W]
-        rh      : relative humidity (each body part) [%]
-        sex     : sex [-]
-        t_artery: arterial temperature (each body part) [°C]
-        t_cb    : central blood temperature [°C]
-        t_core_set: skin set point temperature (each body part) [°C]
-        t_fat   : fat temperature (each body part) [°C]
-        t_muscle: muscle temperature (each body part) [°C]
-        t_skin_set: core set point temperature (each body part) [°C]
-        t_superficial_vein: superficial vein temperature (each body part) [°C]
-        t_vein  : vein temperature (each body part) [°C]
-        tdb     : dry bulb air temperature (each body part) [°C]
-        to      : operative temperature (each body part) [°C]
-        tr      : mean radiant temperature (each body part) [°C]
-        v       : air velocity (each body part) [m/s]
-        weight  : body weight [kg]
+    Returns
+    -------
+    Q_total : total heat production of the whole body [W]
+    cardiac_output: cardiac output (the sum of the whole blood flow) [L/h]
+    cycle_time: the counts of executing one cycle calculation [-]
+    dt      : time step [sec]
+    pythermalcomfort_version: version of pythermalcomfort [-]
+    q_res   : heat loss by respiration [W]
+    q_skin  : total heat loss from the skin (each body part) [W]
+    simulation_time: simulation times [sec]
+    t_core  : core temperature (each body part) [°C]
+    t_skin  : skin temperature (each body part) [°C]
+    t_skin_mean: mean skin temperature [°C]
+    w       : skin wettedness (each body part) [-]
+    w_mean  : mean skin wettedness [-]
+    weight_loss_by_evap_and_res: weight loss by the evaporation and respiration of the whole body [g/sec]
+    OPTIONAL PARAMETERS : the paramters listed below are returned if ex_output = "all"
+    Q_bmr_core: core heat production by basal metabolism (each body part) [W]
+    Q_bmr_muscle: muscle heat production by basal metabolism (each body part) [W]
+    Q_bmr_skin: skin heat production by basal metabolism (each body part) [W]
+    Q_core  : core total heat production (each body part) [W]
+    Q_fat   : fat total heat production (each body part) [W]
+    Q_muscle: muscle total heat production (each body part) [W]
+    Q_nst   : core heat production by non-shivering thermogenesis (each body part) [W]
+    Q_shiv  : core or muscle heat production by shivering thermogenesis (each body part) [W]
+    Q_skin  : skin total heat production (each body part) [W]
+    Q_work  : core or muscle heat production by work (each body part) [W]
+    Ret     : total clothing evaporative heat resistance (each body part) [m2.kPa/W]
+    Rt      : total clothing heat resistance (each body part) [m2.K/W]
+    age     : age [years]
+    bf_ava_foot: AVA blood flow rate of one foot [L/h]
+    bf_ava_hand: AVA blood flow rate of one hand [L/h]
+    bf_core : core blood flow rate (each body part) [L/h]
+    bf_fat  : fat blood flow rate (each body part) [L/h]
+    bf_muscle: muscle blood flow rate (each body part) [L/h]
+    bf_skin : skin blood flow rate (each body part) [L/h]
+    bsa     : body surface area (each body part) [m2]
+    clo     : clothing insulation (each body part) [clo]
+    e_max   : maximum evaporative heat loss from the skin (each body part) [W]
+    e_skin  : evaporative heat loss from the skin (each body part) [W]
+    e_sweat : evaporative heat loss from the skin by only sweating (each body part) [W]
+    fat     : body fat rate [%]
+    height  : body height [m]
+    met_base_fat: fat heat production by basal metabolism (each body part) [W]
+    name    : name of the model [-]
+    par     : physical activity ratio [-]
+    q_res_latent: latent heat loss by respiration (each body part) [W]
+    q_res_sensible: sensible heat loss by respiration (each body part) [W]
+    q_skin_latent: latent heat loss from the skin (each body part) [W]
+    q_skin_sensible: sensible heat loss from the skin (each body part) [W]
+    rh      : relative humidity (each body part) [%]
+    sex     : sex [-]
+    t_artery: arterial temperature (each body part) [°C]
+    t_cb    : central blood temperature [°C]
+    t_core_set: skin set point temperature (each body part) [°C]
+    t_fat   : fat temperature (each body part) [°C]
+    t_muscle: muscle temperature (each body part) [°C]
+    t_skin_set: core set point temperature (each body part) [°C]
+    t_superficial_vein: superficial vein temperature (each body part) [°C]
+    t_vein  : vein temperature (each body part) [°C]
+    tdb     : dry bulb air temperature (each body part) [°C]
+    to      : operative temperature (each body part) [°C]
+    tr      : mean radiant temperature (each body part) [°C]
+    v       : air velocity (each body part) [m/s]
+    weight  : body weight [kg]
 
 
     Examples
     --------
-    # Build a model and set a body built
-    # Create an instance of the JOS3 class with optional body parameters such as body height, weight, age, sex, etc.
+    Build a model and set a body built
+    Create an instance of the JOS3 class with optional body parameters such as body height, weight, age, sex, etc.
 
     .. code-block:: python
 
         >>> import numpy as np
         >>> import pandas as pd
         >>> import matplotlib.pyplot as plt
         >>> import os
@@ -3755,26 +3668,27 @@
         self._cycle = 0  # Cycle time
 
         # Reset set-point temperature and save the last model parameters
         dictout = self._reset_setpt()
         self._history.append(dictout)
 
     def _calculate_operative_temp_when_pmv_is_zero(self, va=0.1, rh=50, met=1, clo=0):
-        """
-        Calculate operative temperature [°C] when PMV=0.
+        """Calculate operative temperature [°C] when PMV=0.
+
         Parameters
         ----------
         va : float, optional
             Air velocity [m/s]. The default is 0.1.
         rh : float, optional
             Relative humidity [%]. The default is 50.
         met : float, optional
             Metabolic rate [met]. The default is 1.
         clo : float, optional
             Clothing insulation [clo]. The default is 0.
+
         Returns
         -------
         to : float
             Operative temperature [°C].
         """
 
         to = 28  # initial operative temperature
```

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/optimized_functions.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/optimized_functions.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/psychrometrics.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/psychrometrics.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort/utilities.py` & `pythermalcomfort-2.7.2/src/pythermalcomfort/utilities.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/PKG-INFO` & `pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pythermalcomfort
-Version: 2.7.1
+Version: 2.7.2
 Summary: Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578
 Home-page: https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort
 Author: Federico Tartarini
 Author-email: cbecomforttool@gmail.com
 License: MIT
 Project-URL: Documentation, https://pythermalcomfort.readthedocs.io/
 Project-URL: Changelog, https://pythermalcomfort.readthedocs.io/en/latest/changelog.html
```

### Comparing `pythermalcomfort-2.7.1/src/pythermalcomfort.egg-info/SOURCES.txt` & `pythermalcomfort-2.7.2/src/pythermalcomfort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/tests/test_jos3.py` & `pythermalcomfort-2.7.2/tests/test_jos3.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/tests/test_models.py` & `pythermalcomfort-2.7.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.7.1/tox.ini` & `pythermalcomfort-2.7.2/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/invocations-3.1.0.tar.gz` & `tmp/invocations-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpaphn4xr8/dist/invocations-3.1.0.tar", last modified: Tue May  2 21:15:20 2023, max compression
+gzip compressed data, was "/tmp/tmpgwujf__9/dist/invocations-3.2.0.tar", last modified: Thu May 11 20:06:37 2023, max compression
```

## Comparing `invocations-3.1.0.tar` & `invocations-3.2.0.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/
--rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.1.0/README.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-02 21:15:20.000000 invocations-3.1.0/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)      295 2023-04-28 19:13:24.000000 invocations-3.1.0/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)     3303 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations.egg-info/dependency_links.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations/
--rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.1.0/invocations/docs.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/autodoc.py
--rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.1.0/invocations/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.1.0/invocations/testing.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.1.0/invocations/__init__.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/invocations/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.1.0/invocations/packaging/semantic_version_monkey.py
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.1.0/invocations/packaging/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/packaging/vendorize.py
--rw-r--r--   0 jforcier  (1000) users      (100)    34493 2023-05-02 21:11:34.000000 invocations-3.1.0/invocations/packaging/release.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/ci.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.1.0/invocations/watch.py
--rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.1.0/invocations/environment.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-02 20:50:00.000000 invocations-3.1.0/invocations/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.1.0/invocations/pytest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1982 2022-12-31 22:11:11.000000 invocations-3.1.0/invocations/checks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.1.0/invocations/console.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     3243 2022-10-29 02:26:37.000000 invocations-3.1.0/tests/checks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/api.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_sources/
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/objects.inv
--rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/py-modindex.html
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/pygments.css
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/minus.png
--rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/alabaster.css
--rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/basic.css
--rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
--rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/file.png
--rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore.js
--rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/documentation_options.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/language_data.js
--rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/custom.css
--rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/searchtools.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/doctools.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
--rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/plus.png
--rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
--rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery.js
--rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/search.html
--rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/genindex.html
--rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/api.html
--rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/index.html
--rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/searchindex.js
--rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.buildinfo
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/
--rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/autodoc/_support/mytasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/autodoc/_support/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/autodoc/base.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/packaging/
--rw-r--r--   0 jforcier  (1000) users      (100)    73728 2023-05-02 21:11:42.000000 invocations-3.1.0/tests/packaging/.release.py.swp
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/packaging/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/no_unreleased_1.1_bugs.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/otherversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/fakepackage/noversion.py
--rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/no_unreleased_1.x_features.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/packaging/_support/unreleased_1.1_bugs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    50230 2023-05-02 21:11:45.000000 invocations-3.1.0/tests/packaging/release.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/console.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/environment.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.1.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.1.0/tests/pytest_.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-02 21:15:20.000000 invocations-3.1.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.1.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.1.0/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/docs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 21:15:20.000000 invocations-3.1.0/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.1.0/docs/api/ci.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/pytest.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/environment.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/packaging.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/autodoc.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/docs.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/api/console.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.1.0/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.1.0/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12475 2023-05-02 21:15:20.000000 invocations-3.1.0/docs/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.1.0/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2091 2022-12-31 22:11:11.000000 invocations-3.2.0/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      189 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    13035 2023-05-11 20:06:36.000000 invocations-3.2.0/docs/changelog.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/autodoc.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/console.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      233 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/packaging.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       53 2022-03-18 00:56:41.000000 invocations-3.2.0/docs/api/ci.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       61 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/docs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/environment.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       69 2021-12-23 21:30:39.000000 invocations-3.2.0/docs/api/pytest.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2737 2023-04-28 15:16:14.000000 invocations-3.2.0/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-11 20:06:37.000000 invocations-3.2.0/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     2335 2021-12-23 21:30:39.000000 invocations-3.2.0/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-11 20:06:37.000000 invocations-3.2.0/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2491 2023-05-11 19:03:55.000000 invocations-3.2.0/invocations/checks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5009 2022-12-17 18:26:26.000000 invocations-3.2.0/invocations/pytest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1264 2021-12-23 21:30:39.000000 invocations-3.2.0/invocations/watch.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3866 2022-12-31 22:11:11.000000 invocations-3.2.0/invocations/ci.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      636 2022-06-17 16:03:46.000000 invocations-3.2.0/invocations/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6534 2023-04-12 22:47:06.000000 invocations-3.2.0/invocations/docs.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations/packaging/
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2021-12-23 21:30:39.000000 invocations-3.2.0/invocations/packaging/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1069 2023-01-16 22:33:01.000000 invocations-3.2.0/invocations/packaging/semantic_version_monkey.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4399 2022-12-31 22:11:11.000000 invocations-3.2.0/invocations/packaging/vendorize.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    34493 2023-05-02 21:11:34.000000 invocations-3.2.0/invocations/packaging/release.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1942 2023-01-16 22:33:01.000000 invocations-3.2.0/invocations/console.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3194 2022-12-31 22:11:11.000000 invocations-3.2.0/invocations/autodoc.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-11 19:04:03.000000 invocations-3.2.0/invocations/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      621 2022-09-08 19:21:52.000000 invocations-3.2.0/invocations/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.2.0/invocations/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5910 2023-01-16 22:33:01.000000 invocations-3.2.0/invocations/testing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-03-17 18:07:11.000000 invocations-3.2.0/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)       12 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3271 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     4123 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      124 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-11 20:06:37.000000 invocations-3.2.0/invocations.egg-info/dependency_links.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/packaging/
+-rw-r--r--   0 jforcier  (1000) users      (100)    50230 2023-05-02 21:11:45.000000 invocations-3.2.0/tests/packaging/release.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/packaging/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      185 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      261 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/no_unreleased_1.1_bugs.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      179 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/no_unreleased_1.x_features.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/unreleased_1.1_bugs.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/
+-rw-r--r--   0 jforcier  (1000) users      (100)       13 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/noversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       22 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/otherversion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/fakepackage/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       50 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/packaging/_support/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1890 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/console.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3873 2023-05-11 20:04:44.000000 invocations-3.2.0/tests/checks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/mytasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      259 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/autodoc/_support/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/api.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)     4418 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      286 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/file.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     4758 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/language_data.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    18215 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/searchtools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    89501 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    11230 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/alabaster.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    68420 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
+-rw-r--r--   0 jforcier  (1000) users      (100)    19530 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     4712 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0 jforcier  (1000) users      (100)   288580 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js
+-rw-r--r--   0 jforcier  (1000) users      (100)      415 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/documentation_options.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     5327 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/pygments.css
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/plus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)       90 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/minus.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     4472 2022-12-22 02:25:27.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/doctools.js
+-rw-r--r--   0 jforcier  (1000) users      (100)       42 2022-09-08 21:39:12.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/custom.css
+-rw-r--r--   0 jforcier  (1000) users      (100)    14621 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/basic.css
+-rw-r--r--   0 jforcier  (1000) users      (100)     3958 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/genindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     5187 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/api.html
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/
+-rw-r--r--   0 jforcier  (1000) users      (100)     7645 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)     2657 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0 jforcier  (1000) users      (100)    14029 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-11 20:06:37.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_sources/
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_sources/api.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     1375 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/searchindex.js
+-rw-r--r--   0 jforcier  (1000) users      (100)     2861 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/search.html
+-rw-r--r--   0 jforcier  (1000) users      (100)      230 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/.buildinfo
+-rw-r--r--   0 jforcier  (1000) users      (100)     3553 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/index.html
+-rw-r--r--   0 jforcier  (1000) users      (100)      296 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/objects.inv
+-rw-r--r--   0 jforcier  (1000) users      (100)     3108 2022-12-22 02:27:13.000000 invocations-3.2.0/tests/autodoc/_support/docs/_build/py-modindex.html
+-rw-r--r--   0 jforcier  (1000) users      (100)     2752 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/autodoc/base.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1116 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/environment.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1066 2021-12-23 21:30:39.000000 invocations-3.2.0/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2542 2022-12-31 22:11:11.000000 invocations-3.2.0/tests/pytest_.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      295 2023-04-28 19:13:24.000000 invocations-3.2.0/dev-requirements.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      243 2022-03-18 00:56:41.000000 invocations-3.2.0/MANIFEST.in
```

### Comparing `invocations-3.1.0/README.rst` & `invocations-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations.egg-info/SOURCES.txt` & `invocations-3.2.0/invocations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 tests/autodoc/_support/docs/_build/_static/minus.png
 tests/autodoc/_support/docs/_build/_static/plus.png
 tests/autodoc/_support/docs/_build/_static/pygments.css
 tests/autodoc/_support/docs/_build/_static/searchtools.js
 tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js
 tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js
 tests/autodoc/_support/docs/_build/_static/underscore.js
-tests/packaging/.release.py.swp
 tests/packaging/release.py
 tests/packaging/_support/conf.py
 tests/packaging/_support/index.rst
 tests/packaging/_support/no_unreleased_1.1_bugs.rst
 tests/packaging/_support/no_unreleased_1.x_features.rst
 tests/packaging/_support/unreleased_1.1_bugs.rst
 tests/packaging/_support/unreleased_1.x_features.rst
```

### Comparing `invocations-3.1.0/invocations.egg-info/PKG-INFO` & `invocations-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.1.0
+Version: 3.2.0
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
```

### Comparing `invocations-3.1.0/invocations/docs.py` & `invocations-3.2.0/invocations/docs.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/autodoc.py` & `invocations-3.2.0/invocations/autodoc.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/util.py` & `invocations-3.2.0/invocations/util.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/testing.py` & `invocations-3.2.0/invocations/testing.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/packaging/semantic_version_monkey.py` & `invocations-3.2.0/invocations/packaging/semantic_version_monkey.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/packaging/vendorize.py` & `invocations-3.2.0/invocations/packaging/vendorize.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/packaging/release.py` & `invocations-3.2.0/invocations/packaging/release.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/ci.py` & `invocations-3.2.0/invocations/ci.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/watch.py` & `invocations-3.2.0/invocations/watch.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/environment.py` & `invocations-3.2.0/invocations/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/pytest.py` & `invocations-3.2.0/invocations/pytest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/invocations/checks.py` & `invocations-3.2.0/invocations/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. versionadded:: 1.2
 """
 
 from invoke import task
 
 
-@task(name="blacken", iterable=["folders"])
+@task(name="blacken", aliases=["format"], iterable=["folders"])
 def blacken(
     c, line_length=79, folders=None, check=False, diff=False, find_opts=None
 ):
     r"""
     Run black on the current source tree (all ``.py`` files).
 
     :param int line_length:
@@ -29,14 +29,16 @@
         command. For example, skip a vendor directory with ``"-and -not -path
         ./vendor\*"``, add ``-mtime N``, or etc. Honors the
         ``blacken.find_opts`` config option.
 
     .. versionadded:: 1.2
     .. versionchanged:: 1.4
         Added the ``find_opts`` argument.
+    .. versionchanged:: 3.2
+        Added the ``format`` alias.
     """
     config = c.config.get("blacken", {})
     default_folders = ["."]
     configured_folders = config.get("folders", default_folders)
     folders = folders or configured_folders
 
     default_find_opts = ""
@@ -53,7 +55,31 @@
     else:
         find_opts = ""
 
     cmd = "find {} -name '*.py'{} | xargs {}".format(
         " ".join(folders), find_opts, black_command_line
     )
     c.run(cmd, pty=True)
+
+
+@task
+def lint(c):
+    """
+    Apply linting.
+
+    .. versionadded:: 3.2
+    """
+    # TODO: configurable and/or switch to ruff
+    c.run("flake8", warn=True, pty=True)
+
+
+@task(default=True)
+def all_(c):
+    """
+    Run all common formatters/linters for the project.
+
+    .. versionadded:: 3.2
+    """
+    # TODO: contextmanager config, if we don't already have that
+    c.config.run.echo = True
+    blacken(c)
+    lint(c)
```

### Comparing `invocations-3.1.0/invocations/console.py` & `invocations-3.2.0/invocations/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/checks.py` & `invocations-3.2.0/tests/checks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from unittest.mock import call
+
 import pytest
 
-from invocations.checks import blacken
+from invocations.checks import blacken, lint, all_ as all_task
 
 
 class checks:
     class blacken_:
         @pytest.mark.parametrize(
             "kwargs,command",
             [
@@ -80,7 +82,26 @@
                 "find . -name '*.py' -and -not -name foo.py" in ctx.run_command
             )
 
         def find_opts_config_loses_to_runtime(self, ctx):
             ctx.blacken = dict(find_opts="-and -not -name foo.py")
             blacken(ctx, find_opts="-or -name '*.js'")
             assert "find . -name '*.py' -or -name '*.js'" in ctx.run_command
+
+        def aliased_to_format(self):
+            assert blacken.aliases == ["format"]
+
+    class lint_:
+        def runs_flake8_by_default(self, ctx):
+            lint(ctx)
+            assert ctx.run_command == "flake8"
+
+    class all_:
+        def runs_blacken_and_lint(self, ctx):
+            all_task(ctx)
+            assert ctx.run.call_args_list == [
+                call("find . -name '*.py' | xargs black -l 79", pty=True),
+                call("flake8", pty=True, warn=True),
+            ]
+
+        def is_default_task(self):
+            assert all_task.is_default
```

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/py-modindex.html` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/pygments.css` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/alabaster.css` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/basic.css` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/underscore.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/language_data.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/searchtools.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/doctools.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/jquery.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/search.html` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/genindex.html` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/api.html` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/api.html`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/index.html` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/searchindex.js` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree` & `invocations-3.2.0/tests/autodoc/_support/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/autodoc/base.py` & `invocations-3.2.0/tests/autodoc/base.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/packaging/release.py` & `invocations-3.2.0/tests/packaging/release.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/console.py` & `invocations-3.2.0/tests/console.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/environment.py` & `invocations-3.2.0/tests/environment.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/conftest.py` & `invocations-3.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/tests/pytest_.py` & `invocations-3.2.0/tests/pytest_.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/PKG-INFO` & `invocations-3.2.0/invocations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invocations
-Version: 3.1.0
+Version: 3.2.0
 Summary: Common/best-practice Invoke tasks and collections
 Home-page: https://invocations.readthedocs.io
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/pyinvoke/invocations
 Project-URL: Changelog, https://invocations.readthedocs.io/en/latest/changelog.html
```

### Comparing `invocations-3.1.0/setup.py` & `invocations-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/LICENSE` & `invocations-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/docs/conf.py` & `invocations-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invocations-3.1.0/docs/changelog.rst` & `invocations-3.2.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 =========
 Changelog
 =========
 
+- :release:`3.2.0 <2023-05-11>`
+- :feature:`-` Minor enhancements to the ``checks`` module:
+
+    - ``blacken`` now has a ``format`` alias (and will likely reverse the real
+      name and the alias in 4.0)
+    - Added ``lint`` task which currently just runs ``flake8``, will likely
+      learn how to be configurable later.
+    - Added ``all_`` default task for the collection, which runs both
+      ``blacken`` (in regular, not diff-only mode - idea is to be useful for
+      devs, not CI, which already does both independently) and ``lint`` in
+      series.
+
 - :release:`3.1.0 <2023-05-02>`
 - :feature:`-` Updated ``packaging.release.test_install`` to attempt imports of
   freshly test-installed packages, to catch import-time errors on top of
   install-time ones. This can be opted out of by giving the ``skip_import``
   kwarg (aka the ``--skip-import`` flag on the CLI).
 - :release:`3.0.2 <2023-04-28>`
 - :support:`- backported` Unpin ``tabulate`` in our install requirements, it's
```


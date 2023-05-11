# Comparing `tmp/dir-content-diff-1.4.0.tar.gz` & `tmp/dir-content-diff-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir-content-diff-1.4.0.tar", last modified: Mon Mar 13 11:40:05 2023, max compression
+gzip compressed data, was "dir-content-diff-1.5.0.tar", last modified: Thu May 11 09:17:20 2023, max compression
```

## Comparing `dir-content-diff-1.4.0.tar` & `dir-content-diff-1.5.0.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.805867 dir-content-diff-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.805867 dir-content-diff-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.gitreview
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/dir_content_diff/
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/dir_content_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/dir_content_diff/base_comparators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/dir_content_diff/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/dir_content_diff/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/dir_content_diff/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/dir_content_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-03-13 11:40:05.000000 dir-content-diff-1.4.0/dir_content_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-13 11:40:05.000000 dir-content-diff-1.4.0/dir_content_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 11:40:05.000000 dir-content-diff-1.4.0/dir_content_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 11:40:05.000000 dir-content-diff-1.4.0/dir_content_diff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-13 11:40:05.000000 dir-content-diff-1.4.0/dir_content_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-13 11:40:05.000000 dir-content-diff-1.4.0/dir_content_diff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:40:05.809867 dir-content-diff-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/generate_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    34499 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-13 11:39:55.000000 dir-content-diff-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.271380 dir-content-diff-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.263380 dir-content-diff-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.263380 dir-content-diff-1.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/dir_content_diff/
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/dir_content_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/dir_content_diff/base_comparators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/dir_content_diff/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/dir_content_diff/pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/dir_content_diff/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/dir_content_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-11 09:17:20.000000 dir-content-diff-1.5.0/dir_content_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-11 09:17:20.000000 dir-content-diff-1.5.0/dir_content_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:17:20.000000 dir-content-diff-1.5.0/dir_content_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 09:17:20.000000 dir-content-diff-1.5.0/dir_content_diff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 09:17:20.000000 dir-content-diff-1.5.0/dir_content_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 09:17:20.000000 dir-content-diff-1.5.0/dir_content_diff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:17:20.271380 dir-content-diff-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:17:20.267380 dir-content-diff-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/generate_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-11 09:17:10.000000 dir-content-diff-1.5.0/tox.ini
```

### Comparing `dir-content-diff-1.4.0/.auto-changelog` & `dir-content-diff-1.5.0/.auto-changelog`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.auto-changelog-template.hbs` & `dir-content-diff-1.5.0/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.copier-answers.yml` & `dir-content-diff-1.5.0/.copier-answers.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changes here will be overwritten by Copier
 
-_commit: 0.1.40
+_commit: 0.1.43
 _src_path: git@bbpgitlab.epfl.ch:neuromath/python-template.git
 author_email: ''
 author_name: Blue Brain Project, EPFL
 copyright_license: Apache License 2.0
 copyright_year: '2022'
 distribution_name: dir-content-diff
 download_url: https://github.com/BlueBrain/dir-content-diff
```

### Comparing `dir-content-diff-1.4.0/.github/dependabot.yml` & `dir-content-diff-1.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.github/workflows/codeql.yml` & `dir-content-diff-1.5.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.github/workflows/commitlint.yml` & `dir-content-diff-1.5.0/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.github/workflows/publish-sdist.yml` & `dir-content-diff-1.5.0/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.github/workflows/run-tox.yml` & `dir-content-diff-1.5.0/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/.pre-commit-config.yaml` & `dir-content-diff-1.5.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,30 @@
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
-    rev: v9.4.0
+    rev: v9.5.0
     hooks:
         - id: commitlint
           stages:
             - commit-msg
           additional_dependencies: ['conventional-changelog-conventionalcommits']
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         args: ["-x", ".codespellignorelines"]
   - repo: https://github.com/PyCQA/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
```

### Comparing `dir-content-diff-1.4.0/.pylintrc` & `dir-content-diff-1.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/CHANGELOG.md` & `dir-content-diff-1.5.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Changelog
 
+## [1.5.0](https://github.com/BlueBrain/dir-content-diff/compare/1.4.0..1.5.0)
+
+> 11 May 2023
+
+### New Features
+
+- Add exception type before arguments (Adrien Berchet - [#36](https://github.com/BlueBrain/dir-content-diff/pull/36))
+
+### Fixes
+
+- Cast exception args to str before joining them (Adrien Berchet - [#35](https://github.com/BlueBrain/dir-content-diff/pull/35))
+
+### Changes to Test Assests
+
+- Fix for Pandas&gt;=2 (Adrien Berchet - [#33](https://github.com/BlueBrain/dir-content-diff/pull/33))
+
+### CI Improvements
+
+- Add template for issues and pull requests (Adrien Berchet - [#34](https://github.com/BlueBrain/dir-content-diff/pull/34))
+
 ## [1.4.0](https://github.com/BlueBrain/dir-content-diff/compare/1.3.0..1.4.0)
 
 > 13 March 2023
 
 ### Build
 
 - Bump dicttoxml (Adrien Berchet - [#26](https://github.com/BlueBrain/dir-content-diff/pull/26))
```

### Comparing `dir-content-diff-1.4.0/CONTRIBUTING.md` & `dir-content-diff-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/LICENSE.txt` & `dir-content-diff-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/PKG-INFO` & `dir-content-diff-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-content-diff
-Version: 1.4.0
+Version: 1.5.0
 Summary: Simple tool to compare directory contents.
 Home-page: https://dir-content-diff.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/dir-content-diff/issues
 Project-URL: Source, https://github.com/BlueBrain/dir-content-diff
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dir-content-diff-1.4.0/README.md` & `dir-content-diff-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/commitlint.config.js` & `dir-content-diff-1.5.0/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/dir_content_diff/__init__.py` & `dir-content-diff-1.5.0/dir_content_diff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,23 @@
         load_kwargs = kwargs.pop("load_kwargs", None)
         format_data_kwargs = kwargs.pop("format_data_kwargs", None)
         filter_kwargs = kwargs.pop("filter_kwargs", None)
         format_diff_kwargs = kwargs.pop("format_diff_kwargs", None)
         sort_kwargs = kwargs.pop("sort_kwargs", None)
         concat_kwargs = kwargs.pop("concat_kwargs", None)
         report_kwargs = kwargs.pop("report_kwargs", None)
+        try:
+            exception_args = "\n".join(str(i) for i in exception.args)
+        except Exception:  # pylint: disable=broad-exception-caught
+            exception_args = "UNKNOWN ERROR: Could not get information from the exception"
+        exc_type = type(exception).__name__
         return diff_msg_formatter(
             ref_file,
             comp_file,
-            reason="Exception raised: " + "\n".join(exception.args),
+            reason=f"Exception raised: ({exc_type}) {exception_args}",
             diff_args=args,
             diff_kwargs=kwargs,
             load_kwargs=load_kwargs,
             format_data_kwargs=format_data_kwargs,
             filter_kwargs=filter_kwargs,
             format_diff_kwargs=format_diff_kwargs,
             sort_kwargs=sort_kwargs,
```

### Comparing `dir-content-diff-1.4.0/dir_content_diff/base_comparators.py` & `dir-content-diff-1.5.0/dir_content_diff/base_comparators.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/dir_content_diff/pandas.py` & `dir-content-diff-1.5.0/dir_content_diff/pandas.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/dir_content_diff/pytest_plugin.py` & `dir-content-diff-1.5.0/dir_content_diff/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/dir_content_diff/util.py` & `dir-content-diff-1.5.0/dir_content_diff/util.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/dir_content_diff.egg-info/PKG-INFO` & `dir-content-diff-1.5.0/dir_content_diff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir-content-diff
-Version: 1.4.0
+Version: 1.5.0
 Summary: Simple tool to compare directory contents.
 Home-page: https://dir-content-diff.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/dir-content-diff/issues
 Project-URL: Source, https://github.com/BlueBrain/dir-content-diff
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dir-content-diff-1.4.0/dir_content_diff.egg-info/SOURCES.txt` & `dir-content-diff-1.5.0/dir_content_diff.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 codecov.yml
 commitlint.config.js
 package.json
 pyproject.toml
 setup.py
 tox.ini
 .github/dependabot.yml
+.github/pull_request_template.md
+.github/ISSUE_TEMPLATE/bug_report.yaml
+.github/ISSUE_TEMPLATE/config.yml
+.github/ISSUE_TEMPLATE/feature_request.yaml
+.github/ISSUE_TEMPLATE/how_to_use.yaml
 .github/workflows/codeql.yml
 .github/workflows/commitlint.yml
 .github/workflows/publish-sdist.yml
 .github/workflows/run-tox.yml
 dir_content_diff/__init__.py
 dir_content_diff/base_comparators.py
 dir_content_diff/pandas.py
```

### Comparing `dir-content-diff-1.4.0/docs/Makefile` & `dir-content-diff-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/docs/source/conf.py` & `dir-content-diff-1.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/package.json` & `dir-content-diff-1.5.0/package.json`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/pyproject.toml` & `dir-content-diff-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/setup.py` & `dir-content-diff-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "dictdiffer>=0.8",
     "diff_pdf_visually>=1.7",
     "PyYaml>=5.3",
 ]
 
 doc_reqs = [
     "m2r2",
-    "sphinx<6",
+    "sphinx",
     "sphinx-bluebrain-theme",
 ]
 
 pandas_reqs = [
     "pandas>=1.4",
     "tables>=3.7",
 ]
```

### Comparing `dir-content-diff-1.4.0/tests/conftest.py` & `dir-content-diff-1.5.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,12 +186,14 @@
     """The diff that should be reported for the CSV files."""
     return (
         r"""The files '\S*/file.csv' and '\S*/file.csv' are different:\n\n"""
         r"""Column 'col_a': Series are different\n\n"""
         r"""Series values are different \(33.33333 %\)\n"""
         r"""\[index\]: \[0, 1, 2\]\n"""
         r"""\[left\]:  \[1, 2, 3\]\n"""
-        r"""\[right\]: \[10, 2, 3\]\n\n"""
+        r"""\[right\]: \[10, 2, 3\]\n"""
+        r"""(At positional index 0, first diff: 1 != 10\n)?\n"""
         r"""Column 'col_b': Series are different\n\n"""
         r"""Series values are different \(33.33333 %\)\n"""
         r"""\[index\]: \[0, 1, 2\]\n\[left\]:  \[a, b, c\]\n\[right\]: \[a, b_new, c\]"""
+        r"""(\nAt positional index 1, first diff: b != b_new)?"""
     )
```

### Comparing `dir-content-diff-1.4.0/tests/generate_test_files.py` & `dir-content-diff-1.5.0/tests/generate_test_files.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/tests/test_base.py` & `dir-content-diff-1.5.0/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -768,16 +768,55 @@
         dir_content_diff.unregister_comparator(".yaml")
         dir_content_diff.register_comparator(".yaml", bad_comparator)
 
         res = compare_trees(ref_tree, res_tree_equal)
 
         assert len(res) == 1
         match = re.match(
-            r"The files '\S*/ref/file.yaml' and '\S*/res/file.yaml' are different:\n"
-            r"Exception raised: Bad\ncomparator",
+            r"The files '\S*/ref/file\.yaml' and '\S*/res/file\.yaml' are different:\n"
+            r"Exception raised: \(RuntimeError\) Bad\ncomparator",
+            res["file.yaml"],
+        )
+        assert match is not None
+
+        def bad_comparator_no_str(ref_path, test_path, *args, **kwargs):
+            raise RuntimeError((1, ("Bad\ncomparator", 2)))
+
+        dir_content_diff.unregister_comparator(".yaml")
+        dir_content_diff.register_comparator(".yaml", bad_comparator_no_str)
+
+        res = compare_trees(ref_tree, res_tree_equal)
+
+        assert len(res) == 1
+        match = re.match(
+            r"The files '\S*/ref/file\.yaml' and '\S*/res/file\.yaml' are different:\n"
+            r"Exception raised: \(RuntimeError\) \(1, \('Bad\\ncomparator', 2\)\)",
+            res["file.yaml"],
+        )
+        assert match is not None
+
+        class NoRepr:
+            """A class to test exception handling failure."""
+
+            def __repr__(self):
+                raise ValueError("This object can not be represented")
+
+        def bad_comparator_exception_failing(ref_path, test_path, *args, **kwargs):
+            raise RuntimeError((NoRepr(), ("Bad\ncomparator", NoRepr())))
+
+        dir_content_diff.unregister_comparator(".yaml")
+        dir_content_diff.register_comparator(".yaml", bad_comparator_exception_failing)
+
+        res = compare_trees(ref_tree, res_tree_equal)
+
+        assert len(res) == 1
+        match = re.match(
+            r"The files '\S*/ref/file\.yaml' and '\S*/res/file\.yaml' are different:\n"
+            r"Exception raised: \(RuntimeError\) UNKNOWN ERROR: Could not get information from "
+            r"the exception",
             res["file.yaml"],
         )
         assert match is not None
 
     def test_specific_args(self, ref_tree, res_tree_diff, dict_diff, xml_diff, ini_diff):
         """Test specific args."""
         specific_args = {
@@ -803,25 +842,25 @@
             assert match_i is not None
 
     def test_unknown_comparator(self, ref_tree, res_tree_diff, registry_reseter):
         """Test with an unknown extension."""
         dir_content_diff.unregister_comparator(".yaml")
         res = compare_trees(ref_tree, res_tree_diff)
         match = re.match(
-            r"The files '\S*/ref/file.yaml' and '\S*/res/file.yaml' are different.",
+            r"The files '\S*/ref/file\.yaml' and '\S*/res/file\.yaml' are different.",
             res["file.yaml"],
         )
         assert match is not None
 
     def test_nested_files(self, ref_with_nested_file, res_diff_with_nested_file):
         """Test with nested files."""
         res = compare_trees(ref_with_nested_file, res_diff_with_nested_file)
         match = re.match(
-            r"The files '\S*/ref/level1/level2/level3/file.pdf' and "
-            r"'\S*/res/level1/level2/level3/file.pdf' are different\.",
+            r"The files '\S*/ref/level1/level2/level3/file\.pdf' and "
+            r"'\S*/res/level1/level2/level3/file\.pdf' are different\.",
             res["level1/level2/level3/file.pdf"],
         )
         assert match is not None
 
     def test_fix_dot_notation(
         self, ref_tree, res_tree_diff, pdf_diff, dict_diff, xml_diff, ini_diff
     ):
```

### Comparing `dir-content-diff-1.4.0/tests/test_pandas.py` & `dir-content-diff-1.5.0/tests/test_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             }
         }
         res = compare_trees(ref_tree, res_tree_equal, specific_args=specific_args)
 
         assert len(res) == 1
         res_csv = res["file.csv"]
         match_res = re.match(
-            r"The files '\S*/ref/file.csv' and '\S*/res/file.csv' are different:\n"
+            r"The files '\S*/ref/file\.csv' and '\S*/res/file\.csv' are different:\n"
             r"Kwargs used for formatting data: {'replace_pattern': {.*}}\n\n"
             r"Column 'test_path_only_in_ref': The column is missing in the compared DataFrame, "
             r"please fix the 'replace_pattern' argument.\n\n"
             r"Column 'test_path_only_in_res': The column is missing in the reference DataFrame, "
             r"please fix the 'replace_pattern' argument.",
             res_csv,
         )
@@ -187,20 +187,20 @@
             }
         }
         res = compare_trees(ref_tree, res_tree_equal, specific_args=specific_args)
 
         assert len(res) == 1
         res_csv = res["file.csv"]
         match_res = re.match(
-            r"The files '\S*/ref/file.csv' and '\S*/res/file.csv' are different:\n"
+            r"The files '\S*/ref/file\.csv' and '\S*/res/file\.csv' are different:\n"
             r"Kwargs used for formatting data: {'replace_pattern': {.*}}\n\n"
             r"Column 'test_path_only_in_ref': The column is missing in the compared DataFrame, "
-            r"please fix the 'replace_pattern' argument.\n\n"
+            r"please fix the 'replace_pattern' argument\.\n\n"
             r"Column 'test_path_only_in_res': The column is missing in the reference DataFrame, "
-            r"please fix the 'replace_pattern' argument.",
+            r"please fix the 'replace_pattern' argument\.",
             res_csv,
         )
         assert match_res is not None
 
         # Test with only nan values in column
         for df_path in [ref_csv, res_csv_equal]:
             df = pd.read_csv(df_path, index_col="index")
@@ -208,20 +208,20 @@
             df.to_csv(df_path, index=True, index_label="index")
 
         res = compare_trees(ref_tree, res_tree_equal, specific_args=specific_args)
 
         assert len(res) == 1
         res_csv = res["file.csv"]
         match_res = re.match(
-            r"The files '\S*/ref/file.csv' and '\S*/res/file.csv' are different:\n"
+            r"The files '\S*/ref/file\.csv' and '\S*/res/file\.csv' are different:\n"
             r"Kwargs used for formatting data: {'replace_pattern': {.*}}\n\n"
             r"Column 'test_path_only_in_ref': The column is missing in the compared DataFrame, "
-            r"please fix the 'replace_pattern' argument.\n\n"
+            r"please fix the 'replace_pattern' argument\.\n\n"
             r"Column 'test_path_only_in_res': The column is missing in the reference DataFrame, "
-            r"please fix the 'replace_pattern' argument.",
+            r"please fix the 'replace_pattern' argument\.",
             res_csv,
         )
         assert match_res is not None
 
     def test_hdf5_comparator(
         self, empty_ref_tree, empty_res_tree, res_hdf5_equal, pandas_registry_reseter
     ):
@@ -248,27 +248,23 @@
         match_res = re.match(csv_diff, res_csv)
         assert match_res is not None
 
     def test_read_csv_kwargs(
         self, ref_tree, ref_csv, res_tree_diff, res_csv_diff, csv_diff, pandas_registry_reseter
     ):
         """Test specific args for the CSV reader."""
-        specific_args = {
-            "file.csv": {"load_kwargs": {"header": None, "skiprows": 1, "prefix": "col_"}}
-        }
+        specific_args = {"file.csv": {"load_kwargs": {"header": None, "skiprows": 1}}}
         res = compare_trees(ref_tree, res_tree_diff, specific_args=specific_args)
 
         assert len(res) == 6
         res_csv = res["file.csv"]
-        kwargs_msg = (
-            "Kwargs used for loading data: {'header': None, 'skiprows': 1, 'prefix': 'col_'}\n"
-        )
+        kwargs_msg = "Kwargs used for loading data: {'header': None, 'skiprows': 1}\n"
         assert kwargs_msg in res_csv
         match_res = re.match(
-            csv_diff.replace("col_a", "col_1").replace("col_b", "col_2"),
+            csv_diff.replace("col_a", "1").replace("col_b", "2"),
             res_csv.replace(kwargs_msg, ""),
         )
         assert match_res is not None
 
     def test_missing_column(
         self, ref_tree, ref_csv, res_tree_diff, res_csv_equal, csv_diff, pandas_registry_reseter
     ):
@@ -280,15 +276,15 @@
 
         # Check that the missing column is found
         res = compare_trees(ref_tree, res_tree_diff)
 
         assert len(res) == 1
         res_csv = res["file.csv"]
         match_res = re.match(
-            r"The files '\S*/ref/file.csv' and '\S*/res/file.csv' are different:\n\n"
+            r"The files '\S*/ref/file\.csv' and '\S*/res/file\.csv' are different:\n\n"
             r"Column 'col_c': The column is missing in the compared DataFrame.\n\n"
             r"Column 'new_col_c': The column is missing in the reference DataFrame.",
             res_csv,
         )
         assert match_res is not None
 
     def test_hdf5_comparator(
@@ -296,19 +292,21 @@
     ):
         """Test the comparator for HDF5 files."""
         res = compare_trees(empty_ref_tree, empty_res_tree)
 
         assert len(res) == 1
         res_hdf = res["file.h5"]
         match_res = re.match(
-            r"The files '\S*/ref/file.h5' and '\S*/res/file.h5' are different:\n\n"
+            r"The files '\S*/ref/file\.h5' and '\S*/res/file\.h5' are different:\n\n"
             r"Column 'col_a': Series are different\n\n"
             r"Series values are different \(33\.33333 %\)\n"
             r"\[index\]: \[idx1, idx2, idx3\]\n"
-            r"\[left\]:  \[1, 2, 3\]\n\[right\]: \[10, 2, 3\]\n\n"
+            r"\[left\]:  \[1, 2, 3\]\n\[right\]: \[10, 2, 3\]\n"
+            r"""(At positional index 0, first diff: 1 != 10\n)?\n"""
             r"Column 'col_b': Series are different\n\n"
             r"Series values are different \(33\.33333 %\)\n"
             r"\[index\]: \[idx1, idx2, idx3\]\n"
-            r"\[left\]:  \[a, b, c\]\n\[right\]: \[a, b_new, c\]",
+            r"\[left\]:  \[a, b, c\]\n\[right\]: \[a, b_new, c\]"
+            r"""(\nAt positional index 1, first diff: b != b_new)?""",
             res_hdf,
         )
         assert match_res is not None
```

### Comparing `dir-content-diff-1.4.0/tests/test_pytest_plugin.py` & `dir-content-diff-1.5.0/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `dir-content-diff-1.4.0/tox.ini` & `dir-content-diff-1.5.0/tox.ini`

 * *Files identical despite different names*


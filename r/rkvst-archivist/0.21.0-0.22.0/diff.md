# Comparing `tmp/rkvst-archivist-0.21.0.tar.gz` & `tmp/rkvst-archivist-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rkvst-archivist-0.21.0.tar", last modified: Fri Mar 31 15:17:43 2023, max compression
+gzip compressed data, was "rkvst-archivist-0.22.0.tar", last modified: Thu May 11 12:39:46 2023, max compression
```

## Comparing `rkvst-archivist-0.21.0.tar` & `rkvst-archivist-0.22.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:17:43.561931 rkvst-archivist-0.21.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-03-31 15:17:43.561931 rkvst-archivist-0.21.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:17:43.557931 rkvst-archivist-0.21.0/archivist/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-31 15:17:35.000000 rkvst-archivist-0.21.0/archivist/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/access_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/appidp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/archivist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/archivistpublic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/assetattachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/attachments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:17:43.557931 rkvst-archivist-0.21.0/archivist/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:17:43.557931 rkvst-archivist-0.21.0/archivist/cmds/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/runner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/runner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:17:43.557931 rkvst-archivist-0.21.0/archivist/cmds/template/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/template/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/cmds/template/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/compliance_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/compliance_policy_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/compliance_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/confirmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/dictmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/or_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/proof_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/retry429.py
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/sboms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/subjects_confirmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/tenancies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/archivist/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-31 15:15:24.000000 rkvst-archivist-0.21.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:17:43.557931 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-03-31 15:17:43.000000 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-31 15:17:43.000000 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 15:17:43.000000 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-31 15:17:43.000000 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-31 15:17:43.000000 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 15:17:43.000000 rkvst-archivist-0.21.0/rkvst_archivist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-31 15:17:43.561931 rkvst-archivist-0.21.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:39:46.347418 rkvst-archivist-0.22.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-05-11 12:39:46.347418 rkvst-archivist-0.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:39:46.343418 rkvst-archivist-0.22.0/archivist/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 12:39:38.000000 rkvst-archivist-0.22.0/archivist/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/appidp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/archivist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/archivistpublic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/assetattachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/attachments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:39:46.343418 rkvst-archivist-0.22.0/archivist/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:39:46.343418 rkvst-archivist-0.22.0/archivist/cmds/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/runner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/runner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:39:46.343418 rkvst-archivist-0.22.0/archivist/cmds/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/template/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/cmds/template/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/compliance_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/compliance_policy_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/compliance_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/proof_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/retry429.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/sboms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/subjects_confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/tenancies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/archivist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-11 12:37:38.000000 rkvst-archivist-0.22.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:39:46.347418 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-05-11 12:39:46.000000 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-11 12:39:46.000000 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:39:46.000000 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 12:39:46.000000 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 12:39:46.000000 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 12:39:46.000000 rkvst-archivist-0.22.0/rkvst_archivist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-11 12:39:46.347418 rkvst-archivist-0.22.0/setup.cfg
```

### Comparing `rkvst-archivist-0.21.0/LICENSE` & `rkvst-archivist-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/PKG-INFO` & `rkvst-archivist-0.22.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rkvst-archivist
-Version: 0.21.0
+Version: 0.22.0
 Summary: RKVST Client
 Home-page: https://github.com/rkvst/rkvst-python
 Author: RKVST Inc.
 Author-email: support@rkvst.com
 License: MIT
 Project-URL: Documentation, https://python.rkvst.com
 Project-URL: Source, https://github.com/rkvst/rkvst-python
```

### Comparing `rkvst-archivist-0.21.0/README.rst` & `rkvst-archivist-0.22.0/README.rst`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/access_policies.py` & `rkvst-archivist-0.22.0/archivist/access_policies.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/appidp.py` & `rkvst-archivist-0.22.0/archivist/appidp.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/applications.py` & `rkvst-archivist-0.22.0/archivist/applications.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/archivist.py` & `rkvst-archivist-0.22.0/archivist/archivist.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/archivistpublic.py` & `rkvst-archivist-0.22.0/archivist/archivistpublic.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/asset.py` & `rkvst-archivist-0.22.0/archivist/asset.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/assetattachments.py` & `rkvst-archivist-0.22.0/archivist/assetattachments.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/assets.py` & `rkvst-archivist-0.22.0/archivist/assets.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/attachments.py` & `rkvst-archivist-0.22.0/archivist/attachments.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/cmds/runner/main.py` & `rkvst-archivist-0.22.0/archivist/cmds/runner/main.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/cmds/runner/run.py` & `rkvst-archivist-0.22.0/archivist/cmds/runner/run.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/cmds/template/main.py` & `rkvst-archivist-0.22.0/archivist/cmds/template/main.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/cmds/template/run.py` & `rkvst-archivist-0.22.0/archivist/cmds/template/run.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/compliance.py` & `rkvst-archivist-0.22.0/archivist/compliance.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/compliance_policies.py` & `rkvst-archivist-0.22.0/archivist/compliance_policies.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/compliance_policy_requests.py` & `rkvst-archivist-0.22.0/archivist/compliance_policy_requests.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/compliance_policy_type.py` & `rkvst-archivist-0.22.0/archivist/compliance_policy_type.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/composite.py` & `rkvst-archivist-0.22.0/archivist/composite.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/confirmer.py` & `rkvst-archivist-0.22.0/archivist/confirmer.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/constants.py` & `rkvst-archivist-0.22.0/archivist/constants.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/dictmerge.py` & `rkvst-archivist-0.22.0/archivist/dictmerge.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/errors.py` & `rkvst-archivist-0.22.0/archivist/errors.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/events.py` & `rkvst-archivist-0.22.0/archivist/events.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/locations.py` & `rkvst-archivist-0.22.0/archivist/locations.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/logger.py` & `rkvst-archivist-0.22.0/archivist/logger.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/parser.py` & `rkvst-archivist-0.22.0/archivist/parser.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/retry429.py` & `rkvst-archivist-0.22.0/archivist/retry429.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/runner.py` & `rkvst-archivist-0.22.0/archivist/runner.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/sboms.py` & `rkvst-archivist-0.22.0/archivist/sboms.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/subjects.py` & `rkvst-archivist-0.22.0/archivist/subjects.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/subjects_confirmer.py` & `rkvst-archivist-0.22.0/archivist/subjects_confirmer.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/tenancies.py` & `rkvst-archivist-0.22.0/archivist/tenancies.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/timestamp.py` & `rkvst-archivist-0.22.0/archivist/timestamp.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/archivist/utils.py` & `rkvst-archivist-0.22.0/archivist/utils.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/pyproject.toml` & `rkvst-archivist-0.22.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/rkvst_archivist.egg-info/PKG-INFO` & `rkvst-archivist-0.22.0/rkvst_archivist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rkvst-archivist
-Version: 0.21.0
+Version: 0.22.0
 Summary: RKVST Client
 Home-page: https://github.com/rkvst/rkvst-python
 Author: RKVST Inc.
 Author-email: support@rkvst.com
 License: MIT
 Project-URL: Documentation, https://python.rkvst.com
 Project-URL: Source, https://github.com/rkvst/rkvst-python
```

### Comparing `rkvst-archivist-0.21.0/rkvst_archivist.egg-info/SOURCES.txt` & `rkvst-archivist-0.22.0/rkvst_archivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.21.0/setup.cfg` & `rkvst-archivist-0.22.0/setup.cfg`

 * *Files identical despite different names*


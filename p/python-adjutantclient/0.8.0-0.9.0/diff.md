# Comparing `tmp/python-adjutantclient-0.8.0.tar.gz` & `tmp/python-adjutantclient-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-adjutantclient-0.8.0.tar", last modified: Fri Mar 12 12:15:20 2021, max compression
+gzip compressed data, was "python-adjutantclient-0.9.0.tar", last modified: Fri Sep 17 16:38:13 2021, max compression
```

## Comparing `python-adjutantclient-0.8.0.tar` & `python-adjutantclient-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.324397 python-adjutantclient-0.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2021-03-12 12:15:20.324397 python-adjutantclient-0.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.316398 python-adjutantclient-0.8.0/adjutantclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.316398 python-adjutantclient-0.8.0/adjutantclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17249 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4849 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.316398 python-adjutantclient-0.8.0/adjutantclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.320397 python-adjutantclient-0.8.0/adjutantclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5120 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/signup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5275 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8635 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/osc/v1/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.320397 python-adjutantclient-0.8.0/adjutantclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.320397 python-adjutantclient-0.8.0/adjutantclient/tests/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/tests/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/tests/v1/test_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.324397 python-adjutantclient-0.8.0/adjutantclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3046 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/signup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/adjutantclient/v1/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-12 12:15:20.324397 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-03-12 12:15:20.000000 python-adjutantclient-0.8.0/python_adjutantclient.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2021-03-12 12:15:20.328397 python-adjutantclient-0.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      566 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2021-03-12 12:14:31.000000 python-adjutantclient-0.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.790098 python-adjutantclient-0.9.0/adjutantclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.790098 python-adjutantclient-0.9.0/adjutantclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17249 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4849 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.790098 python-adjutantclient-0.9.0/adjutantclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5120 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/signup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5275 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8635 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/tests/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/tests/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/tests/v1/test_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3046 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/signup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/tox.ini
```

### Comparing `python-adjutantclient-0.8.0/AUTHORS` & `python-adjutantclient-0.9.0/AUTHORS`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Adrian Turjak <adriant@catalyst.net.nz>
 Adrian Turjak <adriant@catalystcloud.nz>
 Amelia Cordwell <ameliacordwell@catalyst.net.nz>
+Anand Bhat <anandgvbhat@gmail.com>
 Andreas Jaeger <aj@suse.com>
 Arundhati Surpur <arundhati@nectechnologies.in>
 Dale Smith <dale@catalyst-eu.net>
 Doug Hellmann <doug@doughellmann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hervé Beraud <hberaud@redhat.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
```

### Comparing `python-adjutantclient-0.8.0/ChangeLog` & `python-adjutantclient-0.9.0/ChangeLog`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Migrate from testr to stestr
+
 0.8.0
 -----
 
 * bump py37 to py38 in tox.ini
 * Add expected zuul jobs
 
 0.7.0
```

### Comparing `python-adjutantclient-0.8.0/LICENSE` & `python-adjutantclient-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/PKG-INFO` & `python-adjutantclient-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-adjutantclient
-Version: 0.8.0
+Version: 0.9.0
 Summary: Adjutant API Client Library
 Home-page: https://github.com/openstack/python-adjutantclient
 Author: Adrian Turjak
 Author-email: adriant@catalyst.net.nz
 License: UNKNOWN
 Description: AdjutantClient is a command-line and python client for Adjutant.
```

### Comparing `python-adjutantclient-0.8.0/README.rst` & `python-adjutantclient-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/__init__.py` & `python-adjutantclient-0.9.0/adjutantclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/_i18n.py` & `python-adjutantclient-0.9.0/adjutantclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/client.py` & `python-adjutantclient-0.9.0/adjutantclient/client.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/common/base.py` & `python-adjutantclient-0.9.0/adjutantclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/common/http.py` & `python-adjutantclient-0.9.0/adjutantclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/exc.py` & `python-adjutantclient-0.9.0/adjutantclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/plugin.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/notifications.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/notifications.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/quota.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/quota.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/signup.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/signup.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/status.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/status.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/tasks.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/tokens.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/tokens.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/osc/v1/users.py` & `python-adjutantclient-0.9.0/adjutantclient/osc/v1/users.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/tests/v1/test_client.py` & `python-adjutantclient-0.9.0/adjutantclient/tests/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/__init__.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/client.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/notifications.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/notifications.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/quota.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/quota.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/roles.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/roles.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/signup.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/signup.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/status.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/status.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/tasks.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/tokens.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/tokens.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/adjutantclient/v1/users.py` & `python-adjutantclient-0.9.0/adjutantclient/v1/users.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/python_adjutantclient.egg-info/PKG-INFO` & `python-adjutantclient-0.9.0/python_adjutantclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-adjutantclient
-Version: 0.8.0
+Version: 0.9.0
 Summary: Adjutant API Client Library
 Home-page: https://github.com/openstack/python-adjutantclient
 Author: Adrian Turjak
 Author-email: adriant@catalyst.net.nz
 License: UNKNOWN
 Description: AdjutantClient is a command-line and python client for Adjutant.
```

### Comparing `python-adjutantclient-0.8.0/python_adjutantclient.egg-info/SOURCES.txt` & `python-adjutantclient-0.9.0/python_adjutantclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.testr.conf
+.stestr.conf
 .zuul.yaml
 AUTHORS
 ChangeLog
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
```

### Comparing `python-adjutantclient-0.8.0/python_adjutantclient.egg-info/entry_points.txt` & `python-adjutantclient-0.9.0/python_adjutantclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/requirements.txt` & `python-adjutantclient-0.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/setup.cfg` & `python-adjutantclient-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/setup.py` & `python-adjutantclient-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.8.0/test-requirements.txt` & `python-adjutantclient-0.9.0/test-requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 hacking>=3.0,<3.1.0  # Apache-2.0
 coverage>=3.6 # Apache-2.0
 ddt>=1.0.1 # MIT
 discover # BSD
 fixtures>=3.0.0 # Apache-2.0/BSD
 requests-mock>=0.7.0 # Apache-2.0
 os-client-config>=1.13.1 # Apache-2.0
-testrepository>=0.0.18 # Apache-2.0/BSD
+stestr>=2.0.0 # Apache-2.0
 testscenarios>=0.4 # Apache-2.0/BSD
 testtools>=1.4.0 # MIT
 tempest>=11.0.0 # Apache-2.0
 os-testr>=0.8.0  # Apache-2.0
```

### Comparing `python-adjutantclient-0.8.0/tox.ini` & `python-adjutantclient-0.9.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 [tox]
-minversion = 3.1
-envlist = py38
+minversion = 3.18.0
+envlist = py3
 skipsdist = True
 ignore_basepython_conflict = True
 
 [testenv]
 basepython = python3
 usedevelop = True
 setenv = VIRTUAL_ENV={envdir}
          OS_STDOUT_NOCAPTURE=False
          OS_STDERR_NOCAPTURE=False
          PYTHONHASHSEED=0
 deps =
        -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
-commands = ostestr {posargs}
+commands = stestr run --slowest {posargs}
 
-whitelist_externals = find
+allowlist_externals = find
 
 [testenv:pep8]
 commands = flake8
 
 [testenv:cover]
+allowlist_externals = find
+setenv =
+  {[testenv]setenv}
+  PYTHON=coverage run --source adjutantclient --parallel-mode
 commands =
   coverage erase
   find . -type f -name "*.pyc" -delete
-  python setup.py testr --coverage --testr-args='{posargs}'
+  stestr run {posargs}
+  coverage combine
+  coverage html -d cover
+  coverage xml -o cover/coverage.xml
   coverage report
 
 [testenv:venv]
 commands = {posargs}
 
 [flake8]
 show-source = True
```


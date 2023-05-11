# Comparing `tmp/django-vectordb-0.1.2.tar.gz` & `tmp/django-vectordb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vectordb-0.1.2.tar", last modified: Wed May 10 05:40:54 2023, max compression
+gzip compressed data, was "django-vectordb-0.1.3.tar", last modified: Thu May 11 09:00:12 2023, max compression
```

## Comparing `django-vectordb-0.1.2.tar` & `django-vectordb-0.1.3.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.145229 django-vectordb-0.1.2/
--rw-r--r--   0 pride      (501) staff       (20)    11357 2023-05-04 13:28:35.000000 django-vectordb-0.1.2/LICENSE
--rw-r--r--   0 pride      (501) staff       (20)    12009 2023-05-10 05:40:54.145735 django-vectordb-0.1.2/PKG-INFO
--rw-r--r--   0 pride      (501) staff       (20)    10609 2023-05-07 03:33:50.000000 django-vectordb-0.1.2/README.md
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.047330 django-vectordb-0.1.2/django_vectordb.egg-info/
--rw-r--r--   0 pride      (501) staff       (20)    12009 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/PKG-INFO
--rw-r--r--   0 pride      (501) staff       (20)     1387 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 pride      (501) staff       (20)        1 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 pride      (501) staff       (20)      319 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/requires.txt
--rw-r--r--   0 pride      (501) staff       (20)        9 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/top_level.txt
--rw-r--r--   0 pride      (501) staff       (20)       80 2023-05-04 08:19:18.000000 django-vectordb-0.1.2/pyproject.toml
--rw-r--r--   0 pride      (501) staff       (20)     1888 2023-05-10 05:40:54.153980 django-vectordb-0.1.2/setup.cfg
--rw-r--r--   0 pride      (501) staff       (20)      216 2023-05-05 07:20:09.000000 django-vectordb-0.1.2/setup.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.081714 django-vectordb-0.1.2/vectordb/
--rw-r--r--   0 pride      (501) staff       (20)      291 2023-05-04 15:04:49.000000 django-vectordb-0.1.2/vectordb/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)      527 2023-05-05 06:20:34.000000 django-vectordb-0.1.2/vectordb/admin.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.091992 django-vectordb-0.1.2/vectordb/ann/
--rw-r--r--   0 pride      (501) staff       (20)      115 2023-05-03 14:11:45.000000 django-vectordb-0.1.2/vectordb/ann/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     1051 2023-05-03 14:11:45.000000 django-vectordb-0.1.2/vectordb/ann/abcz.py
--rw-r--r--   0 pride      (501) staff       (20)     5918 2023-05-04 15:47:14.000000 django-vectordb-0.1.2/vectordb/ann/indexes.py
--rw-r--r--   0 pride      (501) staff       (20)      603 2023-05-04 15:46:27.000000 django-vectordb-0.1.2/vectordb/ann/singleton.py
--rw-r--r--   0 pride      (501) staff       (20)      248 2023-05-03 20:04:15.000000 django-vectordb-0.1.2/vectordb/apps.py
--rw-r--r--   0 pride      (501) staff       (20)      625 2023-05-06 07:32:16.000000 django-vectordb-0.1.2/vectordb/checks.py
--rw-r--r--   0 pride      (501) staff       (20)     1827 2023-05-04 04:39:07.000000 django-vectordb-0.1.2/vectordb/embedding_functions.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.094206 django-vectordb-0.1.2/vectordb/management/
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:40.000000 django-vectordb-0.1.2/vectordb/management/__init__.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.104687 django-vectordb-0.1.2/vectordb/management/commands/
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:44.000000 django-vectordb-0.1.2/vectordb/management/commands/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     1020 2023-05-06 07:56:41.000000 django-vectordb-0.1.2/vectordb/management/commands/vectordb_reset.py
--rw-r--r--   0 pride      (501) staff       (20)     2276 2023-05-06 07:56:43.000000 django-vectordb-0.1.2/vectordb/management/commands/vectordb_sync.py
--rw-r--r--   0 pride      (501) staff       (20)     2813 2023-05-05 07:01:23.000000 django-vectordb-0.1.2/vectordb/manager.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.112360 django-vectordb-0.1.2/vectordb/migrations/
--rw-r--r--   0 pride      (501) staff       (20)     1892 2023-05-03 14:16:42.000000 django-vectordb-0.1.2/vectordb/migrations/0001_initial.py
--rw-r--r--   0 pride      (501) staff       (20)      887 2023-05-03 20:38:37.000000 django-vectordb-0.1.2/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-03 14:10:09.000000 django-vectordb-0.1.2/vectordb/migrations/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     2099 2023-05-04 20:10:03.000000 django-vectordb-0.1.2/vectordb/models.py
--rw-r--r--   0 pride      (501) staff       (20)     4464 2023-05-06 08:24:10.000000 django-vectordb-0.1.2/vectordb/queryset.py
--rw-r--r--   0 pride      (501) staff       (20)      342 2023-05-03 14:26:35.000000 django-vectordb-0.1.2/vectordb/serializers.py
--rw-r--r--   0 pride      (501) staff       (20)     3541 2023-05-06 07:26:56.000000 django-vectordb-0.1.2/vectordb/settings.py
--rw-r--r--   0 pride      (501) staff       (20)     1073 2023-05-10 05:01:46.000000 django-vectordb-0.1.2/vectordb/shortcuts.py
--rw-r--r--   0 pride      (501) staff       (20)     1528 2023-05-05 06:33:16.000000 django-vectordb-0.1.2/vectordb/signals.py
--rw-r--r--   0 pride      (501) staff       (20)     1971 2023-05-04 20:13:05.000000 django-vectordb-0.1.2/vectordb/sync_signals.py
--rw-r--r--   0 pride      (501) staff       (20)     1475 2023-05-04 04:00:22.000000 django-vectordb-0.1.2/vectordb/tasks.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.143630 django-vectordb-0.1.2/vectordb/tests/
--rw-r--r--   0 pride      (501) staff       (20)       54 2023-05-04 20:37:23.000000 django-vectordb-0.1.2/vectordb/tests/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)      122 2023-05-04 20:37:23.000000 django-vectordb-0.1.2/vectordb/tests/apps.py
--rw-r--r--   0 pride      (501) staff       (20)      106 2023-05-06 07:32:13.000000 django-vectordb-0.1.2/vectordb/tests/dummy_module.py
--rw-r--r--   0 pride      (501) staff       (20)      346 2023-05-04 20:37:23.000000 django-vectordb-0.1.2/vectordb/tests/models.py
--rw-r--r--   0 pride      (501) staff       (20)     1794 2023-05-04 13:22:55.000000 django-vectordb-0.1.2/vectordb/tests/settings.py
--rw-r--r--   0 pride      (501) staff       (20)     1170 2023-05-04 20:41:32.000000 django-vectordb-0.1.2/vectordb/tests/test_api_endpoint.py
--rw-r--r--   0 pride      (501) staff       (20)     2970 2023-05-04 20:41:19.000000 django-vectordb-0.1.2/vectordb/tests/test_db_indexes.py
--rw-r--r--   0 pride      (501) staff       (20)      686 2023-05-03 14:14:51.000000 django-vectordb-0.1.2/vectordb/tests/test_embedding_functions.py
--rw-r--r--   0 pride      (501) staff       (20)     2606 2023-05-06 07:32:11.000000 django-vectordb-0.1.2/vectordb/tests/test_settings.py
--rw-r--r--   0 pride      (501) staff       (20)      627 2023-05-04 20:42:47.000000 django-vectordb-0.1.2/vectordb/tests/test_singleton_meta.py
--rw-r--r--   0 pride      (501) staff       (20)     3547 2023-05-04 19:22:55.000000 django-vectordb-0.1.2/vectordb/tests/test_vectordb.py
--rw-r--r--   0 pride      (501) staff       (20)       60 2023-05-03 14:10:09.000000 django-vectordb-0.1.2/vectordb/tests.py
--rw-r--r--   0 pride      (501) staff       (20)      280 2023-05-04 20:40:02.000000 django-vectordb-0.1.2/vectordb/urls.py
--rw-r--r--   0 pride      (501) staff       (20)     3549 2023-05-06 07:28:17.000000 django-vectordb-0.1.2/vectordb/utils.py
--rw-r--r--   0 pride      (501) staff       (20)     1744 2023-05-04 18:22:43.000000 django-vectordb-0.1.2/vectordb/validators.py
--rw-r--r--   0 pride      (501) staff       (20)     1232 2023-05-05 06:34:07.000000 django-vectordb-0.1.2/vectordb/views.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.512143 django-vectordb-0.1.3/
+-rw-r--r--   0 pride      (501) staff       (20)    11357 2023-05-04 13:28:35.000000 django-vectordb-0.1.3/LICENSE
+-rw-r--r--   0 pride      (501) staff       (20)    14563 2023-05-11 09:00:12.512908 django-vectordb-0.1.3/PKG-INFO
+-rw-r--r--   0 pride      (501) staff       (20)    13163 2023-05-11 08:55:28.000000 django-vectordb-0.1.3/README.md
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.350416 django-vectordb-0.1.3/django_vectordb.egg-info/
+-rw-r--r--   0 pride      (501) staff       (20)    14563 2023-05-11 09:00:12.000000 django-vectordb-0.1.3/django_vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 pride      (501) staff       (20)     1369 2023-05-11 09:00:12.000000 django-vectordb-0.1.3/django_vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 pride      (501) staff       (20)        1 2023-05-11 09:00:12.000000 django-vectordb-0.1.3/django_vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 pride      (501) staff       (20)      335 2023-05-11 09:00:12.000000 django-vectordb-0.1.3/django_vectordb.egg-info/requires.txt
+-rw-r--r--   0 pride      (501) staff       (20)        9 2023-05-11 09:00:12.000000 django-vectordb-0.1.3/django_vectordb.egg-info/top_level.txt
+-rw-r--r--   0 pride      (501) staff       (20)      112 2023-05-11 06:30:28.000000 django-vectordb-0.1.3/pyproject.toml
+-rw-r--r--   0 pride      (501) staff       (20)     1857 2023-05-11 09:00:12.554257 django-vectordb-0.1.3/setup.cfg
+-rw-r--r--   0 pride      (501) staff       (20)      216 2023-05-05 07:20:09.000000 django-vectordb-0.1.3/setup.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.405052 django-vectordb-0.1.3/vectordb/
+-rw-r--r--   0 pride      (501) staff       (20)      291 2023-05-04 15:04:49.000000 django-vectordb-0.1.3/vectordb/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      527 2023-05-05 06:20:34.000000 django-vectordb-0.1.3/vectordb/admin.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.415926 django-vectordb-0.1.3/vectordb/ann/
+-rw-r--r--   0 pride      (501) staff       (20)      139 2023-05-11 07:51:18.000000 django-vectordb-0.1.3/vectordb/ann/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     1051 2023-05-03 14:11:45.000000 django-vectordb-0.1.3/vectordb/ann/abcz.py
+-rw-r--r--   0 pride      (501) staff       (20)     5936 2023-05-11 07:55:37.000000 django-vectordb-0.1.3/vectordb/ann/indexes.py
+-rw-r--r--   0 pride      (501) staff       (20)      601 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/ann/singleton.py
+-rw-r--r--   0 pride      (501) staff       (20)      256 2023-05-11 07:59:02.000000 django-vectordb-0.1.3/vectordb/apps.py
+-rw-r--r--   0 pride      (501) staff       (20)      625 2023-05-06 07:32:16.000000 django-vectordb-0.1.3/vectordb/checks.py
+-rw-r--r--   0 pride      (501) staff       (20)     1862 2023-05-11 08:00:56.000000 django-vectordb-0.1.3/vectordb/embedding_functions.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.417729 django-vectordb-0.1.3/vectordb/management/
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:40.000000 django-vectordb-0.1.3/vectordb/management/__init__.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.422071 django-vectordb-0.1.3/vectordb/management/commands/
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:44.000000 django-vectordb-0.1.3/vectordb/management/commands/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      975 2023-05-11 08:03:58.000000 django-vectordb-0.1.3/vectordb/management/commands/vectordb_reset.py
+-rw-r--r--   0 pride      (501) staff       (20)     3251 2023-05-11 08:43:36.000000 django-vectordb-0.1.3/vectordb/management/commands/vectordb_sync.py
+-rw-r--r--   0 pride      (501) staff       (20)     2663 2023-05-11 08:22:25.000000 django-vectordb-0.1.3/vectordb/manager.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.430416 django-vectordb-0.1.3/vectordb/migrations/
+-rw-r--r--   0 pride      (501) staff       (20)     1892 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/migrations/0001_initial.py
+-rw-r--r--   0 pride      (501) staff       (20)      888 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-03 14:10:09.000000 django-vectordb-0.1.3/vectordb/migrations/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     2062 2023-05-11 08:24:43.000000 django-vectordb-0.1.3/vectordb/models.py
+-rw-r--r--   0 pride      (501) staff       (20)     4467 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/queryset.py
+-rw-r--r--   0 pride      (501) staff       (20)      342 2023-05-03 14:26:35.000000 django-vectordb-0.1.3/vectordb/serializers.py
+-rw-r--r--   0 pride      (501) staff       (20)     3692 2023-05-11 08:19:38.000000 django-vectordb-0.1.3/vectordb/settings.py
+-rw-r--r--   0 pride      (501) staff       (20)     1084 2023-05-11 08:07:52.000000 django-vectordb-0.1.3/vectordb/shortcuts.py
+-rw-r--r--   0 pride      (501) staff       (20)     1469 2023-05-11 08:07:19.000000 django-vectordb-0.1.3/vectordb/signals.py
+-rw-r--r--   0 pride      (501) staff       (20)     1840 2023-05-11 08:05:35.000000 django-vectordb-0.1.3/vectordb/sync_signals.py
+-rw-r--r--   0 pride      (501) staff       (20)     1357 2023-05-11 07:59:52.000000 django-vectordb-0.1.3/vectordb/tasks.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-11 09:00:12.509647 django-vectordb-0.1.3/vectordb/tests/
+-rw-r--r--   0 pride      (501) staff       (20)       54 2023-05-04 20:37:23.000000 django-vectordb-0.1.3/vectordb/tests/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      122 2023-05-04 20:37:23.000000 django-vectordb-0.1.3/vectordb/tests/apps.py
+-rw-r--r--   0 pride      (501) staff       (20)      106 2023-05-06 07:32:13.000000 django-vectordb-0.1.3/vectordb/tests/dummy_module.py
+-rw-r--r--   0 pride      (501) staff       (20)      346 2023-05-04 20:37:23.000000 django-vectordb-0.1.3/vectordb/tests/models.py
+-rw-r--r--   0 pride      (501) staff       (20)     1793 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/tests/settings.py
+-rw-r--r--   0 pride      (501) staff       (20)     1171 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/tests/test_api_endpoint.py
+-rw-r--r--   0 pride      (501) staff       (20)     2971 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/tests/test_db_indexes.py
+-rw-r--r--   0 pride      (501) staff       (20)      687 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/tests/test_embedding_functions.py
+-rw-r--r--   0 pride      (501) staff       (20)     2552 2023-05-11 08:06:58.000000 django-vectordb-0.1.3/vectordb/tests/test_settings.py
+-rw-r--r--   0 pride      (501) staff       (20)      627 2023-05-04 20:42:47.000000 django-vectordb-0.1.3/vectordb/tests/test_singleton_meta.py
+-rw-r--r--   0 pride      (501) staff       (20)     3548 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/tests/test_vectordb.py
+-rw-r--r--   0 pride      (501) staff       (20)      279 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/urls.py
+-rw-r--r--   0 pride      (501) staff       (20)     3532 2023-05-11 08:16:55.000000 django-vectordb-0.1.3/vectordb/utils.py
+-rw-r--r--   0 pride      (501) staff       (20)     1745 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/validators.py
+-rw-r--r--   0 pride      (501) staff       (20)     1233 2023-05-11 06:20:23.000000 django-vectordb-0.1.3/vectordb/views.py
```

### Comparing `django-vectordb-0.1.2/LICENSE` & `django-vectordb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.2/PKG-INFO` & `django-vectordb-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,23 @@
-Metadata-Version: 2.1
-Name: django-vectordb
-Version: 0.1.2
-Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
-Home-page: https://github.com/pkavumba/django-vectordb.git
-Author: Pride Kavumba
-Author-email: pkavumba@gmail.com
-License: Apache License 2.0
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: standard
-Provides-Extra: dev
-Provides-Extra: tests
-License-File: LICENSE
-
-# Django VectorDB
+# [Django VectorDB][docs]
 
 ---
 
-[![pypi-version]][pypi]
+![PyPI](https://img.shields.io/pypi/v/django-vectordb?color=blue)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-vectordb)
+[![Downloads](https://static.pepy.tech/badge/django-vectordb)](https://pepy.tech/project/django-vectordb)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-vectordb)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-**Adding extremely fast, low-latency, and scalable vector search to django apps.**
+**Adding extremely fast, low-latency, and scalable vector similarity search to django applications.**
 
 Full documentation for the project is available at [https://pkavumba.github.io/django-vectordb/][docs].
 
-Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
+[Django Vector Database][docs] is a powerful and flexible toolkit for adding vector similarity search capabilities to your Django applications. It is built on top of the lighteningly fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
 - Native Django integration.
@@ -221,15 +191,35 @@
 vectordb.add_text(text="Hello text", id=3, metadata={"user_id": 1})
 ```
 
 The `text` and `id` are required. Additionally, the `id` must be unique, or an error will occur. `metadata` can be `None` or any valid JSON.
 
 ### Automatically Syncing Your Model to the vector database
 
-To enable auto sync, import the following signals and register them with your models:
+To enable auto sync, register the model to vectordb sync handlers in `apps.py`. The sync handlers are signals defined in `vectordb/sync_signals.py`.
+
+```python
+from django.apps import AppConfig
+
+
+class BlogConfig(AppConfig):
+    default_auto_field = "django.db.models.BigAutoField"
+    name = "blog"
+
+    def ready(self):
+        from .models import Post
+        from vectordb.shortcuts import autosync_model_to_vectordb
+        autosync_model_to_vectordb(Post)
+```
+
+This will automatically sync the vectors when you create and delete instances.
+
+Note that signals are not called in bulk create, so you will need to sync manually when using those methods.
+
+Alternatively, you can import the following signals and register them by yourself:
 
 ```python
 # signals.py
 from django.db.models.signals import post_save, post_delete
 
 from vectordb.sync_signals import (
     sync_vectordb_on_create_update,
@@ -281,42 +271,89 @@
 
 ```python
 vectordb.search("Some text", k=10).only('text', 'content_object')
 ```
 
 If `k` is not provided, the default value is 10.
 
-### Filtering
+## Metadata Filtering with Django Vector Database
+
+Django vector database provides a powerful way to filter on metadata, using the intuitive Django QuerySet methods.
 
-You can filter on `text` or `metadata` with the full power of Django QuerySet filtering:
+You can filter on `text` or `metadata` with the full power of Django QuerySet filtering. You can combine as many filters as needed. And since Django vector database is built on top of Django QuerySet, you can chain the filters with the search method. You can also filter on nested metadata fields.
 
 ```python
 # scope the search to user with an id 1
 vectordb.filter(metadata__user_id=1).search("Some text", k=10)
 
 # example two with more filters
-vectordb.filter(text__icontains="Apple", metadata__title__icontains="IPhone", metadata__description__icontains="2023").search("Apple new phone", k=10)
+vectordb.filter(text__icontains="Apple",
+    metadata__title__icontains="IPhone",
+    metadata__description__icontains="2023"
+    ).search("Apple new phone", k=10)
+```
+
+If our metadata was nested like follows:
+
+```json
+{
+  "text": "Sample text",
+  "metadata": {
+    "date": {
+      "year": 2021,
+      "month": 7,
+      "day": 20,
+      "time": {
+        "hh": 14,
+        "mm": 30,
+        "ss": 45
+      }
+    }
+  }
+}
+```
+
+We can filter on the nested fields like so:
+
+```python
+vectordb.filter(
+    metadata__date__year=2021,
+    metadata__date__time__hh=14
+    ).search("Sample text", k=10)
+```
+
+We can also use model instances instead of text:
+
+```py
+post1 = Post.objects.get(id=1)
+# Limit the search scope to a user with an id of 1
+results = vectordb.filter(metadata__user_id=1).search(post1, k=10)
+
+# Scope the results to text which contains France, belonging to user with id 1 and created in 2023
+vectordb.filter(text__icontains="Apple",
+    metadata__title__icontains="IPhone",
+    metadata__description__icontains="2023").search(post1, k=10)
 ```
 
-Refer to the [Django documentation](https://docs.djangoproject.com/en/4.2/topics/db/queries/) on querying the `JSONField` for more information on filtering.
+Refer to the [Django documentation][django-queries] on querying the `JSONField` for more information on filtering.
 
 ---
 
 ## Settings
 
 You can provide your settings in the `settings.py` file of your project. The following settings are available:
 
 ```python
 # settings.py
 DJANGO_VECTOR_DB = {
-    "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
-    "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+    "DEFAULT_EMBEDDING_CLASS": "vectordb.embedding_functions.SentenceTransformerEncoder",
+    "DEFAULT_EMBEDDING_MODEL": "all-MiniLM-L6-v2",
     # Can be "cosine" or "l2"
-    "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
-    "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+    "DEFAULT_EMBEDDING_SPACE": "l2"
+    "DEFAULT_EMBEDDING_DIMENSION": 384, # Default is 384 for "all-MiniLM-L6-v2"
     "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
     "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
     "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
 }
 ```
 
 ## Quickstart
@@ -326,15 +363,15 @@
 ---
 
 ## Development
 
 Clone the repository
 
 ```bash
-$ git clone
+$ git clone https://github.com/pkavumba/django-vectordb.git
 ```
 
 Install the app in editable mode with all dev dependencies:
 
 ```bash
 pip install -e .[dev]
 ```
@@ -360,7 +397,8 @@
 [sentence-transformers]: https://www.sbert.net
 [hnswlib]: https://github.com/nmslib/hnswlib
 [drf]: https://www.django-rest-framework.org
 [django-filters]: https://pypi.org/project/django-filter/
 [docs]: https://pkavumba.github.io/django-vectordb/
 [pypi]: https://pypi.org/project/django-vectordb/
 [pypi-version]: https://img.shields.io/pypi/v/django-vectordb.svg
+[django-queries]: https://docs.djangoproject.com/en/4.2/topics/db/queries/
```

### Comparing `django-vectordb-0.1.2/README.md` & `django-vectordb-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,58 @@
-# Django VectorDB
+Metadata-Version: 2.1
+Name: django-vectordb
+Version: 0.1.3
+Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
+Home-page: https://github.com/pkavumba/django-vectordb.git
+Author: Pride Kavumba
+Author-email: pkavumba@gmail.com
+License: Apache License 2.0
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: standard
+Provides-Extra: dev
+Provides-Extra: tests
+License-File: LICENSE
+
+# [Django VectorDB][docs]
 
 ---
 
-[![pypi-version]][pypi]
+![PyPI](https://img.shields.io/pypi/v/django-vectordb?color=blue)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-vectordb)
+[![Downloads](https://static.pepy.tech/badge/django-vectordb)](https://pepy.tech/project/django-vectordb)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-vectordb)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-**Adding extremely fast, low-latency, and scalable vector search to django apps.**
+**Adding extremely fast, low-latency, and scalable vector similarity search to django applications.**
 
 Full documentation for the project is available at [https://pkavumba.github.io/django-vectordb/][docs].
 
-Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
+[Django Vector Database][docs] is a powerful and flexible toolkit for adding vector similarity search capabilities to your Django applications. It is built on top of the lighteningly fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
 - Native Django integration.
@@ -186,15 +226,35 @@
 vectordb.add_text(text="Hello text", id=3, metadata={"user_id": 1})
 ```
 
 The `text` and `id` are required. Additionally, the `id` must be unique, or an error will occur. `metadata` can be `None` or any valid JSON.
 
 ### Automatically Syncing Your Model to the vector database
 
-To enable auto sync, import the following signals and register them with your models:
+To enable auto sync, register the model to vectordb sync handlers in `apps.py`. The sync handlers are signals defined in `vectordb/sync_signals.py`.
+
+```python
+from django.apps import AppConfig
+
+
+class BlogConfig(AppConfig):
+    default_auto_field = "django.db.models.BigAutoField"
+    name = "blog"
+
+    def ready(self):
+        from .models import Post
+        from vectordb.shortcuts import autosync_model_to_vectordb
+        autosync_model_to_vectordb(Post)
+```
+
+This will automatically sync the vectors when you create and delete instances.
+
+Note that signals are not called in bulk create, so you will need to sync manually when using those methods.
+
+Alternatively, you can import the following signals and register them by yourself:
 
 ```python
 # signals.py
 from django.db.models.signals import post_save, post_delete
 
 from vectordb.sync_signals import (
     sync_vectordb_on_create_update,
@@ -246,42 +306,89 @@
 
 ```python
 vectordb.search("Some text", k=10).only('text', 'content_object')
 ```
 
 If `k` is not provided, the default value is 10.
 
-### Filtering
+## Metadata Filtering with Django Vector Database
+
+Django vector database provides a powerful way to filter on metadata, using the intuitive Django QuerySet methods.
 
-You can filter on `text` or `metadata` with the full power of Django QuerySet filtering:
+You can filter on `text` or `metadata` with the full power of Django QuerySet filtering. You can combine as many filters as needed. And since Django vector database is built on top of Django QuerySet, you can chain the filters with the search method. You can also filter on nested metadata fields.
 
 ```python
 # scope the search to user with an id 1
 vectordb.filter(metadata__user_id=1).search("Some text", k=10)
 
 # example two with more filters
-vectordb.filter(text__icontains="Apple", metadata__title__icontains="IPhone", metadata__description__icontains="2023").search("Apple new phone", k=10)
+vectordb.filter(text__icontains="Apple",
+    metadata__title__icontains="IPhone",
+    metadata__description__icontains="2023"
+    ).search("Apple new phone", k=10)
+```
+
+If our metadata was nested like follows:
+
+```json
+{
+  "text": "Sample text",
+  "metadata": {
+    "date": {
+      "year": 2021,
+      "month": 7,
+      "day": 20,
+      "time": {
+        "hh": 14,
+        "mm": 30,
+        "ss": 45
+      }
+    }
+  }
+}
+```
+
+We can filter on the nested fields like so:
+
+```python
+vectordb.filter(
+    metadata__date__year=2021,
+    metadata__date__time__hh=14
+    ).search("Sample text", k=10)
+```
+
+We can also use model instances instead of text:
+
+```py
+post1 = Post.objects.get(id=1)
+# Limit the search scope to a user with an id of 1
+results = vectordb.filter(metadata__user_id=1).search(post1, k=10)
+
+# Scope the results to text which contains France, belonging to user with id 1 and created in 2023
+vectordb.filter(text__icontains="Apple",
+    metadata__title__icontains="IPhone",
+    metadata__description__icontains="2023").search(post1, k=10)
 ```
 
-Refer to the [Django documentation](https://docs.djangoproject.com/en/4.2/topics/db/queries/) on querying the `JSONField` for more information on filtering.
+Refer to the [Django documentation][django-queries] on querying the `JSONField` for more information on filtering.
 
 ---
 
 ## Settings
 
 You can provide your settings in the `settings.py` file of your project. The following settings are available:
 
 ```python
 # settings.py
 DJANGO_VECTOR_DB = {
-    "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
-    "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+    "DEFAULT_EMBEDDING_CLASS": "vectordb.embedding_functions.SentenceTransformerEncoder",
+    "DEFAULT_EMBEDDING_MODEL": "all-MiniLM-L6-v2",
     # Can be "cosine" or "l2"
-    "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
-    "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+    "DEFAULT_EMBEDDING_SPACE": "l2"
+    "DEFAULT_EMBEDDING_DIMENSION": 384, # Default is 384 for "all-MiniLM-L6-v2"
     "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
     "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
     "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
 }
 ```
 
 ## Quickstart
@@ -291,15 +398,15 @@
 ---
 
 ## Development
 
 Clone the repository
 
 ```bash
-$ git clone
+$ git clone https://github.com/pkavumba/django-vectordb.git
 ```
 
 Install the app in editable mode with all dev dependencies:
 
 ```bash
 pip install -e .[dev]
 ```
@@ -325,7 +432,8 @@
 [sentence-transformers]: https://www.sbert.net
 [hnswlib]: https://github.com/nmslib/hnswlib
 [drf]: https://www.django-rest-framework.org
 [django-filters]: https://pypi.org/project/django-filter/
 [docs]: https://pkavumba.github.io/django-vectordb/
 [pypi]: https://pypi.org/project/django-vectordb/
 [pypi-version]: https://img.shields.io/pypi/v/django-vectordb.svg
+[django-queries]: https://docs.djangoproject.com/en/4.2/topics/db/queries/
```

### Comparing `django-vectordb-0.1.2/django_vectordb.egg-info/PKG-INFO` & `django-vectordb-0.1.3/django_vectordb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectordb
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 Home-page: https://github.com/pkavumba/django-vectordb.git
 Author: Pride Kavumba
 Author-email: pkavumba@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -29,25 +29,30 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: standard
 Provides-Extra: dev
 Provides-Extra: tests
 License-File: LICENSE
 
-# Django VectorDB
+# [Django VectorDB][docs]
 
 ---
 
-[![pypi-version]][pypi]
+![PyPI](https://img.shields.io/pypi/v/django-vectordb?color=blue)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-vectordb)
+[![Downloads](https://static.pepy.tech/badge/django-vectordb)](https://pepy.tech/project/django-vectordb)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-vectordb)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-**Adding extremely fast, low-latency, and scalable vector search to django apps.**
+**Adding extremely fast, low-latency, and scalable vector similarity search to django applications.**
 
 Full documentation for the project is available at [https://pkavumba.github.io/django-vectordb/][docs].
 
-Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
+[Django Vector Database][docs] is a powerful and flexible toolkit for adding vector similarity search capabilities to your Django applications. It is built on top of the lighteningly fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
 - Native Django integration.
@@ -221,15 +226,35 @@
 vectordb.add_text(text="Hello text", id=3, metadata={"user_id": 1})
 ```
 
 The `text` and `id` are required. Additionally, the `id` must be unique, or an error will occur. `metadata` can be `None` or any valid JSON.
 
 ### Automatically Syncing Your Model to the vector database
 
-To enable auto sync, import the following signals and register them with your models:
+To enable auto sync, register the model to vectordb sync handlers in `apps.py`. The sync handlers are signals defined in `vectordb/sync_signals.py`.
+
+```python
+from django.apps import AppConfig
+
+
+class BlogConfig(AppConfig):
+    default_auto_field = "django.db.models.BigAutoField"
+    name = "blog"
+
+    def ready(self):
+        from .models import Post
+        from vectordb.shortcuts import autosync_model_to_vectordb
+        autosync_model_to_vectordb(Post)
+```
+
+This will automatically sync the vectors when you create and delete instances.
+
+Note that signals are not called in bulk create, so you will need to sync manually when using those methods.
+
+Alternatively, you can import the following signals and register them by yourself:
 
 ```python
 # signals.py
 from django.db.models.signals import post_save, post_delete
 
 from vectordb.sync_signals import (
     sync_vectordb_on_create_update,
@@ -281,42 +306,89 @@
 
 ```python
 vectordb.search("Some text", k=10).only('text', 'content_object')
 ```
 
 If `k` is not provided, the default value is 10.
 
-### Filtering
+## Metadata Filtering with Django Vector Database
+
+Django vector database provides a powerful way to filter on metadata, using the intuitive Django QuerySet methods.
 
-You can filter on `text` or `metadata` with the full power of Django QuerySet filtering:
+You can filter on `text` or `metadata` with the full power of Django QuerySet filtering. You can combine as many filters as needed. And since Django vector database is built on top of Django QuerySet, you can chain the filters with the search method. You can also filter on nested metadata fields.
 
 ```python
 # scope the search to user with an id 1
 vectordb.filter(metadata__user_id=1).search("Some text", k=10)
 
 # example two with more filters
-vectordb.filter(text__icontains="Apple", metadata__title__icontains="IPhone", metadata__description__icontains="2023").search("Apple new phone", k=10)
+vectordb.filter(text__icontains="Apple",
+    metadata__title__icontains="IPhone",
+    metadata__description__icontains="2023"
+    ).search("Apple new phone", k=10)
+```
+
+If our metadata was nested like follows:
+
+```json
+{
+  "text": "Sample text",
+  "metadata": {
+    "date": {
+      "year": 2021,
+      "month": 7,
+      "day": 20,
+      "time": {
+        "hh": 14,
+        "mm": 30,
+        "ss": 45
+      }
+    }
+  }
+}
+```
+
+We can filter on the nested fields like so:
+
+```python
+vectordb.filter(
+    metadata__date__year=2021,
+    metadata__date__time__hh=14
+    ).search("Sample text", k=10)
+```
+
+We can also use model instances instead of text:
+
+```py
+post1 = Post.objects.get(id=1)
+# Limit the search scope to a user with an id of 1
+results = vectordb.filter(metadata__user_id=1).search(post1, k=10)
+
+# Scope the results to text which contains France, belonging to user with id 1 and created in 2023
+vectordb.filter(text__icontains="Apple",
+    metadata__title__icontains="IPhone",
+    metadata__description__icontains="2023").search(post1, k=10)
 ```
 
-Refer to the [Django documentation](https://docs.djangoproject.com/en/4.2/topics/db/queries/) on querying the `JSONField` for more information on filtering.
+Refer to the [Django documentation][django-queries] on querying the `JSONField` for more information on filtering.
 
 ---
 
 ## Settings
 
 You can provide your settings in the `settings.py` file of your project. The following settings are available:
 
 ```python
 # settings.py
 DJANGO_VECTOR_DB = {
-    "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
-    "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+    "DEFAULT_EMBEDDING_CLASS": "vectordb.embedding_functions.SentenceTransformerEncoder",
+    "DEFAULT_EMBEDDING_MODEL": "all-MiniLM-L6-v2",
     # Can be "cosine" or "l2"
-    "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
-    "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+    "DEFAULT_EMBEDDING_SPACE": "l2"
+    "DEFAULT_EMBEDDING_DIMENSION": 384, # Default is 384 for "all-MiniLM-L6-v2"
     "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
     "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
     "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
 }
 ```
 
 ## Quickstart
@@ -326,15 +398,15 @@
 ---
 
 ## Development
 
 Clone the repository
 
 ```bash
-$ git clone
+$ git clone https://github.com/pkavumba/django-vectordb.git
 ```
 
 Install the app in editable mode with all dev dependencies:
 
 ```bash
 pip install -e .[dev]
 ```
@@ -360,7 +432,8 @@
 [sentence-transformers]: https://www.sbert.net
 [hnswlib]: https://github.com/nmslib/hnswlib
 [drf]: https://www.django-rest-framework.org
 [django-filters]: https://pypi.org/project/django-filter/
 [docs]: https://pkavumba.github.io/django-vectordb/
 [pypi]: https://pypi.org/project/django-vectordb/
 [pypi-version]: https://img.shields.io/pypi/v/django-vectordb.svg
+[django-queries]: https://docs.djangoproject.com/en/4.2/topics/db/queries/
```

### Comparing `django-vectordb-0.1.2/django_vectordb.egg-info/SOURCES.txt` & `django-vectordb-0.1.3/django_vectordb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 vectordb/queryset.py
 vectordb/serializers.py
 vectordb/settings.py
 vectordb/shortcuts.py
 vectordb/signals.py
 vectordb/sync_signals.py
 vectordb/tasks.py
-vectordb/tests.py
 vectordb/urls.py
 vectordb/utils.py
 vectordb/validators.py
 vectordb/views.py
 vectordb/ann/__init__.py
 vectordb/ann/abcz.py
 vectordb/ann/indexes.py
```

### Comparing `django-vectordb-0.1.2/setup.cfg` & `django-vectordb-0.1.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-vectordb
-version = 0.1.2
+version = 0.1.3
 description = Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 long_description = file: README.md
 url = https://github.com/pkavumba/django-vectordb.git
 author = Pride Kavumba
 author_email = pkavumba@gmail.com
 license = Apache License 2.0
 classifiers = 
@@ -51,37 +51,35 @@
 	pytest-django
 	sentence-transformers
 	djangorestframework
 	django-filter
 	mkdocs
 	django-stubs
 	pre-commit
+	mkdocs-material
 tests = 
 	pytest
 	pytest-django
 	sentence-transformers
 	djangorestframework
 	django-filter
 
 [options.packages.find]
 exclude = 
 	tests
 
 [flake8]
-exclude = venv/*,tox/*,docs/*,testproject/*,build/*
-max-line-length = 88
+exclude = venv/*,tox/*,docs/*,dist/*,build/*
+max-line-length = 100
 extend-ignore = E203, W503
 
 [isort]
 profile = black
 
 [tool:pytest]
 DJANGO_SETTINGS_MODULE = vectordb.tests.settings
 testpaths = vectordb/tests
 
-[mypy]
-plugins = mypy_django_plugin.main
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-vectordb-0.1.2/vectordb/admin.py` & `django-vectordb-0.1.3/vectordb/admin.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.2/vectordb/ann/abcz.py` & `django-vectordb-0.1.3/vectordb/ann/abcz.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.2/vectordb/ann/indexes.py` & `django-vectordb-0.1.3/vectordb/ann/indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
-import abc
+import json
 import os
-from typing import Any
+
 import hnswlib
-import numpy as np
-import json
 
 from . import AbstractIndex
 
 
 class HSWNLibIndex(AbstractIndex):
     def __init__(self, dim, max_elements, space="cosine", *args, **kwargs):
         self.dim = dim
@@ -90,19 +88,19 @@
     def search(self, query, k=10, **kwargs):
         ids_in = kwargs.get("ids__in", None)
         ids_not_in = kwargs.get("ids__not_in", None)
         ef = kwargs.get("ef", None)
 
         filter_fn = None
         if ids_in is not None and ids_not_in is not None:
-            filter_fn = lambda x: x in ids_in and x not in ids_not_in
+            filter_fn = lambda x: x in ids_in and x not in ids_not_in  # noqa: E731
         elif ids_in is not None:
-            filter_fn = lambda x: x in ids_in
+            filter_fn = lambda x: x in ids_in  # noqa: E731
         elif ids_not_in is not None:
-            filter_fn = lambda x: x not in ids_not_in
+            filter_fn = lambda x: x not in ids_not_in  # noqa: E731
 
         if ef is not None:
             if type(self.index) == hnswlib.Index:
                 self.index.set_ef(ef)
             else:
                 ValueError("ef can only be set for HNSW Index")
 
@@ -154,28 +152,27 @@
     def search(self, query, k=10, **kwargs):
         ids_in = kwargs.get("ids__in", None)
         ids_not_in = kwargs.get("ids__not_in", None)
         ef = kwargs.get("ef", None)
 
         filter_fn = None
         if ids_in is not None and ids_not_in is not None:
-            filter_fn = lambda x: x in ids_in and x not in ids_not_in
+            filter_fn = lambda x: x in ids_in and x not in ids_not_in  # noqa: E731
         elif ids_in is not None:
-            filter_fn = lambda x: x in ids_in
+            filter_fn = lambda x: x in ids_in  # noqa: E731
         elif ids_not_in is not None:
-            filter_fn = lambda x: x not in ids_not_in
+            filter_fn = lambda x: x not in ids_not_in  # noqa: E731
 
         if ef is not None:
             if type(self.index) == hnswlib.Index:
                 self.index.set_ef(ef)
             else:
                 ValueError("ef can only be set for HNSW Index")
 
         if filter_fn is not None:
-            #
             return self.index.knn_query(query, k, filter=filter_fn, num_threads=1)
 
         return self.index.knn_query(query, k, num_threads=-1)
 
     @property
     def metadata(self):
         return {
```

### Comparing `django-vectordb-0.1.2/vectordb/ann/singleton.py` & `django-vectordb-0.1.3/vectordb/ann/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
-from typing import Any
-
-
 import abc
+from typing import Any
 
 
 class SingletonMeta(type):
     _instances: dict[Any, Any] = {}
 
     def __call__(cls, *args, **kwargs):
         should_not_cache = kwargs.pop("should_not_cache", False)
```

### Comparing `django-vectordb-0.1.2/vectordb/checks.py` & `django-vectordb-0.1.3/vectordb/checks.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.2/vectordb/embedding_functions.py` & `django-vectordb-0.1.3/vectordb/embedding_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,31 @@
             instance = super().__new__(cls)
             cls._instances[model_name] = instance
         return cls._instances[model_name]
 
     def __init__(self, model_name="all-MiniLM-L6-v2"):
         if SentenceTransformer is None:
             raise ImportError(
-                "SentenceTransformer is not installed. Please install sentence-transformers package. Or run `$ pip install sentence-transformers`"
+                "SentenceTransformer is not installed. Please install sentence-transformers package."  # noqa
+                " Or run `$ pip install sentence-transformers`"
             )
         if not hasattr(self, "model"):
             self.model = SentenceTransformer(model_name)
 
     def __call__(self, texts: list[str]):
         return self.model.encode(texts, convert_to_numpy=True)
 
 
 class OpenAIEmbeddings:
     def __init__(self):
         if not hasattr(settings, "OPENAI_API_KEY"):
             raise ValueError("OPENAI_API_KEY is not set in Django settings.")
         if openai is None:
             raise ImportError(
-                "OpenAI API is not installed. Please install openai package. Or run `$ pip install openai`"
+                "OpenAI API is not installed. Please install openai package. Or run `$ pip install openai`"  # noqa
             )
         openai.api_key = settings.OPENAI_API_KEY
 
     def get_embedding(self, text, model="text-embedding-ada-002"):
         text = text.replace("\n", " ")
         response = openai.Embedding.create(input=[text], model=model)
         return response["data"][0]["embedding"]
```

### Comparing `django-vectordb-0.1.2/vectordb/management/commands/vectordb_sync.py` & `django-vectordb-0.1.3/vectordb/management/commands/vectordb_sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.apps import apps
-from django.core.management.base import BaseCommand
 from django.contrib.contenttypes.models import ContentType
+from django.core.management.base import BaseCommand
+
 from vectordb.models import Vector
 
 
 class Command(BaseCommand):
     help = "Syncs Vector model with instances of a given model"
 
     def add_arguments(self, parser):
@@ -36,28 +37,51 @@
         num_to_remove = have_been_deleted_qs.count()
 
         if num_to_remove > 0:
             # Remove instances in Vector that are not in the given model
             have_been_deleted_qs.delete()
 
         count_adds = 0
+        count_updates = 0
         count_skips = 0
         # Add instances to Vector that are not already there
         for instance in instances:
             if Vector.objects.filter(
                 content_type=content_type,
                 object_id=instance.pk,
             ).exists():
-                self.stdout.write(f"Skipping {instance} because it already exists")
-                count_skips += 1
+                db_instance = Vector.objects.get(
+                    content_type=content_type,
+                    object_id=instance.pk,
+                )
+                if (
+                    db_instance.text != instance.get_vectordb_text()
+                    or db_instance.metadata != instance.get_vectordb_metadata()
+                ):
+                    db_instance.text = instance.get_vectordb_text()
+                    db_instance.metadata = instance.get_vectordb_metadata()
+                    db_instance.save()
+                    self.stdout.write(
+                        self.style.SUCCESS(
+                            f"Updated {instance} in Vector model because text/metadata changed"
+                        )
+                    )
+                    count_updates += 1
+                else:
+                    self.stdout.write(
+                        f"Skipping {instance} because it exists and hasn't changed"
+                    )
+                    count_skips += 1
             else:
                 Vector.objects.add_instance(instance)
                 self.stdout.write(
                     self.style.SUCCESS(f"Added {instance} to Vector model")
                 )
                 count_adds += 1
 
         self.stdout.write(
             self.style.SUCCESS(
-                f"Synced Vector model with {model_name}. {count_adds} added, {count_skips} skipped, {num_to_remove} removed."
+                f"Synced Vector model with {model_name}. {count_adds} added, "
+                f"{count_updates} updated, {count_skips} skipped,"
+                f" {num_to_remove} removed."
             )
         )
```

### Comparing `django-vectordb-0.1.2/vectordb/manager.py` & `django-vectordb-0.1.3/vectordb/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,49 @@
 from __future__ import annotations
 
-import os
 import logging
+import os
 import time
-from django.conf import settings
+
 from django.db import models
 
 from .ann.indexes import HNSWIndex
 from .queryset import VectorQuerySet
+from .settings import vectordb_settings
 from .utils import (
-    get_embedding_function,
     create_vector_from_instance,
     create_vector_from_text,
+    get_embedding_function,
 )
 
 # Get an instance of a logger
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("VectorDB")
 
 
-EMBEDDING_FN = getattr(settings, "EMBEDDING_FN", None)
-EMBEDDING_DIM = getattr(settings, "EMBEDDING_DIM", None)
-
-if EMBEDDING_FN is not None and EMBEDDING_DIM is None:
-    raise ValueError("EMBEDDING_FN is set but EMBEDDING_DIM is not set")
-
-PERSISTENT_PATH = getattr(
-    settings,
-    "PERSISTENT_PATH",
-    os.path.join(settings.BASE_DIR, ".vectordb", "hnsw_index.bin"),
-)
-
-if not os.path.exists(os.path.dirname(PERSISTENT_PATH)):
-    os.makedirs(os.path.dirname(PERSISTENT_PATH))
+if not os.path.exists(os.path.dirname(vectordb_settings.DEFAULT_PERSISTENT_DIRECTORY)):
+    os.makedirs(os.path.dirname(vectordb_settings.DEFAULT_PERSISTENT_DIRECTORY))
 
 
 class VectorManager(models.Manager):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.index = None
-        self.persistent_path = PERSISTENT_PATH
+        self.persistent_path = os.path.join(
+            vectordb_settings.DEFAULT_PERSISTENT_DIRECTORY, "vector.index"
+        )  # TODO: refactor coz this depends on internal knowledge of the index class
 
         logger.info(
-            "Loading the weights for the embedding model. This may take a few seconds the first time it runs because it downloads the wieghts and caches them."
+            "Loading the weights for the embedding model. This may take a few seconds the first"
+            " time it runs because it downloads the wieghts and caches them."
         )
         start = time.time()
 
         embedding_fn, embedding_dim = get_embedding_function()
-        self.embedding_dim = EMBEDDING_DIM or embedding_dim
+        self.embedding_dim = embedding_dim
         self.embedding_fn = embedding_fn
 
         if os.path.exists(self.persistent_path):
             self.index = HNSWIndex.load(self.persistent_path)
 
         logger.info(
             f"Loading the weights has been completed in {time.time() - start} seconds"
```

### Comparing `django-vectordb-0.1.2/vectordb/migrations/0001_initial.py` & `django-vectordb-0.1.3/vectordb/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 4.2 on 2023-05-03 14:16
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
```

### Comparing `django-vectordb-0.1.2/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py` & `django-vectordb-0.1.3/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Generated by Django 4.2 on 2023-05-03 20:38
 
-from django.db import migrations, models
 import django.utils.timezone
+from django.db import migrations, models
+
 import vectordb.models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("vectordb", "0001_initial"),
     ]
```

### Comparing `django-vectordb-0.1.2/vectordb/models.py` & `django-vectordb-0.1.3/vectordb/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Iterable, Optional
+from __future__ import annotations
+
 import numpy as np
-from django.db import models
+from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
+from django.core.exceptions import ValidationError
+from django.db import models
 
 from .manager import VectorManager
 
-from django.core.exceptions import ValidationError
-
 
 def validate_embedding(value):
     """
     Custom validator to ensure that the embedding is not empty or null.
     """
     if value is None or len(value) == 0:
         raise ValidationError("Embedding must be set and not be an empty bytes.")
@@ -19,15 +19,15 @@
 
 class Vector(models.Model):
     """A vector db model that can be used to store embeddings for any Django model."""
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
-    embedding = models.BinaryField(validators=[validate_embedding], max_length=None)
+    embedding = models.BinaryField(validators=[validate_embedding])
     text = models.TextField()
     metadata = models.JSONField(null=True, blank=True)
     object_id = models.CharField(max_length=255, null=True, blank=True)
 
     # allow null so that texts can be added without an object
     content_type = models.ForeignKey(
         ContentType, on_delete=models.CASCADE, null=True, blank=True
```

### Comparing `django-vectordb-0.1.2/vectordb/queryset.py` & `django-vectordb-0.1.3/vectordb/queryset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import logging
 import time
+
 import numpy as np
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
-from .ann.indexes import HNSWIndex, BFIndex
+
 from vectordb.settings import vectordb_settings
 
+from .ann.indexes import BFIndex, HNSWIndex
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(" VectorDB ")
 
 
 class VectorQuerySet(models.QuerySet):
     def _get_related_vectors(
         self, query_embeddings, vectors, k: int | None = None, ids_list=None
```

### Comparing `django-vectordb-0.1.2/vectordb/settings.py` & `django-vectordb-0.1.3/vectordb/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+from __future__ import annotations
+
 # Inspired by rest framework
-from django.conf import settings
+import os
 
+from django.conf import settings
 from django.core.signals import setting_changed
 from django.utils.module_loading import import_string
 
-
 DEFAULTS = {
     "DEFAULT_EMBEDDING_CLASS": "vectordb.embedding_functions.SentenceTransformerEncoder",
     "DEFAULT_EMBEDDING_MODEL": "all-MiniLM-L6-v2",
     "DEFAULT_EMBEDDING_SPACE": "l2",
     "DEFAULT_EMBEDDING_DIMENSION": 384,
     "DEFAULT_MAX_N_RESULTS": 10,
     "DEFAULT_MIN_SCORE": 0.0,
     "DEFAULT_MAX_BRUTEFORCE_N": 10_000,
+    "DEFAULT_PERSISTENT_DIRECTORY": os.path.join(settings.BASE_DIR, ".vectordb"),
 }
 
 
 IMPORT_STRINGS = [
     "DEFAULT_EMBEDDING_CLASS",
 ]
 
@@ -91,16 +94,16 @@
         setattr(self, attr, val)
         return val
 
     def __check_user_settings(self, user_settings):
         for setting in REMOVED_SETTINGS:
             if setting in user_settings:
                 raise RuntimeError(
-                    "The '%s' setting has been removed. Please refer to '%s' for available settings."
-                    % (setting, "https://github/pkavumba/vectordb")
+                    "The '%s' setting has been removed. Please refer to '%s' for available settings."  # noqa E501
+                    % (setting, "https://github.com/pkavumba/django-vectordb")
                 )
         return user_settings
 
     def reload(self):
         for attr in self._cached_attrs:
             delattr(self, attr)
         self._cached_attrs.clear()
```

### Comparing `django-vectordb-0.1.2/vectordb/shortcuts.py` & `django-vectordb-0.1.3/vectordb/shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.db.models.signals import post_save, post_delete
+from django.db.models.signals import post_delete, post_save
 
 from .sync_signals import sync_vectordb_on_create_update, sync_vectordb_on_delete
 
 # Define a global set to store the registered model classes
 registered_models = set()
 
 
@@ -11,15 +11,16 @@
     app_label = model_class._meta.app_label
     model_name = model_class.__name__
     # Form a unique key for the model class
     model_key = f"vectordb.{app_label}.{model_name}"
 
     # Check if the model class is already registered
     if model_key not in registered_models:
-        # Connect the handler functions to the signals for the model class with the model key as the dispatch uid
+        # Connect the handler functions to the signals for the model class
+        #  with the model key as the dispatch uid
         post_save.connect(
             sync_vectordb_on_create_update, sender=model_class, dispatch_uid=model_key
         )
         post_delete.connect(
             sync_vectordb_on_delete, sender=model_class, dispatch_uid=model_key
         )
         # Add the model key to the set of registered models
```

### Comparing `django-vectordb-0.1.2/vectordb/signals.py` & `django-vectordb-0.1.3/vectordb/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import logging
+
 import numpy as np
-from django.db.models.signals import post_save, post_delete
+from django.db.models.signals import post_delete, post_save
 from django.dispatch import receiver
-from django.contrib.contenttypes.models import ContentType
 
 from .models import Vector
 
-
 # Get an instance of a logger
 logger = logging.getLogger("VectorDB")
 logger.setLevel(logging.DEBUG)
 
 
 @receiver(post_save, sender=Vector, dispatch_uid="update_vector_index_unique_id")
 def update_vector_index(sender, instance, created, **kwargs):
```

### Comparing `django-vectordb-0.1.2/vectordb/sync_signals.py` & `django-vectordb-0.1.3/vectordb/sync_signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from __future__ import annotations
 
-import logging
-import numpy as np
-from django.db.models.signals import post_save, post_delete
-from django.dispatch import receiver
 from django.contrib.contenttypes.models import ContentType
 
 from .models import Vector
 
 
 def sync_vectordb_on_create_update(sender, instance, created, **kwargs):
     """
```

### Comparing `django-vectordb-0.1.2/vectordb/tasks.py` & `django-vectordb-0.1.3/vectordb/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
-from typing import Optional
-import numpy as np
-
-from django.db import models
-from django.contrib.contenttypes.models import ContentType
 
+import numpy as np
 from celery import shared_task
 
-
 from .models import Vector
 from .utils import get_embedding_function
 
 
 @shared_task
 def create_vector(vector_id: int) -> Vector:
     embedding_fn, embedding_dim = get_embedding_function()
```

### Comparing `django-vectordb-0.1.2/vectordb/tests/settings.py` & `django-vectordb-0.1.3/vectordb/tests/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
 
-
 LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "handlers": {
         "console": {
             "class": "logging.StreamHandler",
         },
```

### Comparing `django-vectordb-0.1.2/vectordb/tests/test_api_endpoint.py` & `django-vectordb-0.1.3/vectordb/tests/test_api_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from rest_framework import status
 from rest_framework.test import APIClient
+
 from vectordb.models import Vector
 
 
 @pytest.fixture
 def api_client():
     return APIClient()
```

### Comparing `django-vectordb-0.1.2/vectordb/tests/test_db_indexes.py` & `django-vectordb-0.1.3/vectordb/tests/test_db_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pytest
 import numpy as np
+import pytest
+
 from vectordb.ann.indexes import BFIndex, HNSWIndex
 
 nb = 100
 nq = 10
 d = 64
```

### Comparing `django-vectordb-0.1.2/vectordb/tests/test_embedding_functions.py` & `django-vectordb-0.1.3/vectordb/tests/test_embedding_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from vectordb.embedding_functions import SentenceTransformerEncoder
 
 
 @pytest.fixture
 def encoder():
     return SentenceTransformerEncoder()
```

### Comparing `django-vectordb-0.1.2/vectordb/tests/test_settings.py` & `django-vectordb-0.1.3/vectordb/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pytest
 import os
-from django.core.exceptions import ImproperlyConfigured
+
+import pytest
 from django.test import override_settings
+
 from vectordb.settings import VectorDBSettings, import_from_string, perform_import
 
 # Test data
 TEST_DEFAULTS = {
     "TEST_SETTING_1": "test_value_1",
     "TEST_SETTING_2": "vectordb.tests.dummy_module.TEST_SETTING_2",
 }
```

### Comparing `django-vectordb-0.1.2/vectordb/tests/test_singleton_meta.py` & `django-vectordb-0.1.3/vectordb/tests/test_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.2/vectordb/tests/test_vectordb.py` & `django-vectordb-0.1.3/vectordb/tests/test_vectordb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from django.contrib.contenttypes.models import ContentType
 from django.db.utils import IntegrityError
+
 from vectordb.models import Vector
 
 
 @pytest.mark.django_db
 def test_add_text():
     manager = Vector.objects
     vector = manager.add_text(1, "Sample text", {"field": "value"})
```

### Comparing `django-vectordb-0.1.2/vectordb/utils.py` & `django-vectordb-0.1.3/vectordb/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
-import logging
 import json
-import os
-import importlib
+import logging
+
+import numpy as np
 from django.conf import settings
 from django.core.serializers import serialize
 from django.db import models
-import numpy as np
-from vectordb.settings import vectordb_settings
 
+from vectordb.settings import vectordb_settings
 
 from .validators import validate_vector_data
 
 try:
-    import celery
+    import celery  # noqa
+
     from . import tasks
 
     has_celery = True
     # check if celery settings are configured
     if not hasattr(settings, "CELERY_BROKER_URL"):
         raise ImportError
```

### Comparing `django-vectordb-0.1.2/vectordb/validators.py` & `django-vectordb-0.1.3/vectordb/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
+
+import logging
 from typing import Optional
+
 import numpy as np
 from django.core.exceptions import ValidationError
-from django.db.utils import IntegrityError
 from django.db import models
-
-import logging
+from django.db.utils import IntegrityError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def validate_vector_data(
     manager: models.Manager,
```

### Comparing `django-vectordb-0.1.2/vectordb/views.py` & `django-vectordb-0.1.3/vectordb/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 try:
-    from rest_framework import viewsets, filters
+    from rest_framework import filters, viewsets
 except ImportError:
     raise ImportError("rest_framework is required for the api to work")
 
+from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework.decorators import action
 from rest_framework.response import Response
-from django_filters.rest_framework import DjangoFilterBackend
+
 from .models import Vector
 from .serializers import VectorSerializer
 
 
 class VectorViewSet(viewsets.ModelViewSet):
     queryset = Vector.objects.all()
     serializer_class = VectorSerializer
```


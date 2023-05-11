# Comparing `tmp/unicef-security-1.4.tar.gz` & `tmp/unicef-security-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicef-security-1.4.tar", last modified: Wed Apr  5 05:42:47 2023, max compression
+gzip compressed data, was "unicef-security-1.4.2.tar", last modified: Thu May 11 11:42:48 2023, max compression
```

## Comparing `unicef-security-1.4.tar` & `unicef-security-1.4.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.379926 unicef-security-1.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1842 2023-04-05 05:42:45.000000 unicef-security-1.4/CHANGES
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-04-05 05:42:45.000000 unicef-security-1.4/LICENSE
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      197 2023-04-05 05:42:45.000000 unicef-security-1.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-04-05 05:42:45.000000 unicef-security-1.4/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2023-04-05 05:42:47.379926 unicef-security-1.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2618 2023-04-05 05:42:45.000000 unicef-security-1.4/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-04-05 05:42:47.379926 unicef-security-1.4/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1921 2023-04-05 05:42:45.000000 unicef-security-1.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.371926 unicef-security-1.4/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.375926 unicef-security-1.4/src/unicef_security/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6144 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/backends.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10986 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2276 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/middleware.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.375926 unicef-security-1.4/src/unicef_security/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7279 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/migrations/0002_auto_20201028_0154.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/migrations/0003_auto_20220406_2307.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/migrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3006 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.375926 unicef-security-1.4/src/unicef_security/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.375926 unicef-security-1.4/src/unicef_security/templates/admin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/templates/admin/ad.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/templates/admin/link_user.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/templates/admin/load_users.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      194 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/templates/admin/login.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/templates/unauthorized.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-04-05 05:42:45.000000 unicef-security-1.4/src/unicef_security/views.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.375926 unicef-security-1.4/src/unicef_security.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2023-04-05 05:42:47.000000 unicef-security-1.4/src/unicef_security.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1867 2023-04-05 05:42:47.000000 unicef-security-1.4/src/unicef_security.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-05 05:42:47.000000 unicef-security-1.4/src/unicef_security.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-05 05:42:47.000000 unicef-security-1.4/src/unicef_security.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-04-05 05:42:47.000000 unicef-security-1.4/src/unicef_security.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.375926 unicef-security-1.4/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.379926 unicef-security-1.4/tests/demoproject/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.379926 unicef-security-1.4/tests/demoproject/demo/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.379926 unicef-security-1.4/tests/demoproject/demo/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5140 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/migrations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2432 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/demo/wsgi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/factories.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      810 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/demoproject/manage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      219 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/test_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1095 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/test_azure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      216 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/test_backends.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      439 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/test_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2601 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/test_pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 05:42:47.379926 unicef-security-1.4/tests/vcr_cassettes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9126 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/vcr_cassettes/_test_user_data.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5524 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/vcr_cassettes/load_business_area.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5524 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/vcr_cassettes/load_region.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/vcr_cassettes/test_token.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7655 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/vcr_cassettes/test_user_data.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-04-05 05:42:45.000000 unicef-security-1.4/tests/vcrpy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-05 05:42:45.000000 unicef-security-1.4/tox.ini
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.387187 unicef-security-1.4.2/
+-rw-r--r--   0 jojo       (501) staff       (20)     1962 2023-05-11 11:07:47.000000 unicef-security-1.4.2/CHANGES
+-rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:23:06.000000 unicef-security-1.4.2/LICENSE
+-rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-security-1.4.2/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)     1791 2023-05-05 13:23:06.000000 unicef-security-1.4.2/Makefile
+-rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 11:42:48.387401 unicef-security-1.4.2/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2618 2023-05-05 13:23:06.000000 unicef-security-1.4.2/README.rst
+-rw-r--r--   0 jojo       (501) staff       (20)       82 2023-05-11 11:42:48.388146 unicef-security-1.4.2/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1921 2023-05-05 13:23:06.000000 unicef-security-1.4.2/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.350285 unicef-security-1.4.2/src/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.364639 unicef-security-1.4.2/src/unicef_security/
+-rw-r--r--   0 jojo       (501) staff       (20)       57 2023-05-11 11:07:47.000000 unicef-security-1.4.2/src/unicef_security/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6144 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1373 2023-05-11 11:07:37.000000 unicef-security-1.4.2/src/unicef_security/backends.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1017 2023-05-11 10:50:08.000000 unicef-security-1.4.2/src/unicef_security/config.py
+-rw-r--r--   0 jojo       (501) staff       (20)    11031 2023-05-11 10:50:08.000000 unicef-security-1.4.2/src/unicef_security/graph.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2276 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/middleware.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.369296 unicef-security-1.4.2/src/unicef_security/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     7279 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)      454 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/0002_auto_20201028_0154.py
+-rw-r--r--   0 jojo       (501) staff       (20)      528 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/0003_auto_20220406_2307.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1314 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3006 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/pipeline.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.369705 unicef-security-1.4.2/src/unicef_security/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.372155 unicef-security-1.4.2/src/unicef_security/templates/admin/
+-rw-r--r--   0 jojo       (501) staff       (20)      650 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/ad.html
+-rw-r--r--   0 jojo       (501) staff       (20)     1380 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/link_user.html
+-rw-r--r--   0 jojo       (501) staff       (20)      786 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/load_users.html
+-rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/login.html
+-rw-r--r--   0 jojo       (501) staff       (20)     2625 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/unauthorized.html
+-rw-r--r--   0 jojo       (501) staff       (20)      316 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      223 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)      929 2023-05-11 10:50:08.000000 unicef-security-1.4.2/src/unicef_security/views.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.367449 unicef-security-1.4.2/src/unicef_security.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1867 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      295 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       16 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.378029 unicef-security-1.4.2/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      218 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/.coveragerc
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      129 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/conftest.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.379439 unicef-security-1.4.2/tests/demoproject/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.382507 unicef-security-1.4.2/tests/demoproject/demo/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      172 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/admin.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.383682 unicef-security-1.4.2/tests/demoproject/demo/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/migrations/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      138 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2432 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/settings.py
+-rw-r--r--   0 jojo       (501) staff       (20)      210 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/wsgi.py
+-rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/factories.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      810 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/manage.py
+-rw-r--r--   0 jojo       (501) staff       (20)      219 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/fixtures.py
+-rw-r--r--   0 jojo       (501) staff       (20)      208 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1095 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_azure.py
+-rw-r--r--   0 jojo       (501) staff       (20)      216 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_backends.py
+-rw-r--r--   0 jojo       (501) staff       (20)      439 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2601 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_pipeline.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.386596 unicef-security-1.4.2/tests/vcr_cassettes/
+-rw-r--r--   0 jojo       (501) staff       (20)     9126 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/_test_user_data.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/load_business_area.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/load_region.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     2984 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/test_token.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     7655 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/test_user_data.yml
+-rw-r--r--   0 jojo       (501) staff       (20)      823 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcrpy.py
+-rw-r--r--   0 jojo       (501) staff       (20)      997 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tox.ini
```

### Comparing `unicef-security-1.4/CHANGES` & `unicef-security-1.4.2/CHANGES`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Release 1.4.2
+-----------------------------
+* fix ci
+
+
+Release 1.4.1
+-----------------------------
+* fixed logout url
+
+
 Release 1.4
 -----------------------------
 * added support to django 4.2
 * added support to python 3.11
 * fixed unauthorized template
 * compatible with latest social core
```

### Comparing `unicef-security-1.4/LICENSE` & `unicef-security-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/Makefile` & `unicef-security-1.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/PKG-INFO` & `unicef-security-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-security
-Version: 1.4
+Version: 1.4.2
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 Author-email: rapidpro@unicef.org
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `unicef-security-1.4/README.rst` & `unicef-security-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/setup.py` & `unicef-security-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/admin.py` & `unicef-security-1.4.2/src/unicef_security/admin.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/backends.py` & `unicef-security-1.4.2/src/unicef_security/backends.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from jwt import decode as jwt_decode, DecodeError, ExpiredSignatureError, get_unverified_header
+from jwt import decode, DecodeError, ExpiredSignatureError, get_unverified_header
 from social_core.backends.azuread_b2c import AzureADB2COAuth2
 from social_core.backends.azuread_tenant import AzureADTenantOAuth2
 from social_core.exceptions import AuthTokenError
 
 
 class UNICEFAzureADTenantOAuth2Ext(AzureADTenantOAuth2):
     name = "unicef-azuread-tenant-oauth2"
@@ -20,15 +20,15 @@
         try:
             # retrieve certificate for key_id
             if verify:
                 certificate = self.get_certificate(key_id)
                 key = certificate.public_key()
 
             options = {"verify_signature": verify}
-            return jwt_decode(
+            return decode(
                 id_token,
                 key=key,
                 algorithms=["RS256"],
                 audience=self.setting("KEY"),
                 options=options,
             )
         except (DecodeError, ExpiredSignatureError) as error:
```

### Comparing `unicef-security-1.4/src/unicef_security/config.py` & `unicef-security-1.4.2/src/unicef_security/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 GRAPH_CLIENT_ID = os.environ.get("GRAPH_CLIENT_ID", AZURE_CLIENT_ID)
 GRAPH_CLIENT_SECRET = os.environ.get("GRAPH_CLIENT_SECRET", AZURE_CLIENT_SECRET)
 
 AZURE_SSL = True
 AZURE_URL_EXPIRATION_SECS = 10800
 AZURE_ACCESS_POLICY_EXPIRY = 10800  # length of time before signature expires in seconds
 AZURE_ACCESS_POLICY_PERMISSION = "r"
-AZURE_TOKEN_URL = "https://login.microsoftonline.com/unicef.org/oauth2/token"
+AZURE_URL = "https://login.microsoftonline.com"
 AZURE_GRAPH_API_BASE_URL = "https://graph.microsoft.com"
 AZURE_GRAPH_API_VERSION = os.environ.get("AZURE_GRAPH_API_VERSION", "v1.0")  # beta
 AZURE_GRAPH_API_PAGE_SIZE = 300
 
-AZURE_LOGOUT_BASE_URL = get_setting(
-    ["SOCIAL_AUTH_TENANT_B2C_URL", "TENANT_B2C_URL", "AZURE_LOGOUT_BASE_URL"],
-    default="login.microsoftonline.com",
-)
 AZURE_POLICY = get_setting(["SOCIAL_AUTH_POLICY", "TENANT_POLICY"])
 AZURE_TENANT_ID = get_setting(["SOCIAL_AUTH_TENANT_ID", "TENANT_ID"])
 AZURE_RESET_POLICY = get_setting(
     ["SOCIAL_AUTH_PASSWORD_RESET_POLICY", "PASSWORD_RESET_POLICY"]
 )
 
 UNICEF_EMAIL = os.environ.get("UNICEF_EMAIL", "@unicef.org")
```

### Comparing `unicef-security-1.4/src/unicef_security/graph.py` & `unicef-security-1.4.2/src/unicef_security/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,17 @@
             raise ValueError("Configure AZURE_CLIENT_ID and/or AZURE_CLIENT_SECRET")
         post_dict = {
             "grant_type": "client_credentials",
             "client_id": self.id,
             "client_secret": self.secret,
             "resource": config.AZURE_GRAPH_API_BASE_URL,
         }
-        response = requests.post(config.AZURE_TOKEN_URL, post_dict)
+        response = requests.post(
+            f"{config.AZURE_URL}/unicef.org/oauth2/token", post_dict
+        )
         if response.status_code != 200:  # pragma: no cover
             logger.error(
                 f"Unable to fetch token from Azure. {response.status_code} {response.content}"
             )
             raise BaseException(
                 f"Error during token retrieval: {response.status_code} {response.content}"
             )
```

### Comparing `unicef-security-1.4/src/unicef_security/middleware.py` & `unicef-security-1.4.2/src/unicef_security/middleware.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/migrations/0001_initial.py` & `unicef-security-1.4.2/src/unicef_security/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/migrations/0003_auto_20220406_2307.py` & `unicef-security-1.4.2/src/unicef_security/migrations/0003_auto_20220406_2307.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/models.py` & `unicef-security-1.4.2/src/unicef_security/models.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/pipeline.py` & `unicef-security-1.4.2/src/unicef_security/pipeline.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/templates/admin/ad.html` & `unicef-security-1.4.2/src/unicef_security/templates/admin/ad.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/templates/admin/link_user.html` & `unicef-security-1.4.2/src/unicef_security/templates/admin/link_user.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/templates/admin/load_users.html` & `unicef-security-1.4.2/src/unicef_security/templates/admin/load_users.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/templates/unauthorized.html` & `unicef-security-1.4.2/src/unicef_security/templates/unauthorized.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/src/unicef_security/views.py` & `unicef-security-1.4.2/src/unicef_security/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
             UNICEF_EMAIL
         )
         return context
 
 
 class UNICEFLogoutView(RedirectView):
     def get_redirect_url(self, *args, **kwargs):
-        base_url = config.AZURE_LOGOUT_BASE_URL
+        base_url = config.AZURE_URL
         tenant_id = config.AZURE_TENANT_ID
-        host = self.request.get_host()
-
-        return (
-            f"https://{base_url}/{tenant_id}/oauth2/v2.0/"
-            f"logout?post_logout_redirect_uri={host}/{settings.LOGOUT_URL}"
+        redirect_url = (
+            f"{self.request.scheme}://{self.request.get_host()}{settings.LOGOUT_URL}"
         )
+
+        return f"{base_url}/{tenant_id}/oauth2/v2.0/logout?post_logout_redirect_uri={redirect_url}"
```

### Comparing `unicef-security-1.4/src/unicef_security.egg-info/PKG-INFO` & `unicef-security-1.4.2/src/unicef_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-security
-Version: 1.4
+Version: 1.4.2
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 Author-email: rapidpro@unicef.org
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `unicef-security-1.4/src/unicef_security.egg-info/SOURCES.txt` & `unicef-security-1.4.2/src/unicef_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/demoproject/demo/migrations/0001_initial.py` & `unicef-security-1.4.2/tests/demoproject/demo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/demoproject/demo/settings.py` & `unicef-security-1.4.2/tests/demoproject/demo/settings.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/demoproject/manage.py` & `unicef-security-1.4.2/tests/demoproject/manage.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/test_azure.py` & `unicef-security-1.4.2/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/test_pipeline.py` & `unicef-security-1.4.2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/vcr_cassettes/_test_user_data.yml` & `unicef-security-1.4.2/tests/vcr_cassettes/_test_user_data.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/vcr_cassettes/load_business_area.yml` & `unicef-security-1.4.2/tests/vcr_cassettes/load_business_area.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/vcr_cassettes/load_region.yml` & `unicef-security-1.4.2/tests/vcr_cassettes/load_region.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/vcr_cassettes/test_token.yml` & `unicef-security-1.4.2/tests/vcr_cassettes/test_token.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/vcr_cassettes/test_user_data.yml` & `unicef-security-1.4.2/tests/vcr_cassettes/test_user_data.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tests/vcrpy.py` & `unicef-security-1.4.2/tests/vcrpy.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4/tox.ini` & `unicef-security-1.4.2/tox.ini`

 * *Files identical despite different names*


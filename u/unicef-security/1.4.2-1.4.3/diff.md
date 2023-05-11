# Comparing `tmp/unicef-security-1.4.2.tar.gz` & `tmp/unicef-security-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicef-security-1.4.2.tar", last modified: Thu May 11 11:42:48 2023, max compression
+gzip compressed data, was "unicef-security-1.4.3.tar", last modified: Thu May 11 13:55:17 2023, max compression
```

## Comparing `unicef-security-1.4.2.tar` & `unicef-security-1.4.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.387187 unicef-security-1.4.2/
--rw-r--r--   0 jojo       (501) staff       (20)     1962 2023-05-11 11:07:47.000000 unicef-security-1.4.2/CHANGES
--rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:23:06.000000 unicef-security-1.4.2/LICENSE
--rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-security-1.4.2/MANIFEST.in
--rw-r--r--   0 jojo       (501) staff       (20)     1791 2023-05-05 13:23:06.000000 unicef-security-1.4.2/Makefile
--rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 11:42:48.387401 unicef-security-1.4.2/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     2618 2023-05-05 13:23:06.000000 unicef-security-1.4.2/README.rst
--rw-r--r--   0 jojo       (501) staff       (20)       82 2023-05-11 11:42:48.388146 unicef-security-1.4.2/setup.cfg
--rwxr-xr-x   0 jojo       (501) staff       (20)     1921 2023-05-05 13:23:06.000000 unicef-security-1.4.2/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.350285 unicef-security-1.4.2/src/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.364639 unicef-security-1.4.2/src/unicef_security/
--rw-r--r--   0 jojo       (501) staff       (20)       57 2023-05-11 11:07:47.000000 unicef-security-1.4.2/src/unicef_security/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     6144 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/admin.py
--rw-r--r--   0 jojo       (501) staff       (20)      127 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/apps.py
--rw-r--r--   0 jojo       (501) staff       (20)     1373 2023-05-11 11:07:37.000000 unicef-security-1.4.2/src/unicef_security/backends.py
--rw-r--r--   0 jojo       (501) staff       (20)     1017 2023-05-11 10:50:08.000000 unicef-security-1.4.2/src/unicef_security/config.py
--rw-r--r--   0 jojo       (501) staff       (20)    11031 2023-05-11 10:50:08.000000 unicef-security-1.4.2/src/unicef_security/graph.py
--rw-r--r--   0 jojo       (501) staff       (20)     2276 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/middleware.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.369296 unicef-security-1.4.2/src/unicef_security/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     7279 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)      454 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/0002_auto_20201028_0154.py
--rw-r--r--   0 jojo       (501) staff       (20)      528 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/0003_auto_20220406_2307.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/migrations/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1314 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     3006 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/pipeline.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.369705 unicef-security-1.4.2/src/unicef_security/templates/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.372155 unicef-security-1.4.2/src/unicef_security/templates/admin/
--rw-r--r--   0 jojo       (501) staff       (20)      650 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/ad.html
--rw-r--r--   0 jojo       (501) staff       (20)     1380 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/link_user.html
--rw-r--r--   0 jojo       (501) staff       (20)      786 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/load_users.html
--rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/admin/login.html
--rw-r--r--   0 jojo       (501) staff       (20)     2625 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/templates/unauthorized.html
--rw-r--r--   0 jojo       (501) staff       (20)      316 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      223 2023-05-05 13:23:06.000000 unicef-security-1.4.2/src/unicef_security/utils.py
--rw-r--r--   0 jojo       (501) staff       (20)      929 2023-05-11 10:50:08.000000 unicef-security-1.4.2/src/unicef_security/views.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.367449 unicef-security-1.4.2/src/unicef_security.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1867 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)      295 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       16 2023-05-11 11:42:48.000000 unicef-security-1.4.2/src/unicef_security.egg-info/top_level.txt
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.378029 unicef-security-1.4.2/tests/
--rw-r--r--   0 jojo       (501) staff       (20)      218 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/.coveragerc
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      129 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/conftest.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.379439 unicef-security-1.4.2/tests/demoproject/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.382507 unicef-security-1.4.2/tests/demoproject/demo/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      172 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/admin.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.383682 unicef-security-1.4.2/tests/demoproject/demo/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/migrations/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      138 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2432 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/settings.py
--rw-r--r--   0 jojo       (501) staff       (20)      210 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/demo/wsgi.py
--rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/factories.py
--rwxr-xr-x   0 jojo       (501) staff       (20)      810 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/demoproject/manage.py
--rw-r--r--   0 jojo       (501) staff       (20)      219 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/fixtures.py
--rw-r--r--   0 jojo       (501) staff       (20)      208 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_admin.py
--rw-r--r--   0 jojo       (501) staff       (20)     1095 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_azure.py
--rw-r--r--   0 jojo       (501) staff       (20)      216 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_backends.py
--rw-r--r--   0 jojo       (501) staff       (20)      439 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2601 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/test_pipeline.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 11:42:48.386596 unicef-security-1.4.2/tests/vcr_cassettes/
--rw-r--r--   0 jojo       (501) staff       (20)     9126 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/_test_user_data.yml
--rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/load_business_area.yml
--rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/load_region.yml
--rw-r--r--   0 jojo       (501) staff       (20)     2984 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/test_token.yml
--rw-r--r--   0 jojo       (501) staff       (20)     7655 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcr_cassettes/test_user_data.yml
--rw-r--r--   0 jojo       (501) staff       (20)      823 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tests/vcrpy.py
--rw-r--r--   0 jojo       (501) staff       (20)      997 2023-05-05 13:23:06.000000 unicef-security-1.4.2/tox.ini
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.216199 unicef-security-1.4.3/
+-rw-r--r--   0 jojo       (501) staff       (20)     2025 2023-05-11 13:54:23.000000 unicef-security-1.4.3/CHANGES
+-rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:23:06.000000 unicef-security-1.4.3/LICENSE
+-rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-security-1.4.3/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)     1791 2023-05-05 13:23:06.000000 unicef-security-1.4.3/Makefile
+-rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 13:55:17.216430 unicef-security-1.4.3/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2618 2023-05-05 13:23:06.000000 unicef-security-1.4.3/README.rst
+-rw-r--r--   0 jojo       (501) staff       (20)       82 2023-05-11 13:55:17.217378 unicef-security-1.4.3/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1921 2023-05-05 13:23:06.000000 unicef-security-1.4.3/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.172741 unicef-security-1.4.3/src/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.188282 unicef-security-1.4.3/src/unicef_security/
+-rw-r--r--   0 jojo       (501) staff       (20)       57 2023-05-11 13:54:23.000000 unicef-security-1.4.3/src/unicef_security/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6144 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1373 2023-05-11 11:07:37.000000 unicef-security-1.4.3/src/unicef_security/backends.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1023 2023-05-11 13:54:23.000000 unicef-security-1.4.3/src/unicef_security/config.py
+-rw-r--r--   0 jojo       (501) staff       (20)    11031 2023-05-11 10:50:08.000000 unicef-security-1.4.3/src/unicef_security/graph.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2276 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/middleware.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.193615 unicef-security-1.4.3/src/unicef_security/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     7279 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)      454 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/0002_auto_20201028_0154.py
+-rw-r--r--   0 jojo       (501) staff       (20)      528 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/0003_auto_20220406_2307.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/migrations/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1314 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3006 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/pipeline.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.194013 unicef-security-1.4.3/src/unicef_security/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.196548 unicef-security-1.4.3/src/unicef_security/templates/admin/
+-rw-r--r--   0 jojo       (501) staff       (20)      650 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/ad.html
+-rw-r--r--   0 jojo       (501) staff       (20)     1380 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/link_user.html
+-rw-r--r--   0 jojo       (501) staff       (20)      786 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/load_users.html
+-rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/admin/login.html
+-rw-r--r--   0 jojo       (501) staff       (20)     2625 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/templates/unauthorized.html
+-rw-r--r--   0 jojo       (501) staff       (20)      316 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      223 2023-05-05 13:23:06.000000 unicef-security-1.4.3/src/unicef_security/utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)      925 2023-05-11 13:54:23.000000 unicef-security-1.4.3/src/unicef_security/views.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.191437 unicef-security-1.4.3/src/unicef_security.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      611 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1867 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      295 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       16 2023-05-11 13:55:17.000000 unicef-security-1.4.3/src/unicef_security.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.202236 unicef-security-1.4.3/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      218 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/.coveragerc
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      129 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/conftest.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.203795 unicef-security-1.4.3/tests/demoproject/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.207776 unicef-security-1.4.3/tests/demoproject/demo/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      172 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/admin.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.212909 unicef-security-1.4.3/tests/demoproject/demo/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/migrations/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      138 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2432 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/settings.py
+-rw-r--r--   0 jojo       (501) staff       (20)      210 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/demo/wsgi.py
+-rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/factories.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      810 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/demoproject/manage.py
+-rw-r--r--   0 jojo       (501) staff       (20)      219 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/fixtures.py
+-rw-r--r--   0 jojo       (501) staff       (20)      208 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1095 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_azure.py
+-rw-r--r--   0 jojo       (501) staff       (20)      216 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_backends.py
+-rw-r--r--   0 jojo       (501) staff       (20)      439 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2601 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/test_pipeline.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-11 13:55:17.215711 unicef-security-1.4.3/tests/vcr_cassettes/
+-rw-r--r--   0 jojo       (501) staff       (20)     9126 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/_test_user_data.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/load_business_area.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     5524 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/load_region.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     2984 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/test_token.yml
+-rw-r--r--   0 jojo       (501) staff       (20)     7655 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcr_cassettes/test_user_data.yml
+-rw-r--r--   0 jojo       (501) staff       (20)      823 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tests/vcrpy.py
+-rw-r--r--   0 jojo       (501) staff       (20)      997 2023-05-05 13:23:06.000000 unicef-security-1.4.3/tox.ini
```

### Comparing `unicef-security-1.4.2/CHANGES` & `unicef-security-1.4.3/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Release 1.4.3
+-----------------------------
+* fix logout url
+
+
 Release 1.4.2
 -----------------------------
 * fix ci
 
 
 Release 1.4.1
 -----------------------------
```

### Comparing `unicef-security-1.4.2/LICENSE` & `unicef-security-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/Makefile` & `unicef-security-1.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/PKG-INFO` & `unicef-security-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-security
-Version: 1.4.2
+Version: 1.4.3
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 Author-email: rapidpro@unicef.org
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `unicef-security-1.4.2/README.rst` & `unicef-security-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/setup.py` & `unicef-security-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/admin.py` & `unicef-security-1.4.3/src/unicef_security/admin.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/backends.py` & `unicef-security-1.4.3/src/unicef_security/backends.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/config.py` & `unicef-security-1.4.3/src/unicef_security/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 AZURE_ACCESS_POLICY_PERMISSION = "r"
 AZURE_URL = "https://login.microsoftonline.com"
 AZURE_GRAPH_API_BASE_URL = "https://graph.microsoft.com"
 AZURE_GRAPH_API_VERSION = os.environ.get("AZURE_GRAPH_API_VERSION", "v1.0")  # beta
 AZURE_GRAPH_API_PAGE_SIZE = 300
 
 AZURE_POLICY = get_setting(["SOCIAL_AUTH_POLICY", "TENANT_POLICY"])
-AZURE_TENANT_ID = get_setting(["SOCIAL_AUTH_TENANT_ID", "TENANT_ID"])
+AZURE_TENANT_NAME = get_setting(["SOCIAL_AUTH_TENANT_NAME", "TENANT_NAME"])
 AZURE_RESET_POLICY = get_setting(
     ["SOCIAL_AUTH_PASSWORD_RESET_POLICY", "PASSWORD_RESET_POLICY"]
 )
 
 UNICEF_EMAIL = os.environ.get("UNICEF_EMAIL", "@unicef.org")
```

### Comparing `unicef-security-1.4.2/src/unicef_security/graph.py` & `unicef-security-1.4.3/src/unicef_security/graph.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/middleware.py` & `unicef-security-1.4.3/src/unicef_security/middleware.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/migrations/0001_initial.py` & `unicef-security-1.4.3/src/unicef_security/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/migrations/0003_auto_20220406_2307.py` & `unicef-security-1.4.3/src/unicef_security/migrations/0003_auto_20220406_2307.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/models.py` & `unicef-security-1.4.3/src/unicef_security/models.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/pipeline.py` & `unicef-security-1.4.3/src/unicef_security/pipeline.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/templates/admin/ad.html` & `unicef-security-1.4.3/src/unicef_security/templates/admin/ad.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/templates/admin/link_user.html` & `unicef-security-1.4.3/src/unicef_security/templates/admin/link_user.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/templates/admin/load_users.html` & `unicef-security-1.4.3/src/unicef_security/templates/admin/load_users.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/templates/unauthorized.html` & `unicef-security-1.4.3/src/unicef_security/templates/unauthorized.html`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/src/unicef_security/views.py` & `unicef-security-1.4.3/src/unicef_security/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,13 @@
         )
         return context
 
 
 class UNICEFLogoutView(RedirectView):
     def get_redirect_url(self, *args, **kwargs):
         base_url = config.AZURE_URL
-        tenant_id = config.AZURE_TENANT_ID
+        tenant = config.AZURE_TENANT_NAME
         redirect_url = (
             f"{self.request.scheme}://{self.request.get_host()}{settings.LOGOUT_URL}"
         )
 
-        return f"{base_url}/{tenant_id}/oauth2/v2.0/logout?post_logout_redirect_uri={redirect_url}"
+        return f"{base_url}/{tenant}/oauth2/v2.0/logout?post_logout_redirect_uri={redirect_url}"
```

### Comparing `unicef-security-1.4.2/src/unicef_security.egg-info/PKG-INFO` & `unicef-security-1.4.3/src/unicef_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-security
-Version: 1.4.2
+Version: 1.4.3
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 Author-email: rapidpro@unicef.org
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `unicef-security-1.4.2/src/unicef_security.egg-info/SOURCES.txt` & `unicef-security-1.4.3/src/unicef_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/demoproject/demo/migrations/0001_initial.py` & `unicef-security-1.4.3/tests/demoproject/demo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/demoproject/demo/settings.py` & `unicef-security-1.4.3/tests/demoproject/demo/settings.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/demoproject/manage.py` & `unicef-security-1.4.3/tests/demoproject/manage.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/test_azure.py` & `unicef-security-1.4.3/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/test_pipeline.py` & `unicef-security-1.4.3/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/vcr_cassettes/_test_user_data.yml` & `unicef-security-1.4.3/tests/vcr_cassettes/_test_user_data.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/vcr_cassettes/load_business_area.yml` & `unicef-security-1.4.3/tests/vcr_cassettes/load_business_area.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/vcr_cassettes/load_region.yml` & `unicef-security-1.4.3/tests/vcr_cassettes/load_region.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/vcr_cassettes/test_token.yml` & `unicef-security-1.4.3/tests/vcr_cassettes/test_token.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/vcr_cassettes/test_user_data.yml` & `unicef-security-1.4.3/tests/vcr_cassettes/test_user_data.yml`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tests/vcrpy.py` & `unicef-security-1.4.3/tests/vcrpy.py`

 * *Files identical despite different names*

### Comparing `unicef-security-1.4.2/tox.ini` & `unicef-security-1.4.3/tox.ini`

 * *Files identical despite different names*


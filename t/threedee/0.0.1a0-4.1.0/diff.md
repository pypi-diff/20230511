# Comparing `tmp/threedee-0.0.1a0.tar.gz` & `tmp/threedee-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedee-0.0.1a0.tar", last modified: Thu May 11 10:32:01 2023, max compression
+gzip compressed data, was "threedee-4.1.0.tar", last modified: Thu May 11 14:29:59 2023, max compression
```

## Comparing `threedee-0.0.1a0.tar` & `threedee-4.1.0.tar`

### file list

```diff
@@ -1,17 +1,48 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 10:32:01.628984 threedee-0.0.1a0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 threedee-0.0.1a0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 threedee-0.0.1a0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)       38 2022-11-21 19:45:36.000000 threedee-0.0.1a0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)      796 2023-05-11 10:32:01.629110 threedee-0.0.1a0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      143 2023-05-11 10:21:31.000000 threedee-0.0.1a0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 threedee-0.0.1a0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)      776 2023-05-11 10:32:01.630057 threedee-0.0.1a0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 10:32:01.621208 threedee-0.0.1a0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 10:32:01.622904 threedee-0.0.1a0/src/placeholder/
--rw-r--r--   0 work       (505) staff       (20)        0 2023-05-11 10:21:44.000000 threedee-0.0.1a0/src/placeholder/__init__.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 10:32:01.628727 threedee-0.0.1a0/src/threedee.egg-info/
--rw-r--r--   0 work       (505) staff       (20)      796 2023-05-11 10:32:01.000000 threedee-0.0.1a0/src/threedee.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      273 2023-05-11 10:32:01.000000 threedee-0.0.1a0/src/threedee.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 10:32:01.000000 threedee-0.0.1a0/src/threedee.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)       12 2023-05-11 10:32:01.000000 threedee-0.0.1a0/src/threedee.egg-info/top_level.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 10:32:01.000000 threedee-0.0.1a0/src/threedee.egg-info/zip-safe
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.804359 threedee-4.1.0/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 threedee-4.1.0/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 threedee-4.1.0/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)      301 2022-11-21 19:49:53.000000 threedee-4.1.0/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)     1246 2023-05-11 14:29:59.804502 threedee-4.1.0/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      594 2023-05-11 12:59:30.000000 threedee-4.1.0/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 threedee-4.1.0/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)      939 2023-05-11 14:29:59.806127 threedee-4.1.0/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.741553 threedee-4.1.0/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.751196 threedee-4.1.0/src/threedee/
+-rw-r--r--   0 work       (505) staff       (20)       92 2022-04-10 19:11:14.000000 threedee-4.1.0/src/threedee/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1414 2023-03-06 23:18:44.000000 threedee-4.1.0/src/threedee/apps.py
+-rw-r--r--   0 work       (505) staff       (20)       39 2023-02-07 12:21:16.000000 threedee-4.1.0/src/threedee/default_settings.py
+-rw-r--r--   0 work       (505) staff       (20)     5303 2023-02-07 12:21:05.000000 threedee-4.1.0/src/threedee/fields.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.763018 threedee-4.1.0/src/threedee/migrations/
+-rw-r--r--   0 work       (505) staff       (20)     1926 2023-01-27 21:16:47.000000 threedee-4.1.0/src/threedee/migrations/0001_initial.py
+-rw-r--r--   0 work       (505) staff       (20)      665 2023-02-20 22:39:59.000000 threedee-4.1.0/src/threedee/migrations/0002_add_attachment_roles.py
+-rw-r--r--   0 work       (505) staff       (20)        0 2018-12-05 17:28:26.000000 threedee-4.1.0/src/threedee/migrations/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     6042 2023-02-20 21:30:16.000000 threedee-4.1.0/src/threedee/models.py
+-rw-r--r--   0 work       (505) staff       (20)     4000 2022-09-26 14:31:49.000000 threedee-4.1.0/src/threedee/paraview_import.py
+-rw-r--r--   0 work       (505) staff       (20)      295 2023-02-16 21:37:47.000000 threedee-4.1.0/src/threedee/permissions.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.741844 threedee-4.1.0/src/threedee/static/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.742015 threedee-4.1.0/src/threedee/static/threedee/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.765054 threedee-4.1.0/src/threedee/static/threedee/css/
+-rw-r--r--   0 work       (505) staff       (20)      778 2022-06-05 12:16:18.000000 threedee-4.1.0/src/threedee/static/threedee/css/common.css
+-rw-r--r--   0 work       (505) staff       (20)     7245 2022-12-12 19:28:10.000000 threedee-4.1.0/src/threedee/static/threedee/css/paraview_webgl_model.css
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-03-07 14:16:52.000000 threedee-4.1.0/src/threedee/static/threedee/css/threedee.css
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.767755 threedee-4.1.0/src/threedee/static/threedee/js/
+-rw-r--r--   0 work       (505) staff       (20)   693247 2023-03-07 14:16:52.000000 threedee-4.1.0/src/threedee/static/threedee/js/threedee.js
+-rw-r--r--   0 work       (505) staff       (20)    21353 2023-01-27 14:18:13.000000 threedee-4.1.0/src/threedee/static/threedee/js/threedee_worker.js
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.742192 threedee-4.1.0/src/threedee/templates/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.769314 threedee-4.1.0/src/threedee/templates/threedee/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.770254 threedee-4.1.0/src/threedee/templates/threedee/examples/
+-rw-------   0 work       (505) staff       (20) 12637632 2019-06-24 15:56:02.000000 threedee-4.1.0/src/threedee/templates/threedee/examples/paraview_mesh.html
+-rw-r--r--   0 work       (505) staff       (20)     2083 2022-12-12 22:29:14.000000 threedee-4.1.0/src/threedee/templates/threedee/paraview_webgl_model.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.802235 threedee-4.1.0/src/threedee/templates/threedee/tags/
+-rw-r--r--   0 work       (505) staff       (20)     1704 2022-12-12 14:43:59.000000 threedee-4.1.0/src/threedee/templates/threedee/tags/support.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.803575 threedee-4.1.0/src/threedee/templatetags/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-04-29 20:48:33.000000 threedee-4.1.0/src/threedee/templatetags/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)      508 2023-01-26 14:08:40.000000 threedee-4.1.0/src/threedee/templatetags/threedee_tags.py
+-rw-r--r--   0 work       (505) staff       (20)       60 2018-12-05 17:28:26.000000 threedee-4.1.0/src/threedee/tests.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:29:59.761151 threedee-4.1.0/src/threedee.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)     1246 2023-05-11 14:29:59.000000 threedee-4.1.0/src/threedee.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)     1112 2023-05-11 14:29:59.000000 threedee-4.1.0/src/threedee.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:29:59.000000 threedee-4.1.0/src/threedee.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:29:59.000000 threedee-4.1.0/src/threedee.egg-info/not-zip-safe
+-rw-r--r--   0 work       (505) staff       (20)      158 2023-05-11 14:29:59.000000 threedee-4.1.0/src/threedee.egg-info/requires.txt
+-rw-r--r--   0 work       (505) staff       (20)        9 2023-05-11 14:29:59.000000 threedee-4.1.0/src/threedee.egg-info/top_level.txt
```

### Comparing `threedee-0.0.1a0/LICENSE.txt` & `threedee-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

